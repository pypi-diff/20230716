# Comparing `tmp/citizenk-0.1.49.tar.gz` & `tmp/citizenk-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.49.tar", max compression
+gzip compressed data, was "citizenk-0.1.50.tar", max compression
```

## Comparing `citizenk-0.1.49.tar` & `citizenk-0.1.50.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    18975 2023-07-16 09:28:22.216839 citizenk-0.1.49/README.md
--rw-r--r--   0        0        0      382 2023-06-11 19:27:45.145664 citizenk-0.1.49/citizenk/__init__.py
--rw-r--r--   0        0        0     8794 2023-07-16 08:47:29.905433 citizenk-0.1.49/citizenk/agent.py
--rw-r--r--   0        0        0    20708 2023-07-16 09:00:15.851212 citizenk-0.1.49/citizenk/citizenk.py
--rw-r--r--   0        0        0    24499 2023-07-16 09:00:15.980386 citizenk-0.1.49/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-06-11 19:27:45.146160 citizenk-0.1.49/citizenk/murmur2.py
--rw-r--r--   0        0        0     8055 2023-07-16 09:22:38.668288 citizenk-0.1.49/citizenk/topic.py
--rw-r--r--   0        0        0      407 2023-07-16 09:00:15.900741 citizenk-0.1.49/citizenk/utils.py
--rw-r--r--   0        0        0     1864 2023-07-16 09:28:11.749538 citizenk-0.1.49/pyproject.toml
--rw-r--r--   0        0        0    20644 1970-01-01 00:00:00.000000 citizenk-0.1.49/PKG-INFO
+-rw-r--r--   0        0        0    18975 2023-07-16 10:27:05.374297 citizenk-0.1.50/README.md
+-rw-r--r--   0        0        0      437 2023-07-16 10:24:04.938149 citizenk-0.1.50/citizenk/__init__.py
+-rw-r--r--   0        0        0     8794 2023-07-16 08:47:29.905433 citizenk-0.1.50/citizenk/agent.py
+-rw-r--r--   0        0        0    20808 2023-07-16 09:49:52.814769 citizenk-0.1.50/citizenk/citizenk.py
+-rw-r--r--   0        0        0    24499 2023-07-16 09:00:15.980386 citizenk-0.1.50/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-06-11 19:27:45.146160 citizenk-0.1.50/citizenk/murmur2.py
+-rw-r--r--   0        0        0     8512 2023-07-16 10:26:46.583887 citizenk-0.1.50/citizenk/topic.py
+-rw-r--r--   0        0        0      407 2023-07-16 09:00:15.900741 citizenk-0.1.50/citizenk/utils.py
+-rw-r--r--   0        0        0     1889 2023-07-16 10:23:06.345152 citizenk-0.1.50/pyproject.toml
+-rw-r--r--   0        0        0    20690 1970-01-01 00:00:00.000000 citizenk-0.1.50/PKG-INFO
```

### Comparing `citizenk-0.1.49/README.md` & `citizenk-0.1.50/README.md`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.49/citizenk/agent.py` & `citizenk-0.1.50/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.49/citizenk/citizenk.py` & `citizenk-0.1.50/citizenk/citizenk.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from confluent_kafka import KafkaException
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 
 from .agent import Agent, WebSocketAgent
 from .kafka_adapter import KafkaAdapter, KafkaConfig, KafkaRole
-from .topic import Topic, TopicDir
+from .topic import Topic, TopicDir, SchemaType
 from .utils import CitizenKError
 
 logger = logging.getLogger(__name__)
 
 
 class AppType(Enum):
     SOURCE = 1
@@ -343,24 +343,26 @@
                 await asyncio.sleep(3)
 
     def topic(
         self,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
+        schema_type: SchemaType = SchemaType.JSON,
         subject_name: Optional[str] = None,
         partitioner: Callable[[Union[str, bytes]], int] = None,
     ) -> Topic:
         if name in self.topics:
             raise CitizenKError(f"Topic {name} already exists")
         t = Topic(
             self,
             name=name,
             value_type=value_type,
             topic_dir=topic_dir,
+            schema_type=schema_type,
             subject_name=subject_name,
             partitioner=partitioner,
         )
         self.topics[name] = t
         logger.debug("Adding topic %s", name)
         return t
```

