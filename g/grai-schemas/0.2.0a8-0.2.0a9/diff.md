# Comparing `tmp/grai_schemas-0.2.0a8.tar.gz` & `tmp/grai_schemas-0.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.2.0a8.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a9.tar", max compression
```

## Comparing `grai_schemas-0.2.0a8.tar` & `grai_schemas-0.2.0a9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3793 2023-05-26 18:12:59.756317 grai_schemas-0.2.0a8/LICENSE
--rw-r--r--   0        0        0      322 2023-05-26 18:12:59.756709 grai_schemas-0.2.0a8/README.md
--rw-r--r--   0        0        0      885 2023-07-13 21:42:57.997963 grai_schemas-0.2.0a8/pyproject.toml
--rw-r--r--   0        0        0      210 2023-07-13 21:42:58.003093 grai_schemas-0.2.0a8/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      848 2023-07-10 15:57:25.736802 grai_schemas-0.2.0a8/src/grai_schemas/base.py
--rw-r--r--   0        0        0     3618 2023-07-13 19:24:12.951398 grai_schemas-0.2.0a8/src/grai_schemas/generics.py
--rw-r--r--   0        0        0    41788 2023-06-14 21:10:34.453210 grai_schemas-0.2.0a8/src/grai_schemas/human_ids.py
--rw-r--r--   0        0        0      175 2023-06-01 16:01:43.271004 grai_schemas-0.2.0a8/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-05-26 18:12:59.757931 grai_schemas-0.2.0a8/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      669 2023-07-10 15:57:25.737338 grai_schemas-0.2.0a8/src/grai_schemas/schema.py
--rw-r--r--   0        0        0     2564 2023-07-10 15:57:25.737534 grai_schemas-0.2.0a8/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      451 2023-07-10 15:57:25.737795 grai_schemas-0.2.0a8/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     3737 2023-07-13 16:32:19.161602 grai_schemas-0.2.0a8/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0      845 2023-07-10 15:57:25.738097 grai_schemas-0.2.0a8/src/grai_schemas/v1/events.py
--rw-r--r--   0        0        0      793 2023-07-10 15:57:25.738417 grai_schemas-0.2.0a8/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0     1738 2023-07-10 15:57:25.738789 grai_schemas-0.2.0a8/src/grai_schemas/v1/merge.py
--rw-r--r--   0        0        0      279 2023-06-15 00:41:57.158195 grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     2179 2023-07-10 15:57:25.739070 grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      240 2023-07-10 15:57:25.739286 grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/generics.py
--rw-r--r--   0        0        0      928 2023-07-13 19:24:12.948758 grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     2228 2023-07-11 00:38:07.412504 grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     7149 2023-07-13 21:42:36.456526 grai_schemas-0.2.0a8/src/grai_schemas/v1/mock.py
--rw-r--r--   0        0        0     3727 2023-07-13 16:32:19.172713 grai_schemas-0.2.0a8/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0      940 2023-07-10 15:57:25.740065 grai_schemas-0.2.0a8/src/grai_schemas/v1/organization.py
--rw-r--r--   0        0        0     1203 2023-07-10 15:57:25.740281 grai_schemas-0.2.0a8/src/grai_schemas/v1/source.py
--rw-r--r--   0        0        0     3696 2023-07-10 15:57:25.740372 grai_schemas-0.2.0a8/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a8/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-05-26 18:12:59.756317 grai_schemas-0.2.0a9/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-26 18:12:59.756709 grai_schemas-0.2.0a9/README.md
+-rw-r--r--   0        0        0      886 2023-07-14 15:00:25.545332 grai_schemas-0.2.0a9/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-07-14 15:00:25.551220 grai_schemas-0.2.0a9/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      848 2023-07-10 15:57:25.736802 grai_schemas-0.2.0a9/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3642 2023-07-14 14:59:13.274303 grai_schemas-0.2.0a9/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-14 21:10:34.453210 grai_schemas-0.2.0a9/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-01 16:01:43.271004 grai_schemas-0.2.0a9/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-05-26 18:12:59.757931 grai_schemas-0.2.0a9/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      669 2023-07-10 15:57:25.737338 grai_schemas-0.2.0a9/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2564 2023-07-10 15:57:25.737534 grai_schemas-0.2.0a9/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      451 2023-07-10 15:57:25.737795 grai_schemas-0.2.0a9/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     3737 2023-07-14 14:55:41.775204 grai_schemas-0.2.0a9/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:57:25.738097 grai_schemas-0.2.0a9/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      793 2023-07-10 15:57:25.738417 grai_schemas-0.2.0a9/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0     1738 2023-07-10 15:57:25.738789 grai_schemas-0.2.0a9/src/grai_schemas/v1/merge.py
+-rw-r--r--   0        0        0      279 2023-06-15 00:41:57.158195 grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2179 2023-07-10 15:57:25.739070 grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      240 2023-07-14 14:55:41.776841 grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0      930 2023-07-13 22:06:56.324899 grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     2228 2023-07-11 00:38:07.412504 grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     7173 2023-07-14 14:55:41.777627 grai_schemas-0.2.0a9/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     3727 2023-07-14 14:55:41.779072 grai_schemas-0.2.0a9/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-07-14 14:55:41.779946 grai_schemas-0.2.0a9/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1203 2023-07-10 15:57:25.740281 grai_schemas-0.2.0a9/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3696 2023-07-14 14:55:41.780953 grai_schemas-0.2.0a9/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a9/PKG-INFO
```

### Comparing `grai_schemas-0.2.0a8/LICENSE` & `grai_schemas-0.2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/pyproject.toml` & `grai_schemas-0.2.0a9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.2.0-alpha8"
+version = "0.2.0-alpha9"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^1.10.4"
+pydantic = "^1.10.11"
 multimethod = "^1.9.1"
 polyfactory = "^2.6.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pre-commit = "^2.21.0"
