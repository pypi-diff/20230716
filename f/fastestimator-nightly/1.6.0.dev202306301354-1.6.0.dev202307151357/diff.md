# Comparing `tmp/fastestimator-nightly-1.6.0.dev202306301354.tar.gz` & `tmp/fastestimator-nightly-1.6.0.dev202307151357.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastestimator-nightly-1.6.0.dev202306301354.tar", last modified: Fri Jun 30 13:54:16 2023, max compression
+gzip compressed data, was "fastestimator-nightly-1.6.0.dev202307151357.tar", last modified: Sat Jul 15 13:57:48 2023, max compression
```

## Comparing `fastestimator-nightly-1.6.0.dev202306301354.tar` & `fastestimator-nightly-1.6.0.dev202307151357.tar`

### file list

```diff
@@ -1,784 +1,801 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.787844 fastestimator-nightly-1.6.0.dev202306301354/
--rw-r--r--   0 root         (0) root         (0)    11356 2023-06-30 13:46:03.000000 fastestimator-nightly-1.6.0.dev202306301354/LICENSE
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-30 13:54:16.787844 fastestimator-nightly-1.6.0.dev202306301354/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6271 2023-06-30 13:46:03.000000 fastestimator-nightly-1.6.0.dev202306301354/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.519854 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.519854 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.523854 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1609 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7452 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/lenet.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/unet.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.527854 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1624 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4800 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/lenet.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/resnet9.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/unet.py
--rw-r--r--   0 root         (0) root         (0)     5580 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.547853 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/
--rw-r--r--   0 root         (0) root         (0)    10420 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_abs.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_argmax.py
--rw-r--r--   0 root         (0) root         (0)     4853 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     3989 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_cast.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2539 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_concat.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_convert_tensor_precision.py
--rw-r--r--   0 root         (0) root         (0)     7866 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_exp.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2502 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_flip.py
--rw-r--r--   0 root         (0) root         (0)     6816 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     3148 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_gather.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_gather_from_batch.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     2512 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_shape.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_huber.py
--rw-r--r--   0 root         (0) root         (0)     4476 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_iwd.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     4558 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_load_model.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_matmul.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_maximum.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_permute.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_pow.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4323 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_roll.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_save_model.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_sign.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_smooth_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     4987 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     5742 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     4394 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5214 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_update_model.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_watch.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_where.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.551853 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/
--rw-r--r--   0 root         (0) root         (0)     1618 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/history.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/logs.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/plot.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     6574 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.559852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16450 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/combined_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/csv_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.571852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)     3956 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifair10.py
--rw-r--r--   0 root         (0) root         (0)     3118 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifair100.py
--rw-r--r--   0 root         (0) root         (0)     3447 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifar10.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifar100.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cub200.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/em_3d.py
--rw-r--r--   0 root         (0) root         (0)     3698 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/food101.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/horse2zebra.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/imdb_review.py
--rw-r--r--   0 root         (0) root         (0)     4488 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/medmnist.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mendeley.py
--rw-r--r--   0 root         (0) root         (0)     4039 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mitmovie_ner.py
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mnist.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/montgomery.py
--rw-r--r--   0 root         (0) root         (0)    12377 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mscoco.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/nih_chestxray.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/omniglot.py
--rw-r--r--   0 root         (0) root         (0)     9767 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/pascal_voc.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/penn_treebank.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/shakespeare.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/skl_digits.py
--rw-r--r--   0 root         (0) root         (0)     6097 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/svhn.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/svhn_cropped.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/tednmt.py
--rw-r--r--   0 root         (0) root         (0)     4183 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/tiny_imagenet.py
--rw-r--r--   0 root         (0) root         (0)     5324 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/usps.py
--rw-r--r--   0 root         (0) root         (0)    20504 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    26711 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3599 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10094 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/op_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     9011 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/siamese_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    32466 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.571852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.571852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)     1200 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     6553 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.571852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)     1370 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/reflection_padding_2d.py
--rw-r--r--   0 root         (0) root         (0)    52739 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/network.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.571852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.575852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.575852 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)     5847 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.587851 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)     5956 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7544 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/affine.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/center_crop.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/crop.py
--rw-r--r--   0 root         (0) root         (0)     5041 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     4920 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     4302 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/flip.py
--rw-r--r--   0 root         (0) root         (0)     4555 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     4807 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/multivariate.py
--rw-r--r--   0 root         (0) root         (0)     4654 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     5222 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_crop.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     5091 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     4294 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_scale.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     5023 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/read_mat.py
--rw-r--r--   0 root         (0) root         (0)     4755 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/resize.py
--rw-r--r--   0 root         (0) root         (0)     5430 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/rotate.py
--rw-r--r--   0 root         (0) root         (0)     6186 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/transpose.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)    16402 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.611850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)    10320 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/binarize.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/blur.py
--rw-r--r--   0 root         (0) root         (0)     3497 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/brightness.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/calibate.py
--rw-r--r--   0 root         (0) root         (0)     2501 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2580 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/clahe.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/color.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/contrast.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/downscale.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/equalize.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/from_float.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/hadamard.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/median_blur.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/minmax.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2978 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/normalize.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/onehot.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/posterize.py
--rw-r--r--   0 root         (0) root         (0)     3022 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_rain.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     5438 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_snow.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/read_image.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/rua.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/sharpness.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/shear_x.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/solarize.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_array.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_float.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_gray.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/tokenize.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/translate_x.py
--rw-r--r--   0 root         (0) root         (0)     3711 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/translate_y.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/univariate.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/word_to_id.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.615850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)     2326 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/argmax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.615850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)     1226 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7214 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/cutmix_batch.py
--rw-r--r--   0 root         (0) root         (0)     4108 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/mixup_batch.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/average.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.615850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/fgsm.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/gradient.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.619850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5748 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     5174 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/dice_loss.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/focal_loss.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/hinge.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/l1_loss.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/loss.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     9186 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.623850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/fuse.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/one_of.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/repeat.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.623850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10587 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/model.py
--rw-r--r--   0 root         (0) root         (0)    12067 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/update.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/normalize.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/permute.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/resize3d.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/tensorop.py
--rw-r--r--   0 root         (0) root         (0)     4326 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)    35970 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.627850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8667 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)    10488 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.627850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5793 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/golden_section.py
--rw-r--r--   0 root         (0) root         (0)     3425 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/grid_search.py
--rw-r--r--   0 root         (0) root         (0)     9239 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.631850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/cartesian.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/heatmap.py
--rw-r--r--   0 root         (0) root         (0)     4789 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/parallel_coordinate_plot.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/vis_util.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.631850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/
--rw-r--r--   0 root         (0) root         (0)     1621 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41454 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.635850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/log_parse.py
--rw-r--r--   0 root         (0) root         (0)    33817 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/log_plot.py
--rw-r--r--   0 root         (0) root         (0)     9909 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/summary.py
--rw-r--r--   0 root         (0) root         (0)    18174 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.635850 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/nightly_util.py
--rw-r--r--   0 root         (0) root         (0)    10332 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.639849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/
--rw-r--r--   0 root         (0) root         (0)     1410 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.639849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)     1678 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3867 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.647849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/
--rw-r--r--   0 root         (0) root         (0)     2539 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7889 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     9018 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/grid_display.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/image_saver.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4974 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)    23754 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    22579 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/test_report.py
--rw-r--r--   0 root         (0) root         (0)    41953 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.647849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/meta/
--rw-r--r--   0 root         (0) root         (0)      965 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/meta/_per_ds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.655849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/
--rw-r--r--   0 root         (0) root         (0)     2419 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4100 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/accuracy.py
--rw-r--r--   0 root         (0) root         (0)     8151 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/auc.py
--rw-r--r--   0 root         (0) root         (0)    10591 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/bleu_score.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/dice.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/f1_score.py
--rw-r--r--   0 root         (0) root         (0)     5061 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/mcc.py
--rw-r--r--   0 root         (0) root         (0)    18372 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     4895 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/precision.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/recall.py
--rw-r--r--   0 root         (0) root         (0)    21156 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/trace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.659849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10667 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/eigen_cam.py
--rw-r--r--   0 root         (0) root         (0)     7808 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/grad_cam.py
--rw-r--r--   0 root         (0) root         (0)     7266 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     6905 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/label_tracker.py
--rw-r--r--   0 root         (0) root         (0)     9267 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.659849 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/types/
--rw-r--r--   0 root         (0) root         (0)     4101 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.667848 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/
--rw-r--r--   0 root         (0) root         (0)     4218 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27753 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/base_util.py
--rw-r--r--   0 root         (0) root         (0)     4225 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/cli_util.py
--rw-r--r--   0 root         (0) root         (0)     4353 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/data.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/google_download_util.py
--rw-r--r--   0 root         (0) root         (0)    31984 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/img_data.py
--rw-r--r--   0 root         (0) root         (0)     8260 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/latex_util.py
--rw-r--r--   0 root         (0) root         (0)    58364 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/util.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.667848 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/xai/
--rw-r--r--   0 root         (0) root         (0)     1030 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12171 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator/xai/saliency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.787844 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-30 13:54:16.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35224 2023-06-30 13:54:16.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 13:54:16.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-30 13:54:16.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-30 13:54:16.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-30 13:54:16.000000 fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 13:54:16.787844 fastestimator-nightly-1.6.0.dev202306301354/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4700 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.671848 fastestimator-nightly-1.6.0.dev202306301354/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.671848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.671848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.675848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_get_lr.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_save_model_load_model.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_set_lr.py
--rw-r--r--   0 root         (0) root         (0)     4617 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_update_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.675848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4980 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/test_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.679848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/dataset/test_batch_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.679848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.679848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.679848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     1975 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.679848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.679848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.683848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.683848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.683848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
--rw-r--r--   0 root         (0) root         (0)     3632 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.687848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
--rw-r--r--   0 root         (0) root         (0)    10341 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     8292 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.687848 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.691847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
--rw-r--r--   0 root         (0) root         (0)    22429 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_average.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     4149 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.695847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_arc.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)    14280 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_schedule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.695847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.695847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/visualize/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/visualize/test_visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.695847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11980 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)    17978 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/test_system.py
--rw-r--r--   0 root         (0) root         (0)    23833 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/test_estimator.py
--rw-r--r--   0 root         (0) root         (0)    28311 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/test_network.py
--rw-r--r--   0 root         (0) root         (0)    98463 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/test_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.699847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.699847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.707847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_batch_display.py
--rw-r--r--   0 root         (0) root         (0)     4498 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_best_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     7106 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_csv_logger.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_image_saver.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_image_viewer.py
--rw-r--r--   0 root         (0) root         (0)     8180 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_model_saver.py
--rw-r--r--   0 root         (0) root         (0)     4049 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_restore_wizard.py
--rw-r--r--   0 root         (0) root         (0)     3146 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_tensorboard.py
--rw-r--r--   0 root         (0) root         (0)    13603 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_test_report.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_traceability.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.711847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4671 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_accuracy.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_calibration_error.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_dice.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_f1_score.py
--rw-r--r--   0 root         (0) root         (0)     7268 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_mcc.py
--rw-r--r--   0 root         (0) root         (0)     3575 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
--rw-r--r--   0 root         (0) root         (0)     8730 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_precision.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_recall.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_eval_essential.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_test_essential.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_trace.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_train_essential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.711847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/
--rw-r--r--   0 root         (0) root         (0)      702 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9440 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
--rw-r--r--   0 root         (0) root         (0)     8956 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/test_label_tracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.711847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/test_img_data.py
--rw-r--r--   0 root         (0) root         (0)    11100 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.715847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.715847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.715847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.719847 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.735846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_abs.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_argmax.py
--rw-r--r--   0 root         (0) root         (0)     6396 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_binary_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_cast.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_check_nan.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_clip_by_value.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_concat.py
--rw-r--r--   0 root         (0) root         (0)     8362 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_dice_score.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_exp.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_feed_forward.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_gather.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_gather_from_batch.py
--rwxr-xr-x   0 root         (0) root         (0)     3742 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_get_gradient.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_get_image_dims.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_hinge.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_iwd.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_lambertw.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_matmul.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_maximum.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_mean_squared_error.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_ones_like.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_percentile.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_permute.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_pow.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_random_normal_like.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_random_uniform_like.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_max.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_mean.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_min.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_std.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_sum.py
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_roll.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_sign.py
--rw-r--r--   0 root         (0) root         (0)     3534 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
--rw-r--r--   0 root         (0) root         (0)     2305 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_squeeze.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_pow.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_round.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_sqrt.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_to_shape.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_to_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_to_type.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_watch.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_where.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_zeros_like.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_zscore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.735846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/cli/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/cli/test_cli_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.739846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_batch_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_combine_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_csv_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_data.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_extend_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_generator_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13000 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_numpy_dataset.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_pickle_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.739846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.739846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.743846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.743846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.743846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/loss/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/loss/test_focal_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.743846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.743846 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)     5323 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.755845 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2057 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/test_numpyop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.771844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
--rw-r--r--   0 root         (0) root         (0)     2644 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
--rw-r--r--   0 root         (0) root         (0)     2021 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.771844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.771844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/augmentation/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.775844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
--rw-r--r--   0 root         (0) root         (0)     7142 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
--rw-r--r--   0 root         (0) root         (0)     5434 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/test_normalize.py
--rw-r--r--   0 root         (0) root         (0)     3686 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/test_resize3d.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/test_tensorop.py
--rw-r--r--   0 root         (0) root         (0)     2279 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/test_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.775844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/test_lr_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1188 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.779844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/test_golden_section_search.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/test_grid_search.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/test_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.779844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.779844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/logs/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/logs/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/test_history.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/test_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.779844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/test/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/test/test_unittest_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.779844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.783844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/test_auc_score.py
--rw-r--r--   0 root         (0) root         (0)     3591 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/test_bleu_score.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.783844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/types/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/types/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.783844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_data.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_traceability_util.py
--rw-r--r--   0 root         (0) root         (0)    19505 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_util.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_wget_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:54:16.783844 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/xai/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/xai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/xai/test_saliency.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-06-30 13:46:04.000000 fastestimator-nightly-1.6.0.dev202306301354/test/run_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.102642 fastestimator-nightly-1.6.0.dev202307151357/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-07-15 13:49:41.000000 fastestimator-nightly-1.6.0.dev202307151357/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-15 13:57:48.102642 fastestimator-nightly-1.6.0.dev202307151357/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6271 2023-07-15 13:49:41.000000 fastestimator-nightly-1.6.0.dev202307151357/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.878650 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.878650 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.878650 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7452 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/unet.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.882650 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/lenet.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/unet.py
+-rw-r--r--   0 root         (0) root         (0)     5580 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.902649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/
+-rw-r--r--   0 root         (0) root         (0)    10420 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     4853 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_cast.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_concat.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_convert_tensor_precision.py
+-rw-r--r--   0 root         (0) root         (0)     7866 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_flip.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_gather_from_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_shape.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_huber.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     4558 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4323 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_roll.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_save_model.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_smooth_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     5742 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_update_model.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_watch.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_where.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.902649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/history.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/logs.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     6574 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.910649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16450 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/combined_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/csv_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.918649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifair10.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifair100.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifar10.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifar100.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cub200.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/em_3d.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/food101.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/horse2zebra.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/imdb_review.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/medmnist.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mendeley.py
+-rw-r--r--   0 root         (0) root         (0)     4039 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mitmovie_ner.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mnist.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/montgomery.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mscoco.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/nih_chestxray.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/omniglot.py
+-rw-r--r--   0 root         (0) root         (0)     9767 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/pascal_voc.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/penn_treebank.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/shakespeare.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/skl_digits.py
+-rw-r--r--   0 root         (0) root         (0)     6097 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/svhn.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/svhn_cropped.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/tednmt.py
+-rw-r--r--   0 root         (0) root         (0)     4183 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/tiny_imagenet.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/usps.py
+-rw-r--r--   0 root         (0) root         (0)    20743 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    26711 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3599 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10140 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/op_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     9011 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/siamese_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    33059 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.918649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.918649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.922649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/reflection_padding_2d.py
+-rw-r--r--   0 root         (0) root         (0)    55423 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/network.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.922649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.922649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.922649 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5847 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.934648 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7544 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/affine.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/crop.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     4302 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/flip.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     4807 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/multivariate.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     5091 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/read_mat.py
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/resize.py
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     6186 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/transpose.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)    16598 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.950647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)    10320 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/binarize.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/blur.py
+-rw-r--r--   0 root         (0) root         (0)     3497 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/brightness.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/calibate.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/clahe.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/color.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/equalize.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/from_float.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/onehot.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/posterize.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/read_image.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/rua.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/solarize.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/univariate.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/word_to_id.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.954647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/argmax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.954647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7214 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/cutmix_batch.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/mixup_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/average.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.958647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/gradient.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.958647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/dice_loss.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/focal_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/hinge.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/loss.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     9186 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.962647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/fuse.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/one_of.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.962647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10480 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/model.py
+-rw-r--r--   0 root         (0) root         (0)    12067 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/update.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/permute.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     5991 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)    36605 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.962647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8667 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)    10488 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.966647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/golden_section.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     9239 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.966647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/cartesian.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)     4789 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/parallel_coordinate_plot.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/vis_util.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.970647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/slicer/
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/slicer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/slicer/axis_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/slicer/mean_unslicer.py
+-rw-r--r--   0 root         (0) root         (0)    10974 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/slicer/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    13977 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/slicer/sliding_slicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.970647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41454 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.974647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/log_parse.py
+-rw-r--r--   0 root         (0) root         (0)    33817 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/log_plot.py
+-rw-r--r--   0 root         (0) root         (0)     9909 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/summary.py
+-rw-r--r--   0 root         (0) root         (0)    18385 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.974647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/nightly_util.py
+-rw-r--r--   0 root         (0) root         (0)    10332 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.974647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.978647 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.982646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     9018 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/grid_display.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4974 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)    23746 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    22579 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/test_report.py
+-rw-r--r--   0 root         (0) root         (0)    43469 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.982646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/meta/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/meta/_per_ds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.986646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/auc.py
+-rw-r--r--   0 root         (0) root         (0)    10591 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/bleu_score.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/dice.py
+-rw-r--r--   0 root         (0) root         (0)     4950 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/mcc.py
+-rw-r--r--   0 root         (0) root         (0)    18372 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/precision.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/recall.py
+-rw-r--r--   0 root         (0) root         (0)    21156 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/trace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.990646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10667 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/eigen_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7808 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/grad_cam.py
+-rw-r--r--   0 root         (0) root         (0)     7266 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/label_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.990646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/types/
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.994646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/
+-rw-r--r--   0 root         (0) root         (0)     4218 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27829 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/base_util.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/cli_util.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/data.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/google_download_util.py
+-rw-r--r--   0 root         (0) root         (0)    31984 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/img_data.py
+-rw-r--r--   0 root         (0) root         (0)     8260 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/latex_util.py
+-rw-r--r--   0 root         (0) root         (0)    58481 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    19812 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/util.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.998646 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/xai/
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12171 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator/xai/saliency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.102642 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-15 13:57:47.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35887 2023-07-15 13:57:47.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 13:57:47.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-15 13:57:47.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-15 13:57:47.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-15 13:57:47.000000 fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 13:57:48.102642 fastestimator-nightly-1.6.0.dev202307151357/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4700 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.998646 fastestimator-nightly-1.6.0.dev202307151357/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.998646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:47.998646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.002646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_get_lr.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_save_model_load_model.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_set_lr.py
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_update_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.002646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/test_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.002646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/dataset/test_batch_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.002646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.002646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.006646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.006646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.006646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.006646 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.010645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.010645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.010645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py
+-rw-r--r--   0 root         (0) root         (0)    10341 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     8292 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.014645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.014645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/test_modelop.py
+-rw-r--r--   0 root         (0) root         (0)    22429 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/test_updateop.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_average.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.018645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_arc.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    14280 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_repeat_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_schedule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.018645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.018645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/visualize/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/visualize/test_visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.018645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/slicer/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/slicer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/slicer/test_axis_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/slicer/test_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     4719 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/slicer/test_sliding_slicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.018645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)    17978 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/test_system.py
+-rw-r--r--   0 root         (0) root         (0)    23833 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/test_estimator.py
+-rw-r--r--   0 root         (0) root         (0)    28311 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/test_network.py
+-rw-r--r--   0 root         (0) root         (0)    98463 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/test_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.022645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.022645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_early_stopping.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.026645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_batch_display.py
+-rw-r--r--   0 root         (0) root         (0)     4498 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_best_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_csv_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_image_saver.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_image_viewer.py
+-rw-r--r--   0 root         (0) root         (0)     8180 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_model_saver.py
+-rw-r--r--   0 root         (0) root         (0)     4049 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_restore_wizard.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_tensorboard.py
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_test_report.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_traceability.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.030645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_accuracy.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_calibration_error.py
+-rw-r--r--   0 root         (0) root         (0)     8046 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_dice.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_f1_score.py
+-rw-r--r--   0 root         (0) root         (0)     7268 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_mcc.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_precision.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_recall.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_eval_essential.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_test_essential.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_train_essential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.030645 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9440 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/test_instance_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/test_label_tracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.034644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/test_img_data.py
+-rw-r--r--   0 root         (0) root         (0)    11100 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.034644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.034644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.034644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.038644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_unet.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.050644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_abs.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_argmax.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_binary_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_cast.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_check_nan.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_clip_by_value.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_concat.py
+-rw-r--r--   0 root         (0) root         (0)     8362 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_dice_score.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_exp.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_feed_forward.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_gather_from_batch.py
+-rwxr-xr-x   0 root         (0) root         (0)     3742 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_get_gradient.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_get_image_dims.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_hinge.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_iwd.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_lambertw.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_maximum.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_mean_squared_error.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_ones_like.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_percentile.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_permute.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_random_normal_like.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_random_uniform_like.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_max.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_mean.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_min.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_std.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_sum.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_roll.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_sign.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_squeeze.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_pow.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_round.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_sqrt.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_to_shape.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_to_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_to_type.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_watch.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_where.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_zeros_like.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_zscore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.054644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/cli/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/cli/test_cli_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.054644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_batch_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_combine_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_csv_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_extend_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_generator_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13000 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_numpy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_pickle_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.058644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.058644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/test_hadamard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.058644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.058644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.058644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/loss/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/loss/test_focal_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.058644 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.062643 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)     5323 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.070643 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/test_numpyop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.086643 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_color.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.090642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.090642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/augmentation/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.090642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py
+-rw-r--r--   0 root         (0) root         (0)     7142 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/test_normalize.py
+-rw-r--r--   0 root         (0) root         (0)     3686 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/test_resize3d.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/test_tensorop.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/test_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.090642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/test_epoch_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/test_lr_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/test_repeat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.094642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/test_golden_section_search.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/test_grid_search.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/test_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.094642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/slicer/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/slicer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7315 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/slicer/test_axis_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/slicer/test_mean_slicer.py
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/slicer/test_slicer.py
+-rw-r--r--   0 root         (0) root         (0)    22534 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/slicer/test_sliding_slicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.094642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.098642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/logs/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/logs/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/test_history.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/test_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.098642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/test/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/test/test_unittest_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.098642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.098642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/test_auc_score.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/test_bleu_score.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.098642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/types/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/types/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.102642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_traceability_util.py
+-rw-r--r--   0 root         (0) root         (0)    19505 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_wget_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:57:48.102642 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/xai/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/xai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/xai/test_saliency.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-07-15 13:49:42.000000 fastestimator-nightly-1.6.0.dev202307151357/test/run_pr_test.py
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/LICENSE` & `fastestimator-nightly-1.6.0.dev202307151357/LICENSE`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202307151357/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.6.0.dev202306301354
+Version: 1.6.0.dev202307151357
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 License: Apache License 2.0
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/README.md` & `fastestimator-nightly-1.6.0.dev202307151357/README.md`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/lenet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/resnet9.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/pytorch/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/pytorch/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/lenet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/lenet.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Tuple
+from typing import TYPE_CHECKING, Tuple
 
 import tensorflow as tf
