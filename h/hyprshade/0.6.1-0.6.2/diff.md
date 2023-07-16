# Comparing `tmp/hyprshade-0.6.1.tar.gz` & `tmp/hyprshade-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.6.1.tar", max compression
+gzip compressed data, was "hyprshade-0.6.2.tar", max compression
```

## Comparing `hyprshade-0.6.1.tar` & `hyprshade-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-07-14 05:53:08.754014 hyprshade-0.6.1/LICENSE
--rw-r--r--   0        0        0     2440 2023-07-14 05:53:08.754014 hyprshade-0.6.1/README.md
--rw-r--r--   0        0        0      125 2023-07-14 05:53:08.754014 hyprshade-0.6.1/examples/config.toml
--rw-r--r--   0        0        0        0 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/__main__.py
--rw-r--r--   0        0        0     2466 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/cli.py
--rw-r--r--   0        0        0     3709 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/config.py
--rw-r--r--   0        0        0      483 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/constants.py
--rw-r--r--   0        0        0      643 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/helpers.py
--rw-r--r--   0        0        0      803 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/hyprctl.py
--rw-r--r--   0        0        0      812 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/utils.py
--rw-r--r--   0        0        0     1036 2023-07-14 05:53:08.754014 hyprshade-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-14 05:53:08.754014 hyprshade-0.6.1/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-14 05:53:08.754014 hyprshade-0.6.1/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-16 16:02:20.602370 hyprshade-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2440 2023-07-16 16:02:20.602370 hyprshade-0.6.2/README.md
+-rw-r--r--   0        0        0      125 2023-07-16 16:02:20.606370 hyprshade-0.6.2/examples/config.toml
+-rw-r--r--   0        0        0        0 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2466 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/cli.py
+-rw-r--r--   0        0        0     3709 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/config.py
+-rw-r--r--   0        0        0      483 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/constants.py
+-rw-r--r--   0        0        0      566 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/helpers.py
+-rw-r--r--   0        0        0      803 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/hyprctl.py
+-rw-r--r--   0        0        0      812 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/utils.py
+-rw-r--r--   0        0        0     1036 2023-07-16 16:02:20.606370 hyprshade-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-16 16:02:20.606370 hyprshade-0.6.2/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-16 16:02:20.606370 hyprshade-0.6.2/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.6.2/PKG-INFO
```

### Comparing `hyprshade-0.6.1/LICENSE` & `hyprshade-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/README.md` & `hyprshade-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/hyprshade/cli.py` & `hyprshade-0.6.2/hyprshade/cli.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/hyprshade/config.py` & `hyprshade-0.6.2/hyprshade/config.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/hyprshade/helpers.py` & `hyprshade-0.6.2/hyprshade/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
+from glob import iglob
 from os import path
 
+from more_itertools import first
+
 from .constants import SHADER_DIRS
 
 
 def resolve_shader_path(shader_name_or_path: str) -> str:
-    shader_path = shader_name_or_path
-    if not path.isfile(shader_path):
-        for shaders_dir in SHADER_DIRS:
-            shader_path = path.join(shaders_dir, glsl_ext(shader_name_or_path))
-            if path.isfile(shader_path):
-                break
-
-    if not path.isfile(shader_path):
-        raise FileNotFoundError(f"Shader {shader_name_or_path} does not exist")
-
-    return shader_path
-
-
-def glsl_ext(pathname: str) -> str:
-    if pathname.endswith(".glsl"):
-        return pathname
-    return f"{pathname}.glsl"
+    if path.isfile(shader_name_or_path):
+        return shader_name_or_path
+
+    for shaders_dir in SHADER_DIRS:
+        shader_path = first(
+            iglob(f"{shader_name_or_path}*", root_dir=shaders_dir), None
+        )
+        if shader_path is not None:
+            return path.join(shaders_dir, shader_path)
+
+    raise FileNotFoundError(f"Shader {shader_name_or_path} does not exist")
```

### Comparing `hyprshade-0.6.1/hyprshade/hyprctl.py` & `hyprshade-0.6.2/hyprshade/hyprctl.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/hyprshade/utils.py` & `hyprshade-0.6.2/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/pyproject.toml` & `hyprshade-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["examples", "shaders"]
```

### Comparing `hyprshade-0.6.1/shaders/blue-light-filter.glsl` & `hyprshade-0.6.2/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/shaders/vibrance.glsl` & `hyprshade-0.6.2/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.1/PKG-INFO` & `hyprshade-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

