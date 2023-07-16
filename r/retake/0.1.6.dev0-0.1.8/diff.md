# Comparing `tmp/retake-0.1.6.dev0.tar.gz` & `tmp/retake-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake-0.1.6.dev0.tar", max compression
+gzip compressed data, was "retake-0.1.8.tar", max compression
```

## Comparing `retake-0.1.6.dev0.tar` & `retake-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,37 @@
--rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.6.dev0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.6.dev0/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.6.dev0/core/extract/__init__.py
--rw-r--r--   0        0        0      326 2023-07-05 22:15:59.015798 retake-0.1.6.dev0/core/extract/base.py
--rw-r--r--   0        0        0     2025 2023-07-05 22:50:15.971238 retake-0.1.6.dev0/core/extract/postgres.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.6.dev0/core/load/__init__.py
--rw-r--r--   0        0        0      575 2023-07-05 19:36:34.019152 retake-0.1.6.dev0/core/load/base.py
--rw-r--r--   0        0        0     5629 2023-07-06 00:13:55.542173 retake-0.1.6.dev0/core/load/elasticsearch.py
--rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.6.dev0/core/load/opensearch.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.6.dev0/core/transform/__init__.py
--rw-r--r--   0        0        0      171 2023-07-05 22:15:59.016190 retake-0.1.6.dev0/core/transform/base.py
--rw-r--r--   0        0        0      646 2023-07-05 22:15:59.018406 retake-0.1.6.dev0/core/transform/embedding.py
--rw-r--r--   0        0        0      523 2023-07-06 00:13:53.416457 retake-0.1.6.dev0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-05 19:05:09.416653 retake-0.1.6.dev0/retake/__init__.py
--rw-r--r--   0        0        0      594 2023-07-05 22:15:59.021471 retake-0.1.6.dev0/retake/embedding.py
--rw-r--r--   0        0        0     4030 2023-07-06 00:09:45.837821 retake-0.1.6.dev0/retake/pipeline.py
--rw-r--r--   0        0        0      812 2023-07-05 21:03:51.198603 retake-0.1.6.dev0/retake/sink.py
--rw-r--r--   0        0        0      384 2023-07-05 19:05:09.417695 retake-0.1.6.dev0/retake/source.py
--rw-r--r--   0        0        0      703 2023-07-06 00:13:55.523454 retake-0.1.6.dev0/retake/target.py
--rw-r--r--   0        0        0      752 2023-07-05 19:05:09.418073 retake-0.1.6.dev0/retake/transform.py
--rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 retake-0.1.6.dev0/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-07-16 17:39:33.445915 retake-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3136 2023-07-16 17:39:33.445915 retake-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/extract/__init__.py
+-rw-r--r--   0        0        0      549 2023-07-16 17:39:33.445915 retake-0.1.8/core/extract/base.py
+-rw-r--r--   0        0        0     2194 2023-07-16 17:39:33.445915 retake-0.1.8/core/extract/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/__init__.py
+-rw-r--r--   0        0        0     1502 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/base.py
+-rw-r--r--   0        0        0     5407 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/elasticsearch.py
+-rw-r--r--   0        0        0      632 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/opensearch.py
+-rw-r--r--   0        0        0     2707 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/pinecone.py
+-rw-r--r--   0        0        0     2892 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/tests/test_pinecone.py
+-rw-r--r--   0        0        0     2817 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/weaviate.py
+-rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/embedding.py
+-rw-r--r--   0        0        0     9040 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/pipeline.py
+-rw-r--r--   0        0        0      629 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/realtime.py
+-rw-r--r--   0        0        0     1438 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/sink.py
+-rw-r--r--   0        0        0      453 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/source.py
+-rw-r--r--   0        0        0     1823 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/target.py
+-rw-r--r--   0        0        0       41 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/tests/test_pipeline.py
+-rw-r--r--   0        0        0      853 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/transform.py
+-rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/base.py
+-rw-r--r--   0        0        0      488 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/cohere.py
+-rw-r--r--   0        0        0      323 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/custom.py
+-rw-r--r--   0        0        0      463 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/openai.py
+-rw-r--r--   0        0        0      415 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/sentence_transformers.py
+-rw-r--r--   0        0        0     1198 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_cohere.py
+-rw-r--r--   0        0        0      629 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_custom.py
+-rw-r--r--   0        0        0     1002 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_openai.py
+-rw-r--r--   0        0        0     1180 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_sentence_transformers.py
+-rw-r--r--   0        0        0      965 2023-07-16 17:39:51.702107 retake-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-07-16 17:39:33.449915 retake-0.1.8/retake/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 17:39:33.449915 retake-0.1.8/streams/__init__.py
+-rw-r--r--   0        0        0     2722 2023-07-16 17:39:33.449915 retake-0.1.8/streams/app.py
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 retake-0.1.8/PKG-INFO
```

### Comparing `retake-0.1.6.dev0/core/extract/postgres.py` & `retake-0.1.8/core/extract/postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,54 +2,55 @@
 import select
 import json
 import threading
 import queue
 
 from psycopg2.extras import LogicalReplicationConnection
 from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