-from tensorflow.keras import Sequential, layers
+
+if TYPE_CHECKING:
+    from tensorflow.python.keras import Sequential, layers
+else:
+    from tensorflow.keras import Sequential, layers
 
 
 # noinspection PyPep8Naming
 def LeNet(input_shape: Tuple[int, int, int] = (28, 28, 1), classes: int = 10) -> tf.keras.Model:
     """A standard LeNet implementation in TensorFlow.
 
     The LeNet model has 3 convolution layers and 2 dense layers.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/resnet9.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/architecture/tensorflow/wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/architecture/tensorflow/wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_abs.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_sign.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,45 +17,45 @@
 import numpy as np
 import tensorflow as tf
 import torch
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor, np.ndarray)
 
 
-def abs(tensor: Tensor) -> Tensor:
-    """Compute the absolute value of a tensor.
+def sign(tensor: Tensor) -> Tensor:
+    """Compute the sign of a tensor.
 
     This method can be used with Numpy data:
     ```python
     n = np.array([-2, 7, -19])
-    b = fe.backend.abs(n)  # [2, 7, 19]
+    b = fe.backend.sign(n)  # [-1, 1, -1]
     ```
 
     This method can be used with TensorFlow tensors:
     ```python
     t = tf.constant([-2, 7, -19])
-    b = fe.backend.abs(t)  # [2, 7, 19]
+    b = fe.backend.sign(t)  # [-1, 1, -1]
     ```
 
     This method can be used with PyTorch tensors:
     ```python
     p = torch.tensor([-2, 7, -19])
-    b = fe.backend.abs(p)  # [2, 7, 19]
+    b = fe.backend.sign(p)  # [-1, 1, -1]
     ```
 
     Args:
         tensor: The input value.
 
     Returns:
-        The absolute value of `tensor`.
+        The sign of each value of the `tensor`.
 
     Raises:
         ValueError: If `tensor` is an unacceptable data type.
     """
     if tf.is_tensor(tensor):
-        return tf.abs(tensor)
+        return tf.sign(tensor)
     elif isinstance(tensor, torch.Tensor):
-        return torch.abs(tensor)
+        return tensor.sign()
     elif isinstance(tensor, np.ndarray):
-        return np.abs(tensor)
+        return np.sign(tensor)
     else:
         raise ValueError("Unrecognized tensor type {}".format(type(tensor)))
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_argmax.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_cast.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_check_nan.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_concat.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_convert_tensor_precision.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_convert_tensor_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_dice_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_exp.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_gather.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_lr.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_get_shape.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_get_shape.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import TypeVar
+from typing import Tuple
 
 import numpy as np
 import tensorflow as tf
 import torch
 
-Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor, np.ndarray)
+from fastestimator.types import Array
 
 
-def get_shape(tensor: Tensor) -> Tensor:
+def get_shape(tensor: Array) -> Tuple[int, ...]:
     """Find shape of a given `tensor`.
 
     This method can be used with Numpy data:
     ```python
     n = np.array([[[0, 1], [2, 3]], [[4, 5], [6, 7]], [[8, 9], [10, 11]]])
     b = fe.backend.get_shape(n)  # [3,2,2]
     ```
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_hinge.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_huber.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_huber.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_iwd.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_lambertw.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_load_model.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_matmul.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_maximum.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_ones_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_percentile.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_permute.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_pow.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_reshape.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_resize3d.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_roll.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_save_model.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_save_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_set_lr.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_sign.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_transpose.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,45 +17,45 @@
 import numpy as np
 import tensorflow as tf
 import torch
 
 Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor, np.ndarray)
 
 
-def sign(tensor: Tensor) -> Tensor:
-    """Compute the sign of a tensor.
+def transpose(tensor: Tensor) -> Tensor:
+    """Transpose the `tensor`.
 
     This method can be used with Numpy data:
     ```python
-    n = np.array([-2, 7, -19])
-    b = fe.backend.sign(n)  # [-1, 1, -1]
+    n = np.array([[0,1,2],[3,4,5],[6,7,8]])
+    b = fe.backend.transpose(n)  # [[0, 3, 6], [1, 4, 7], [2, 5, 8]]
     ```
 
     This method can be used with TensorFlow tensors:
     ```python
-    t = tf.constant([-2, 7, -19])
-    b = fe.backend.sign(t)  # [-1, 1, -1]
+    t = tf.constant([[0,1,2],[3,4,5],[6,7,8]])
+    b = fe.backend.transpose(t)  # [[0, 3, 6], [1, 4, 7], [2, 5, 8]]
     ```
 
     This method can be used with PyTorch tensors:
     ```python
-    p = torch.tensor([-2, 7, -19])
-    b = fe.backend.sign(p)  # [-1, 1, -1]
+    p = torch.tensor([[0,1,2],[3,4,5],[6,7,8]])
+    b = fe.backend.transpose(p)  # [[0, 3, 6], [1, 4, 7], [2, 5, 8]]
     ```
 
     Args:
         tensor: The input value.
 
     Returns:
-        The sign of each value of the `tensor`.
+        The transposed `tensor`.
 
     Raises:
         ValueError: If `tensor` is an unacceptable data type.
     """
     if tf.is_tensor(tensor):
-        return tf.sign(tensor)
+        return tf.transpose(tensor)
     elif isinstance(tensor, torch.Tensor):
-        return tensor.sign()
+        return tensor.T
     elif isinstance(tensor, np.ndarray):
-        return np.sign(tensor)
+        return np.transpose(tensor)
     else:
         raise ValueError("Unrecognized tensor type {}".format(type(tensor)))
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_smooth_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_smooth_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_squeeze.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_to_shape.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_to_tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,41 +8,56 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Collection, TypeVar, Union, overload
+from typing import Collection, Literal, Union, overload
 
 import numpy as np
 import tensorflow as tf
 import torch
 
-Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor, np.ndarray)
-CollectionT = TypeVar('CollectionT', bound=Collection)
+from fastestimator.types import Array, ArrayT, CollectionT
 
 
 @overload
 def to_tensor(data: CollectionT, target_type: str, shared_memory: bool = False) -> CollectionT:
     ...
 
 
 @overload
-def to_tensor(data: Union[Tensor, float, int], target_type: str, shared_memory: bool = False) -> Tensor:
+def to_tensor(data: Union[Array, float, int], target_type: Literal['tf'], shared_memory: bool = False) -> tf.Tensor:
+    ...
+
+
+@overload
+def to_tensor(data: Union[Array, float, int], target_type: Literal['torch'],
+              shared_memory: bool = False) -> torch.Tensor:
+    ...
+
+
+@overload
+def to_tensor(data: Union[Array, float, int], target_type: Literal['np'], shared_memory: bool = False) -> np.ndarray:
+    ...
+
+
+@overload
+def to_tensor(data: Union[Array, float, int], target_type: str, shared_memory: bool = False) -> Array:
     ...
 
 
 @overload
 def to_tensor(data: None, target_type: str, shared_memory: bool = False) -> None:
     ...
 
 
-def to_tensor(data: Union[Collection, Tensor, float, int, None], target_type: str,
-              shared_memory: bool = False) -> Union[Collection, Tensor, None]:
+def to_tensor(data: Union[Collection, Array, float, int, None], target_type: str,
+              shared_memory: bool = False) -> Union[Collection, ArrayT, Array, None]:
     """Convert tensors within a collection of `data` to a given `target_type` recursively.
 
     This method can be used with Numpy data:
     ```python
     data = {"x": np.ones((10,15)), "y":[np.ones((4)), np.ones((5, 3))], "z":{"key":np.ones((2,2))}}
     t = fe.backend.to_tensor(data, target_type='tf')
     # {"x": <tf.Tensor>, "y":[<tf.Tensor>, <tf.Tensor>], "z": {"key": <tf.Tensor>}}
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_to_type.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_update_model.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_watch.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_where.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/backend/_zscore.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/backend/_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/history.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/logs.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/logs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/main.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/plot.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/run.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/run.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/cli/train.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/cli/train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/combined_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/combined_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/csv_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             output is a boolean (include_if=lambda mode: mode in ['eval', 'test']). This last option is very flexible,
             but also slower to execute.
         fill_na: A fill value if data is missing. By default, this will follow pandas convention and use different types
             of NaNs.
         kwargs: Other arguments to be passed through to pandas csv reader function. See the pandas docs for details:
             https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html.
     """
-
     def __init__(self,
                  file_path: str,
                  delimiter: str = ",",
                  include_if: Union[None, Dict[str, Union[Any, Iterable[Any]]], str, Callable[..., bool]] = None,
                  fill_na: Optional[Any] = 'pandas_default',
                  **kwargs) -> None:
         df = pd.read_csv(file_path, delimiter=delimiter, **kwargs)
@@ -72,8 +71,11 @@
                     if col not in df.columns:
                         raise ValueError(f"The provided filter function requested '{col}' which was not found in the "
                                          f"csv columns: {list(df.columns)}")
                 df = df[df[cols].apply(lambda row: include_if(**row), axis=1)]
             else:
                 raise ValueError(f"Received an unexpected datatype for include_if: {type(include_if)}")
         self.parent_path = os.path.dirname(file_path)
+        # Remove banned characters from column names since users won't be able to access them later. This can happen,
+        # for example, when a csv file is missing one or more headers (which would normally then render as "Unnamed: 1")
+        df.rename(lambda x: x.replace(":", "").replace("|", "").replace(";", ""), axis='columns', inplace=True)
         super().__init__(df.to_dict(orient='index'))
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/breast_cancer.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifair10.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifair10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifair100.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifair100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifar10.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifar10.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cifar100.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cifar100.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/cub200.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/cub200.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/em_3d.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/em_3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -68,24 +68,24 @@
     """
     encoded_label = np.zeros(label_data.shape[:-1], np.uint8)
     for i, value in color_mapping.items():
         encoded_label[np.all(label_data == value, axis=-1)] = i
     return encoded_label
 
 
-def load_data(root_dir: Optional[str] = None, image_key: str = "image",
-              label_key: str = "label") -> Tuple[NumpyDataset, NumpyDataset]:
+def load_data(root_dir: Optional[str] = None, image_key: str = "image", label_key: str = "label",
+              tile: bool = True) -> Tuple[NumpyDataset, NumpyDataset]:
     """Load and return the 3d electron microscope platelet dataset.
 
 
     Sourced from https://bio3d-vision.github.io/platelet-description.
     Electronic Microscopy 3D cell dataset, consists of 2 3D images, one 800x800x50 and the other 800x800x24.
-    The 800x800x50 is used as training dataset and 800x800x24 is used for validation. Instead of using the entire
-    800x800 images, the 800x800x50 is tiled into 256x256x24 tiles with an overlap of 128 producing around 75 training
-    images and similarly the 800x800x24 image is tiled to produce 25 validation images.
+    The 800x800x50 is used as training dataset and 800x800x24 is used for validation. If `tile` is True, then instead
+    of using the entire 800x800 images, the 800x800x50 is tiled into 256x256x24 tiles with an overlap of 128 producing
+    around 75 training images and similarly the 800x800x24 image is tiled to produce 25 validation images.
 
     The method downloads the dataset from google drive and provides train and validation NumpyDataset.
     While the dataset contains encoded value 0 as background, its omitted in the one hot encoded class label provided
     by this method. Below indexes represent the labels in channel layer.
         Index	Class name
         0		Cell
         1		Mitochondria
@@ -95,14 +95,15 @@
         5		Dense granule core
 
     Args:
         root_dir: The path to store the downloaded data. When `path` is not provided,
             the data will be saved into `fastestimator_data` under the user's home directory.
         image_key: The key for image.
         label_key: The key for label.