```

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/base.py` & `grai_schemas-0.2.0a9/src/grai_schemas/base.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/generics.py` & `grai_schemas-0.2.0a9/src/grai_schemas/generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     class Config:
         """ """
 
         json_encoders = {UUID: lambda x: str(x)}
         validate_all = True
         validate_assignment = True
         allow_population_by_field_name = True
+        orm_mode = True
 
 
 class PlaceHolderSchema(GraiBaseModel):
     """ """
 
     is_active: Optional[bool] = True
```

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/human_ids.py` & `grai_schemas-0.2.0a9/src/grai_schemas/human_ids.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/schema.py` & `grai_schemas-0.2.0a9/src/grai_schemas/schema.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/utilities.py` & `grai_schemas-0.2.0a9/src/grai_schemas/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/edge.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/edge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/events.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/events.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/generics.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/merge.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/merge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/edges.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/metadata.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     """"""
 
     sources: Dict[UUID, GraiMetadataV1]
 
 
 class MetadataV1(GraiMetadataV1, SourcesMetadataV1):
     """ """
+
     pass
 
+
 class GraiMalformedNodeMetadataV1(MalformedMetadata, MetadataV1):
     """ """
 
     grai: nodes.MalformedNodeMetadataV1 = nodes.MalformedNodeMetadataV1()  # type: ignore
     sources: Dict[UUID, GraiMetadataV1] = {}
```

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/metadata/nodes.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/mock.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/mock.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,35 +208,37 @@
 
 
 class WorkspaceSpecFactory(ModelFactory[WorkspaceSpec]):
     __model__ = WorkspaceSpec
     __set_as_default_factory_for_type__ = True
 
     name = get_human_id
-    organisation = get_human_id
+    organisation = OrganisationSpecFactory.build
 
     @post_generated
     @classmethod
     def ref(cls, name, organisation) -> str:
         """ """
-        return f"{organisation}/{name}"
+        return f"{organisation.name}/{name}"
+
 
 class WorkspaceFactory(ModelFactory[WorkspaceV1]):
     __model__ = WorkspaceV1
 
 
 class MockWorkspace:
     @classmethod
     def workspace(cls, **kwargs):
         """ """
         return WorkspaceFactory.build(factory_use_construct=True, **kwargs)
 
     @classmethod
     def workspace_spec(cls, **kwargs):
         """ """
+
         return WorkspaceSpecFactory.build(factory_use_construct=True, **kwargs)
 
 
 class SourceSpecFactory(ModelFactory[SourceSpec]):
     __model__ = SourceSpec
     __set_as_default_factory_for_type__ = True
```

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/node.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/node.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/organization.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/organization.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/source.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/source.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/src/grai_schemas/v1/workspace.py` & `grai_schemas-0.2.0a9/src/grai_schemas/v1/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a8/PKG-INFO` & `grai_schemas-0.2.0a9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: multimethod (>=1.9.1,<2.0.0)
 Requires-Dist: polyfactory (>=2.6.1,<3.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-schemas
 Description-Content-Type: text/markdown
 
 # Grai Schemas
 
 Grai Schemas provide reference implementations in Python for objects used in Grai.
```