### Comparing `citizenk-0.1.49/citizenk/kafka_adapter.py` & `citizenk-0.1.50/citizenk/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.49/citizenk/murmur2.py` & `citizenk-0.1.50/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.49/citizenk/topic.py` & `citizenk-0.1.50/citizenk/topic.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING, Any, Callable
 
 from confluent_kafka.schema_registry import Schema, SchemaRegistryClient
 from confluent_kafka.schema_registry.avro import AvroDeserializer, AvroSerializer
 from confluent_kafka.serialization import SerializationError
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
+from pydantic_avro.base import AvroBase
 
 from .utils import CitizenKError, annotate_function
 
 if TYPE_CHECKING:
     from .citizenk import CitizenK
 
 logger = logging.getLogger(__name__)
@@ -134,30 +135,39 @@
     def manage_schema(self):
         """Handle schema registry registration and validation"""
         # https://yokota.blog/2021/03/29/understanding-json-schema-compatibility/
         if self.app.schema_registry_url is not None:
             # Schema registration
             schema_registry_conf = {"url": self.app.schema_registry_url}
             schema_registry_client = SchemaRegistryClient(schema_registry_conf)
+            if self.schema_type == SchemaType.AVRO:
+                schema_str=self.value_type.avro_schema()
+            elif self.schema_type == SchemaType.JSON:
+                schema_str=self.value_type.schema_json()
+            else:
+                raise CitizenKError("Unsupported schema type")
+            logger.debug(schema_str)
             schema = Schema(
-                schema_str=self.value_type.schema_json(),
+                schema_str=schema_str,
                 schema_type=self.schema_type.name,
             )
-            if self.topic_dir != TopicDir.OUTPUT:
+            # Schema registration for Output and Bidir topics
+            if self.topic_dir != TopicDir.INPUT:
                 if self.schema_type == SchemaType.AVRO:
-                    self.serializer = AvroSerializer(schema_registry_client, schema)
+                    self.serializer = AvroSerializer(schema_registry_client, schema_str)
+
                 schema_id = schema_registry_client.register_schema(
                     subject_name=self.subject_name, schema=schema
                 )
                 logger.info("Schema id registered for %s is %s", self.name, schema_id)
                 self.schema_id = schema_id
-            # Schema validation
-            if self.topic_dir != TopicDir.INPUT:
+            # Schema validation for Input and Bidir topics
+            if self.topic_dir != TopicDir.OUTPUT:
                 if self.schema_type == SchemaType.AVRO:
-                    self.deserializer = AvroDeserializer(schema_registry_client, schema)
+                    self.deserializer = AvroDeserializer(schema_registry_client, schema_str)
 
                 if not schema_registry_client.test_compatibility(
                     subject_name=self.subject_name, schema=schema
                 ):
                     logger.error(
                         "Schema for %s is not compatible with the latest schema registry",
                         self.name,
```

### Comparing `citizenk-0.1.49/pyproject.toml` & `citizenk-0.1.50/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.49"
+version = "0.1.50"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi", "confluent", "pydantic", "distributed", "real-time"]
@@ -26,14 +26,15 @@
 python = "^3.7"
 confluent-kafka = {extras = ["schema-registry","avro"], version = "2.0.2"}
 certifi = "^2022.12.7"
 fastapi = "^0.92.0"
 fastapi-utils = "^0.2.1"
 httpx = "^0.23.3"
 websockets = "^10.4"
+pydantic-avro = "^0.5.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 assertpy = "^1.1"
 pytest-xdist = "^2.5.0"
 pytest-mock = "^3.8.2"
 pytest-asyncio = "^0.21.0"
```

### Comparing `citizenk-0.1.49/PKG-INFO` & `citizenk-0.1.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.49
+Version: 0.1.50
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi,confluent,pydantic,distributed,real-time
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
@@ -28,14 +28,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: confluent-kafka[avro,schema-registry] (==2.0.2)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: pydantic-avro (>=0.5.1,<0.6.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Repository, https://github.com/Valerann/citizenk
 Description-Content-Type: text/markdown
 
 # CitizenK
 **CitizienK** is a simple but powerful Python Library for developing reactive async Kafka microservices, built on top of [Confluent Kafka Python](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html), [FastAPI](https://fastapi.tiangolo.com/) and [Pydantic](https://docs.pydantic.dev/).
```