+        tile: Whether to tile the image into multiple smaller images, or to return the individual volumes directly.
 
     Returns:
         (train_data, eval_data)
     """
     home = str(Path.home())
 
     if root_dir is None:
@@ -121,25 +122,38 @@
     val_data = tifffile.imread(os.path.join(root_dir, 'platelet-em/images/24-images.tif'))
     train_label_data = tifffile.imread(os.path.join(root_dir, 'platelet-em/labels-semantic/50-semantic.tif'))
     val_label_data = tifffile.imread(os.path.join(root_dir, 'platelet-em/labels-semantic/24-semantic.tif'))
 
     encoded_train_label = get_encode_label(train_label_data)
     encoded_val_label = get_encode_label(val_label_data)
 
+    if not tile:
+        train_data = np.expand_dims(np.moveaxis(train_data, 0, -1), 0)
+        train_labels = np.expand_dims(np.moveaxis(encoded_train_label, 0, -1), 0)
+        train_labels = np.eye(7, dtype=np.float32)[train_labels].take(indices=range(1, 7), axis=-1)
+
+        val_data = np.expand_dims(np.moveaxis(val_data, 0, -1), 0)
+        val_labels = np.expand_dims(np.moveaxis(encoded_val_label, 0, -1), 0)
+        val_labels = np.eye(7, dtype=np.float32)[val_labels].take(indices=range(1, 7), axis=-1)
+
+        train_data = NumpyDataset({image_key: train_data, label_key: train_labels})
+        eval_data = NumpyDataset({image_key: val_data, label_key: val_labels})
+        return train_data, eval_data
+
     train_data_slices = [train_data[0:24], train_data[13:37], train_data[26:50]]
     train_label_slices = [encoded_train_label[0:24], encoded_train_label[13:37], encoded_train_label[26:50]]
 
     training_data_tiles = np.moveaxis(
         np.concatenate([generate_tiles(slice_data) for slice_data in train_data_slices], axis=0), 1, -1)
     training_label_tiles = np.moveaxis(
         np.concatenate([generate_tiles(slice_data) for slice_data in train_label_slices], axis=0), 1, -1)
 
     val_data_tiles = np.moveaxis(generate_tiles(val_data), 1, -1)
     val_label_tiles = np.moveaxis(generate_tiles(encoded_val_label), 1, -1)
 
-    val_label_tiles = np.eye(7)[val_label_tiles].take(indices=range(1, 7), axis=-1)
-    training_label_tiles = np.eye(7)[training_label_tiles].take(indices=range(1, 7), axis=-1)
+    val_label_tiles = np.eye(7, dtype=np.float32)[val_label_tiles].take(indices=range(1, 7), axis=-1)
+    training_label_tiles = np.eye(7, dtype=np.float32)[training_label_tiles].take(indices=range(1, 7), axis=-1)
 
     train_data = NumpyDataset({image_key: training_data_tiles, label_key: training_label_tiles})
     eval_data = NumpyDataset({image_key: val_data_tiles, label_key: val_label_tiles})
 
     return train_data, eval_data
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/food101.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/food101.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/horse2zebra.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/horse2zebra.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/imdb_review.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/imdb_review.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/medmnist.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/medmnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mendeley.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mendeley.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mitmovie_ner.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mitmovie_ner.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mnist.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mnist.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/montgomery.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/montgomery.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/mscoco.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/mscoco.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/nih_chestxray.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/nih_chestxray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/omniglot.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/omniglot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/pascal_voc.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/penn_treebank.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/penn_treebank.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/shakespeare.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/shakespeare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/skl_digits.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/skl_digits.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/svhn.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/svhn.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/svhn_cropped.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/svhn_cropped.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/tednmt.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/tednmt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/tiny_imagenet.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/data/usps.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/data/usps.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/dataloader.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import functools
 import random
 from abc import ABC
-from typing import Any, Callable, Dict, List, Optional, Sized, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Protocol, Sized, Tuple, Union
 
 import numpy as np
 from torch import Tensor
 from torch.utils.data import DataLoader, Sampler, _DatasetKind
 from torch.utils.data._utils.collate import default_collate, default_convert
 from torch.utils.data._utils.fetch import _MapDatasetFetcher
 from torch.utils.data.dataloader import _BaseDataLoaderIter, _MultiProcessingDataLoaderIter, \
     _SingleProcessDataLoaderIter
 
 from fastestimator.dataset.extend_dataset import ExtendDataset
 from fastestimator.dataset.op_dataset import OpDataset
-from fastestimator.types import MapDataset
-from fastestimator.types import FilteredData
+from fastestimator.types import FilteredData, MapDataset
 from fastestimator.util.util import Suppressor
 
 
+class PostProcessFunction(Protocol):
+    def __call__(self, data: Dict[str, Any], shared: bool = True) -> Union[Dict[str, Any], FilteredData]:
+        ...
+
+
 class FEDataLoader(DataLoader):
     """A Data Loader that can handle filtering data.
 
     This class is intentionally not @traceable.
 
     Args:
         dataset: The dataset to be drawn from. The dataset may optionally implement .fe_reset_ds(bool) and/or
@@ -62,15 +66,15 @@
     FE_LOADER_KIND = 7
 
     # The typing for 'dataset' should be an 'and' rather than 'or' but that feature is still under development:
     # https://github.com/python/typing/issues/213
 
     def __init__(self,
                  dataset: MapDataset,
-                 postprocess_fn: Optional[Callable[[Dict[str, Any]], Union[Dict[str, Any], FilteredData]]] = None,
+                 postprocess_fn: Optional[PostProcessFunction] = None,
                  batch_size: Optional[int] = 1,
                  steps_per_epoch: Optional[int] = None,
                  shuffle: bool = False,
                  num_workers: int = 0,
                  collate_fn: Optional[Callable] = None,
                  drop_last: bool = False):
         reset_fn = dataset.fe_reset_ds if hasattr(dataset, 'fe_reset_ds') else None
@@ -271,15 +275,16 @@
     if not real_batch or (self.fe_drop_last and len(real_batch) < self.fe_batch_size):
         self.fe_extra_data.clear()  # Throw out any extra data
         raise StopIteration
     # Collate the batch
     collated = self.fe_collate_fn(real_batch)
     # Apply any batch-level operations
     if self.fe_postprocess_fn is not None:
-        collated = self.fe_postprocess_fn(collated)
+        # Don't place tensor into shared memory if it's already on the host device as this can lead to infinite lockup
+        collated = self.fe_postprocess_fn(collated, shared=False)
         if isinstance(collated, FilteredData):
             if collated.replacement:
                 self.fe_samples_yielded -= len(real_batch)
             return _next_pre_batch(self)
     return collated
 
 
@@ -310,15 +315,15 @@
                     if not instance.replacement:
                         self.fe_samples_yielded += 1
                     break
             else:
                 # The else block is reached iff the for loop never breaks (probably should never get here)
                 collated = self.fe_collate_fn(candidate_batch)
                 if self.fe_postprocess_fn is not None:
-                    collated = self.fe_postprocess_fn(collated)
+                    collated = self.fe_postprocess_fn(collated, shared=False)
                     if isinstance(collated, FilteredData):
                         if not collated.replacement:
                             self.fe_samples_yielded += 1
                         return _next_post_batch(self)
                 self.fe_samples_yielded += 1
                 return collated
     raise StopIteration
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/op_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/op_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,16 @@
     @classmethod
     def handle_warning(cls, candidates: Set[str]) -> None:
         """A function which prints warning messages about unused keys if such messages haven't already been printed.
 
         Args:
             candidates: Unused keys which you might need to print a warning message about.
         """
