# Comparing `tmp/citizenk-0.1.48.tar.gz` & `tmp/citizenk-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.48.tar", max compression
+gzip compressed data, was "citizenk-0.1.49.tar", max compression
```

## Comparing `citizenk-0.1.48.tar` & `citizenk-0.1.49.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    18975 2023-06-16 13:57:46.346216 citizenk-0.1.48/README.md
--rw-r--r--   0        0        0      382 2023-06-11 19:27:45.145664 citizenk-0.1.48/citizenk/__init__.py
--rw-r--r--   0        0        0     8805 2023-06-11 19:27:45.145758 citizenk-0.1.48/citizenk/agent.py
--rw-r--r--   0        0        0    20706 2023-06-16 13:36:58.623566 citizenk-0.1.48/citizenk/citizenk.py
--rw-r--r--   0        0        0    24505 2023-06-16 13:36:28.101104 citizenk-0.1.48/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-06-11 19:27:45.146160 citizenk-0.1.48/citizenk/murmur2.py
--rw-r--r--   0        0        0     5664 2023-06-16 13:50:06.593517 citizenk-0.1.48/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-06-11 19:27:45.146294 citizenk-0.1.48/citizenk/utils.py
--rw-r--r--   0        0        0     1799 2023-06-16 13:57:45.883745 citizenk-0.1.48/pyproject.toml
--rw-r--r--   0        0        0    20639 1970-01-01 00:00:00.000000 citizenk-0.1.48/PKG-INFO
+-rw-r--r--   0        0        0    18975 2023-07-16 09:28:22.216839 citizenk-0.1.49/README.md
+-rw-r--r--   0        0        0      382 2023-06-11 19:27:45.145664 citizenk-0.1.49/citizenk/__init__.py
+-rw-r--r--   0        0        0     8794 2023-07-16 08:47:29.905433 citizenk-0.1.49/citizenk/agent.py
+-rw-r--r--   0        0        0    20708 2023-07-16 09:00:15.851212 citizenk-0.1.49/citizenk/citizenk.py
+-rw-r--r--   0        0        0    24499 2023-07-16 09:00:15.980386 citizenk-0.1.49/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-06-11 19:27:45.146160 citizenk-0.1.49/citizenk/murmur2.py
+-rw-r--r--   0        0        0     8055 2023-07-16 09:22:38.668288 citizenk-0.1.49/citizenk/topic.py
+-rw-r--r--   0        0        0      407 2023-07-16 09:00:15.900741 citizenk-0.1.49/citizenk/utils.py
+-rw-r--r--   0        0        0     1864 2023-07-16 09:28:11.749538 citizenk-0.1.49/pyproject.toml
+-rw-r--r--   0        0        0    20644 1970-01-01 00:00:00.000000 citizenk-0.1.49/PKG-INFO
```

### Comparing `citizenk-0.1.48/README.md` & `citizenk-0.1.49/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -86,30 +86,30 @@
 ### Creating CitizienK agents
 And lastly, we create gents that process the Kafka messages.
 
 Agents can listen to multiple topics and accept either values or the entire Kafka event (key, value, offset, partition, timestamp...)
 
 ``` python
 @app.agent(topics=t1, batch_size=100)
-async def process_videos_t1(events: List[KafkaEvent]):
+async def process_videos_t1(events: list[KafkaEvent]):
     # Process incoming video
     for event in events:
         camera_id = event.value.camera_id
         video_counts[camera_id] += 1
         v = ProcessedVideo(
             camera_id=camera_id,
             path=event.value.path,
             timestamp=event.value.timestamp,
             valid=bool(camera_id % 2),
         )
         t2.send(value=v, key=str(v.camera_id))
 
 
 @app.agent(topics=t2, batch_size=100)
-async def process_videos_t2(values: List[BaseModel]):
+async def process_videos_t2(values: list[BaseModel]):
     # Process incoming video
     for value in values:
         if value.valid:
             t3.send(value=value, key=str(value.camera_id))
 
 ```
 