-from typing import List
+from typing import List, Generator, Dict, Any, Optional, cast
 
-from core.extract.base import Extractor
+from core.extract.base import Extractor, ExtractorResult
 
 
 class ConnectionError(Exception):
     pass
 
 
 class PostgresExtractor(Extractor):
-    def __init__(self, dsn: str):
+    def __init__(self, dsn: str) -> None:
         self.dsn = dsn
-        self.connection = None
-        self.cursor = None
-
         self._connect(dsn)
 
-    def _connect(self, dsn: str):
+    def _connect(self, dsn: str) -> None:
         try:
             self.connection = psycopg2.connect(
                 self.dsn, connection_factory=LogicalReplicationConnection
             )
         except psycopg2.ProgrammingError:
             raise ConnectionError("Unable to connect to database")
         except psycopg2.OperationalError:
             raise ConnectionError("Unable to connect to database")
 
         self.cursor = self.connection.cursor()
 
-    def teardown(self):
-        self.cursor.close()
+    def teardown(self) -> None:
+        self.cursor.close()  # type: ignore
         self.connection.close()
 
-    def count(self, relation: str):
+    def count(self, relation: str) -> int:
         self.cursor.execute(f"SELECT COUNT(*) FROM {relation}")
-        return self.cursor.fetchone()[0]
+        row = self.cursor.fetchone()
+        if row:
+            return cast(int, row[0])
+        else:
+            return 0
 
     def extract_all(
         self, relation: str, columns: List[str], primary_key: str, chunk_size: int
-    ):
+    ) -> Generator[ExtractorResult, None, None]:
         offset = 0
         columns_str = ", ".join(columns)
 
         while True:
             self.cursor.execute(
                 f"""
                 SELECT {columns_str}, {primary_key}
```

### Comparing `retake-0.1.6.dev0/core/load/elasticsearch.py` & `retake-0.1.8/core/load/elasticsearch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,86 @@
 from abc import ABC, abstractmethod
 from elasticsearch import Elasticsearch, helpers
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Optional, Any, cast
 from core.load.base import Loader
+from core.sdk.target import ElasticSearchTarget
 
 
 class FieldTypeError(Exception):
     pass
 
 
 class ElasticSearchLoader(Loader):
     def __init__(
         self,
-        host: str = None,
-        user: str = None,
-        password: str = None,
-        ssl_assert_fingerprint: str = None,
-        cloud_id: str = None,
-        index: bool = False,
-        similarity: str = None,
-    ):
+        host: Optional[str] = None,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        ssl_assert_fingerprint: Optional[str] = None,
+        cloud_id: Optional[str] = None,
+        index: Optional[bool] = False,
+        similarity: Optional[str] = None,
+    ) -> None:
         if index and similarity is None:
             raise ValueError("Similarity must be provided if index is True")
 
-        kwargs = {
-            "hosts": [host] if host else None,
-            "basic_auth": (user, password) if user and password else None,
-            "ssl_assert_fingerprint": ssl_assert_fingerprint
-            if ssl_assert_fingerprint
-            else None,
-            "verify_certs": True if host else None,
-            "cloud_id": cloud_id if cloud_id else None,
-        }
+        if cloud_id:
+            self.es = Elasticsearch(cloud_id=cloud_id)
+        elif host and user and password and ssl_assert_fingerprint:
+            self.es = Elasticsearch(
+                hosts=[host],
+                basic_auth=(user, password),
+                ssl_assert_fingerprint=ssl_assert_fingerprint,
+                verify_certs=True,
+            )
+        else:
+            raise ValueError(
+                "Either cloud_id or host, user, password, and ssl_assert_fingerprint must be provided"
+            )
 
-        self.es = Elasticsearch(**{k: v for k, v in kwargs.items() if v is not None})
         self.index = index
         self.similarity = similarity
 
-    ### Private Methods ###
+    def _check_index_exists(self, index_name: str) -> bool:
+        return cast(bool, self.es.indices.exists(index=index_name))
 
-    def _check_index_exists(self, index_name: str):
-        return self.es.indices.exists(index=index_name)
-
-    def _create_index(self, index_name: str, field_name: str, num_dimensions: int):
+    def _create_index(
+        self, index_name: str, field_name: str, num_dimensions: int
+    ) -> None:
         if self._check_index_exists(index_name=index_name):
-            raise IndexAlreadyExistsError(f"Index {index_name} already exists")
+            raise ValueError(f"Index {index_name} already exists")
 
-        mapping = {
-            "mappings": {
+        mapping = cast(
+            Dict[str, Any],
+            {
                 "dynamic": True,
                 "_source": {"enabled": True},
                 "properties": {
                     field_name: {
                         "type": "dense_vector",
                         "dims": num_dimensions,
                         "index": self.index,
                     }
                 },
-            }
-        }
+            },
+        )
 
         if self.similarity is not None:
-            mapping["mappings"]["properties"][field_name][
-                "similarity"
-            ] = self.similarity
+            mapping["properties"][field_name]["similarity"] = self.similarity
 
-        self.es.indices.create(index=index_name, body=mapping)
+        self.es.indices.create(index=index_name, mappings=mapping)
+
+    ### Public Methods ###
+
+    def check_and_setup_index(
+        self, target: ElasticSearchTarget, num_dimensions: int
+    ) -> None:
+        index_name = target.index_name
+        field_name = target.field_name
 
-    def _check_and_setup_index(
-        self, index_name: str, field_name: str, num_dimensions: int
-    ):
         if not self._check_index_exists(index_name=index_name):
             self._create_index(
                 index_name=index_name,
                 field_name=field_name,
                 num_dimensions=num_dimensions,
             )
         else:
@@ -84,76 +92,52 @@
                 ]
                 if field_mapping["type"] != "dense_vector":
                     raise FieldTypeError(
                         f"Field '{field_name}' exists but is not a dense_vector field"
                     )
                 if field_mapping["dims"] != num_dimensions:
                     raise FieldTypeError(
-                        f"Field '{field_name}' expects {field_mapping['dims']} dimensions but the embedding has {len(embedding)}"
+                        f"Field '{field_name}' expects {field_mapping['dims']} dimensions but the embedding has {num_dimensions}"
                     )
             else:
                 # The field does not exist, create it
                 new_field_mapping = {
-                    "properties": {
-                        field_name: {
-                            "type": "dense_vector",
-                            "dims": num_dimensions,
-                            "index": True,
-                        }
+                    field_name: {
+                        "type": "dense_vector",
+                        "dims": num_dimensions,
+                        "index": True,
                     }
                 }
-                self.es.indices.put_mapping(index=index_name, body=new_field_mapping)
+                self.es.indices.put_mapping(
+                    index=index_name, properties=new_field_mapping
+                )
 
     ### Public Methods ###
 
-    def upsert_embedding(
-        self,
-        index_name: str,
-        embedding: List[float],
-        id: Union[str, int],
-        field_name: str,
-        metadata: Dict[str, any] = None,
-    ):
-        self._check_and_setup_index(
-            index_name=index_name,
-            field_name=field_name,
-            num_dimensions=len(embedding),
-        )
-
-        doc = dict()
-        doc[field_name] = embedding
-
-        if not metadata is None:
-            doc.update(metadata)
-
-        self.es.update(
-            index=index_name, id=id, body={"doc": doc, "doc_as_upsert": True}
-        )
-
+    @Loader.validate
     def bulk_upsert_embeddings(
         self,
-        index_name: str,
+        target: ElasticSearchTarget,
         embeddings: List[List[float]],
         ids: List[Union[str, int]],
-        field_name: str,
-        metadata: List[Dict[str, any]] = None,
-    ):
+        metadata: Optional[List[Dict[str, Any]]],
+    ) -> None:
+        index_name = target.index_name
+        field_name = target.field_name
         num_dimensions = len(embeddings[0])
+        num_embeddings = len(embeddings)
 
         if not all(len(embedding) == num_dimensions for embedding in embeddings):
             raise ValueError("Not all embeddings have the same number of dimensions")
 
-        self._check_and_setup_index(
-            index_name=index_name,
-            field_name=field_name,
-            num_dimensions=num_dimensions,
-        )
+        if not len(ids) == num_embeddings:
+            raise ValueError("Number of ids does not match number of embeddings")
 
         if metadata is None:
-            metadata = [{}] * len(ids)
+            metadata = [{}] * num_embeddings
 
         docs = [
             {"_id": doc_id, "_source": {**{field_name: embedding}, **meta}}
             for doc_id, embedding, meta in zip(ids, embeddings, metadata)
         ]
 
         actions = [
```

### Comparing `retake-0.1.6.dev0/pyproject.toml` & `retake-0.1.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 [tool.poetry]
 name = "retake"
-version = "0.1.6-dev"
-description = "Real-time pipelines for vectors"
-authors = ["Ming Ying <ming.ying.nyc@gmail.com>"]
+version = "0.1.8"
+description = "Open Source Infrastructure for Vector Data Streams"
+authors = ["Ming Ying <ming.ying.nyc@gmail.com>", "Philippe Noël <philippemnoel@gmail.com>"]
 readme = "README.md"
-packages = [{include = "retake"}, {include = "core"}]
+packages = [{include = "retake"}, {include = "core"}, {include = "streams"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psycopg2-binary = "^2.9.6"
 pydantic = "^2.0.2"
 sentence-transformers = "^2.2.2"
 tqdm = "^4.65.0"
+types-psycopg2 = "^2.9.21.10"
+types-tqdm = "^4.65.0.1"
+pinecone-client = "^2.2.2"
+elasticsearch = "^8.8.2"
+cohere = "^4.12.0"
+openai = "^0.27.8"
+faust-streaming = "^0.10.14"
+requests = "^2.31.0"
+python-dotenv = "^1.0.0"
+fastavro = "^1.8.0"
+weaviate-client = "^3.22.1"
+confluent-kafka = "^2.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.1"
+pytest = "^7.4.0"
+numpy = "^1.25.1"
+types-requests = "^2.31.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `retake-0.1.6.dev0/retake/embedding.py` & `retake-0.1.8/core/sdk/embedding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 from pydantic import BaseModel
+from typing import Callable, List
 
 
 class OpenAIEmbedding(BaseModel):
     api_key: str
     model: str
 
 
 class SentenceTransformerEmbedding(BaseModel):
     model: str
 
 
+class CohereEmbedding(BaseModel):
+    api_key: str
+    model: str
+
+
+class CustomEmbedding(BaseModel):
+    func: Callable[[List[str]], List[List[float]]]
+
+
 class Embedding:
     @classmethod
     def OpenAI(cls, api_key: str, model: str) -> OpenAIEmbedding:
         return OpenAIEmbedding(api_key=api_key, model=model)
 
     @classmethod
     def SentenceTransformer(
         cls, model: str = "all-MiniLM-L6-v2"
     ) -> SentenceTransformerEmbedding:
         return SentenceTransformerEmbedding(model=model)
 
-    # TODO: Add more embedding models, e.g. Cohere, Google, custom model, etc.
+    @classmethod
+    def Cohere(cls, api_key: str, model: str) -> CohereEmbedding:
+        return CohereEmbedding(api_key=api_key, model=model)
+
+    @classmethod
+    def Custom(cls, func: Callable[[List[str]], List[List[float]]]) -> CustomEmbedding:
+        return CustomEmbedding(func=func)
```

### Comparing `retake-0.1.6.dev0/retake/transform.py` & `retake-0.1.8/core/sdk/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from pydantic import BaseModel
-from typing import Callable, Any
+from typing import Callable, Any, List, Optional
 
 
 class PostgresTransform(BaseModel):
     relation: str
     primary_key: str
-    columns: list
+    columns: List[str]
     transform_func: Callable[..., Any]
-    optional_metadata: Callable[..., Any] = None
+    schema_name: str = "public"
+    optional_metadata: Optional[Callable[..., Any]]
 
 
 class Transform:
     @classmethod
     def Postgres(
         cls,
         relation: str,
         primary_key: str,
-        columns: list,
-        transform_func: Callable[..., Any] = None,
-        optional_metadata: Callable[..., Any] = None,
+        columns: List[str],
+        transform_func: Callable[..., Any],
+        schema_name: str = "public",
+        optional_metadata: Optional[Callable[..., Any]] = None,
     ) -> PostgresTransform:
         return PostgresTransform(
             relation=relation,
             primary_key=primary_key,
             columns=columns,
             transform_func=transform_func,
             optional_metadata=optional_metadata,
```