+        if not candidates:
+            return
         # Keys can't contain the ":" or ";" character due to check_io_names base_util function
         warned = set((str(cls.warned.value, 'utf8') or "").split(":"))
         if ";" not in warned:
             # We use ; as a special character to indicate that the warned buffer was overflowed by too many keys
             to_warn = candidates - warned
             if to_warn:
                 warn("The following key(s) are being pruned since they are unused outside of the "
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/dataset/siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/dataset/siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/estimator.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,63 +231,79 @@
         Args:
             eager: Whether to run the training in eager mode. This is only related to TensorFlow training because
                 PyTorch by nature is always in eager mode.
         """
         all_traces = get_current_items(self.traces_in_use, run_modes={"train", "eval"})
         sort_traces(all_traces, ds_ids=[])  # This ensures that the traces can sort properly for on_begin and on_end
         monitor_names = self.monitor_names
+        unmet_monitor_names = set(monitor_names)
         for mode in self.pipeline.get_modes() - {"test"}:
             scheduled_items = self.pipeline.get_scheduled_items(mode) + self.network.get_scheduled_items(
                 mode) + self.get_scheduled_items(mode)
             signature_epochs = get_signature_epochs(scheduled_items, self.system.total_epochs, mode=mode)
             epochs_with_data = self.pipeline.get_epochs_with_data(total_epochs=self.system.total_epochs, mode=mode)
             for epoch in signature_epochs:
                 if epoch not in epochs_with_data:
                     continue
                 ds_ids = self.pipeline.get_ds_ids(epoch, mode)
                 for ds_id in ds_ids:
-                    network_output_keys = self.network.get_all_output_keys(mode, epoch, ds_id=ds_id)
-                    network_input_keys = self.network.get_effective_input_keys(mode, epoch, ds_id=ds_id)
                     trace_input_keys = set()
                     trace_output_keys = {"*"}
                     traces = get_current_items(self.traces_in_use, run_modes=mode, epoch=epoch, ds_id=ds_id)
                     for idx, trace in enumerate(traces):
-                        if idx > 0:  # ignore TrainEssential and EvalEssential's inputs for unmet requirement checking
+                        if idx == 0:
+                            # Trace 0 is either TrainEssential or EvalEssential. Their inputs are the keys which should
+                            # be monitored, which is a union of self.monitor_names and potentially other keys which were
+                            # found when looping through traces to look for fe_monitor_names.
+                            monitor_names.update(trace.inputs)
+                        else:
+                            # We want to ignore monitor_names for for unmet requirement checking
                             trace_input_keys.update(trace.inputs)
                         trace_output_keys.update(trace.get_outputs(ds_ids=ds_ids))
-                    # key checking
-                    with self.pipeline(mode=mode,
-                                       epoch=epoch,
-                                       ds_id=ds_id,
-                                       steps_per_epoch=None,
-                                       output_keys=trace_input_keys - network_output_keys
-                                       | network_input_keys) as loader:
-                        loader = self._configure_loader(loader)
-                        if isinstance(loader, tf.data.Dataset):
-                            batch = list(loader.take(1))[0]
-                        else:
-                            with Suppressor(allow_pyprint=True, show_if_exception=True):
-                                # TF multi-gpu print-spams here in version 2.11
-                                batch = next(iter(loader))
-                        batch = self._configure_tensor(loader, batch)
-                    assert isinstance(batch, dict), "please make sure data output format is dictionary"
-                    pipeline_output_keys = to_set(batch.keys())
-
-                    monitor_names = monitor_names - (pipeline_output_keys | network_output_keys)
-                    unmet_requirements = trace_input_keys - (pipeline_output_keys | network_output_keys
-                                                             | trace_output_keys)
-                    assert not unmet_requirements, \
-                        "found missing key(s) during epoch {} mode {} ds_id {}: {}".format(epoch, mode, ds_id,
-                                                                                           unmet_requirements)
-                    sort_traces(traces, ds_ids=ds_ids, available_outputs=pipeline_output_keys | network_output_keys)
-                    trace_input_keys.update(traces[0].inputs)
-                    self.network.load_epoch(mode, epoch, ds_id, output_keys=trace_input_keys, warmup=True, eager=eager)
-                    self.network.run_step(batch)
-                    self.network.unload_epoch()
-        assert not monitor_names, "found missing key(s): {}".format(monitor_names)
+
+                    with self.network(mode=mode,
+                                      epoch=epoch,
+                                      ds_id=ds_id,
+                                      desired_output_keys=trace_input_keys | monitor_names,
+                                      warmup=True,
+                                      eager=eager):
+
+                        network_input_keys = self.network.ctx_inputs
+                        network_output_keys = self.network.ctx_outputs
+
+                        # key checking
+                        with self.pipeline(
+                                mode=mode,
+                                epoch=epoch,
+                                ds_id=ds_id,
+                                steps_per_epoch=None,
+                                output_keys=(trace_input_keys - network_output_keys)
+                                | network_input_keys | monitor_names) as loader:
+                            loader = self._configure_loader(loader)
+                            if isinstance(loader, tf.data.Dataset):
+                                batch = list(loader.take(1))[0]
+                            else:
+                                with Suppressor(allow_pyprint=True, show_if_exception=True):
+                                    # TF multi-gpu print-spams here in version 2.11
+                                    batch = next(iter(loader))
+                            batch = self._configure_tensor(loader, batch)
+                        assert isinstance(batch, dict), \
+                            f"please make sure data output format is dictionary (got {type(batch)})"
+                        pipeline_output_keys = to_set(batch.keys())
+
+                        unmet_monitor_names = unmet_monitor_names - (pipeline_output_keys | network_output_keys)
+                        unmet_requirements = trace_input_keys - (pipeline_output_keys | network_output_keys
+                                                                 | trace_output_keys)
+                        assert not unmet_requirements, \
+                            "found missing key(s) during epoch {} mode {} ds_id {}: {}".format(epoch, mode, ds_id,
+                                                                                            unmet_requirements)
+                        sort_traces(traces, ds_ids=ds_ids, available_outputs=pipeline_output_keys | network_output_keys)
+                        trace_input_keys.update(traces[0].inputs)
+                        self.network.run_step(batch)
+        assert not unmet_monitor_names, "found missing key(s): {}".format(unmet_monitor_names)
 
     def get_scheduled_items(self, mode: str) -> List[Any]:
         """Get a list of items considered for scheduling.
 
         Args:
             mode: Current execution mode.
 
@@ -355,71 +371,71 @@
             ds_traces = get_current_items(self.traces_in_use,
                                           run_modes=self.system.mode,
                                           epoch=self.system.epoch_idx,
                                           ds_id=self.system.ds_id)
             trace_input_keys = set()
             for ds_trace in ds_traces:
                 trace_input_keys.update(ds_trace.inputs)
-            network_input_keys = self.network.get_effective_input_keys(mode=self.system.mode,
-                                                                       epoch=self.system.epoch_idx,
-                                                                       ds_id=self.system.ds_id)
-            network_output_keys = self.network.get_all_output_keys(mode=self.system.mode,
-                                                                   epoch=self.system.epoch_idx,
-                                                                   ds_id=self.system.ds_id)
-            self.network.load_epoch(mode=self.system.mode,
-                                    epoch=self.system.epoch_idx,
-                                    ds_id=self.system.ds_id,
-                                    output_keys=trace_input_keys,
-                                    eager=eager)
-
-            with self.pipeline(mode=self.system.mode,
-                               epoch=self.system.epoch_idx,
-                               ds_id=self.system.ds_id,
-                               steps_per_epoch=self.system.steps_per_epoch,
-                               output_keys=trace_input_keys - network_output_keys | network_input_keys) as loader:
-
-                if self.system.mode == 'eval':
-                    log_steps_per_epoch = math.ceil(
-                        len(loader) /
-                        loader.get_batch_size()) if not self.system.steps_per_epoch else self.system.steps_per_epoch
-                    self.system.eval_log_steps = ([
-                        1, log_steps_per_epoch // 3, (2 * log_steps_per_epoch) // 3, log_steps_per_epoch
-                    ], log_steps_per_epoch) if not self.system.eval_log_steps_request else \
-                        (self.system.eval_log_steps_request, log_steps_per_epoch)
-
-                loader = self._configure_loader(loader)
-                iterator = iter(loader)
-                with Suppressor(allow_pyprint=True, show_if_exception=True):
-                    # multi-gpu tensorflow prints a ton of complaint messages here
-                    batch = next(iterator)
-                ds_traces = sort_traces(ds_traces,
-                                        available_outputs=to_set(batch.keys()) | network_output_keys,
-                                        ds_ids=ds_ids)
-                per_ds_traces = [trace for trace in ds_traces if isinstance(trace, PerDSTrace)]
-                self._run_traces_on_ds_begin(traces=per_ds_traces)
-                while True:
-                    try:
-                        if self.system.mode == "train":
-                            self.system.update_global_step()
-                        self.system.update_batch_idx()
-                        batch = self._configure_tensor(loader, batch)
-                        self._run_traces_on_batch_begin(batch, traces=ds_traces)
-
-                        batch, prediction = self.network.run_step(batch)
-                        self._run_traces_on_batch_end(batch, prediction, traces=ds_traces)
-                        if isinstance(loader, DataLoader) and (
-                            (self.system.batch_idx == self.system.train_steps_per_epoch and self.system.mode == "train")
-                                or
-                            (self.system.batch_idx == self.system.eval_steps_per_epoch and self.system.mode == "eval")):
-                            raise StopIteration
+            # Note that monitor_names are included in the trace_inputs here, rather than being excluded and then
+            # manually union-ed again later as was done in in _warmup.
+
+            with self.network(mode=self.system.mode,
+                              epoch=self.system.epoch_idx,
+                              ds_id=self.system.ds_id,
+                              desired_output_keys=trace_input_keys,
+                              eager=eager):
+
+                network_input_keys = self.network.ctx_inputs
+                network_output_keys = self.network.ctx_outputs
+
+                with self.pipeline(mode=self.system.mode,
+                                   epoch=self.system.epoch_idx,
+                                   ds_id=self.system.ds_id,
+                                   steps_per_epoch=self.system.steps_per_epoch,
+                                   output_keys=(trace_input_keys - network_output_keys)
+                                   | network_input_keys) as loader:
+
+                    if self.system.mode == 'eval':
+                        log_steps_per_epoch = math.ceil(
+                            len(loader) /
+                            loader.get_batch_size()) if not self.system.steps_per_epoch else self.system.steps_per_epoch
+                        self.system.eval_log_steps = ([
+                            1, log_steps_per_epoch // 3, (2 * log_steps_per_epoch) // 3, log_steps_per_epoch
+                        ], log_steps_per_epoch) if not self.system.eval_log_steps_request else \
+                            (self.system.eval_log_steps_request, log_steps_per_epoch)
+
+                    loader = self._configure_loader(loader)
+                    iterator = iter(loader)
+                    with Suppressor(allow_pyprint=True, show_if_exception=True):
+                        # multi-gpu tensorflow prints a ton of complaint messages here
                         batch = next(iterator)
-                    except StopIteration:
-                        break
-                self._run_traces_on_ds_end(traces=per_ds_traces, data=end_epoch_data)
-            self.network.unload_epoch()
+                    ds_traces = sort_traces(ds_traces,
+                                            available_outputs=to_set(batch.keys()) | network_output_keys,
+                                            ds_ids=ds_ids)
+                    per_ds_traces = [trace for trace in ds_traces if isinstance(trace, PerDSTrace)]
+                    self._run_traces_on_ds_begin(traces=per_ds_traces)
+                    while True:
+                        try:
+                            if self.system.mode == "train":
+                                self.system.update_global_step()
+                            self.system.update_batch_idx()
+                            batch = self._configure_tensor(loader, batch)
+                            self._run_traces_on_batch_begin(batch, traces=ds_traces)
+                            batch = self.network.run_step(batch)
+                            self._run_traces_on_batch_end(batch, traces=ds_traces)
+                            if isinstance(loader,
+                                          DataLoader) and ((self.system.batch_idx == self.system.train_steps_per_epoch
+                                                            and self.system.mode == "train") or
+                                                           (self.system.batch_idx == self.system.eval_steps_per_epoch
+                                                            and self.system.mode == "eval")):
+                                raise StopIteration
+                            batch = next(iterator)
+                        except StopIteration:
+                            break
+                    self._run_traces_on_ds_end(traces=per_ds_traces, data=end_epoch_data)
         self._run_traces_on_epoch_end(traces=epoch_traces, data=end_epoch_data)
 
     def _configure_loader(self, loader: Union[DataLoader, tf.data.Dataset]) -> Union[DataLoader, tf.data.Dataset]:
         """A method to configure a given dataloader for use with this Estimator's Network.
 
         This method will ensure that the `loader` returns the correct data type (tf.Tensor or torch.Tensor) depending on
          the requirements of the Network. It also handles issues with multi-gpu data sharding.
@@ -533,24 +549,22 @@
             traces: List of traces.
         """
         data = Data(batch)
         for trace in traces:
             trace.on_batch_begin(data)
         self._check_early_exit()
 
-    def _run_traces_on_batch_end(self, batch: Dict[str, Any], prediction: Dict[str, Any],
-                                 traces: Iterable[Trace]) -> None:
+    def _run_traces_on_batch_end(self, batch: Dict[str, Any], traces: Iterable[Trace]) -> None:
         """Invoke the on_batch_end methods of given traces.
 
         Args:
             batch: The batch data which was provided by the pipeline.
-            prediction: The prediction data which was generated by the network.
             traces: List of traces.
         """
-        data = Data(ChainMap(prediction, batch))
+        data = Data(batch)
         for trace in traces:
             trace.on_batch_end(data)
         self._check_early_exit()
 
     def _run_traces_on_ds_end(self, traces: Iterable[PerDSTrace], data: Data) -> None:
         """Invoke the on_ds_begin methods of given traces.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/pytorch/hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/pytorch/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/instance_norm.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/layers/tensorflow/reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/layers/tensorflow/reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/network.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,236 +13,261 @@
 # limitations under the License.
 # ==============================================================================
 import gc
 import os
 import sys
 import tempfile
 from collections import ChainMap
-from typing import Any, Callable, Dict, Iterable, List, MutableMapping, Optional, Sequence, Set, Tuple, TypeVar, \
+from threading import Lock
+from typing import Any, Callable, Dict, Iterable, List, MutableMapping, Optional, Sequence, Set, Tuple, Type, TypeVar, \
     Union, overload
 
 import gdown
 import keras.mixed_precision as mixed_precision_tf
 import numpy as np
 import tensorflow as tf
 import torch
 from keras.engine.sequential import Sequential
 from keras.mixed_precision.loss_scale_optimizer import LossScaleOptimizer, LossScaleOptimizerV3
 from tensorflow.python.distribute.values import DistributedValues
+from typing_extensions import Self
 
 import fastestimator as fe
 from fastestimator.backend._load_model import load_model
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.op.numpyop import Batch, NumpyOp, RemoveIf, forward_numpyop
 from fastestimator.op.op import get_inputs_by_op, write_outputs_by_op
 from fastestimator.op.tensorop.model.update import UpdateOp
 from fastestimator.op.tensorop.tensorop import TensorOp
 from fastestimator.pipeline import Pipeline
 from fastestimator.schedule.schedule import EpochScheduler, RepeatScheduler, Scheduler, get_current_items
+from fastestimator.slicer.slicer import Slicer, forward_slicers, reverse_slicers, sanity_assert_slicers
+from fastestimator.types import Array, Model
 from fastestimator.util.base_util import NonContext, filter_nones, to_list, warn
 from fastestimator.util.traceability_util import trace_model, traceable
 from fastestimator.util.util import Suppressor, detach_tensors, get_batch_size, get_device, get_num_gpus, \
     move_tensors_to_device
 
-Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
 T = TypeVar('T')
 
 GOOGLE_DRIVE_URL = "https://drive.google.com"
 _MAC_BUILD_WARNING = False
 
 
-@traceable()
+@traceable(blacklist=('ctx_lock', ))
 class BaseNetwork:
     """A base class for Network objects.
 
     Networks are used to define the computation graph surrounding one or more models during training.
 
     Args:
         target_type: What tensor type is expected by this network ('torch' or 'tf').
         ops: The operators to be executed throughout training / testing / inference. These are likely to contain one or
             more model ops, as well as loss ops and update ops.
         postprocessing: A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been executed.
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
+        slicers: Slicers to use if you want to cut apart a single batch of data into multiple slices in order to fit
+            them onto a smaller GPU. After cutting the data apart and running through the `ops`, the samples are fused
+            back together into a single batch on the CPU before being handed over to the `pops`.
 
     Raises:
         ValueError: Mixed precision settings for all models are not the same.
     """
     def __init__(
         self,
         target_type: str,
         device: Optional[torch.device],
         ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
         postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp,
-                                                                                Scheduler[NumpyOp]]]] = None
+                                                                                Scheduler[NumpyOp]]]] = None,
+        slicers: Union[None, Slicer, Scheduler[Slicer], Sequence[Union[None, Slicer, Scheduler[Slicer]]]] = None,
     ) -> None:
         self.ops = filter_nones(to_list(ops))
         self.target_type = target_type
         self.device = device
         for op in get_current_items(self.ops):
             op.build(framework=self.target_type, device=self.device)
         self.models = to_list(_collect_models(self.ops))
+        self.mixed_precision = any([model.mixed_precision for model in self.models])
+        if self.mixed_precision and not all([model.mixed_precision for model in self.models]):
+            raise ValueError("Cannot mix full precision and mixed-precision models")
         self.postprocessing = filter_nones(to_list(postprocessing))
         for pop in self.postprocessing:
             if isinstance(pop, RemoveIf):
                 raise ValueError("Filtering is currently not supported in network post-processing")
             if isinstance(pop, Batch):
                 raise ValueError("Post-processing data is already batched, so Batch Op is not supported here.")
+        self.slicers = filter_nones(to_list(slicers))
         self._verify_inputs()
-        self.effective_inputs = dict()
-        self.effective_outputs = dict()
-        self.epoch_ops = []
-        self.epoch_postprocessing = []
-        self.epoch_models = set()
-        self.epoch_state = dict()
-        self.mixed_precision = any([model.mixed_precision for model in self.models])
-
-        if self.mixed_precision and not all([model.mixed_precision for model in self.models]):
-            raise ValueError("Cannot mix full precision and mixed-precision models")
+        # Per-Epoch/Mode/DS-ID Variables
+        self.ctx_lock = Lock()
+        self.ctx_inputs: Set[str] = set()
+        self.ctx_gpu_inputs: Set[str] = set()  # The inputs needed by TensorOps specifically
+        self.ctx_outputs: Set[str] = set()
+        self.ctx_ops: List[TensorOp] = []
+        self.ctx_postprocessing: List[NumpyOp] = []
+        self.ctx_slicers: List[Slicer] = []
+        self.ctx_models: Set[Model] = set()
+        self.ctx_state: Dict[str, Any] = dict()
 
     def _verify_inputs(self) -> None:
         """Ensure that all ops are TensorOps.
 
         Raises:
             AssertionError: If any of the ops are not TensorOps.
         """
         for op in get_current_items(self.ops):
             assert isinstance(op, TensorOp), "unsupported op format, Network ops must be TensorOps"
         for op in get_current_items(self.postprocessing):
             assert isinstance(op, NumpyOp), "unsupported op format, Network postprocessing must be NumpyOps"
+        for slicer in get_current_items(self.slicers):
+            assert isinstance(slicer, Slicer), f"unsupported slicer object detected of type: {type(slicer)}"
 
     def get_scheduled_items(self, mode: str) -> List[Any]:
         """Get a list of items considered for scheduling.
 
         Args:
             mode: Current execution mode.
 
         Returns:
             List of schedulable items in Network.
         """
         if mode == "train":
-            all_items = self.ops + [model.optimizer for model in self.models] + self.postprocessing
+            all_items = self.ops + [model.optimizer for model in self.models] + self.postprocessing + self.slicers
         else:
-            all_items = self.ops + self.postprocessing
+            all_items = self.ops + self.postprocessing + self.slicers
         return all_items
 
-    def load_epoch(self,
-                   mode: str,
-                   epoch: int,
-                   ds_id: str,
-                   output_keys: Optional[Set[str]] = None,
-                   warmup: bool = False,
-                   eager: bool = False) -> None:
-        """Prepare the network to run a given epoch and mode.
-
-        This method is necessary since schedulers and op mode restrictions may result in different computation graphs
-        every epoch.
-
-        Args:
-            mode: The mode to prepare to execute. One of 'train', 'eval', 'test', or 'infer'.
-            epoch: The epoch to prepare to execute.
-            ds_id: The current dataset id.
-            output_keys: What keys can be moved from the GPU back to the CPU after executing a step.
-            warmup: Whether to prepare to execute it warmup mode or not (end users can likely ignore this argument).
-            eager: Whether to run the training in eager mode. This is only related to TensorFlow training because
-                PyTorch by nature is always in eager mode.
-        """
-        self.effective_inputs[mode] = self.get_effective_input_keys(mode, epoch, ds_id)
-        self.effective_outputs[mode] = self.get_all_output_keys(mode, epoch, ds_id)
-        if output_keys:
-            self.effective_outputs[mode] = self.effective_outputs[mode].intersection(
-                output_keys) | self._get_effective_postprocessing_input_keys(mode, epoch, ds_id)
-        self.epoch_ops = get_current_items(self.ops, mode, epoch, ds_id=ds_id)
-        self.epoch_postprocessing = get_current_items(self.postprocessing, mode, epoch, ds_id=ds_id)
-        self.epoch_models = set.union(*[op.get_fe_models() for op in self.epoch_ops])
-        gradient_ops = [op for op in self.epoch_ops if op.fe_retain_graph() is not None]
+    def __call__(self,
+                 mode: str,
+                 epoch: int,
+                 ds_id: str,
+                 desired_output_keys: Optional[Set[str]] = None,
+                 warmup: bool = False,
+                 eager: bool = False) -> Self:
+        # Make sure that a network isn't currently instantiated with other settings
+        acquired = self.ctx_lock.acquire(blocking=False)
+        if not acquired:
+            raise ValueError("You cannot invoke a Network's __call__ method while it is already active.")
+        self.ctx_inputs, self.ctx_gpu_inputs, self.ctx_outputs = self._get_ctx_inputs_and_outputs(
+            mode, epoch, ds_id, desired_keys=desired_output_keys)
+        self.ctx_ops = get_current_items(self.ops, mode, epoch, ds_id=ds_id)
+        self.ctx_postprocessing = get_current_items(self.postprocessing, mode, epoch, ds_id=ds_id)
+        self.ctx_slicers = get_current_items(self.slicers, mode, epoch, ds_id=ds_id)
+        sanity_assert_slicers(self.ctx_slicers)
+        self.ctx_models = set.union(*[op.get_fe_models() for op in self.ctx_ops])
+        gradient_ops = [op for op in self.ctx_ops if op.fe_retain_graph() is not None]
         for idx, gradient_op in enumerate(gradient_ops):
             gradient_op.fe_retain_graph(idx != len(gradient_ops) - 1)
-        self.epoch_state = {
+        self.ctx_state = {
             "warmup": warmup,
             "mode": mode,
             "req_grad": len(gradient_ops) > 0,
             "epoch": epoch,
             "deferred": {},
             "eager": eager
         }
         # warmup: bool, mode: str, req_grad: bool, epoch: int, deferred: Dict[str, List[Callable]]]
-        for model in self.epoch_models:
+        for model in self.ctx_models:
             if hasattr(model, "optimizer") and model.optimizer is not None:
                 if isinstance(model.optimizer, Scheduler):
                     model.current_optimizer = model.optimizer.get_current_value(epoch)
                 else:
                     model.current_optimizer = model.optimizer
+        self.ctx_lock.release()
+        return self
+
+    def __enter__(self) -> Self:
+        acquired = self.ctx_lock.acquire(blocking=False)
+        if not acquired:
+            raise ValueError("This network is already in use.")
+        return self
 
-    def unload_epoch(self) -> None:
+    def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
         """Clean up the network after running an epoch.
         """
-        pass
+        self.ctx_inputs = set()
+        self.ctx_outputs = set()
+        self.ctx_gpu_inputs = set()
+        self.ctx_ops = []
+        self.ctx_postprocessing = []
+        self.ctx_slicers = []
+        self.ctx_models = set()
+        self.ctx_state = dict()
+
+        self.ctx_lock.release()
 
     def get_loss_keys(self) -> Set[str]:
         """Find all of the keys associated with model losses.
 
         Returns:
             All of the keys associated with model losses in this network.
         """
         loss_keys = set()
         for op in get_current_items(self.ops):
             loss_keys |= op.get_fe_loss_keys()
         return loss_keys
 
-    def get_effective_input_keys(self, mode: str, epoch: int, ds_id: str = '') -> Set[str]:
-        """Determine which keys need to be provided as input to the network during the given `epoch`.
+    def _get_ctx_inputs_and_outputs(self,
+                                    mode: str,
+                                    epoch: int,
+                                    ds_id: str = '',
+                                    desired_keys: Optional[Set[str]] = None) -> Tuple[Set[str], Set[str], Set[str]]:
+        """Figure out the Network's input and output keys for the current mode/epoch/ds_id.
 
         Args:
             mode: The execution mode to consider. One of 'train', 'eval', 'test', or 'infer'.
             epoch: The epoch number to consider for determining inputs.
             ds_id: The current dataset id.
+            desired_keys: Which outputs do you actually want returned from the network for further processing.
 
         Returns:
-            The necessary inputs for the network to execute the given `epoch` and `mode`.
+            A tuple consisting of:
+                1) The necessary inputs for the network to execute
+                2) The inputs which need to be given to the GPU ops
+                3) The outputs the network will return
         """
-        input_keys = set()
+        network_input_keys = set()
+        gpu_input_keys = set()
         produced_keys = set()
-        for op in get_current_items(self.ops + self.postprocessing, mode, epoch, ds_id=ds_id):
-            input_keys.update(set(key for key in op.inputs if key not in produced_keys))
+        slice_inputs = set()
+        unslice_inputs = set()
+        pops_inputs = set()
+        pops_produced_keys = set()
+        for slicer in get_current_items(self.slicers, mode, epoch, ds_id=ds_id):
+            network_input_keys.update(set(slicer.slice_inputs))
+            unslice_inputs.update(set(slicer.unslice_inputs))
+        slice_inputs.update(network_input_keys)
+        for op in get_current_items(self.ops, mode, epoch, ds_id=ds_id):
+            unsatisfied_inputs = set(key for key in op.inputs if key not in produced_keys)
+            network_input_keys.update(unsatisfied_inputs)
+            gpu_input_keys.update(unsatisfied_inputs)
             produced_keys.update(op.outputs)
-        return input_keys
-
-    def _get_effective_postprocessing_input_keys(self, mode: str, epoch: int, ds_id: str = '') -> Set[str]:
-        """Determine which keys need to be provided as input to the postprocessing during the given `epoch`.
-
-        Args:
-            mode: The execution mode to consider. One of 'train', 'eval', 'test', or 'infer'.
-            epoch: The epoch number to consider for determining inputs.
-            ds_id: The current dataset id.
-
-        Returns:
-            The necessary inputs for the postprocessing to execute the given `epoch` and `mode`.
-        """
-        input_keys = set()
-        produced_keys = set()
+        network_input_keys.update(unslice_inputs - produced_keys)
         for op in get_current_items(self.postprocessing, mode, epoch, ds_id=ds_id):
-            input_keys.update(set(key for key in op.inputs if key not in produced_keys))
+            network_input_keys.update(set(key for key in op.inputs if key not in produced_keys))
             produced_keys.update(op.outputs)
-        return input_keys
+            pops_inputs.update(set(key for key in op.inputs if key not in pops_produced_keys))
+            pops_produced_keys.update(op.outputs)
+        # Figure out outputs
+        output_keys = produced_keys
+        if desired_keys:
+            # If pops require a key then we can't throw it away on the GPU, even if Traces won't use that key later
+            output_keys = (output_keys & desired_keys) | pops_inputs
+        if slice_inputs:
+            # You want the key (output_keys) AND you sliced the key (slice_inputs | produced_keys) but you didn't
+            # unslice it
+            sliced_but_not_unsliced = (output_keys & (slice_inputs | produced_keys)) - unslice_inputs
+            if sliced_but_not_unsliced:
+                state = {'epoch': epoch, 'mode': mode, 'ds_id': ds_id}
+                raise ValueError(
+                    "Since you are using Slicers, you must specify how you would like the following keys to be" +
+                    f" un-sliced during {state}: {sliced_but_not_unsliced}")
 
-    def get_all_output_keys(self, mode: str, epoch: int, ds_id: str = '') -> Set[str]:
-        """Get all of the keys that will be generated by the network during the given `epoch` and `mode`.
-
-        Args:
-            mode: The execution mode to consider. One of 'train', 'eval', 'test', or 'infer'.
-            epoch: The epoch number to consider when searching for outputs.
-            ds_id: The current dataset id.
-
-        Returns:
-            The keys that will be generated by the network's Ops during the `epoch` for the given `mode`.
-        """
-        output_keys = set()
-        for op in get_current_items(self.ops + self.postprocessing, mode, epoch, ds_id=ds_id):
-            output_keys.update(op.outputs)
-        return output_keys
+        return network_input_keys, gpu_input_keys, output_keys
 
     @staticmethod
     def _forward_batch(batch: MutableMapping[str, Any], state: Dict[str, Any], ops: List[TensorOp]) -> None:
         """Run a forward pass through the network's Op chain given a `batch` of data.
 
         Args:
             batch: A batch of input data. Predictions from the network will be written back into this dictionary.
@@ -256,31 +281,49 @@
             if op.outputs:
                 write_outputs_by_op(op, batch, data)
         for fn_list in state['deferred'].values():
             for fn in fn_list:
                 fn()
         state['deferred'].clear()
 
-    def run_step(self, batch: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:  # Batch, Prediction
+    def run_step(self, batch: Dict[str, Array]) -> Dict[str, Array]:  # Batch, Prediction
         """Run a forward step through the Network on a batch of data, including postprocessing.
 
-        This method expects that Network.load_epoch() has already been invoked. The return data will be on the CPU.
+        Usage:
+
+        ```python
+        with network(epoch=1, mode='train', ds_id=''):
+            network.run_step()
+        ```
+
+        The return data will be on the CPU.
 
         Args:
             batch: The batch of data serving as input to the Network.
 
         Returns:
-            (batch_data, prediction_data)
+            The input data along with prediction data (input keys may be overwritten/obscured).
         """
-        batch, prediction = self._run_step(batch)
-        forward_numpyop(ops=self.epoch_postprocessing,
-                        data=ChainMap(prediction, batch),
-                        state=self.epoch_state,
-                        batched=self.target_type)
-        return batch, prediction
+        if not self.ctx_lock.locked:
+            raise ValueError("To invoke the run_step method you must first enter the network (see the doc string)")
+        if not self.ctx_state:
+            raise ValueError("To invoke the run_step method you must first configure the network (see the doc string)")
+        if self.ctx_slicers:
+            minibatches = forward_slicers(self.ctx_slicers, data=batch)
+            results: List[Tuple[Dict[str, Array], Dict[str, Array]]] = []
+            for minibatch in minibatches:
+                results.append(self._run_step(minibatch))
+            batch = reverse_slicers(self.ctx_slicers,
+                                    data=[ChainMap(result[1], result[0]) for result in results],
+                                    original_data=batch)
+        else:
+            batch, prediction = self._run_step(batch)
+            batch = ChainMap(prediction, batch)
+        forward_numpyop(ops=self.ctx_postprocessing, data=batch, state=self.ctx_state, batched=self.target_type)
+        return batch
 
     def _run_step(self, batch: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:  # Batch, Prediction
         """Run a forward step through the Network on a batch of data, excluding postprocessing.
 
         Implementations of this method within derived classes should handle bringing the prediction data back from the
         (multi-)GPU environment to the CPU. This method expects that Network.load_epoch() has already been invoked.
 
@@ -289,62 +332,69 @@
 
         Returns:
             (batch_data, prediction_data)
         """
         raise NotImplementedError
 
     @overload
-    def transform(self, data: Dict[str, Any], mode: str, epoch: int = 1, ds_id: str = '') -> Dict[str, Any]:
+    def transform(self, data: Dict[str, Array], mode: str, epoch: int = 1, ds_id: str = '') -> Dict[str, Array]:
         ...
 
     @overload
-    def transform(self, data: Iterable[Dict[str, Any]], mode: str, epoch: int = 1,
-                  ds_id: str = '') -> List[Dict[str, Any]]:
+    def transform(self, data: Iterable[Dict[str, Array]], mode: str, epoch: int = 1,
+                  ds_id: str = '') -> List[Dict[str, Array]]:
         ...
 
     @overload
-    def transform(self, data: Pipeline, mode: str, epoch: int = 1, ds_id: str = '') -> List[Dict[str, Any]]:
+    def transform(self, data: Pipeline, mode: str, epoch: int = 1, ds_id: str = '') -> List[Dict[str, Array]]:
         ...
 
     def transform(self,
-                  data: Union[Dict[str, Any], Iterable[Dict[str, Any]], Pipeline],
+                  data: Union[Dict[str, Array], Iterable[Dict[str, Array]], Pipeline],
                   mode: str,
                   epoch: int = 1,
-                  ds_id: str = '') -> Union[Dict[str, Any], List[Dict[str, Any]]]:
+                  ds_id: str = '') -> Union[Dict[str, Array], List[Dict[str, Array]]]:
         """Run a forward step through the Network on one or more elements of data.
 
         Args:
             data: The data to use as input (or a pipeline to process an entire dataset at once).
             mode: The mode in which to run the transform. One of 'train', 'eval', 'test', or 'infer'.
             epoch: The epoch in which to run the transform.
             ds_id: The current dataset id.
 
         Returns:
             prediction_data overlaid on the input `data`.
         """
-        self.load_epoch(mode, epoch, ds_id, warmup=False, eager=isinstance(data, dict))
         results = []
-
-        if isinstance(data, Pipeline):
-            with data(mode=mode, epoch=epoch, ds_id=ds_id, shuffle=False) as loader:
-                for batch in loader:
+        with self(mode=mode, epoch=epoch, ds_id=ds_id, warmup=False, eager=isinstance(data, dict) and not self.slicers):
+            if isinstance(data, Pipeline):
+                with data(mode=mode, epoch=epoch, ds_id=ds_id, shuffle=False) as loader:
+                    for batch in loader:
+                        batch = to_tensor(batch, target_type=self.target_type)
+                        results.append(self._do_transform(batch))
+            else:
+                batches = to_list(data)
+                for batch in batches:
                     batch = to_tensor(batch, target_type=self.target_type)
-                    batch, prediction = self.run_step(batch)
-                    results.append({**batch, **prediction})
-        else:
-            batches = to_list(data)
-            for batch in batches:
-                batch = to_tensor(batch, target_type=self.target_type)
-                batch, prediction = self.run_step(batch)
-                results.append({**batch, **prediction})
-        self.unload_epoch()
+                    results.append(self._do_transform(batch))
         if isinstance(data, dict):
             return results[0]
         return results
 
+    def _do_transform(self, batch: Dict[str, Array]) -> Dict[str, Array]:
+        """A handle to allow subclasses to modify the behavior of the transform method before it calls run_step
+
+        Args:
+            batch: A single batch of data on which to run.
+
+        Returns:
+            The predictions overlaid on the input batch dictionary.
+        """
+        return self.run_step(batch)
+
 
 def _collect_models(
     ops: Union[None, TensorOp, Scheduler[TensorOp], Iterable[Union[None, TensorOp,
                                                                    Scheduler[TensorOp]]]]) -> Set[Model]:
     """Collect all model instances from amongst a list of ops.
 
     Args:
@@ -359,25 +409,29 @@
         models |= op.get_fe_models()
     return models
 
 
 # noinspection PyPep8Naming
 def Network(
     ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
-    pops: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp, Scheduler[NumpyOp]]]] = None
+    pops: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp, Scheduler[NumpyOp]]]] = None,
+    slicers: Union[None, Slicer, Scheduler[Slicer], Sequence[Union[None, Slicer, Scheduler[Slicer]]]] = None
 ) -> BaseNetwork:
     """A function to automatically instantiate the correct Network derived class based on the given `ops`.
 
     Args:
         ops: A collection of Ops defining the graph for this Network. It should contain at least one ModelOp, and all
             models should be either TensorFlow or Pytorch. We currently do not support mixing TensorFlow and Pytorch
             models within the same network.
         pops: Postprocessing Ops. A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been
             executed. Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than
             single points.
+        slicers: Slicers to use if you want to cut apart a single batch of data into multiple slices in order to fit
+            them onto a smaller GPU. After cutting the data apart and running through the `ops`, the samples are fused
+            back together into a single batch on the CPU before being handed over to the `pops`.
 
     Returns:
         A network instance containing the given `ops`.
 
     Raises:
         AssertionError: If TensorFlow and PyTorch models are mixed, or if no models are provided.
         ValueError: If a model is provided whose type cannot be identified as either TensorFlow or PyTorch.
@@ -397,79 +451,79 @@
     if len(framework) == 0:
         framework.add('tf')  # We will use tf as default framework if no models are found
     assert len(framework) == 1, "please make sure either tensorflow or torch model is used in network"
     assert len(model_names) == len(models), "all models must have unique model names"
 
     framework = framework.pop()
     if framework == "tf":
-        network = TFNetwork(ops, pops)
+        network = TFNetwork(ops, pops, slicers)
     elif framework == "torch":
-        network = TorchNetwork(ops, pops)
+        network = TorchNetwork(ops, pops, slicers)
     else:
         raise ValueError("Unknown model type")
     return network
 
 
-@traceable()
+@traceable(blacklist=('ctx_lock', ))
 class TorchNetwork(BaseNetwork):
     """An extension of BaseNetwork for PyTorch models.
 
     Args:
         ops: The ops defining the execution graph for this Network.
         postprocessing: A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been executed.
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
+        slicers: Slicers to use if you want to cut apart a single batch of data into multiple slices in order to fit
+            them onto a smaller GPU. After cutting the data apart and running through the `ops`, the samples are fused
+            back together into a single batch on the CPU before being handed over to the `pops`.
 
     """
     device: torch.device
 
     def __init__(
         self,
         ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
         postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp,
-                                                                                Scheduler[NumpyOp]]]] = None
+                                                                                Scheduler[NumpyOp]]]] = None,
+        slicers: Union[None, Slicer, Scheduler[Slicer], Sequence[Union[None, Slicer, Scheduler[Slicer]]]] = None,
     ) -> None:
-        super().__init__(target_type='torch', device=get_device(), ops=ops, postprocessing=postprocessing)
-
-    def load_epoch(self,
-                   mode: str,
-                   epoch: int,
-                   ds_id: str,
-                   output_keys: Optional[Set[str]] = None,
-                   warmup: bool = False,
-                   eager: bool = False) -> None:
-        """Prepare the network to run a given epoch and mode.
-
-        This method is necessary since schedulers and op mode restrictions may result in different computation graphs
-        every epoch. This also moves all of the necessary models from the CPU onto the GPU(s).
-
-        Args:
-            mode: The mode to prepare to execute. One of 'train', 'eval', 'test', or 'infer'.
-            epoch: The epoch to prepare to execute.
-            ds_id: The current dataset id.
-            output_keys: What keys must be moved from the GPU back to the CPU after executing a step.
-            warmup: Whether to prepare to execute it warmup mode or not (end users can likely ignore this argument).
-            eager: Whether to run the training in eager mode. This is only related to TensorFlow training because
-                PyTorch by nature is always in eager mode.
-        """
-        super().load_epoch(mode=mode, epoch=epoch, ds_id=ds_id, output_keys=output_keys, warmup=warmup, eager=eager)
+        super().__init__(target_type='torch',
+                         device=get_device(),
+                         ops=ops,
+                         postprocessing=postprocessing,
+                         slicers=slicers)
+
+    def __call__(self,
+                 mode: str,
+                 epoch: int,
+                 ds_id: str,
+                 desired_output_keys: Optional[Set[str]] = None,
+                 warmup: bool = False,
+                 eager: bool = False) -> Self:
+        super().__call__(mode=mode,
+                         epoch=epoch,
+                         ds_id=ds_id,
+                         desired_output_keys=desired_output_keys,
+                         warmup=warmup,
+                         eager=eager)
         if self.device.type != "cpu":
-            for model in self.epoch_models:
+            for model in self.ctx_models:
                 # move model variables to gpu
                 model.to(self.device)
                 if model.current_optimizer and mode == "train":
                     # move optimizer variables to gpu
                     self._move_optimizer_between_device(model.current_optimizer.state, self.device)
         # Set all of the contiguous final updates to defer their updates by default to enable things like CycleGan
         # This is not necessary for TF because overriding tf weights does not confuse the gradient tape computation
-        for op in reversed(self.epoch_ops):
+        for op in reversed(self.ctx_ops):
             if isinstance(op, UpdateOp):
                 op._old_defer = op.defer
                 op.defer = True
             else:
                 break
+        return self
 
     def _move_optimizer_between_device(self, data: Dict[str, Any], device: Union[str, torch.device]) -> None:
         """Move optimizer state between gpu and cpu recursively.
 
         Args:
             data: Optimizer state.
             device: The target device.