@@ -126,15 +126,15 @@
 
 ### Creating additional CitizienK endpoints
 Just like any other FastAPI app, you can create get, post and put endpoints that either interact with Kafka or perform some other tasks, non Kafka related
 
 ``` python
 @router.post("/events", response_class=JSONResponse)
 async def produce_video_events(
-    values: List[Video],
+    values: list[Video],
     topic: str = Query(),
 ):
     """Sends events to the given topic"""
     if topic not in app.topics:
         raise HTTPException(status_code=400, detail="Topic not supported by app")
     t = app.topics[topic]
     for v in values:
@@ -174,15 +174,15 @@
 ```
 
 ### Websocket
 CitizenK support for Websocket agents
 
 ``` python
 @app.agent(topics=t2, batch_size=100, websocket_route=prefix + "/ws")
-async def websocket_agent(values: List[BaseModel]) -> str:
+async def websocket_agent(values: list[BaseModel]) -> str:
     values = [json.loads(v.json()) for v in values if not v.valid]
     return json.dumps(values, indent=4)
 ```
 
 This agent exposes a WebSocket endpoint for one or more clients to connect to. It then processes incoming Kafka messages from topic t2 and sends the returned string value to all the existing live WebSocket "/ws" connections. The main use case for this is to bridge between Kafka and Websocket. One possible use case for this feature is to send filtered Kafka events to a web app or mobile app.
```

### Comparing `citizenk-0.1.48/citizenk/agent.py` & `citizenk-0.1.49/citizenk/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 import logging
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, List
+from typing import TYPE_CHECKING, Any, Callable
 
 from confluent_kafka import Message as ConfluentMessage
 from fastapi import WebSocket, WebSocketDisconnect
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
 
 from .kafka_adapter import KafkaAdapter, KafkaRole
@@ -66,15 +66,15 @@
                 result = await self.coroutine(values=values)
                 return result
 
             annotate_function(
                 endpoint,
                 name=f"send_to_agent_{self.name}_from_{topic.name}",
                 doc=f"This endpoint sends value to agent {self.name} from topic {topic.name}",
-                argument_types={"values": List[topic.value_type]},
+                argument_types={"values": list[topic.value_type]},
             )
 
             self.app.add_api_route(
                 path=f"{self.app.api_router_prefix}/agent/{self.name}/{topic.name}",
                 response_class=JSONResponse,
                 methods=["POST"],
                 endpoint=endpoint,
@@ -86,20 +86,20 @@
     ) -> list[KafkaEvent]:
         """Validate the incoming Kafka messages"""
         events = []
         for msg in msgs:
             topic_name = msg.topic()
             topic = topics[topic_name]
             try:
-                value = topic.value_type(**json.loads(msg.value()))
-            except json.decoder.JSONDecodeError as e:
-                logger.error("For now, CitizenK only supports JSON values %s", e)
+                value = topic.deserialize(msg.value())
+            except json.decoder.JSONDecodeError as exp:
+                logger.error("For now, CitizenK only supports JSON values %s", exp)
                 continue
