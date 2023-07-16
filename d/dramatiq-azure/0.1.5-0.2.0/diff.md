# Comparing `tmp/dramatiq_azure-0.1.5.tar.gz` & `tmp/dramatiq_azure-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_azure-0.1.5.tar", max compression
+gzip compressed data, was "dramatiq_azure-0.2.0.tar", max compression
```

## Comparing `dramatiq_azure-0.1.5.tar` & `dramatiq_azure-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2022-03-02 04:17:32.887185 dramatiq_azure-0.1.5/LICENSE
--rw-r--r--   0        0        0     2755 2022-03-02 04:17:32.887185 dramatiq_azure-0.1.5/README.md
--rw-r--r--   0        0        0       52 2022-03-02 04:17:32.887185 dramatiq_azure-0.1.5/dramatiq_azure/__init__.py
--rw-r--r--   0        0        0     8087 2022-03-02 04:17:32.887185 dramatiq_azure-0.1.5/dramatiq_azure/asq.py
--rw-r--r--   0        0        0      910 2022-03-02 04:17:32.887185 dramatiq_azure-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3615 2022-03-02 04:17:43.042131 dramatiq_azure-0.1.5/setup.py
--rw-r--r--   0        0        0     3678 2022-03-02 04:17:43.042447 dramatiq_azure-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-16 18:27:59.930139 dramatiq_azure-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2459 2023-07-16 18:27:59.930139 dramatiq_azure-0.2.0/README.md
+-rw-r--r--   0        0        0       52 2023-07-16 18:27:59.930139 dramatiq_azure-0.2.0/dramatiq_azure/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-16 18:27:59.930139 dramatiq_azure-0.2.0/dramatiq_azure/__version__.py
+-rw-r--r--   0        0        0     8561 2023-07-16 18:27:59.930139 dramatiq_azure-0.2.0/dramatiq_azure/asq.py
+-rw-r--r--   0        0        0     1435 2023-07-16 18:27:59.934139 dramatiq_azure-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 dramatiq_azure-0.2.0/PKG-INFO
```

### Comparing `dramatiq_azure-0.1.5/LICENSE` & `dramatiq_azure-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq_azure-0.1.5/README.md` & `dramatiq_azure-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # dramatiq-azure
 [![CI](https://github.com/bidossessi/dramatiq-azure/actions/workflows/ci.yml/badge.svg)](https://github.com/bidossessi/dramatiq-azure/actions/workflows/ci.yml)
 [![Pypi](https://github.com/bidossessi/dramatiq-azure/actions/workflows/python-publish.yml/badge.svg)](https://github.com/bidossessi/dramatiq-azure/actions/workflows/python-publish.yml)
 [![codecov](https://codecov.io/gh/bidossessi/dramatiq-azure/branch/main/graph/badge.svg?token=6LLEDAM3SG)](https://codecov.io/gh/bidossessi/dramatiq-azure)
-[![BCH compliance](https://bettercodehub.com/edge/badge/bidossessi/dramatiq-azure?branch=main)](https://bettercodehub.com/)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/bidossessi/dramatiq-azure.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/bidossessi/dramatiq-azure/alerts/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
 
 
 A [Dramatiq](https://dramatiq.io) broker that can be used with [Microsoft Azure](https://azure.microsoft.com/en-us/) queue services.
 
 Heavily inspired by [Dramatiq SQS](https://github.com/Bogdanp/dramatiq_sqs), this package currently implements a broker for [Azure Storage Queue](https://docs.microsoft.com/en-us/azure/storage/queues/).
```

### Comparing `dramatiq_azure-0.1.5/dramatiq_azure/asq.py` & `dramatiq_azure-0.2.0/dramatiq_azure/asq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from dataclasses import dataclass
-from typing import Iterable, List, Optional
-import time
+import logging
 import os
+import time
+from dataclasses import dataclass
+from typing import (
+    Iterable,
+    List,
+    Optional,
+)
+
 import dramatiq
 from azure.core.exceptions import (
-    ResourceExistsError,
     HttpResponseError,
+    ResourceExistsError,
 )
 from azure.storage.queue import (
-    QueueClient,
-    BinaryBase64EncodePolicy,
     BinaryBase64DecodePolicy,
+    BinaryBase64EncodePolicy,
+    QueueClient,
     QueueMessage,
 )
-
-
-import logging
-
 from dramatiq.common import compute_backoff
 
 # Set the logging level for all azure-storage-* libraries
 azure_logger = logging.getLogger("azure")
 azure_logger.setLevel(logging.WARNING)
 
 
@@ -33,62 +35,68 @@
 #: The minimum time to wait between polls in second.
 MIN_TIMEOUT = int(os.getenv("DRAMATIQ_ASQ_MIN_TIMEOUT", "20"))
 
 #: to the dead-letter queue (if enabled).
 MAX_RECEIVES = 3
 
 #: Azure Storage authentication
-CONN_STR = os.getenv("AZURE_STORAGE_CONNECTION_STR")
+CONN_STR = os.getenv("AZURE_STORAGE_CONNECTION_STR", "")
 
 
-def _get_client(queue_name) -> QueueClient:
+def _get_client(queue_name: str) -> QueueClient:
     return QueueClient.from_connection_string(
         conn_str=CONN_STR,
         queue_name=queue_name,
         message_encode_policy=BinaryBase64EncodePolicy(),
         message_decode_policy=BinaryBase64DecodePolicy(),
     )
 
 
-def _get_dlq_client(queue_name) -> QueueClient:
+def _get_dlq_client(queue_name: str) -> QueueClient:
     dlqueue_name = f"{queue_name}-dlq"
     return _get_client(dlqueue_name)
 
 
 @dataclass
 class ConsumerOptions:
     queue_name: str
     prefetch: int
     timeout: int
     dead_letter: bool = False
 
 
 class _ASQMessage(dramatiq.MessageProxy):
-    def __init__(self, asq_message: QueueMessage, message: dramatiq.Message) -> None:
+    def __init__(
+        self, asq_message: QueueMessage, message: dramatiq.Message
+    ) -> None:
         super().__init__(message)
         # force type hint
         self.message_id = message.message_id
         self._message = message
         self._asq_message = asq_message
 
     @classmethod
     def from_queue_message(cls, _message: QueueMessage):
         dramatiq_message = dramatiq.Message.decode(_message.content)
         return cls(_message, dramatiq_message)
 
 
-class _ASQConsumer(dramatiq.Consumer):
-    def __init__(self, broker: dramatiq.Broker, options: ConsumerOptions) -> None:
+class ASQConsumer(dramatiq.Consumer):
+    def __init__(
+        self, broker: dramatiq.Broker, options: ConsumerOptions
+    ) -> None:
         self.prefetch = min(options.prefetch, MAX_PREFETCH)
         self.timeout = options.timeout
         self.visibility_timeout = int(options.timeout / 1000)
         self.queue_name = options.queue_name
         self.dead_letter = options.dead_letter
         self.q_client = _get_client(options.queue_name)
-        self.dlq_client = _get_dlq_client(options.queue_name) if options.dead_letter else None
+        self.dlq_client = (
+            _get_dlq_client(options.queue_name) if options.dead_letter else None
+        )
 
         # local cache
         self.message_cache: List[_ASQMessage] = []
         self.queued_message_ids = set()
         self.misses = 0
 
     @property
@@ -125,26 +133,31 @@
                 self.misses = 0
                 self.queued_message_ids.add(match.message_id)
                 return match
             except IndexError:
                 msg_batch = []
                 if self.outstanding_message_count < self.prefetch:
                     fillout = self.prefetch - self.outstanding_message_count
-                    pager = self.q_client.receive_messages(
-                        messages_per_page=fillout,
-                        visibility_timeout=self.visibility_timeout,
-                    )
+                    kw = {"messages_per_page": fillout}
+                    if self.visibility_timeout is not None:
+                        kw["visibility_timeout"] = self.visibility_timeout
+                    pager = self.q_client.receive_messages(**kw)
                     try:
                         msg_batch = [item for item in next(pager.by_page())]
-                        self.message_cache = [_ASQMessage.from_queue_message(_msg) for _msg in msg_batch]
+                        self.message_cache = [
+                            _ASQMessage.from_queue_message(_msg)
+                            for _msg in msg_batch
+                        ]
                     except StopIteration:
                         self.message_cache = []
 
                 if not msg_batch:
-                    self.misses, backoff_ms = compute_backoff(self.misses, max_backoff=self.timeout)
+                    self.misses, backoff_ms = compute_backoff(
+                        self.misses, max_backoff=self.timeout
+                    )
                     time.sleep(backoff_ms / 1000)
                     return None
 
 
 class ASQBroker(dramatiq.Broker):
     """A Dramatiq_ broker that can be used with `Azure Storage Queues`_
     This backend has a number of limitations compared to the built-in
@@ -165,30 +178,36 @@
         dead_letter: bool = False,
         middleware=None,
     ) -> None:
         super().__init__(middleware=middleware)
         self.queues: set = set()
         self.dead_letter = dead_letter
 
+    @property
+    def consumer_class(self):
+        """Allows overriding the default consumer"""
+        return ASQConsumer
+
     def validate_queue(self, queue_name: str):
         if queue_name not in self.queues:
             raise dramatiq.errors.QueueNotFound(queue_name)
 
-    def consume(self, queue_name: str, prefetch: int = 1, timeout: int = 5000) -> dramatiq.Consumer:
+    def consume(
+        self, queue_name: str, prefetch: int = 1, timeout: int = 5000
+    ) -> dramatiq.Consumer:
         self.validate_queue(queue_name)
         options = ConsumerOptions(
             queue_name=queue_name,
             prefetch=prefetch,
             timeout=timeout,
             dead_letter=self.dead_letter,
         )
-        return _ASQConsumer(self, options)
+        return self.consumer_class(self, options)
 
     def declare_queue(self, queue_name: str) -> None:
-
         if queue_name not in self.queues:
             self.emit_before("declare_queue", queue_name)
             try:
                 q_client = _get_client(queue_name)
                 q_client.create_queue()
             except ResourceExistsError:
                 logger.warning(f"Queue already exists: {queue_name}")
@@ -197,25 +216,31 @@
                     dlq_client = _get_dlq_client(queue_name)
                     dlq_client.create_queue()
                 except ResourceExistsError:
                     logger.warning(f"DL Queue already exists: {queue_name}")
             self.queues.add(queue_name)
             self.emit_after("declare_queue", queue_name)
 
-    def enqueue(self, message: dramatiq.Message, *, delay: Optional[int] = None) -> dramatiq.Message:
+    def enqueue(
+        self, message: dramatiq.Message, *, delay: Optional[int] = None
+    ) -> dramatiq.Message:
         queue_name = message.queue_name
         self.validate_queue(queue_name)
 
         delay_sec = int(delay / 1000) if delay else 0
 
-        logger.debug(f"Enqueueing message {message.message_id} on queue {queue_name}.")
+        logger.debug(
+            f"Enqueueing message {message.message_id} on queue {queue_name}."
+        )
         self.emit_before("enqueue", message, delay)
         q_client = _get_client(queue_name)
         try:
-            q_client.send_message(message.encode(), visibility_timeout=delay_sec)
+            q_client.send_message(
+                message.encode(), visibility_timeout=delay_sec
+            )
             self.emit_after("enqueue", message, delay)
             return message
         except HttpResponseError as e:
             raise RuntimeError(str(e))
 
     def flush(self, queue_name: str):
         self.validate_queue(queue_name)
```

### Comparing `dramatiq_azure-0.1.5/PKG-INFO` & `dramatiq_azure-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 Metadata-Version: 2.1
 Name: dramatiq-azure
-Version: 0.1.5
+Version: 0.2.0
 Summary: Azure Queue Brokers for Dramatiq
 Home-page: https://github.com/bidossessi/dramatiq-azure
 License: Apache-2.0
 Keywords: dramatiq,azure,queue,broker
 Author: Stanislas H.B. Sodonon
 Author-email: stanislas.sodonon@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-core (>=1.20.1,<2.0.0)
 Requires-Dist: azure-storage-queue (>=12.1.6,<13.0.0)
 Requires-Dist: dramatiq (>=1.12.0,<2.0.0)
-Requires-Dist: pre-commit (>=2.17.0,<3.0.0)
 Project-URL: Repository, https://github.com/bidossessi/dramatiq-azure
 Description-Content-Type: text/markdown
 
 # dramatiq-azure
 [![CI](https://github.com/bidossessi/dramatiq-azure/actions/workflows/ci.yml/badge.svg)](https://github.com/bidossessi/dramatiq-azure/actions/workflows/ci.yml)
 [![Pypi](https://github.com/bidossessi/dramatiq-azure/actions/workflows/python-publish.yml/badge.svg)](https://github.com/bidossessi/dramatiq-azure/actions/workflows/python-publish.yml)
 [![codecov](https://codecov.io/gh/bidossessi/dramatiq-azure/branch/main/graph/badge.svg?token=6LLEDAM3SG)](https://codecov.io/gh/bidossessi/dramatiq-azure)
-[![BCH compliance](https://bettercodehub.com/edge/badge/bidossessi/dramatiq-azure?branch=main)](https://bettercodehub.com/)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/bidossessi/dramatiq-azure.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/bidossessi/dramatiq-azure/alerts/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
 
 
 A [Dramatiq](https://dramatiq.io) broker that can be used with [Microsoft Azure](https://azure.microsoft.com/en-us/) queue services.
 
 Heavily inspired by [Dramatiq SQS](https://github.com/Bogdanp/dramatiq_sqs), this package currently implements a broker for [Azure Storage Queue](https://docs.microsoft.com/en-us/azure/storage/queues/).
```