@@ -479,180 +533,178 @@
                 self._move_optimizer_between_device(data[key], device)
             else:
                 try:
                     data[key] = data[key].to(device)
                 except (RuntimeError, AssertionError, AttributeError):
                     pass
 
-    def unload_epoch(self) -> None:
+    def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
         """Clean up the network after running an epoch.
 
         In this case we move all of the models from the GPU(s) back to the CPU.
         """
         if self.device.type != "cpu":
-            for model in self.epoch_models:
+            for model in self.ctx_models:
                 # move model variables to cpu
                 model.to("cpu")
-                if model.current_optimizer and self.epoch_state["mode"] == "train":
+                if model.current_optimizer and self.ctx_state["mode"] == "train":
                     # move optimizer variables to cpu
                     self._move_optimizer_between_device(model.current_optimizer.state, "cpu")
         # Set the final update ops back to their original defer status
-        for op in reversed(self.epoch_ops):
+        for op in reversed(self.ctx_ops):
             if isinstance(op, UpdateOp):
                 op.defer = op.__dict__.get('_old_defer', op.defer)
             else:
                 break
+        super().__exit__(*exc)
 
-    def _get_effective_batch_input(self, batch: MutableMapping[str, Any], mode: str) -> Dict[str, Any]:
+    def _get_effective_batch_input(self, batch: MutableMapping[str, Any]) -> Dict[str, Any]:
         """Copy input data from the the CPU onto the GPU(s).
 
         This method will filter inputs from the batch so that only data required by the network during execution will be
         copied to the GPU.
 
         Args:
             batch: The input data to be moved.
-            mode: The current execution mode. One of 'train', 'eval', 'test', or 'infer'.
 
         Returns:
             The input data ready for use on GPU(s).
         """
         if self.device.type != "cpu":
             new_batch = {
                 key: move_tensors_to_device(batch[key], self.device)
-                for key in self.effective_inputs[mode] if key in batch
+                for key in self.ctx_gpu_inputs if key in batch
             }
         else:
-            new_batch = {key: batch[key] for key in self.effective_inputs[mode] if key in batch}
+            new_batch = {key: batch[key] for key in self.ctx_gpu_inputs if key in batch}
         return new_batch
 
     def _run_step(self, batch: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         """Run a forward step through the Network on a batch of data.
 
         Implementations of this method within derived classes should handle bringing the prediction data back from the
         (multi-)GPU environment to the CPU. This method expects that Network.load_epoch() has already been invoked.
 
         Args:
             batch: The batch of data serving as input to the Network.
 
         Returns:
             (batch_data, prediction_data)
         """
-        mode = self.epoch_state["mode"]
-        batch_in = self._get_effective_batch_input(batch, mode)
-        self.epoch_state["tape"] = NonContext()
+        batch_in = self._get_effective_batch_input(batch)
+        self.ctx_state["tape"] = NonContext()
         # gpu operation
-        with torch.no_grad() if not self.epoch_state["req_grad"] else NonContext():
+        with torch.no_grad() if not self.ctx_state["req_grad"] else NonContext():
             with torch.autocast(device_type=self.device.type) if self.mixed_precision else NonContext():
-                self._forward_batch(batch_in, self.epoch_state, self.epoch_ops)
+                self._forward_batch(batch_in, self.ctx_state, self.ctx_ops)
 
         # copy data to cpu
         if self.device.type != "cpu":
             prediction = {
                 key: move_tensors_to_device(detach_tensors(batch_in[key]), "cpu")
-                for key in self.effective_outputs[mode] if key in batch_in
+                for key in self.ctx_outputs if key in batch_in
             }
         else:
-            prediction = {key: detach_tensors(batch_in[key]) for key in self.effective_outputs[mode] if key in batch_in}
+            prediction = {key: detach_tensors(batch_in[key]) for key in self.ctx_outputs if key in batch_in}
         return batch, prediction
 
 
-@traceable()
+@traceable(blacklist=('ctx_lock', ))
 class TFNetwork(BaseNetwork):
     """An extension of BaseNetwork for TensorFlow models.
 
     Args:
         ops: The ops defining the execution graph for this Network.
         postprocessing: A collection of NumpyOps to be run on the CPU after all of the normal `ops` have been executed.
             Unlike the NumpyOps found in the pipeline, these ops will run on batches of data rather than single points.
+        slicers: Slicers to use if you want to cut apart a single batch of data into multiple slices in order to fit
+            them onto a smaller GPU. After cutting the data apart and running through the `ops`, the samples are fused
+            back together into a single batch on the CPU before being handed over to the `pops`.
     """
     def __init__(
         self,
         ops: Sequence[Union[None, TensorOp, Scheduler[TensorOp]]],
         postprocessing: Union[None, NumpyOp, Scheduler[NumpyOp], Sequence[Union[None, NumpyOp,
-                                                                                Scheduler[NumpyOp]]]] = None
+                                                                                Scheduler[NumpyOp]]]] = None,
+        slicers: Union[None, Slicer, Scheduler[Slicer], Sequence[Union[None, Slicer, Scheduler[Slicer]]]] = None,
     ) -> None:
-        super().__init__(target_type='tf', device=None, ops=ops, postprocessing=postprocessing)
-
-    def load_epoch(self,
-                   mode: str,
-                   epoch: int,
-                   ds_id: str,
-                   output_keys: Optional[Set[str]] = None,
-                   warmup: bool = False,
-                   eager: bool = False) -> None:
-        """Prepare the network to run a given epoch and mode.
+        super().__init__(target_type='tf', device=None, ops=ops, postprocessing=postprocessing, slicers=slicers)
 
-        This method is necessary since schedulers and op mode restrictions may result in different computation graphs
-        every epoch. This also converts the epoch index a tensor to avoid tensorflow graph rebuilding.
-
-        Args:
-            mode: The mode to prepare to execute. One of 'train', 'eval', 'test', or 'infer'.
-            epoch: The epoch to prepare to execute.
-            ds_id: The current dataset id.
-            output_keys: What keys must be moved from the GPU back to the CPU after executing a step.
-            warmup: Whether to prepare to execute it warmup mode or not (end users can likely ignore this argument).
-            eager: Whether to run the training in eager mode. This is only related to TensorFlow training because
-                PyTorch by nature is always in eager mode.
-        """
-        super().load_epoch(mode=mode, epoch=epoch, ds_id=ds_id, output_keys=output_keys, warmup=warmup, eager=eager)
+    def __call__(self,
+                 mode: str,
+                 epoch: int,
+                 ds_id: str,
+                 desired_output_keys: Optional[Set[str]] = None,
+                 warmup: bool = False,
+                 eager: bool = False) -> Self:
+        super().__call__(mode=mode,
+                         epoch=epoch,
+                         ds_id=ds_id,
+                         desired_output_keys=desired_output_keys,
+                         warmup=warmup,
+                         eager=eager)
         # Don't cause a re-trace just because epoch changed
