# Comparing `tmp/image_analyst_tf-0.1.0.tar.gz` & `tmp/image_analyst_tf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst_tf-0.1.0.tar", max compression
+gzip compressed data, was "image_analyst_tf-0.1.1.tar", max compression
```

## Comparing `image_analyst_tf-0.1.0.tar` & `image_analyst_tf-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_tf-0.1.0/LICENSE
--rw-r--r--   0        0        0     1165 2023-07-14 20:17:08.543945 image_analyst_tf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      884 2023-07-14 20:19:02.371375 image_analyst_tf-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_tf-0.1.0/src/image_analyst/tf/__init__.py
--rw-r--r--   0        0        0    13715 2023-07-14 20:23:07.577978 image_analyst_tf-0.1.0/src/image_analyst/tf/models.py
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 image_analyst_tf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-25 12:15:37.802723 image_analyst_tf-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1174 2023-07-16 20:03:50.261260 image_analyst_tf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      884 2023-07-14 20:19:02.371375 image_analyst_tf-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 12:23:00.936940 image_analyst_tf-0.1.1/src/image_analyst/tf/__init__.py
+-rw-r--r--   0        0        0    13634 2023-07-16 19:43:37.542678 image_analyst_tf-0.1.1/src/image_analyst/tf/models.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 image_analyst_tf-0.1.1/PKG-INFO
```

### Comparing `image_analyst_tf-0.1.0/LICENSE` & `image_analyst_tf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst_tf-0.1.0/pyproject.toml` & `image_analyst_tf-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image-analyst-tf"
-version = "0.1.0"
+version = "0.1.1"
 description = "ImageAnalyst TF is an extension to the ImageAnalyst library, providing additional models and functions using tensorflow."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
 repository = "https://github.com/BergLucas/ImageAnalystTF"
 keywords = ["image", "analysis", "tf"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -12,17 +12,17 @@
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 numpy = "^1.24.3"
-image-analyst = "^0.1.0"
-tensorflow = "^2.13.0"
-tensorflow-io-gcs-filesystem = "0.31.0"
+image-analyst = "^0.1.1"
+tensorflow = "^2.10.0"
+tensorflow-io-gcs-filesystem = "^0.29, !=0.32.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
```

### Comparing `image_analyst_tf-0.1.0/README.md` & `image_analyst_tf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst_tf-0.1.0/src/image_analyst/tf/models.py` & `image_analyst_tf-0.1.1/src/image_analyst/tf/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     ModelLoadingFailedException,
     InvalidDtypeException,
     DetectionFailedException,
 )
 from image_analyst.image import (
     ImageFormat,
     BoundingBox,
-    verify_image,
     ImageEmbedder,
     EmbeddingFunction,
 )
 from image_analyst.utils import NmsFunction, NmsPython
 from image_analyst.models import ODModel, Detection
 from typing import Optional
 import tensorflow as tf
@@ -195,16 +194,14 @@
         return np.float32
 
     @property
     def supported_format(self) -> ImageFormat:  # noqa: D102
         return ImageFormat.RGB
 
     def __call__(self, image: np.ndarray) -> list[Detection]:  # noqa: D102
-        verify_image(image)
-
         if image.dtype != self.supported_dtype:
             raise InvalidDtypeException("The image dtype is not supported.")
 
         logger.info("Started Image preprocessing")
         embedded_image, bounding_box = self.__embedding_function(
             image, *self.__model_size
         )
@@ -309,16 +306,14 @@
         return np.float32
 
     @property
     def supported_format(self) -> ImageFormat:  # noqa: D102
         return ImageFormat.RGB
 
     def __call__(self, image: np.ndarray) -> list[Detection]:  # noqa: D102
-        verify_image(image)
-
         if image.dtype != self.supported_dtype:
             raise InvalidDtypeException("The image dtype is not supported.")
 
         logger.info("Started Image preprocessing")
         embedded_image, bounding_box = self.__embedding_function(
             image, *self.__model_size
         )
```

### Comparing `image_analyst_tf-0.1.0/PKG-INFO` & `image_analyst_tf-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: image-analyst-tf
-Version: 0.1.0
+Version: 0.1.1
 Summary: ImageAnalyst TF is an extension to the ImageAnalyst library, providing additional models and functions using tensorflow.
 Home-page: https://github.com/BergLucas/ImageAnalystTF
 Keywords: image,analysis,tf
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: image-analyst (>=0.1.0,<0.2.0)
+Requires-Dist: image-analyst (>=0.1.1,<0.2.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: tensorflow (>=2.13.0,<3.0.0)
-Requires-Dist: tensorflow-io-gcs-filesystem (==0.31.0)
+Requires-Dist: tensorflow (>=2.10.0,<3.0.0)
+Requires-Dist: tensorflow-io-gcs-filesystem (>=0.29,<0.30)
 Project-URL: Repository, https://github.com/BergLucas/ImageAnalystTF
 Description-Content-Type: text/markdown
 
 # ImageAnalyst TF
 
 ImageAnalyst TF is an extension to the [ImageAnalyst](https://github.com/BergLucas/ImageAnalyst) library, providing additional models and functions using [tensorflow](https://pypi.org/project/tensorflow/).
```