-            except ValidationError as e:
-                logger.error("Error while validating received value %s", e.json())
+            except ValidationError as exp:
+                logger.error("Error while validating received value %s", exp.json())
                 continue
 
             events.append(
                 KafkaEvent(
                     key=msg.key(),
                     value=value,
                     topic=topic,
@@ -220,15 +220,15 @@
                 await self.websocket_broadcast_result(result)
                 return result
 
             annotate_function(
                 endpoint,
                 name=f"send_to_websocket_agent_{self.name}_from_{topic.name}",
                 doc=f"This endpoint sends value to agent {self.name} from topic {topic.name}",
-                argument_types={"values": List[topic.value_type]},
+                argument_types={"values": list[topic.value_type]},
             )
 
             self.app.add_api_route(
                 path=f"{self.app.api_router_prefix}/agent/{self.name}/{topic.name}",
                 response_class=JSONResponse,
                 methods=["POST"],
                 endpoint=endpoint,
```

### Comparing `citizenk-0.1.48/citizenk/citizenk.py` & `citizenk-0.1.49/citizenk/citizenk.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import socket
 import threading
 import time
 from datetime import datetime
 from enum import Enum
 from functools import wraps
 from inspect import signature
-from typing import Callable, List, Optional, Union
+from typing import Callable, Optional, Union
 
 import httpx
 from confluent_kafka import KafkaException
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 
@@ -263,16 +263,16 @@
             self.background_loop.stop()
 
     def background_consumer_thread(self, loop: asyncio.BaseEventLoop):
         logger.debug("CitizenK background consumer thread started...")
         asyncio.set_event_loop(loop)
         try:
             loop.run_forever()
-        except asyncio.CancelledError as e:
-            logger.error("Background consumer loop cancelled %s", e)
+        except asyncio.CancelledError as exp:
+            logger.error("Background consumer loop cancelled %s", exp)
         finally:
             for task in asyncio.all_tasks():
                 logger.info("Stopping %s", task.get_name())
                 task.cancel()
             loop.run_until_complete(loop.shutdown_asyncgens())
             loop.stop()
             loop.close()
@@ -334,16 +334,16 @@
                     # Just to give other tasks opportunity to run
                     await asyncio.sleep(0)
                 else:
                     # Wait a bit until messages arrive
                     logger.debug("No kafka events, sleeping")
                     await asyncio.sleep(1)
 
-            except Exception as e:
-                logger.exception("Exception in main loop: %s", str(e))
+            except Exception as exp:
+                logger.exception("Exception in main loop: %s", str(exp))
                 await asyncio.sleep(3)
 
     def topic(
         self,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
@@ -362,24 +362,24 @@
         )
         self.topics[name] = t
         logger.debug("Adding topic %s", name)
         return t
 
     def agent(
         self,
-        topics: Union[Topic, List[Topic]],
+        topics: Union[Topic, list[Topic]],
         batch_size: int = 1,
         websocket_route: Optional[str] = None,
     ) -> Callable:
         """
         decorates a function of this type:
-        async def processing_agent(events: List[KafkaEvent])
+        async def processing_agent(events: list[KafkaEvent])
 
         Or this type:
-        async def processing_agent(values: List[BaseModel])
+        async def processing_agent(values: list[BaseModel])
 
         Both of these functions consumes from in_topics and produce to out_topics
         """
 
         if isinstance(topics, Topic):
             topics = [topics]
```

### Comparing `citizenk-0.1.48/citizenk/kafka_adapter.py` & `citizenk-0.1.49/citizenk/kafka_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import os
 import subprocess
 import sys
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Optional, Tuple, Union
 
 import certifi
 from confluent_kafka import (
     Consumer,
     ConsumerGroupTopicPartitions,
     KafkaError,
     KafkaException,
     Message,
     Producer,
     TopicPartition,
 )
 from confluent_kafka.admin import AdminClient, NewTopic
+
 from .murmur2 import murmur2_partition
 
 logger = logging.getLogger(__name__)
 
 
 class KafkaRole(Enum):
     ADMIN = 1
@@ -36,28 +37,28 @@
     """Kafka connection details"""
 
     bootstrap_servers: str
     tls: bool = True
     sasl_mechanism: str = "PLAIN"
     sasl_username: Optional[str] = None
     sasl_password: Optional[str] = None
-    extra_config: Optional[Dict[str, str]] = None
+    extra_config: Optional[dict[str, str]] = None
 
 
 class KafkaAdapter:
     """Kafka adapter Using confluent API"""
 
     def __init__(
         self,
         config: KafkaConfig,
         role: KafkaRole = KafkaRole.ADMIN,
         consumer_group_name: Optional[str] = None,
         consumer_group_init_offset: Optional[str] = "latest",
         consumer_group_auto_commit: Optional[bool] = True,
-        extra_config: Optional[Dict[str, str]] = None,
+        extra_config: Optional[dict[str, str]] = None,
     ):
         self.role = role
         self.consumer_group_name = consumer_group_name
         self.consumer_group_auto_commit = consumer_group_auto_commit
         self.consumer_started = False
         self.consumer_topics = {}
         self.assigned_partitions = defaultdict(set)
@@ -110,25 +111,25 @@
             self.config["partitioner"] = "murmur2"
             self.connection = Producer(self.config, logger=logger)
         else:
             self.connection = AdminClient(self.admin_config)
         metadata = self.connection.list_topics(timeout=10)
         logger.debug("Connected to %s cluster %s", self.role.name, metadata.cluster_id)
 
-    def get_all_broker_groups(self) -> List[str]:
+    def get_all_broker_groups(self) -> list[str]:
         connection = AdminClient(self.admin_config)
         future = connection.list_consumer_groups(request_timeout=10)
         try:
             groups = future.result()
         except KafkaException:
             logger.error("Failed to get consumer groups")
             return []
         return [g.group_id for g in groups.valid]
 
-    def get_group_members(self, groups: Optional[List[str]] = None) -> Dict[Tuple, str]:
+    def get_group_members(self, groups: Optional[list[str]] = None) -> dict[Tuple, str]:
         connection = AdminClient(self.admin_config)
         if groups is None:
             if self.consumer_group_name is None:
                 return {}
             groups = [self.consumer_group_name]
         members = {}
         future_map = connection.describe_consumer_groups(groups, request_timeout=10)
@@ -157,40 +158,40 @@
         """Get list of all topics in the broker"""
         topics = self.connection.list_topics(topic, timeout=10).topics
         if len(topics) == 0:
             return 0
         else:
             return len(topics[topic].partitions)
 
-    def get_all_broker_topics(self) -> Dict[str, Any]:
+    def get_all_broker_topics(self) -> dict[str, Any]:
         """Get list of all topics in the broker"""
         topics = self.connection.list_topics(timeout=10).topics
         return {
             topic_name: topic
             for topic_name, topic in topics.items()
             if not topic_name.startswith("__")
         }
 
-    def get_all_broker_partitions(self) -> List[TopicPartition]:
+    def get_all_broker_partitions(self) -> list[TopicPartition]:
         """Get list of all partiotions in the broker"""
         topics = self.get_all_broker_topics()
         return [
             TopicPartition(topic_name, p)
             for topic_name, topic in topics.items()
             for p in topic.partitions
         ]
 
     def get_partitions_with_offsets(
         self,
-        topics: List[str],
+        topics: list[str],
         strategy: str = "latest",
         x: int = 0,
         epoch: int = 0,
-        partition_filter: List[int] = [],
-    ) -> List[TopicPartition]:
+        partition_filter: list[int] = [],
+    ) -> list[TopicPartition]:
         """
         Get a list of partitions in the broker for the given topics
         And set offsets based on the specified strategy:
             p = num partitions
             latest-x/p
             earielst+x/p
             x
@@ -261,15 +262,15 @@
         for topic, f in fs.items():
             try:
                 f.result()  # The result itself is None
                 logger.debug("Topic %s created", topic)
             except KafkaException as ex:
                 logger.error("Failed to create topic %s: %s", topic, ex)
 
-    def get_own_group_topics(self) -> List[str]:
+    def get_own_group_topics(self) -> list[str]:
         """Get a list of all the topics in the replicator consumer group"""
         if self.role != KafkaRole.CONSUMER or self.consumer_group_name is None:
             return []
 
         group_topics = set()
         partitions = self.get_all_broker_partitions()
         # Find which topic has stored offset for the group
@@ -284,27 +285,27 @@
             return []
 
         for p in committed:
             if p.offset > 0:
                 group_topics.add(p.topic)
         return list(group_topics)
 
-    def get_group_lag(self) -> Dict[str, int]:
+    def get_group_lag(self) -> dict[str, int]:
         """Get the total lag of the group for each topic"""
         group_topics = defaultdict(int)
         if self.role != KafkaRole.CONSUMER or self.consumer_group_name is None:
             return group_topics
 
         partitions = self.get_all_broker_partitions()
         try:
             committed = self.connection.committed(partitions, timeout=10)
             for p in committed:
                 if p.offset >= 0:
                     (_, hi) = self.connection.get_watermark_offsets(
-                        p, timeout=10, cached=False
+                        p, timeout=10, cached=True
                     )
                     if hi < 0:
                         continue
                     topic = p.topic
                     lag = hi - p.offset
                     group_topics[topic] += lag
             logger.debug(
@@ -316,15 +317,15 @@
                 self.consumer_group_name,
                 ex,
             )
             return group_topics
 
         return group_topics
 
-    def delete_groups(self, groups: List[str]) -> int:
+    def delete_groups(self, groups: list[str]) -> int:
         """Delete the given consumer groups"""
         if len(groups) == 0:
             return 0
         connection = AdminClient(self.admin_config)
         future_map = connection.delete_consumer_groups(groups, request_timeout=10)
         count = 0
         for group_id, future in future_map.items():
@@ -415,15 +416,15 @@
             )
         else:
             logger.debug(
                 "Successfully deleted offsets for group %s topic %s", group, topic
             )
         return error_code
 
-    def group_ops(self, group: str, ops_params: Dict[str, str]) -> int:
+    def group_ops(self, group: str, ops_params: dict[str, str]) -> int:
         """
         Perform the given ops on the group
 
         Which op:
         --describe
         --delete to delete the group
         --delete-offsets to delete offsets for a topic / all topics
@@ -492,19 +493,19 @@
                 logger.info("topic %s is no longer replicated, deleting offsets", t)
                 self.delete_offset_for_group(self.consumer_group_name, t)
                 count += 1
         return count
 
     def start_consumer(
         self,
-        topics: List[str],
+        topics: list[str],
         count: int = 0,
         strategy: str = "latest",
         epoch: int = 0,
-        partition_filter: List[int] = [],
+        partition_filter: list[int] = [],
     ):
         """Start the consumer with the given topics. offset = latest-n"""
         self.stop_consumer()
 
         if self.consumer_group_name is not None:
             # Subscribe to desired source topics
             logger.debug("Subscribing to %s", topics)
@@ -540,97 +541,97 @@
         elif isinstance(key, bytes):
             return key.decode()
         else:
             logger.error("Unexpected key type %s", type(key))
             return str(key)
 
     @staticmethod
-    def messages_to_dict(messages: List[Message]) -> List[Dict[str, Any]]:
+    def messages_to_dict(messages: list[Message]) -> list[dict[str, Any]]:
         try:
             return [
                 {
                     "topic": m.topic(),
                     "key": KafkaAdapter.stringify_key(m.key()),
                     "value": json.loads(m.value()),
                     "partition": m.partition(),
                     "offset": m.offset(),
                     "timestamp": m.timestamp()[1],
                 }
                 for m in messages
             ]
-        except json.decoder.JSONDecodeError as e:
-            logger.debug("JSON Decode error %s", e)
+        except json.decoder.JSONDecodeError as exp:
+            logger.debug("JSON Decode error %s", exp)
             return []
 
-    def consume(self, num_messages: int = 1, timeout: float = 1.0) -> List[Message]:
+    def consume(self, num_messages: int = 1, timeout: float = 1.0) -> list[Message]:
         """Consume records from the topics"""
         confluent_msgs = self.connection.consume(num_messages, timeout)
         msgs = []
         for msg in confluent_msgs:
             error = msg.error()
             if error is None:
                 msgs.append(msg)
             else:
                 self._on_kafka_error(error)
             self.topic_stats[msg.topic()] += 1
         logger.debug("Consumed %s Kafka messages", len(msgs))
         return msgs
 
-    def commit(self,msgs:List[Message]):
+    def commit(self, msgs: list[Message]):
         if self.consumer_group_name is None:
             return
         if self.consumer_group_auto_commit:
             return
         self.connection.commit(msgs)
 
     def produce(
         self,
         topic: str,
         value: Any,
         key: Optional[Any] = None,
         partition: int = -1,
-        headers: Optional[Dict[str, bytes]] = None,
+        headers: Optional[dict[str, bytes]] = None,
     ):
         if not isinstance(key, bytes):
             key = str(key).encode()
         """Produce a message to the given topic"""
         self.topic_stats[topic] += 1
         self.connection.produce(
             topic, value=value, key=key, partition=partition, headers=headers
         )
 
-    def _on_kafka_commit(self, err: KafkaError, partitions: List[TopicPartition]):
+    def _on_kafka_commit(self, err: KafkaError, partitions: list[TopicPartition]):
         logger.debug("Kafka committed %s %s", err, partitions)
 
     def _on_kafka_stats(self, json_str: str):
         self.last_stats = json.loads(json_str)
 
     def _on_kafka_error(self, err: KafkaError):
         self.kafka_error = err
         logger.error("Kafka error %s", err)
 
-    def _on_kafka_assign(self, consumer, partitions: List[TopicPartition]):
+    def _on_kafka_assign(self, consumer, partitions: list[TopicPartition]):
         logger.info("Group rebalancing. Partitions assigned %s", partitions)
         for p in partitions:
             self.assigned_partitions[p.topic].add(p.partition)
 
-    def _on_kafka_revoke(self, consumer, partitions: List[TopicPartition]):
+    def _on_kafka_revoke(self, consumer, partitions: list[TopicPartition]):
         logger.info("Group rebalancing. Partition revoked %s", partitions)
         for p in partitions:
             self.assigned_partitions[p.topic].discard(p.partition)
 
-    def _on_kafka_lost(self, consumer, partitions: List[TopicPartition]):
+    def _on_kafka_lost(self, consumer, partitions: list[TopicPartition]):
         logger.info("Group rebalancing. Partitions lost %s", partitions)
         for p in partitions:
             self.assigned_partitions[p.topic].discard(p.partition)
 
     def is_assigned(self, topic):
         return len(self.assigned_partitions[topic]) > 0
 
-    def get_topic_stats(self) -> Dict[str, int]:
+    def get_topic_stats(self) -> dict[str, int]:
         result = self.topic_stats
         self.topic_stats = defaultdict(int)
         return result
 
     def messages_in_queue(self) -> int:
         if self.role != KafkaRole.PRODUCER:
             return 0
```

### Comparing `citizenk-0.1.48/citizenk/murmur2.py` & `citizenk-0.1.49/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.48/citizenk/topic.py` & `citizenk-0.1.49/citizenk/topic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
+import json
 import logging
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable
 
 from confluent_kafka.schema_registry import Schema, SchemaRegistryClient
+from confluent_kafka.schema_registry.avro import AvroDeserializer, AvroSerializer
+from confluent_kafka.serialization import SerializationError
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, ValidationError
 
 from .utils import CitizenKError, annotate_function
 
 if TYPE_CHECKING:
     from .citizenk import CitizenK
@@ -24,47 +27,58 @@
 
 class TopicDir(Enum):
     INPUT = 1
     OUTPUT = 2
     BIDIR = 3
 
 
+class SchemaType(Enum):
+    JSON = 1
+    AVRO = 2
+    PROTOBUF = 3
+
+
 class Topic:
     def __init__(
         self,
         app: CitizenK,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
+        schema_type: SchemaType = SchemaType.JSON,
         subject_name: str | None = None,
         partitioner: Callable[[str | bytes], int] = None,
     ):
         self.app = app
         self.name = name
         self.value_type = value_type
         self.topic_dir = topic_dir
+        self.schema_type = schema_type
         self.subject_name = (
             f"{name}-value".lower() if subject_name is None else subject_name
         )
         self.schema_id = None
         self.partitioner = partitioner
         self.partition_count = None
         self.replica_count = None
         if self.app.auto_generate_apis:
             self._generate_apis()
 
         # Register topic schema
+        self.serializer = None
+        self.deserializer = None
         self.manage_schema()
 
     def info(self, lags: dict[str, int] = {}, assignments: dict[str, list[int]] = {}):
         topic_info = {
             "name": self.name,
             "dir": self.topic_dir.name,
             "value": self.value_type.__name__,
             "subject": self.subject_name,
+            "schema_type": self.schema_type.name,
             "partitions": self.partition_count,
             "replicas": self.replica_count,
         }
         if self.name in lags:
             topic_info["lag"] = lags[self.name]
         if self.name in assignments:
             topic_info["assignments"] = assignments[self.name]
@@ -100,62 +114,109 @@
         key: str | bytes = None,
         partition: int = -1,
     ):
         if self.app.is_sink():
             raise CitizenKError("Trying to produce in a sink app")
         if self.topic_dir == TopicDir.INPUT:
             raise CitizenKError("Trying to produce to an input topic")
-
-        if isinstance(value, dict):
-            try:
-                value = self.value_type(**value)
-            except ValidationError as e:
-                logger.error("Error while validating send value %s", e.json())
-                return False
-        if not isinstance(value, BaseModel):
-            raise CitizenKError("Value should be a pydantic model", value)
+        value = self.serialize(value)
+        if value is None:
+            return False
         if not isinstance(key, (str, bytes)):
             raise CitizenKError("Key should be a either a str or bytes", key)
         if self.partitioner is not None and partition == -1:
             partition = self.partitioner(key)
         # TODO: Add schema to headers
         self.app.producer.produce(
-            topic=self.name, value=value.json(), key=key, partition=partition
+            topic=self.name, value=value, key=key, partition=partition
         )
         return True
 
     def manage_schema(self):
         """Handle schema registry registration and validation"""
         # https://yokota.blog/2021/03/29/understanding-json-schema-compatibility/
         if self.app.schema_registry_url is not None:
             # Schema registration
             schema_registry_conf = {"url": self.app.schema_registry_url}
             schema_registry_client = SchemaRegistryClient(schema_registry_conf)
             schema = Schema(
-                schema_str=self.value_type.schema_json(), schema_type="JSON"
+                schema_str=self.value_type.schema_json(),
+                schema_type=self.schema_type.name,
             )
-            if self.topic_dir != TopicDir.INPUT:
+            if self.topic_dir != TopicDir.OUTPUT:
+                if self.schema_type == SchemaType.AVRO:
+                    self.serializer = AvroSerializer(schema_registry_client, schema)
                 schema_id = schema_registry_client.register_schema(
                     subject_name=self.subject_name, schema=schema
                 )
                 logger.info("Schema id registered for %s is %s", self.name, schema_id)
                 self.schema_id = schema_id
             # Schema validation
-            if self.topic_dir != TopicDir.OUTPUT:
+            if self.topic_dir != TopicDir.INPUT:
+                if self.schema_type == SchemaType.AVRO:
+                    self.deserializer = AvroDeserializer(schema_registry_client, schema)
+
                 if not schema_registry_client.test_compatibility(
                     subject_name=self.subject_name, schema=schema
                 ):
                     logger.error(
                         "Schema for %s is not compatible with the latest schema registry",
                         self.name,
                     )
                 else:
                     logger.info(
                         "Schema for %s is compatible with the latest schema registry",
                         self.name,
                     )
+        elif self.schema_type == SchemaType.AVRO:
+            raise CitizenKError("AVRO Schema requires a schema registry")
+
+    def serialize(self, value: dict[Any, Any] | BaseModel) -> bytes:
+        if isinstance(value, dict):
+            try:
+                value = self.value_type(**value)
+            except ValidationError as exp:
+                logger.error("Error while validating send value %s", exp.json())
+                return None
+        if not isinstance(value, BaseModel):
+            raise CitizenKError("Value should be a pydantic model", value)
+        if self.schema_type == SchemaType.JSON:
+            return value.json()
+        elif self.schema_type == SchemaType.AVRO:
+            try:
+                return self.serializer(value)
+            except SerializationError:
+                logger.error("Failed to serialise value %s", value)
+                return None
+        else:
+            raise CitizenKError("No available serializer")
+
+    def deserialize(self, value: bytes) -> BaseModel:
+        # convert bytes to dict
+        if self.schema_type == SchemaType.JSON:
+            try:
+                value = json.loads(value)
+            except json.decoder.JSONDecodeError as exp:
+                logger.error("For now, CitizenK only supports JSON values %s", exp)
+                return None
+        elif self.schema_type == SchemaType.AVRO:
+            try:
+                value = self.deserializer(value)
+            except SerializationError as exp:
+                logger.error("Failed to deserialise value %s", exp.json())
+                return None
+        else:
+            raise CitizenKError("No available serializer")
+
+        # convert dict to pydantic model
+        try:
+            value = self.value_type(**value)
+        except ValidationError as exp:
+            logger.error("Error while validating received value %s", exp.json())
+            return None
+        return value
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
```

### Comparing `citizenk-0.1.48/pyproject.toml` & `citizenk-0.1.49/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.48"
+version = "0.1.49"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi", "confluent", "pydantic", "distributed", "real-time"]
@@ -20,15 +20,15 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-confluent-kafka = {extras = ["schema-registry"], version = "2.0.2"}
+confluent-kafka = {extras = ["schema-registry","avro"], version = "2.0.2"}
 certifi = "^2022.12.7"
 fastapi = "^0.92.0"
 fastapi-utils = "^0.2.1"
 httpx = "^0.23.3"
 websockets = "^10.4"
 
 [tool.poetry.dev-dependencies]
@@ -36,14 +36,17 @@
 assertpy = "^1.1"
 pytest-xdist = "^2.5.0"
 pytest-mock = "^3.8.2"
 pytest-asyncio = "^0.21.0"
 websocket-client = "^1.5.1"
 pytest-dotenv = "^0.5.2"
 
+[tool.poetry.group.dev.dependencies]
+coverage = "^7.2.7"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
     py36 = true
     include = '\.pyi?$'
```

### Comparing `citizenk-0.1.48/PKG-INFO` & `citizenk-0.1.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.48
+Version: 0.1.49
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi,confluent,pydantic,distributed,real-time
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
-Requires-Dist: confluent-kafka[schema-registry] (==2.0.2)
+Requires-Dist: confluent-kafka[avro,schema-registry] (==2.0.2)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Repository, https://github.com/Valerann/citizenk
 Description-Content-Type: text/markdown
 
@@ -124,30 +124,30 @@
 ### Creating CitizienK agents
 And lastly, we create gents that process the Kafka messages.
 
 Agents can listen to multiple topics and accept either values or the entire Kafka event (key, value, offset, partition, timestamp...)
 
 ``` python
 @app.agent(topics=t1, batch_size=100)
-async def process_videos_t1(events: List[KafkaEvent]):
+async def process_videos_t1(events: list[KafkaEvent]):
     # Process incoming video
     for event in events:
         camera_id = event.value.camera_id
         video_counts[camera_id] += 1
         v = ProcessedVideo(
             camera_id=camera_id,
             path=event.value.path,
             timestamp=event.value.timestamp,
             valid=bool(camera_id % 2),
         )
         t2.send(value=v, key=str(v.camera_id))
 
 
 @app.agent(topics=t2, batch_size=100)
-async def process_videos_t2(values: List[BaseModel]):
+async def process_videos_t2(values: list[BaseModel]):
     # Process incoming video
     for value in values:
         if value.valid:
             t3.send(value=value, key=str(value.camera_id))
 
 ```
 
@@ -164,15 +164,15 @@
 
 ### Creating additional CitizienK endpoints
 Just like any other FastAPI app, you can create get, post and put endpoints that either interact with Kafka or perform some other tasks, non Kafka related
 
 ``` python
 @router.post("/events", response_class=JSONResponse)
 async def produce_video_events(
-    values: List[Video],
+    values: list[Video],
     topic: str = Query(),
 ):
     """Sends events to the given topic"""
     if topic not in app.topics:
         raise HTTPException(status_code=400, detail="Topic not supported by app")
     t = app.topics[topic]
     for v in values:
@@ -212,15 +212,15 @@
 ```
 
 ### Websocket
 CitizenK support for Websocket agents
 
 ``` python
 @app.agent(topics=t2, batch_size=100, websocket_route=prefix + "/ws")
-async def websocket_agent(values: List[BaseModel]) -> str:
+async def websocket_agent(values: list[BaseModel]) -> str:
     values = [json.loads(v.json()) for v in values if not v.valid]
     return json.dumps(values, indent=4)
 ```
 
 This agent exposes a WebSocket endpoint for one or more clients to connect to. It then processes incoming Kafka messages from topic t2 and sends the returned string value to all the existing live WebSocket "/ws" connections. The main use case for this is to bridge between Kafka and Websocket. One possible use case for this feature is to send filtered Kafka events to a web app or mobile app.
```