-        self.epoch_state["epoch"] = tf.convert_to_tensor(self.epoch_state["epoch"])
+        self.ctx_state["epoch"] = tf.convert_to_tensor(self.ctx_state["epoch"])
         # Need to re-trace the TF graph if optimizer or layer trainable setting is changing:
-        trainable_str = "".join([str(layer.trainable) for model in self.epoch_models for layer in model.layers])
+        trainable_str = "".join([str(layer.trainable) for model in self.ctx_models for layer in model.layers])
         opt_str = "x".join(
-            [str(id(model.current_optimizer)) for model in self.epoch_models if hasattr(model, 'current_optimizer')])
-        self.epoch_state["_force_tf_retrace"] = hash(trainable_str + opt_str)  # Hash to keep at fixed memory overhead
+            [str(id(model.current_optimizer)) for model in self.ctx_models if hasattr(model, 'current_optimizer')])
+        self.ctx_state["_force_tf_retrace"] = hash(trainable_str + opt_str)  # Hash to keep at fixed memory overhead
+        self.ctx_manual_gpu_data_handling = False
+        return self
 
-    def unload_epoch(self) -> None:
+    def __exit__(self, *exc: Tuple[Optional[Type], Optional[Exception], Optional[Any]]) -> None:
         # This prevents a tf graph memory leak that would slow down long trainings. Since we
         # re-build graphs every epoch there is no reason to keep old ones around.
         strategy = tf.distribute.get_strategy()
         if isinstance(strategy, tf.distribute.MirroredStrategy):
-            return  # TODO - Find a way to clear graph for multi-gpu
+            pass  # TODO - Find a way to clear graph for multi-gpu
         else:
             tf.keras.backend.clear_session()
+        super().__exit__(*exc)
 
     def _run_step(self, batch: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         """Run a forward step through the Network on a batch of data.
 
         Implementations of this method within derived classes should handle bringing the prediction data back from the
         (multi-)GPU environment to the CPU. This method expects that Network.load_epoch() has already been invoked.
 
         Args:
             batch: The batch of data serving as input to the Network.
 
         Returns:
             (batch_data, prediction_data)
         """
-        mode = self.epoch_state["mode"]
-        batch_in = self._get_effective_batch_input(batch, mode)
+        batch_in = self._get_effective_batch_input(batch)
         strategy = tf.distribute.get_strategy()
         if isinstance(strategy, tf.distribute.MirroredStrategy):
-            if self.epoch_state["eager"]:
-                prediction = strategy.run(
-                    self._forward_step_eager,
-                    args=(batch_in, self.epoch_state, self.epoch_ops, to_list(self.effective_outputs[mode])))
-            else:
-                prediction = strategy.run(
-                    self._forward_step_static,
-                    args=(batch_in, self.epoch_state, self.epoch_ops, to_list(self.effective_outputs[mode])))
+            with Suppressor(allow_pyprint=True, show_if_exception=True):
+                if self.ctx_manual_gpu_data_handling:
+                    batch_in = next(
+                        iter(strategy.experimental_distribute_dataset(tf.data.Dataset.from_tensors(batch_in))))
+                if self.ctx_state["eager"]:
+                    prediction = strategy.run(self._forward_step_eager,
+                                              args=(batch_in, self.ctx_state, self.ctx_ops, to_list(self.ctx_outputs)))
+                else:
+                    prediction = strategy.run(self._forward_step_static,
+                                              args=(batch_in, self.ctx_state, self.ctx_ops, to_list(self.ctx_outputs)))
             batch = self._per_replica_to_global(batch)
             prediction = self._per_replica_to_global(prediction)
         else:
-            if self.epoch_state["eager"]:
-                prediction = self._forward_step_eager(batch_in,
-                                                      self.epoch_state,
-                                                      self.epoch_ops,
-                                                      to_list(self.effective_outputs[mode]))
-            else:
-                with Suppressor(allow_pyprint=True, show_if_exception=True):
+            with Suppressor(allow_pyprint=True, show_if_exception=True):
+                if self.ctx_state["eager"]:
+                    prediction = self._forward_step_eager(batch_in,
+                                                          self.ctx_state,
+                                                          self.ctx_ops,
+                                                          to_list(self.ctx_outputs))
+                else:
                     prediction = self._forward_step_static(batch_in,
-                                                           self.epoch_state,
-                                                           self.epoch_ops,
-                                                           to_list(self.effective_outputs[mode]))
+                                                           self.ctx_state,
+                                                           self.ctx_ops,
+                                                           to_list(self.ctx_outputs))
         return batch, prediction
 
     def _per_replica_to_global(self, data: T) -> T:
         """Combine data from "per-replica" values recursively.
 
         For multi-GPU training, data are distributed using `tf.distribute.Strategy.experimental_distribute_dataset`.
         This method collects data from all replicas and combines them into one.
@@ -678,26 +730,25 @@
         elif isinstance(data, tuple):
             return tuple([self._per_replica_to_global(val) for val in data])
         elif isinstance(data, set):
             return set([self._per_replica_to_global(val) for val in data])
         else:
             return data
 
-    def _get_effective_batch_input(self, batch: MutableMapping[str, Any], mode: str) -> Dict[str, Any]:
+    def _get_effective_batch_input(self, batch: MutableMapping[str, Any]) -> Dict[str, Any]:
         """Filter input data so that only the data required by the Network is moved onto the GPU.
 
         Args:
             batch: An unfiltered batch of input data.
-            mode: The current execution mode. One of 'train', 'eval', 'test', or 'infer'.
 
         Returns:
             The filtered input data ready for use on GPU(s).
         """
         new_batch = {}
-        for key in self.effective_inputs[mode]:
+        for key in self.ctx_gpu_inputs:
             if key in batch:
                 new_batch[key] = batch[key]
         return new_batch
 
     def _forward_step_eager(self,
                             batch: Dict[str, Any],
                             state: Dict[str, Any],
@@ -753,39 +804,29 @@
         del state['tape']
         del tape
         for key in effective_outputs:
             if key in batch:
                 prediction[key] = batch[key]
         return prediction
 
-    def transform(self, data: Dict[str, Any], mode: str, epoch: int = 1, ds_id: str = '') -> Dict[str, Any]:
-        """Run a forward step through the Network on an element of data.
-
-        Args:
-            data: The element to data to use as input.
-            mode: The mode in which to run the transform. One of 'train', 'eval', 'test', or 'infer'.
-            epoch: The epoch in which to run the transform.
-            ds_id: The current dataset id.
-
-        Returns:
-            (batch_data, prediction_data)
-        """
+    def _do_transform(self, batch: Dict[str, Array]) -> Dict[str, Array]:
         # Distribute multi-gpu data for processing
         sub_sample = False
         strategy = tf.distribute.get_strategy()
         if isinstance(strategy, tf.distribute.MirroredStrategy):
-            batch_size, num_devices = get_batch_size(data), strategy.num_replicas_in_sync
+            batch_size, num_devices = get_batch_size(batch), strategy.num_replicas_in_sync
             if batch_size < num_devices:
-                data = self._fill_batch(data, num_devices - batch_size)
+                batch = self._fill_batch(batch, num_devices - batch_size)
                 sub_sample = True
-            data = next(iter(strategy.experimental_distribute_dataset(tf.data.Dataset.from_tensors(data))))
-        results = super().transform(data, mode, epoch, ds_id=ds_id)
+            self.ctx_manual_gpu_data_handling = True
+        batch = super()._do_transform(batch)
         if sub_sample:
-            results = self._subsample_data(results, batch_size)
-        return results
+            batch = self._subsample_data(batch, batch_size)
+            self.ctx_manual_gpu_data_handling = False
+        return batch
 
     def _fill_batch(self, data: T, n: int) -> T:
         """Fill data on batch dimension repeating the first n indices at the end.
 
         Args:
             data: The data to be filled.
             n: The number of times to be repeated.
@@ -799,29 +840,29 @@
             return [self._fill_batch(val, n) for val in data]
         elif isinstance(data, tuple):
             return tuple([self._fill_batch(val, n) for val in data])
         elif isinstance(data, set):
             return set([self._fill_batch(val, n) for val in data])
         elif hasattr(data, "shape"):
             paddings = [[0, n]] + [[0, 0] for _ in range(len(data.shape) - 1)]
-            return np.pad(data, pad_width=paddings, mode="symmetric")
+            return tf.pad(data, paddings=paddings, mode="symmetric")
         else:
             return data
 
     def _subsample_data(self, data: T, n: int) -> T:
         """Subsample data by selecting the first n indices recursively.
 
         Args:
             data: The data to be subsampled.
             n: The number of indices to be subsampled.
 
         Returns:
             Subsampled data.
         """
-        if isinstance(data, dict):
+        if isinstance(data, (dict, ChainMap)):
             return {key: self._subsample_data(val, n) for (key, val) in data.items()}
         elif isinstance(data, list):
             return [self._subsample_data(val, n) for val in data]
         elif isinstance(data, tuple):
             return tuple([self._subsample_data(val, n) for val in data])
         elif isinstance(data, set):
             return set([self._subsample_data(val, n) for val in data])
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/affine.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/center_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/crop_non_empty_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/multivariate.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/multivariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_scale.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/read_mat.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/resize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/rotate.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/transpose.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/multivariate/vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/multivariate/vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/numpyop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/numpyop.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,23 +267,26 @@
     def forward_batch(self, data: Union[Tensor, List[Tensor]], state: Dict[str, Any]) -> Optional[FilteredData]:
         return self.forward(data, state)
 
 
 def forward_numpyop(ops: List[NumpyOp],
                     data: MutableMapping[str, Any],
                     state: Dict[str, Any],
-                    batched: Optional[str] = None) -> Optional[FilteredData]:
+                    batched: Optional[str] = None,
+                    shared: bool = True) -> Optional[FilteredData]:
     """Call the forward function for list of NumpyOps, and modify the data dictionary in place.
 
     Args:
         ops: A list of NumpyOps to execute.
         data: The data dictionary.
         state: Information about the current execution context, ex. {"mode": "train"}. Must contain at least the mode.
         batched: Whether the `data` is batched or not. If it is batched, provide the string ('tf', 'torch', or 'np')
             indicating which type of tensors the batch contains.
+        shared: Whether you want to place the resulting data into multi-processing shared memory. Only applicable when
+            `batched` is 'torch'.
     """
     if not ops:
         # Shortcut to prevent wasting time in to_tensor calls if there aren't any ops
         return None
     if batched:
         # Cast data to Numpy before performing batch forward
         for key, val in data.items():
@@ -306,9 +309,9 @@
             for key in op.inputs:
                 del data[key]
         if op.outputs:
             write_outputs_by_op(op, data, op_data)
     if batched:
         # Cast data back to original tensor type after performing batch forward
         for key, val in data.items():
-            data[key] = to_tensor(val, target_type=batched, shared_memory=True)
+            data[key] = to_tensor(val, target_type=batched, shared_memory=shared)
     return None
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/autocontrast.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/binarize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/brightness.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/calibate.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/calibate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/clahe.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/color.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/color_jitter.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/contrast.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/downscale.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/equalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/from_float.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/from_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/image_compression.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/invert_img.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/iso_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/median_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/minmax.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/motion_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/normalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/onehot.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/posterize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_fog.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_gamma.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_rain.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_shadow.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_shapes.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_snow.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/read_image.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/reshape.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/rua.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/sharpness.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/shear_x.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/shear_y.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/solarize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_array.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_float.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_gray.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/to_sepia.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/tokenize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/translate_x.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/translate_y.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/univariate.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/univariate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/numpyop/univariate/word_to_id.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/numpyop/univariate/word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/op.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/argmax.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/augmentation/mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/augmentation/mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/average.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gather.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/fgsm.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/gradient.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/gradient/watch.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/gradient/watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/dice_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/dice_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/focal_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/hinge.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/loss/super_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/loss/super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/fuse.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/one_of.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/repeat.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/meta/sometimes.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/meta/sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/model.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import inspect
 from functools import partial
-from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, TypeVar, Union
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import tensorflow as tf
 import torch
 
 from fastestimator.backend._feed_forward import feed_forward
 from fastestimator.op.tensorop.tensorop import TensorOp
+from fastestimator.types import Model, Tensor
 from fastestimator.util.base_util import to_list, warn
 from fastestimator.util.traceability_util import FeInputSpec, traceable
 from fastestimator.util.util import get_num_devices
 
-Tensor = TypeVar('Tensor', tf.Tensor, torch.Tensor)
-Model = TypeVar('Model', tf.keras.Model, torch.nn.Module)
-
 
 @traceable()
 class ModelOp(TensorOp):
     """This class performs forward passes of a neural network over batch data to generate predictions.
 
     Args:
         model: A model compiled by fe.build.
@@ -51,15 +49,15 @@
             a name will be autogenerated for you (ex. conv2d_2). This autogenerated name will change if you build a new
             model within the same python session (for example, if you re-run a Jupyter notebook cell, the name could now
             be conv2d_5). Any `intermediate_layers` you request will be appended in order to the end of the Op output,
             so you must provide output key names for them within the `outputs` argument. Note that layer names may be
             different between single-gpu and multi-gpu environments, though we attempt to prevent this.
     """
     def __init__(self,
-                 model: Union[tf.keras.Model, torch.nn.Module],
+                 model: Model,
                  inputs: Union[None, str, Iterable[str]] = None,
                  outputs: Union[None, str, Iterable[str]] = None,
                  mode: Union[None, str, Iterable[str]] = None,
                  ds_id: Union[None, str, Iterable[str]] = None,
                  trainable: bool = True,
                  intermediate_layers: Union[None, str, int, List[Union[str, int]]] = None):
         super().__init__(inputs=inputs, outputs=outputs, mode=mode, ds_id=ds_id)
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/model/update.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/model/update.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/normalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/permute.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/reshape.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/resize3d.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/tensorop.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/op/tensorop/un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/op/tensorop/un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/pipeline.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 import gc
 import multiprocessing as mp
 import os
 import time
 from copy import deepcopy
 from operator import mul
 from threading import Lock
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Literal, Optional, Set, Tuple, Type, TypeVar, Union, cast, overload
 
 import numpy as np
 import tensorflow as tf
 from torch.utils.data import DataLoader, Dataset
+from typing_extensions import Self
 
 from fastestimator.backend._to_tensor import to_tensor
 from fastestimator.dataset.dataloader import FEDataLoader
 from fastestimator.dataset.op_dataset import OpDataset
 from fastestimator.op.numpyop.meta.fuse import Fuse
 from fastestimator.op.numpyop.meta.one_of import OneOf
 from fastestimator.op.numpyop.meta.repeat import Repeat
@@ -512,14 +513,32 @@
             return op_data
         data = batch_spec.collate_fn([data])
         op_data = forward_numpyop(batch_ops, data, state, batched='torch')
         if isinstance(op_data, FilteredData):
             return op_data
         return to_tensor(data, target_type=target_type)
 
+    @overload
+    def get_results(self,
+                    mode: str = "train",
+                    epoch: int = 1,
+                    ds_id: str = '',
+                    num_steps: Literal[1] = 1,
+                    shuffle: bool = False) -> Dict[str, Any]:
+        ...
+
+    @overload
+    def get_results(self,
+                    mode: str = "train",
+                    epoch: int = 1,
+                    ds_id: str = '',
+                    num_steps: int = 1,
+                    shuffle: bool = False) -> List[Dict[str, Any]]:
+        ...
+
     def get_results(self,
                     mode: str = "train",
                     epoch: int = 1,
                     ds_id: str = '',
                     num_steps: int = 1,
                     shuffle: bool = False) -> Union[List[Dict[str, Any]], Dict[str, Any]]:
         """Get sample Pipeline outputs.
@@ -549,15 +568,15 @@
 
     def __call__(self,
                  mode: str,
                  epoch: int = 1,
                  ds_id: str = '',
                  shuffle: Optional[bool] = None,
                  steps_per_epoch: Optional[int] = None,
-                 output_keys: Optional[Set[str]] = None) -> 'Pipeline':
+                 output_keys: Optional[Set[str]] = None) -> Self:
         """Prepare this Pipeline for a given `mode` and `epoch`.
 
         A given pipeline can only provide one loader at a time. This helps to prevent issues with multi-threading.
 
         ```python
         pipe = Pipeline(...)
         with pipe(mode='eval', epoch=2) as loader:
@@ -677,17 +696,17 @@
             self.ctx_loader = None
         # Manually triggering gc here seems to be necessary in order to avoid problems with repeated invocations of FE
         # killing one another through multi-processing.
         gc.collect()
         self.ctx_lock.release()
 
 
-def _batch_postprocess(data: Dict[str, Any], ops: List[NumpyOp], output_keys: Set[str], mode: str) -> \
+def _batch_postprocess(data: Dict[str, Any], ops: List[NumpyOp], output_keys: Set[str], mode: str, shared: bool = True) -> \
         Union[Dict[str, Any], FilteredData]:
-    op_data = forward_numpyop(ops=ops, data=data, state={'mode': mode}, batched='torch')
+    op_data = forward_numpyop(ops=ops, data=data, state={'mode': mode}, batched='torch', shared=shared)
     if isinstance(op_data, FilteredData):
         return op_data
     if output_keys:
         unused_keys = data.keys() - output_keys
         OpDataset.handle_warning(unused_keys)
         for key in unused_keys:
             data.pop(key)
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/schedule/schedule.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/schedule/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,26 +183,26 @@
         if epoch_config not in unique_configs:
             unique_configs.append(epoch_config)
             signature_epochs.append(epoch)
     return signature_epochs
 
 
 @overload
-def get_current_items(items: Iterable[Union[T, Scheduler[T]]],
+def get_current_items(items: Iterable[Union[T, Scheduler[T], T2, Scheduler[T2]]],
                       run_modes: Optional[Union[str, Iterable[str]]] = None,
                       epoch: Optional[int] = None,
-                      ds_id: Optional[str] = None) -> List[T]:
+                      ds_id: Optional[str] = None) -> List[Union[T, T2]]:
     ...
 
 
 @overload
-def get_current_items(items: Iterable[Union[T, T2, Scheduler[T], Scheduler[T2]]],
+def get_current_items(items: Iterable[Union[T, Scheduler[T]]],
                       run_modes: Optional[Union[str, Iterable[str]]] = None,
                       epoch: Optional[int] = None,
-                      ds_id: Optional[str] = None) -> List[Union[T, T2]]:
+                      ds_id: Optional[str] = None) -> List[T]:
     ...
 
 
 def get_current_items(items: Iterable[Union[Any, Scheduler[Any]]],
                       run_modes: Optional[Union[str, Iterable[str]]] = None,
                       epoch: Optional[int] = None,
                       ds_id: Optional[str] = None) -> List[Any]:
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/golden_section.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/golden_section.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/grid_search.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/search.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/cartesian.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/cartesian.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/heatmap.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/heatmap.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/parallel_coordinate_plot.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/parallel_coordinate_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/vis_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/vis_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/search/visualize/visualize.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/search/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/history.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/log_parse.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/log_parse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/logs/log_plot.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/logs/log_plot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/summary.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/summary/system.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/summary/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,19 +260,22 @@
             save_model(model, save_dir=save_dir, save_optimizer=hasattr(model, "optimizer") and model.optimizer)
         # Save everything else
         objects = {
             'summary': self.summary,
             'custom_graphs': self.custom_graphs,
             'traces': [trace.__getstate__() if hasattr(trace, '__getstate__') else {} for trace in self.traces],
             'tops': [op.__getstate__() if hasattr(op, '__getstate__') else {} for op in self.network.ops],
+            'slops': [sl.__getstate__() if hasattr(sl, '__getstate__') else {} for sl in self.network.slicers],
             'pops': [op.__getstate__() if hasattr(op, '__getstate__') else {} for op in self.network.postprocessing],
             'nops': [op.__getstate__() if hasattr(op, '__getstate__') else {} for op in self.pipeline.ops],
             'ds': {
-                mode: {key: value.__getstate__()
-                       for key, value in ds.items() if hasattr(value, '__getstate__')}
+                mode: {
+                    key: value.__getstate__()
+                    for key, value in ds.items() if hasattr(value, '__getstate__')
+                }
                 for mode,
                 ds in self.pipeline.data.items()
             }
         }
         with open(os.path.join(save_dir, 'objects.pkl'), 'wb') as file:
             # We need to use a custom pickler here to handle MirroredStrategy, which will show up inside of tf
             # MirroredVariables in multi-gpu systems.
@@ -306,14 +309,15 @@
             raise FileNotFoundError(f"Could not find the objects summary file at {objects_path}")
         with open(objects_path, 'rb') as file:
             objects = pickle.load(file)
         self.summary.__dict__.update(objects['summary'].__dict__)
         self.custom_graphs = objects['custom_graphs']
         self._load_list(objects, 'traces', self.traces)
         self._load_list(objects, 'tops', self.network.ops)
+        self._load_list(objects, 'slops', self.network.slicers)
         self._load_list(objects, 'pops', self.network.postprocessing)
         self._load_list(objects, 'nops', self.pipeline.ops)
         self._load_dict(objects, 'ds', self.pipeline.data)
 
     @staticmethod
     def _load_model(model: Model, base_path: str) -> None:
         """Load model and optimizer weights from disk.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/nightly_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/nightly_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/test/unittest_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/test/unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/early_stopping.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/adapt/terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/adapt/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/batch_display.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/csv_logger.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/grid_display.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/grid_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/image_saver.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/image_viewer.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/model_saver.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/tensorboard.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     def write_epoch_models(self, mode: str, epoch: int) -> None:
         with self.tf_summary_writers[mode].as_default(), summary_ops_v2.always_record_summaries():
             # Record the overall execution summary
             if hasattr(self.network._forward_step_static, '_concrete_stateful_fn'):
                 # noinspection PyProtectedMember
                 summary_ops_v2.graph(self.network._forward_step_static._concrete_stateful_fn.graph)
             # Record the individual model summaries
-            for model in self.network.epoch_models:
+            for model in self.network.ctx_models:
                 summary_writable = (model.__class__.__name__ == 'Sequential'
                                     or (hasattr(model, '_is_graph_network') and model._is_graph_network))
                 if summary_writable:
                     keras_model_summary(model.model_name, model, step=epoch)
 
     def write_weights(self, mode: str, models: Iterable[Model], step: int, visualize: bool) -> None:
         # Similar to TF implementation, but multiple models
@@ -250,15 +250,15 @@
 
 class _TorchWriter(_BaseWriter):
     """A class to write various Pytorch data into TensorBoard summary files.
 
     This class is intentionally not @traceable.
     """
     def write_epoch_models(self, mode: str, epoch: int) -> None:
-        for model in self.network.epoch_models:
+        for model in self.network.ctx_models:
             inputs = model.fe_input_spec.get_dummy_input()
             self.summary_writers[mode].add_graph(model.module if get_num_gpus() > 1 else model, input_to_model=inputs)
 
     def write_weights(self, mode: str, models: Iterable[Model], step: int, visualize: bool) -> None:
         for model in models:
             for name, params in model.named_parameters():
                 name = name.replace(".", "/")
@@ -361,17 +361,17 @@
         self.writer = _TfWriter(self.root_log_dir, self.system.experiment_time, self.system.network) if isinstance(
             self.system.network, TFNetwork) else _TorchWriter(
                 self.root_log_dir, self.system.experiment_time, self.system.network)
         if self.write_graph and self.system.global_step == 1:
             self.painted_graphs = set()
 
     def on_batch_end(self, data: Data) -> None:
-        if self.write_graph and self.system.network.epoch_models.symmetric_difference(self.painted_graphs):
+        if self.write_graph and self.system.network.ctx_models.symmetric_difference(self.painted_graphs):
             self.writer.write_epoch_models(mode=self.system.mode, epoch=self.system.epoch_idx)
-            self.painted_graphs = self.system.network.epoch_models
+            self.painted_graphs = self.system.network.ctx_models
         # Collect embeddings if present in batch but viewing per epoch. Don't aggregate during training though
         if self.system.mode != 'train' and self.embedding_freq.freq and not self.embedding_freq.is_step and \
                 self.system.epoch_idx % self.embedding_freq.freq == 0:
             for elem in self.write_embeddings:
                 name, lbl, img = elem
                 if name in data:
                     self.collected_embeddings[name].append((data.get(name), data.get(lbl), data.get(img)))
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/test_report.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/io/traceability.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/io/traceability.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,31 @@
 from fastestimator.op.tensorop.meta.fuse import Fuse as FuseT
 from fastestimator.op.tensorop.meta.one_of import OneOf as OneOfT
 from fastestimator.op.tensorop.meta.repeat import Repeat as RepeatT
 from fastestimator.op.tensorop.meta.sometimes import Sometimes as SometimesT
 from fastestimator.op.tensorop.model import ModelOp
 from fastestimator.pipeline import Pipeline
 from fastestimator.schedule.schedule import Scheduler, get_current_items, get_signature_epochs
+from fastestimator.slicer.slicer import Slicer
 from fastestimator.summary.logs.log_plot import visualize_logs
 from fastestimator.trace.io.restore_wizard import RestoreWizard
 from fastestimator.trace.trace import Trace, sort_traces
 from fastestimator.util.base_util import FEID, DefaultKeyDict, LogSplicer, NonContext, prettify_metric_name, to_list, \
     warn
 from fastestimator.util.data import Data
 from fastestimator.util.latex_util import AdjustBox, Center, ContainerList, HrefFEID, Verbatim
 from fastestimator.util.traceability_util import FeSummaryTable, traceable
 from fastestimator.util.util import Suppressor, cpu_count, get_gpu_info, get_num_gpus
 
 
+class _UnslicerWrapper():
+    def __init__(self, slicer: Slicer) -> None:
+        self.slicer = slicer
+
+
 @traceable()
 class Traceability(Trace):
     """Automatically generate summary reports of the training.
 
     Args:
         save_path: Where to save the output files. Note that this will generate a new folder with the given name, into
             which the report and corresponding graphics assets will be written.
@@ -297,14 +303,15 @@
             start = self._loop_tables(start,
                                       classes=Scheduler,
                                       name="Schedulers",
                                       model_ids=model_ids,
                                       datasets=datasets)
             start = self._loop_tables(start, classes=Trace, name="Traces", model_ids=model_ids, datasets=datasets)
             start = self._loop_tables(start, classes=Op, name="Operators", model_ids=model_ids, datasets=datasets)
+            start = self._loop_tables(start, classes=Slicer, name="Slicers", model_ids=model_ids, datasets=datasets)
             start = self._loop_tables(start,
                                       classes=(Dataset, tf.data.Dataset),
                                       name="Datasets",
                                       model_ids=model_ids,
                                       datasets=datasets)
             start = self._loop_tables(start,
                                       classes=(tf.keras.Model, torch.nn.Module),
@@ -541,14 +548,15 @@
         """
         ds = self.system.pipeline.data[mode][ds_id]
         if isinstance(ds, Scheduler):
             ds = ds.get_current_value(epoch)
         pipe_ops = get_current_items(self.system.pipeline.ops, run_modes=mode, epoch=epoch, ds_id=ds_id) if isinstance(
             ds, Dataset) else []
         net_ops = get_current_items(self.system.network.ops, run_modes=mode, epoch=epoch, ds_id=ds_id)
+        net_slicers = get_current_items(self.system.network.slicers, run_modes=mode, epoch=epoch, ds_id=ds_id)
         net_post = get_current_items(self.system.network.postprocessing, run_modes=mode, epoch=epoch, ds_id=ds_id)
         traces = sort_traces(get_current_items(self.system.traces, run_modes=mode, epoch=epoch, ds_id=ds_id),
                              ds_ids=self.system.pipeline.get_ds_ids(epoch=epoch, mode=mode))
         diagram = pydot.Dot(compound='true')  # Compound lets you draw edges which terminate at sub-graphs
         diagram.set('rankdir', 'TB')
         diagram.set('dpi', 300)
         diagram.set_node_defaults(shape='box')
@@ -566,15 +574,20 @@
                 if isinstance(batch_size, Scheduler):
                     batch_size = batch_size.get_current_value(epoch)
                 if isinstance(batch_size, dict):
                     batch_size = batch_size[mode]
         if batch_size is not None:
             batch_size = f" (Batch Size: {batch_size})"
         self._draw_subgraph(diagram, diagram, label_last_seen, f'Pipeline{batch_size}', pipe_ops, ds_id)
-        self._draw_subgraph(diagram, diagram, label_last_seen, 'Network', net_ops + net_post, ds_id)
+        self._draw_subgraph(diagram,
+                            diagram,
+                            label_last_seen,
+                            'Network',
+                            net_slicers + net_ops + [_UnslicerWrapper(slicer) for slicer in net_slicers] + net_post,
+                            ds_id)
         self._draw_subgraph(diagram, diagram, label_last_seen, 'Traces', traces, ds_id)
         return diagram
 
     def _draw_subgraph(self,
                        progenitor: pydot.Dot,
                        diagram: Union[pydot.Dot, pydot.Cluster],
                        label_last_seen: DefaultKeyDict[str, str],
@@ -680,19 +693,29 @@
                 texlbl = HrefFEID(FEID(id(op)), name=op.__class__.__name__, color='purple').dumps()
                 if op.batch_size is not None:
                     diagram.set_label(f"Pipeline (Batch Size: {op.batch_size})")
                 label_last_seen.factory = functools.partial(self._delayed_edge,
                                                             progenitor=progenitor,
                                                             old_source=label_last_seen.factory(''),
                                                             new_source=str(id(op)))
+            elif isinstance(op, Slicer):
+                label = f"{op.__class__.__name__} ({FEID(id(op))})"
+                texlbl = HrefFEID(FEID(id(op)), name=op.__class__.__name__, color='purple').dumps()
+                if op.minibatch_size:
+                    diagram.set_label(f"Network (Slices Per Step: {op.minibatch_size})")
+            elif isinstance(op, _UnslicerWrapper):
+                # The corresponding Slicer is already in the graph earlier
+                label = None
+                texlbl = None
             else:
                 label = f"{op.__class__.__name__} ({FEID(id(op))})"
                 texlbl = HrefFEID(FEID(id(op)), name=op.__class__.__name__).dumps()
-            diagram.add_node(pydot.Node(node_id, label=label, texlbl=texlbl))
-            if isinstance(op, (Op, Trace)) and edges:
+            if label is not None:
+                diagram.add_node(pydot.Node(node_id, label=label, texlbl=texlbl))
+            if isinstance(op, (Op, Trace, Slicer, _UnslicerWrapper)) and edges:
                 # Need the instance check since subgraph_ops might contain a tf dataset or torch data loader
                 self._add_edge(progenitor, op, label_last_seen, ds_id)
 
     @staticmethod
     def _delayed_edge(key: str, progenitor: pydot.Dot, old_source: str, new_source: str) -> str:
         """Draw a specific edge between two nodes, modifying the old label if applicable.
 
@@ -712,38 +735,40 @@
             edge.set_label(label)
         else:
             progenitor.add_edge(pydot.Edge(src=old_source, dst=new_source, label=f" {key}"))
         return new_source
 
     def _add_edge(self,
                   progenitor: pydot.Dot,
-                  op: Union[Trace, Op],
+                  op: Union[Trace, Op, Slicer, _UnslicerWrapper],
                   label_last_seen: Dict[str, str],
                   ds_id: Optional[str]):
         """Draw edges into a given Node.
 
         Args:
             progenitor: The very top level diagram onto which Edges should be written.
             op: The op (or trace) to be visualized.
             label_last_seen: A mapping of {data_dict_key: node_id} indicating the last node which generated the key.
             ds_id: The ds_id under which the node is currently running.
         """
-        node_id = str(id(op))
+        node_id = str(id(op.slicer)) if isinstance(op, _UnslicerWrapper) else str(id(op))
         edge_srcs = defaultdict(lambda: [])
         global_ds_ids = {key for vals in self.system.pipeline.data.values() for key in vals.keys() if key is not None}
-        for inp in label_last_seen.keys() if isinstance(op, Batch) else op.inputs:
+        for inp in label_last_seen.keys() if isinstance(op, Batch) else op.slice_inputs if isinstance(
+                op, Slicer) else op.slicer.unslice_inputs if isinstance(op, _UnslicerWrapper) else op.inputs:
             if inp == '*':
                 continue
             _, candidate_id, *_ = f"{inp}|".split('|')
             if candidate_id in global_ds_ids and candidate_id != ds_id:
                 continue  # Skip inputs which will be provided in other ds_id plots
             edge_srcs[label_last_seen[inp]].append(inp)
         for src, labels in edge_srcs.items():
             progenitor.add_edge(pydot.Edge(src=src, dst=node_id, label=f" {', '.join(labels)} "))
-        outputs = op.get_outputs(ds_ids=ds_id) if isinstance(op, Trace) else op.outputs
+        outputs = op.get_outputs(ds_ids=ds_id) if isinstance(op, Trace) else op.slice_inputs if isinstance(
+            op, Slicer) else op.slicer.unslice_inputs if isinstance(op, _UnslicerWrapper) else op.outputs
         for out in label_last_seen.keys() if isinstance(op, Batch) else outputs:
             label_last_seen[out] = node_id
 
     @staticmethod
     def _get_all_nodes(diagram: Union[pydot.Dot, pydot.Cluster]) -> List[pydot.Node]:
         """Recursively search through a `diagram` looking for Nodes.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/meta/_per_ds.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/meta/_per_ds.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/accuracy.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/auc.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/auc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/bleu_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/calibration_error.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/dice.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/f1_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/mcc.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/mcc.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Union, Iterable
+from typing import Any, Dict, Union, Iterable
 
 import numpy as np
 from sklearn.metrics import matthews_corrcoef
 
 from fastestimator.trace.meta._per_ds import per_ds
 from fastestimator.trace.trace import Trace
-from fastestimator.util.data import Any, Data, Dict
+from fastestimator.util.data import Data
 from fastestimator.util.traceability_util import traceable
 from fastestimator.util.util import to_number
 
 
 @per_ds
 @traceable()
 class MCC(Trace):
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/precision.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/metric/recall.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/metric/recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/trace.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/eigen_cam.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/eigen_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/grad_cam.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/grad_cam.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/label_tracker.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/trace/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/trace/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/types/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/types/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Protocol, Sequence, Sized, Union, \
-    runtime_checkable
+from typing import TYPE_CHECKING, Any, Callable, Collection, Dict, List, Optional, Protocol, Sequence, Sized, TypeVar, \
+    Union, runtime_checkable
 
 
 class FilteredData:
     """A placeholder to indicate that this data instance should not be used.
 
     This class is intentionally not @traceable.
 
@@ -42,31 +42,44 @@
         ...
 
     fe_batch: Optional[int]
     fe_reset_ds: Optional[Callable[[bool], None]]
     fe_batch_indices: Optional[Callable[[int], List[List[int]]]]
 
 
+CollectionT = TypeVar('CollectionT', bound=Collection)
+
 if TYPE_CHECKING:
     # Hide these imports for speed
     import numpy as np
     import tensorflow as tf
     import torch
 
     Tensor = Union[torch.Tensor, tf.Tensor, tf.Variable]
     Array = Union[np.ndarray, Tensor]
     DataSequence = Union[Sequence, Array]
+    Model = Union[tf.keras.Model, torch.nn.Module]
+
+    # Use these when you want to indicate that you will return the same class that was input
+    TensorT = TypeVar('TensorT', torch.Tensor, tf.Tensor, tf.Variable)
+    ArrayT = TypeVar('ArrayT', torch.Tensor, tf.Tensor, tf.Variable, np.ndarray)
+    ModelT = TypeVar('ModelT', tf.keras.Model, torch.nn.Module)
 
 else:
+    TensorT = TypeVar('TensorT')
+    ArrayT = TypeVar('ArrayT')
+    ModelT = TypeVar('ModelT')
+
     # The following allow runtime isinstance() checks against the types defined above, without incurring import speed
     # penalties if the user doesn't run the isinstance check (by hiding the tf import). In python 3.10+ we could simply
     # do isinstance() checks on Union[] types, but even in that case we would incur speed penalty from importing
     # tensorflow during the Union definition, which would make the types unsuitable for fast-path code like the log
     # visualization CLI.
 
+
     class _MetaTensor(type):
         def __instancecheck__(self, __instance: Any) -> bool:
             import tensorflow as tf
             import torch
             return isinstance(__instance, torch.Tensor) or tf.is_tensor(__instance)
 
         def __subclasscheck__(self, __subclass: type) -> bool:
@@ -95,7 +108,21 @@
 
         def __subclasscheck__(self, __subclass: type) -> bool:
 
             return issubclass(__subclass, (Sequence, Array))
 
     class DataSequence(metaclass=_MetaDataSequence):
         ...
+
+    class _MetaModel(type):
+        def __instancecheck__(self, __instance: Any) -> bool:
+            import tensorflow as tf
+            import torch
+            return isinstance(__instance, (tf.keras.Model, torch.nn.Module))
+
+        def __subclasscheck__(self, __subclass: type) -> bool:
+            import tensorflow as tf
+            import torch
+            return issubclass(__subclass, (tf.keras.Model, torch.nn.Module))
+
+    class Model(metaclass=_MetaModel):
+        ...
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/base_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/base_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,19 @@
             data = set(data)
         else:
             data = {data}
     return data
 
 
 @overload
+def to_list(data: Set[KT]) -> List[KT]:
+    ...
+
+
+@overload
 def to_list(data: Union[None, Dict[KT, VT], Iterable[Dict[KT, VT]]]) -> List[Dict[KT, VT]]:
     ...
 
 
 @overload
 def to_list(data: Union[None, VT, Iterable[VT]]) -> List[VT]:
     ...
@@ -492,15 +497,16 @@
     Raises:
         AssertionError: if blacklisted modes and whitelisted modes are mixed.
     """
     negation = set([ds_id.startswith("!") for ds_id in ds_ids])
     assert len(negation) < 2, "cannot mix !ds_id with ds_id, found {}".format(ds_ids)
     forbidden_ds_id_chars = {":", ";", "|"}
     for ds_id in ds_ids:
-        assert isinstance(ds_id, str) and len(ds_id) > 0, "dataset id must be a string, found {}".format(ds_id)
+        assert isinstance(ds_id, str) and len(ds_id) > 0, \
+            f"dataset id must be a non-empty string, found {ds_id}"
         assert not any(char in ds_id for char in forbidden_ds_id_chars), \
             "dataset id should not contain forbidden characters like ':', ';', '|', found {}".format(ds_id)
     return ds_ids
 
 
 def is_number(arg: str) -> bool:
     """Check if a given string can be converted into a number.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/cli_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/data.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Any, ChainMap, Dict, List, MutableMapping, Optional
+from typing import Any, ChainMap, List, MutableMapping, Optional
 
 
 class Data(ChainMap[str, Any]):
     """A class which contains prediction and batch data.
 
     This class is intentionally not @traceable.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/google_download_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/google_download_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/img_data.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/latex_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/latex_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/traceability_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/traceability_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,16 +512,18 @@
         if inp_id not in tables:
             kwargs = {}
             path = None
             if hasattr(inp, '__dict__') and '_fe_state_whitelist' not in inp.__dict__:
                 # Prevent circular recursion
                 tables[inp_id] = FeSummaryTable(name=inp.__class__.__name__, target_type=type(inp), fe_id=inp_id)
                 # This object isn't @traceable but does have some stored variables that we can summarize.
-                kwargs = _trace_value({k: v
-                                       for k, v in inp.__dict__.items() if not k.startswith("_")},
+                kwargs = _trace_value({
+                    k: v
+                    for k, v in inp.__dict__.items() if not k.startswith("_")
+                },
                                       tables,
                                       ret_ref,
                                       wrap_str=False).raw_input
                 path = "Not @traceable, so summary is approximate"
             tables[inp_id] = FeSummaryTable(name=inp.__class__.__name__,
                                             target_type=type(inp),
                                             path=path,
@@ -1022,27 +1024,29 @@
     from torch.utils.data import Dataset
 
     from fastestimator.estimator import Estimator
     from fastestimator.network import TFNetwork, TorchNetwork
     from fastestimator.op.op import Op
     from fastestimator.pipeline import Pipeline
     from fastestimator.schedule.schedule import Scheduler
+    from fastestimator.slicer.slicer import Slicer
     from fastestimator.trace.trace import Trace
 
     # re-number the references for nicer viewing
     ordered_items = sorted(
         self._fe_traceability_summary.items(),
         key=lambda x: 0 if issubclass(x[1].type, Estimator) else 1
         if issubclass(x[1].type, (TFNetwork, TorchNetwork)) else 2 if issubclass(x[1].type, Pipeline) else 3
         if issubclass(x[1].type, Scheduler) else 4 if issubclass(x[1].type, Trace) else 5
-        if issubclass(x[1].type, Op) else 6 if issubclass(x[1].type, (Dataset, tf.data.Dataset)) else 7
-        if issubclass(x[1].type, (tf.keras.Model, torch.nn.Module)) else 8
-        if issubclass(x[1].type, types.FunctionType) else 9
-        if issubclass(x[1].type, (np.ndarray, tf.Tensor, tf.Variable, torch.Tensor)) else 10)
-    key_mapping = {fe_id: f"@FE{idx}" for idx, (fe_id, val) in enumerate(ordered_items)}
+        if issubclass(x[1].type, Op) else 6 if issubclass(x[1].type, Slicer) else 7
+        if issubclass(x[1].type, (Dataset, tf.data.Dataset)) else 8
+        if issubclass(x[1].type, (tf.keras.Model, torch.nn.Module)) else 9
+        if issubclass(x[1].type, types.FunctionType) else 10
+        if issubclass(x[1].type, (np.ndarray, tf.Tensor, tf.Variable, torch.Tensor)) else 11)
+    key_mapping = {fe_id: f"@FE{idx}" for idx, (fe_id, _) in enumerate(ordered_items)}
     FEID.set_translation_dict(key_mapping)
     return [item[1] for item in ordered_items]
 
 
 def __getstate__(self) -> Dict[str, Any]:
     """Return a summary of this class' state variables (for restore wizard).
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 from contextlib import ContextDecorator
+from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List, MutableMapping, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 import tensorflow as tf
 import torch
 import torch.backends.mps
@@ -381,14 +382,15 @@
     elif isinstance(data, set):
         return set([detach_tensors(val) for val in data])
     elif isinstance(data, torch.Tensor):
         return data.detach()
     return data
 
 
+@lru_cache()
 def get_device() -> torch.device:
     """Get the torch device for the current hardware.
 
     Returns:
         The torch device most appropriate for the current hardware.
     """
     if torch.backends.mps.is_available():
@@ -396,28 +398,30 @@
     elif torch.cuda.is_available():
         device = torch.device("cuda:0")
     else:
         device = torch.device("cpu")
     return device
 
 
+@lru_cache()
 def get_num_gpus() -> int:
     """Get the number of GPUs available.
 
     Returns:
         The number of GPUs available.
     """
     if torch.backends.mps.is_available():
         return 1
     elif torch.cuda.is_available():
         return torch.cuda.device_count()
     else:
         return 0
 
 
+@lru_cache()
 def get_gpu_info() -> List[str]:
     """Get summaries of all of the GPUs accessible on this machine.
 
     Returns:
         A formatted summary of the GPUs available on the machine (one list entry per GPU).
     """
     if shutil.which('nvidia-smi') is not None:
@@ -438,23 +442,25 @@
         output = subprocess.check_output(["sysctl", "-n", "hw.memsize"])
         output = output.decode('utf-8')
         gpu_mem = f"{float(output)*1e-9:0.2f} GB"  # Convert from bytes to GB
         return [f"{get_cpu_info()['brand_raw']} ({gpu_mem}, {core_count} Cores)"]  # On mac the CPU name is the GPU name
     return []
 
 
+@lru_cache()
 def get_num_devices() -> int:
     """Determine the number of available GPUs.
 
     Returns:
         The number of available GPUs, or 1 if none are found.
     """
     return max(torch.cuda.device_count(), 1)
 
 
+@lru_cache()
 def cpu_count(limit: Optional[int] = None) -> int:
     """Determine the number of available CPUs (correcting for docker container limits).
 
     Args:
         limit: If provided, the TF and Torch backends will be told to use `limit` number of threads, or the available
             number of cpus if the latter is lower (`limit` cannot raise the number of threads). A limit can only be
             enforced once per python session, before starting anything like pipeline which requires multiprocessing.
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/util/wget_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/util/wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator/xai/saliency.py` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator/xai/saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/PKG-INFO` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastestimator-nightly
-Version: 1.6.0.dev202306301354
+Version: 1.6.0.dev202307151357
 Summary: Deep learning framework
 Home-page: https://github.com/fastestimator/fastestimator
 Author: FastEstimator Dev
 License: Apache License 2.0
 Keywords: fastestimator tensorflow pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/SOURCES.txt` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,19 @@
 ./fastestimator/search/search.py
 ./fastestimator/search/visualize/__init__.py
 ./fastestimator/search/visualize/cartesian.py
 ./fastestimator/search/visualize/heatmap.py
 ./fastestimator/search/visualize/parallel_coordinate_plot.py
 ./fastestimator/search/visualize/vis_util.py
 ./fastestimator/search/visualize/visualize.py
+./fastestimator/slicer/__init__.py
+./fastestimator/slicer/axis_slicer.py
+./fastestimator/slicer/mean_unslicer.py
+./fastestimator/slicer/slicer.py
+./fastestimator/slicer/sliding_slicer.py
 ./fastestimator/summary/__init__.py
 ./fastestimator/summary/history.py
 ./fastestimator/summary/summary.py
 ./fastestimator/summary/system.py
 ./fastestimator/summary/logs/__init__.py
 ./fastestimator/summary/logs/log_parse.py
 ./fastestimator/summary/logs/log_plot.py
@@ -409,14 +414,18 @@
 ./test/PR_test/integration_test/schedule/test_arc.py
 ./test/PR_test/integration_test/schedule/test_epoch_scheduler.py
 ./test/PR_test/integration_test/schedule/test_repeat_scheduler.py
 ./test/PR_test/integration_test/schedule/test_schedule.py
 ./test/PR_test/integration_test/search/__init__.py
 ./test/PR_test/integration_test/search/visualize/__init__.py
 ./test/PR_test/integration_test/search/visualize/test_visualize.py
+./test/PR_test/integration_test/slicer/__init__.py
+./test/PR_test/integration_test/slicer/test_axis_slicer.py
+./test/PR_test/integration_test/slicer/test_slicer.py
+./test/PR_test/integration_test/slicer/test_sliding_slicer.py
 ./test/PR_test/integration_test/summary/__init__.py
 ./test/PR_test/integration_test/summary/test_history.py
 ./test/PR_test/integration_test/summary/test_system.py
 ./test/PR_test/integration_test/trace/__init__.py
 ./test/PR_test/integration_test/trace/test_eval_essential.py
 ./test/PR_test/integration_test/trace/test_logger.py
 ./test/PR_test/integration_test/trace/test_test_essential.py
@@ -655,14 +664,19 @@
 ./test/PR_test/unit_test/schedule/test_epoch_scheduler.py
 ./test/PR_test/unit_test/schedule/test_lr_schedule.py
 ./test/PR_test/unit_test/schedule/test_repeat_scheduler.py
 ./test/PR_test/unit_test/search/__init__.py
 ./test/PR_test/unit_test/search/test_golden_section_search.py
 ./test/PR_test/unit_test/search/test_grid_search.py
 ./test/PR_test/unit_test/search/test_search.py
+./test/PR_test/unit_test/slicer/__init__.py
+./test/PR_test/unit_test/slicer/test_axis_slicer.py
+./test/PR_test/unit_test/slicer/test_mean_slicer.py
+./test/PR_test/unit_test/slicer/test_slicer.py
+./test/PR_test/unit_test/slicer/test_sliding_slicer.py
 ./test/PR_test/unit_test/summary/__init__.py
 ./test/PR_test/unit_test/summary/test_history.py
 ./test/PR_test/unit_test/summary/test_summary.py
 ./test/PR_test/unit_test/summary/logs/__init__.py
 ./test/PR_test/unit_test/summary/logs/test_metrics.py
 ./test/PR_test/unit_test/test/__init__.py
 ./test/PR_test/unit_test/test/test_unittest_util.py
```

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/fastestimator_nightly.egg-info/requires.txt` & `fastestimator-nightly-1.6.0.dev202307151357/fastestimator_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/setup.py` & `fastestimator-nightly-1.6.0.dev202307151357/setup.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_get_lr.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_get_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_save_model_load_model.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_save_model_load_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_set_lr.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_set_lr.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/backend/test_update_model.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/backend/test_update_model.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/test_main.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/cli/test_train.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/cli/test_train.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/multivariate/test_read_mat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/numpyop/univariate/test_read_image.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/augmentation/test_cutmix_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/test_fgsm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/test_gradientop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/gradient/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_l1_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_l2_regularization.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/loss/test_super_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/test_modelop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/test_modelop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/model/test_updateop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/model/test_updateop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_average.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_average.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/tensorop/test_un_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_arc.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_arc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/schedule/test_schedule.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/schedule/test_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/visualize/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/search/visualize/test_visualize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/search/visualize/test_visualize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/summary/test_system.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/summary/test_system.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/test_estimator.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/test_estimator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/test_network.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/test_network.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/test_pipeline.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_early_stopping.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_pbm_calibrator.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/adapt/test_terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_batch_display.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_batch_display.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_best_model_saver.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_best_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_csv_logger.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_csv_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_image_saver.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_image_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_image_viewer.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_image_viewer.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_model_saver.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_restore_wizard.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_restore_wizard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_tensorboard.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_test_report.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_test_report.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/io/test_traceability.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/io/test_traceability.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_accuracy.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_calibration_error.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_calibration_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_dice.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_dice.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_f1_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_f1_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_mcc.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_mcc.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_precision.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_precision.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/metric/test_recall.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/metric/test_recall.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_eval_essential.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_eval_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_logger.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_logger.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_test_essential.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_test_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_trace.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_trace.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/test_train_essential.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/test_train_essential.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/test_instance_tracker.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/test_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/trace/xai/test_label_tracker.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/trace/xai/test_label_tracker.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/test_img_data.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/test_img_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/integration_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/pytorch/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_attention_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_lenet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_resnet9.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_unet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_unet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/architecture/tensorflow/test_wideresnet.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_abs.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_abs.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_argmax.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_argmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_binary_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_binary_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_cast.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_cast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_check_nan.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_check_nan.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_clip_by_value.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_clip_by_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_concat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_concat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_dice_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_dice_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_exp.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_exp.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_feed_forward.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_gather.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_gather.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_gather_from_batch.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_gather_from_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_get_gradient.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_get_gradient.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_get_image_dims.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_get_image_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_hinge.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_hinge.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_iwd.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_iwd.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_lambertw.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_lambertw.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_matmul.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_matmul.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_maximum.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_maximum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_mean_squared_error.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_ones_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_ones_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_percentile.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_percentile.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_permute.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_permute.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_pow.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_random_normal_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_random_normal_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_random_uniform_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_random_uniform_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_max.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_max.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_mean.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_mean.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_min.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_min.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_std.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_std.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reduce_sum.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reduce_sum.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_roll.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_roll.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_sign.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_sign.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_sparse_categorical_crossentropy.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_squeeze.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_normalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_pow.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_pow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_round.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_round.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_tensor_sqrt.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_tensor_sqrt.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_to_shape.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_to_shape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_to_tensor.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_to_type.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_to_type.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_watch.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_watch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_where.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_where.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_zeros_like.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_zeros_like.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/backend/test_zscore.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/backend/test_zscore.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/cli/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/cli/test_cli_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_batch_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_batch_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_combine_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_combine_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_csv_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_data.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_extend_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_extend_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_generator_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_generator_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_labeled_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_numpy_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_pickle_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/dataset/test_siamese_dir_dataset.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/test_cropping_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/pytorch/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/pytorch/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/test_instance_norm.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/layers/tensorflow/test_reflection_padding_2d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/loss/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/loss/test_focal_loss.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/loss/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_affine.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_center_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_crop_non_empy_mask_if_exists.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_elastic_transform.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_horizontal_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_iaa_crop_and_pad.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_longest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_mask_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_optical_distortion.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_pad_if_needed.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_crop_near_bbox.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_grid_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_rotate_90.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_scale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_bbox_safe_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_random_sized_crop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_resize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_shift_scale_rotate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_smallest_max_size.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/multivariate/test_vertical_flip.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/test_numpyop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/test_numpyop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_autocontrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_binarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_brightness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_channel_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_channel_transpose.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_clahe.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_color.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_color.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_color_jitter.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_downscale.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_equalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_expand_dims.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_fromfloat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_hue_saturation_value.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_iaa_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_image_compression.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_invert_img.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_iso_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_median_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_minmax.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_motion_blur.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_multiplicative_noise.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_onehot.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_pad_sequence.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_posterize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_fog.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_gamma.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_rain.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_shadow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_shapes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_snow.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_random_sun_flare.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_reshape.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_rgb_shift.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_rua.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_sharpness.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_shear_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_shear_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_solarize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_array.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_float.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_gray.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_to_sepia.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_translate_x.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_translate_y.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/numpyop/univariate/test_word_to_id.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/augmentation/test_mixup_batch.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_fuse.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_one_of.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_repeat.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/meta/test_sometimes.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/test_normalize.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/test_normalize.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/test_resize3d.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/test_resize3d.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/tensorop/test_tensorop.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/tensorop/test_tensorop.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/op/test_op.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/op/test_op.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/test_epoch_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/test_epoch_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/test_lr_schedule.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/test_lr_schedule.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/schedule/test_repeat_scheduler.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/schedule/test_repeat_scheduler.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/test_golden_section_search.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/test_golden_section_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/test_grid_search.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/search/test_search.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/search/test_search.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/logs/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/logs/test_metrics.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/logs/test_metrics.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/test_history.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/test_history.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/summary/test_summary.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/summary/test_summary.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/test/test_unittest_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/test/test_unittest_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/test_auc_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/test_auc_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/trace/metric/test_bleu_score.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/trace/metric/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/types/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/integration_test/slicer/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/types/test_types.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/types/test_types.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_data.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_data.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_traceability_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_traceability_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/util/test_wget_util.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/util/test_wget_util.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/xai/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/xai/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/PR_test/unit_test/xai/test_saliency.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/PR_test/unit_test/xai/test_saliency.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/__init__.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fastestimator-nightly-1.6.0.dev202306301354/test/run_pr_test.py` & `fastestimator-nightly-1.6.0.dev202307151357/test/run_pr_test.py`

 * *Files identical despite different names*

