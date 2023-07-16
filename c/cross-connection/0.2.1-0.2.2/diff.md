# Comparing `tmp/cross_connection-0.2.1-py3-none-any.whl.zip` & `tmp/cross_connection-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,63 +1,64 @@
-Zip file size: 33935 bytes, number of entries: 61
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/__init__.py
--rw-r--r--  2.0 unx     1750 b- defN 22-Nov-27 13:12 cconn/connection.py
--rw-r--r--  2.0 unx     1180 b- defN 22-Oct-31 08:21 cconn/connection_factory.py
--rw-r--r--  2.0 unx      206 b- defN 22-Oct-28 06:03 cconn/module.py
--rw-r--r--  2.0 unx      908 b- defN 22-Oct-31 08:21 cconn/server.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/comm/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:06 cconn/comm/base/__init__.py
--rw-r--r--  2.0 unx      444 b- defN 22-Oct-28 06:03 cconn/comm/base/comm.py
--rw-r--r--  2.0 unx     8700 b- defN 22-Dec-07 14:44 cconn/comm/base/comm_handler.py
--rw-r--r--  2.0 unx      793 b- defN 22-Nov-22 14:06 cconn/comm/base/comm_server_wrapper.py
--rw-r--r--  2.0 unx     4199 b- defN 22-Nov-27 15:17 cconn/comm/base/msg.py
--rw-r--r--  2.0 unx      428 b- defN 22-Oct-28 06:03 cconn/comm/base/topic_mapper.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/comm/base/pubsub/__init__.py
--rw-r--r--  2.0 unx     1316 b- defN 22-Oct-28 06:03 cconn/comm/base/pubsub/client_comm_pubsub_manager.py
--rw-r--r--  2.0 unx     2976 b- defN 22-Nov-27 15:17 cconn/comm/base/pubsub/server_comm_pubsub_manager.py
--rw-r--r--  2.0 unx      231 b- defN 22-Oct-28 06:03 cconn/comm/base/pubsub/subscription.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-31 08:38 cconn/comm/bus/__init__.py
--rw-r--r--  2.0 unx      726 b- defN 22-Oct-31 08:39 cconn/comm/bus/bus.py
--rw-r--r--  2.0 unx     3538 b- defN 22-Nov-22 14:34 cconn/comm/bus/cross_connection_bus.py
--rw-r--r--  2.0 unx      233 b- defN 22-Oct-31 08:38 cconn/comm/bus/server_struct.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/comm/tcp/__init__.py
--rw-r--r--  2.0 unx      689 b- defN 22-Dec-13 07:39 cconn/comm/tcp/tcp_comm.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/comm/tcp/client/__init__.py
--rw-r--r--  2.0 unx    12059 b- defN 22-Dec-07 14:26 cconn/comm/tcp/client/tcp_client.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-31 08:21 cconn/comm/tcp/server/__init__.py
--rw-r--r--  2.0 unx     4809 b- defN 22-Dec-07 14:03 cconn/comm/tcp/server/tcp_server.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/definitions/__init__.py
--rw-r--r--  2.0 unx      141 b- defN 22-Dec-07 13:45 cconn/definitions/constants.py
--rw-r--r--  2.0 unx      575 b- defN 22-Dec-13 08:15 cconn/definitions/prop_keys.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/log/__init__.py
--rw-r--r--  2.0 unx     1501 b- defN 22-Oct-28 06:03 cconn/log/logger.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:07 cconn/network/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:07 cconn/network/detect/__init__.py
--rw-r--r--  2.0 unx      427 b- defN 22-Oct-28 06:03 cconn/network/detect/network_detector.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:07 cconn/network/detect/udp/__init__.py
--rw-r--r--  2.0 unx     1133 b- defN 22-Oct-28 06:03 cconn/network/detect/udp/broadcast_msg.py
--rw-r--r--  2.0 unx     2749 b- defN 22-Dec-14 04:38 cconn/network/detect/udp/udp_detector.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-31 08:21 cconn/network/register/__init__.py
--rw-r--r--  2.0 unx      348 b- defN 22-Oct-31 08:21 cconn/network/register/network_register.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-31 08:21 cconn/network/register/udp/__init__.py
--rw-r--r--  2.0 unx     3175 b- defN 22-Dec-13 08:23 cconn/network/register/udp/udp_register.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-28 06:03 cconn/utils/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 22-Nov-22 15:05 cconn/utils/address_utils.py
--rw-r--r--  2.0 unx      319 b- defN 22-Nov-27 15:16 cconn/utils/data_converter.py
--rw-r--r--  2.0 unx     2062 b- defN 22-Oct-31 08:21 cconn/utils/msg_thread.py
--rw-r--r--  2.0 unx     1544 b- defN 22-Oct-28 06:03 cconn/utils/props.py
--rw-r--r--  2.0 unx      102 b- defN 22-Oct-28 06:03 cconn/utils/str.py
--rw-r--r--  2.0 unx       95 b- defN 22-Oct-28 06:03 cconn/utils/time.py
--rw-r--r--  2.0 unx      955 b- defN 22-Oct-28 06:03 cconn/utils/topic_utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-21 03:10 tests/__init__.py
--rw-r--r--  2.0 unx    10369 b- defN 22-Nov-27 15:17 tests/test_comm_handler.py
--rw-r--r--  2.0 unx      294 b- defN 22-Oct-31 02:39 tests/test_ip_utils.py
--rw-r--r--  2.0 unx     2452 b- defN 22-Nov-27 15:17 tests/test_msg.py
--rw-r--r--  2.0 unx      448 b- defN 22-Oct-31 08:21 tests/test_msg_thread.py
--rw-r--r--  2.0 unx     1896 b- defN 22-Oct-28 06:03 tests/test_topic_mapper.py
--rw-r--r--  2.0 unx     1511 b- defN 22-Oct-28 06:03 tests/test_topic_utils.py
--rw-r--r--  2.0 unx    10786 b- defN 22-Dec-14 04:40 cross_connection-0.2.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      196 b- defN 22-Dec-14 04:40 cross_connection-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-14 04:40 cross_connection-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Dec-14 04:40 cross_connection-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5168 b- defN 22-Dec-14 04:40 cross_connection-0.2.1.dist-info/RECORD
-61 files, 94612 bytes uncompressed, 25641 bytes compressed:  72.9%
+Zip file size: 34386 bytes, number of entries: 62
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/__init__.py
+-rw-r--r--  2.0 unx     1783 b- defN 23-Jul-16 09:39 cconn/connection.py
+-rw-r--r--  2.0 unx     1509 b- defN 23-Jul-16 10:07 cconn/connection_factory.py
+-rw-r--r--  2.0 unx      206 b- defN 23-Mar-01 04:13 cconn/module.py
+-rw-r--r--  2.0 unx      911 b- defN 23-Jul-16 09:40 cconn/server.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/bus/__init__.py
+-rw-r--r--  2.0 unx      771 b- defN 23-Jul-16 09:47 cconn/bus/bus.py
+-rw-r--r--  2.0 unx     3613 b- defN 23-Jul-16 09:45 cconn/bus/cross_connection_bus.py
+-rw-r--r--  2.0 unx      233 b- defN 23-Mar-01 04:13 cconn/bus/server_struct.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/comm/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/comm/base/__init__.py
+-rw-r--r--  2.0 unx      444 b- defN 23-Mar-01 04:13 cconn/comm/base/comm.py
+-rw-r--r--  2.0 unx     8780 b- defN 23-Mar-01 04:13 cconn/comm/base/comm_handler.py
+-rw-r--r--  2.0 unx      793 b- defN 23-Mar-01 04:13 cconn/comm/base/comm_server_wrapper.py
+-rw-r--r--  2.0 unx     4199 b- defN 23-Jul-16 09:48 cconn/comm/base/msg.py
+-rw-r--r--  2.0 unx      428 b- defN 23-Mar-01 04:13 cconn/comm/base/topic_mapper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/comm/base/pubsub/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-Mar-01 04:13 cconn/comm/base/pubsub/client_comm_pubsub_manager.py
+-rw-r--r--  2.0 unx     2976 b- defN 23-Mar-01 04:13 cconn/comm/base/pubsub/server_comm_pubsub_manager.py
+-rw-r--r--  2.0 unx      231 b- defN 23-Mar-01 04:13 cconn/comm/base/pubsub/subscription.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/comm/tcp/__init__.py
+-rw-r--r--  2.0 unx      689 b- defN 23-Mar-01 04:13 cconn/comm/tcp/tcp_comm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/comm/tcp/client/__init__.py
+-rw-r--r--  2.0 unx    12288 b- defN 23-Jul-16 10:07 cconn/comm/tcp/client/tcp_client.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/comm/tcp/server/__init__.py
+-rw-r--r--  2.0 unx     4809 b- defN 23-Mar-01 04:13 cconn/comm/tcp/server/tcp_server.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/definitions/__init__.py
+-rw-r--r--  2.0 unx      141 b- defN 23-Mar-01 04:13 cconn/definitions/constants.py
+-rw-r--r--  2.0 unx      575 b- defN 23-Mar-01 04:13 cconn/definitions/prop_keys.py
+-rw-r--r--  2.0 unx      129 b- defN 23-Jul-16 10:07 cconn/definitions/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/log/__init__.py
+-rw-r--r--  2.0 unx     1501 b- defN 23-Mar-01 04:13 cconn/log/logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/network/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/network/detect/__init__.py
+-rw-r--r--  2.0 unx      433 b- defN 23-Jul-16 09:39 cconn/network/detect/network_detector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/network/detect/udp/__init__.py
+-rw-r--r--  2.0 unx     1133 b- defN 23-Mar-01 04:13 cconn/network/detect/udp/broadcast_msg.py
+-rw-r--r--  2.0 unx     2932 b- defN 23-Jul-16 10:06 cconn/network/detect/udp/udp_detector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/network/register/__init__.py
+-rw-r--r--  2.0 unx      351 b- defN 23-Jul-16 09:41 cconn/network/register/network_register.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/network/register/udp/__init__.py
+-rw-r--r--  2.0 unx     3178 b- defN 23-Jul-16 09:41 cconn/network/register/udp/udp_register.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 cconn/utils/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 23-Mar-01 04:13 cconn/utils/address_utils.py
+-rw-r--r--  2.0 unx      337 b- defN 23-Jul-16 04:36 cconn/utils/data_converter.py
+-rw-r--r--  2.0 unx     2007 b- defN 23-Mar-01 04:13 cconn/utils/msg_thread.py
+-rw-r--r--  2.0 unx     1544 b- defN 23-Mar-01 04:13 cconn/utils/props.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Mar-01 04:13 cconn/utils/str.py
+-rw-r--r--  2.0 unx       95 b- defN 23-Mar-01 04:13 cconn/utils/time.py
+-rw-r--r--  2.0 unx      955 b- defN 23-Mar-01 04:13 cconn/utils/topic_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Mar-01 04:13 tests/__init__.py
+-rw-r--r--  2.0 unx    10369 b- defN 23-Mar-01 04:13 tests/test_comm_handler.py
+-rw-r--r--  2.0 unx      294 b- defN 23-Mar-01 04:13 tests/test_ip_utils.py
+-rw-r--r--  2.0 unx     2452 b- defN 23-Mar-01 04:13 tests/test_msg.py
+-rw-r--r--  2.0 unx      448 b- defN 23-Mar-01 04:13 tests/test_msg_thread.py
+-rw-r--r--  2.0 unx     1896 b- defN 23-Mar-01 04:13 tests/test_topic_mapper.py
+-rw-r--r--  2.0 unx     1511 b- defN 23-Mar-01 04:13 tests/test_topic_utils.py
+-rw-r--r--  2.0 unx    10786 b- defN 23-Jul-16 10:08 cross_connection-0.2.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      196 b- defN 23-Jul-16 10:08 cross_connection-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 10:08 cross_connection-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-16 10:08 cross_connection-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5230 b- defN 23-Jul-16 10:08 cross_connection-0.2.2.dist-info/RECORD
+62 files, 95755 bytes uncompressed, 26004 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -9,14 +9,26 @@
 
 Filename: cconn/module.py
 Comment: 
 
 Filename: cconn/server.py
 Comment: 
 
+Filename: cconn/bus/__init__.py
+Comment: 
+
+Filename: cconn/bus/bus.py
+Comment: 
+
+Filename: cconn/bus/cross_connection_bus.py
+Comment: 
+
+Filename: cconn/bus/server_struct.py
+Comment: 
+
 Filename: cconn/comm/__init__.py
 Comment: 
 
 Filename: cconn/comm/base/__init__.py
 Comment: 
 
 Filename: cconn/comm/base/comm.py
@@ -42,26 +54,14 @@
 
 Filename: cconn/comm/base/pubsub/server_comm_pubsub_manager.py
 Comment: 
 
 Filename: cconn/comm/base/pubsub/subscription.py
 Comment: 
 
-Filename: cconn/comm/bus/__init__.py
-Comment: 
-
-Filename: cconn/comm/bus/bus.py
-Comment: 
-
-Filename: cconn/comm/bus/cross_connection_bus.py
-Comment: 
-
-Filename: cconn/comm/bus/server_struct.py
-Comment: 
-
 Filename: cconn/comm/tcp/__init__.py
 Comment: 
 
 Filename: cconn/comm/tcp/tcp_comm.py
 Comment: 
 
 Filename: cconn/comm/tcp/client/__init__.py
@@ -81,14 +81,17 @@
 
 Filename: cconn/definitions/constants.py
 Comment: 
 
 Filename: cconn/definitions/prop_keys.py
 Comment: 
 
+Filename: cconn/definitions/types.py
+Comment: 
+
 Filename: cconn/log/__init__.py
 Comment: 
 
 Filename: cconn/log/logger.py
 Comment: 
 
 Filename: cconn/network/__init__.py
@@ -162,23 +165,23 @@
 
 Filename: tests/test_topic_mapper.py
 Comment: 
 
 Filename: tests/test_topic_utils.py
 Comment: 
 
-Filename: cross_connection-0.2.1.dist-info/LICENSE.md
+Filename: cross_connection-0.2.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: cross_connection-0.2.1.dist-info/METADATA
+Filename: cross_connection-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: cross_connection-0.2.1.dist-info/WHEEL
+Filename: cross_connection-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: cross_connection-0.2.1.dist-info/top_level.txt
+Filename: cross_connection-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cross_connection-0.2.1.dist-info/RECORD
+Filename: cross_connection-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cconn/connection.py

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Callable, Dict
+from typing import Callable, Dict, Optional
 from cconn.module import Module
 from cconn.comm.base.msg import Method
 
 
 class ConnectionState(Enum):
     CONNECTING = 0
     CONNECTED = 1
@@ -33,15 +33,15 @@
     @abstractmethod
     def remove_on_connection_state_changed_listener(
             self,
             listener: Callable[[ConnectionState, Exception], None]):
         raise NotImplementedError
 
     @abstractmethod
-    def start(self, config_props: Dict[str, str]):
+    def start(self, config_props: Dict[str, object]):
         raise NotImplementedError
 
     @abstractmethod
     def close(self):
         raise NotImplementedError
 
     @abstractmethod
@@ -50,24 +50,24 @@
 
     @abstractmethod
     def publish(
         self,
         topic: str,
         method: Method,
         data: bytes,
-        on_action_listener: OnActionListener = None
+        on_action_listener: Optional[OnActionListener] = None
     ):
         raise NotImplementedError
 
     @abstractmethod
     def subscribe(
         self,
         topic: str,
         method: Method,
         on_data_listener: Callable[[str, Method, bytes], None],
-        on_action_listener: OnActionListener = None
+        on_action_listener: Optional[OnActionListener] = None
     ):
         raise NotImplementedError
 
     @abstractmethod
     def unsubscribe(self, topic: str, method: Method):
         raise NotImplementedError
```

## cconn/connection_factory.py

```diff
@@ -1,39 +1,41 @@
 # coding: utf-8
 
-from enum import Enum
+from typing import Optional
+from cconn.bus.bus import Bus
+from cconn.bus.cross_connection_bus import CrossConnectionBus
 from cconn.comm.tcp.client.tcp_client import TcpClient
 from cconn.connection import Connection
+from cconn.definitions.types import ConnectionType, NetworkDiscoveryType
 from cconn.network.detect.network_detector import NetworkDetector
 from cconn.network.detect.udp.udp_detector import UdpDetector
 from cconn.network.register.network_register import NetworkRegister
 from cconn.network.register.udp.udp_register import UdpRegister
 
 
-class ConnectionType(Enum):
-    TCP = 1
-
-
-class NetworkDiscoveryType(Enum):
-    UDP = 2
-
-
 class ConnectionFactory:
+    @staticmethod
     def create_connection(connection_type: ConnectionType) -> Connection:
         if connection_type == ConnectionType.TCP:
             return TcpClient()
         else:
-            return None
+            raise RuntimeError('Unsupported connection type')
 
+    @staticmethod
     def create_detector(
             network_discovery_type: NetworkDiscoveryType) -> NetworkDetector:
         if network_discovery_type == NetworkDiscoveryType.UDP:
             return UdpDetector()
         else:
-            return None
+            raise RuntimeError('Unsupported detector type')
 
+    @staticmethod
     def create_register(
             network_discovery_type: NetworkDiscoveryType) -> NetworkRegister:
         if network_discovery_type == NetworkDiscoveryType.UDP:
             return UdpRegister()
         else:
-            return None
+            raise RuntimeError('Unsupported register type')
+
+    @staticmethod
+    def create_bus() -> Bus:
+        return CrossConnectionBus()
```

## cconn/server.py

```diff
@@ -18,15 +18,15 @@
             raise NotImplementedError
 
         @abstractmethod
         def on_publish(self, msg: Msg):
             raise NotImplementedError
 
     @abstractmethod
-    def start(self, config_props: Dict[str, str]) -> bool:
+    def start(self, config_props: Dict[str, object]) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def stop(self):
         raise NotImplementedError
 
     @abstractmethod
```

## cconn/comm/base/comm_handler.py

```diff
@@ -215,18 +215,19 @@
             )
         except Exception as e:
             self.__logger.warn(f'recv exception: {str(e)}')
             return None
 
         if length <= 0:
             self.__logger.warn(f'recv len == {length}')
-            if length == 0:
+            if length == 0 and \
+                    self.__buffer_data_len == self.__recv_buffer_size:
                 self.__logger.warn(
-                    f'msg length already meets max size of buffer: \
-                    {self.__buffer_data_len}')
+                    f'msg length already meets max size of buffer: '
+                    + f'{self.__buffer_data_len}')
 
             return None
 
         self.__buffer_data_len += length
 
         if self.__msg_completeness == MsgCompleteness.NONE:
             return self.__read_msg_flag_from_buffer()
```

## cconn/comm/tcp/client/tcp_client.py

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 import time
 from concurrent.futures import ThreadPoolExecutor
 from socket import AF_INET, SOCK_STREAM, socket
 from threading import Thread
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, Optional
 from cconn.comm.base.msg import Msg, MsgHeader, MsgType
 from cconn.comm.base.comm_handler import CommHandler
 from cconn.comm.base.pubsub.client_comm_pubsub_manager import (
     ClientCommPubSubManager)
 from cconn.comm.base.pubsub.subscription import Subscription
 from cconn.comm.base.topic_mapper import TopicMapper
 from cconn.comm.tcp.tcp_comm import TcpComm
@@ -35,15 +35,15 @@
         self.__is_init = False
         self.__connection_state = ConnectionState.DISCONNECTED
         self.__tcp_socket = None
         self.__comm_handler = None
         self.__logger = DefaultLogger()
         self.__subscribe_manager = ClientCommPubSubManager(self.__logger)
         self.__on_connection_state_changed_listener_list: \
-            List[Callable[[ConnectionState, Exception], None]] = []
+            List[Callable[[ConnectionState, Optional[Exception]], None]] = []
         self.__address = ''
         self.__port = TcpClient.PROPERTY_PORT_DEFAULT
         self.__auto_reconnect = False
         self.__min_reconnect_retry_time = \
             TcpClient.PROPERTY_MIN_RECONNECT_RETRY_TIME_DEFAULT
         self.__max_reconnect_retry_time = \
             TcpClient.PROPERTY_MAX_RECONNECT_RETRY_TIME_DEFAULT
@@ -54,24 +54,24 @@
 
     def set_logger(self, logger: Logger):
         self.__logger = logger
         self.__subscribe_manager.set_logger(logger)
 
     def add_on_connection_state_changed_listener(
             self,
-            listener: Callable[[ConnectionState, Exception], None]):
+            listener: Callable[[ConnectionState, Optional[Exception]], None]):
         if listener not in self.__on_connection_state_changed_listener_list:
             self.__on_connection_state_changed_listener_list.append(listener)
 
     def remove_on_connection_state_changed_listener(
             self,
-            listener: Callable[[ConnectionState, Exception], None]):
+            listener: Callable[[ConnectionState, Optional[Exception]], None]):
         self.__on_connection_state_changed_listener_list.remove(listener)
 
-    def start(self, config_props: Dict[str, str]):
+    def start(self, config_props: Dict[str, object]):
         self.__address = PropsUtils.get_prop_str(
             config_props,
             PropKeys.PROP_IP,
             ''
         )
         self.__port = PropsUtils.get_prop_int(
             config_props,
@@ -104,29 +104,29 @@
         )
 
         self.__tcp_connect()
         self.__is_init = True
 
     def __close_task(self):
         if self.__comm_handler is not None:
-            self.__comm_handler.close()
+            self.__comm_handler.close(False)
 
         self.__subscribe_manager.clear()
         self.__address = ''
         self.__port = TcpClient.PROPERTY_PORT_DEFAULT
         self.__auto_reconnect = False
         self.__is_init = False
 
     def close(self):
         self.__executor.submit(self.__close_task)
 
     def __change_connection_state(
         self, state:
         ConnectionState,
-        e: Exception = None
+        e: Optional[Exception] = None
     ):
         self.__connection_state = state
         if state == ConnectionState.CONNECTED:
             self.__current_reconnect_retry_time = \
                 self.__min_reconnect_retry_time
 
         for listener in self.__on_connection_state_changed_listener_list:
@@ -187,15 +187,15 @@
         return self.__connection_state
 
     def __publish_task(
             self,
             topic: str,
             method: Method,
             data: bytes,
-            on_action_listener: OnActionListener):
+            on_action_listener: Optional[OnActionListener]):
         full_topic = TopicMapper.to_full_topic(topic, method)
         full_topic_bytes = DataConverter.str_to_bytes(full_topic)
         try:
             if self.__comm_handler is not None:
                 send_len = self.__comm_handler.send(
                     Msg(
                         header=MsgHeader(
@@ -207,15 +207,16 @@
                     )
                 )
 
                 if on_action_listener is not None:
                     if send_len > 0:
                         on_action_listener.on_success()
                     else:
-                        on_action_listener.on_failure('Error send data failed')
+                        on_action_listener.on_failure(
+                            Exception('Error send data failed'))
             else:
                 if on_action_listener is not None:
                     on_action_listener.on_failure(
                         Exception(
                             'Error send data failed: comm_hander is None'))
         except Exception as e:
             self.__logger.error(
@@ -224,15 +225,15 @@
                 on_action_listener.on_failure(e)
 
     def publish(
         self,
         topic: str,
         method: Method,
         data: bytes,
-        on_action_listener: OnActionListener = None
+        on_action_listener: Optional[OnActionListener] = None
     ):
         if not self.__is_init:
             if on_action_listener is not None:
                 on_action_listener.on_failure(Exception('TcpClient not init'))
 
             return
 
@@ -240,15 +241,15 @@
             self.__publish_task, topic, method, data, on_action_listener)
 
     def __subscribe_task(
         self,
         topic: str,
         method: Method,
         on_data_listener: Callable[[str, Method, bytes], None],
-        on_action_listener: OnActionListener
+        on_action_listener: Optional[OnActionListener]
     ):
         full_topic = TopicMapper.to_full_topic(topic, method)
         full_topic_bytes = DataConverter.str_to_bytes(full_topic)
 
         try:
             if self.__comm_handler is not None:
                 send_len = self.__comm_handler.send(
@@ -267,31 +268,33 @@
                         callback=on_data_listener
                     ))
 
                     if on_action_listener is not None:
                         on_action_listener.on_success()
                 else:
                     if on_action_listener is not None:
-                        on_action_listener.on_failure('Error send data failed')
+                        on_action_listener.on_failure(
+                            Exception('Error send data failed'))
             else:
                 if on_action_listener is not None:
                     on_action_listener.on_failure(
                         Exception(
                             'Error send data failed: comm_hander is None'))
         except Exception as e:
             self.__logger.error(
                 'Error occurred when sending data: {0}'.format(str(e)))
-            on_action_listener.on_failure(e)
+            if on_action_listener is not None:
+                on_action_listener.on_failure(e)
 
     def subscribe(
         self,
         topic: str,
         method: Method,
         on_data_listener: Callable[[str, Method, bytes], None],
-        on_action_listener: OnActionListener = None
+        on_action_listener: Optional[OnActionListener] = None
     ):
         if not self.__is_init:
             if on_action_listener is not None:
                 on_action_listener.on_failure(Exception('TcpClient not init'))
 
             return
```

## cconn/network/detect/network_detector.py

```diff
@@ -5,15 +5,15 @@
 from cconn.module import Module
 
 
 class NetworkDetector(Module):
     @abstractmethod
     def start_discover(
         self,
-        config_props: Dict[str, str],
-        on_found_service: Callable[[Dict[str, str]], None]
+        config_props: Dict[str, object],
+        on_found_service: Callable[[Dict[str, object]], None]
     ):
         raise NotImplementedError
 
     @abstractmethod
     def stop_discover(self):
         raise NotImplementedError
```

## cconn/network/detect/udp/udp_detector.py

```diff
@@ -5,14 +5,15 @@
     socket,
     AF_INET,
     SOCK_DGRAM,
     SOL_SOCKET,
     SO_BROADCAST
 )
 from typing import Callable, Dict, Final
+from threading import Thread
 from cconn.log.logger import DefaultLogger, Logger
 from cconn.network.detect.network_detector import NetworkDetector
 from cconn.definitions.prop_keys import PropKeys
 from cconn.utils.props import PropsUtils
 from cconn.network.detect.udp.broadcast_msg import (
     BROADCAST_MSG_HEADER_LEN,
     DEFAULT_BROADCAST_FLAG,
@@ -35,15 +36,15 @@
 
     def set_logger(self, logger: Logger):
         self.__logger = logger
 
     def start_discover(
         self,
         config_props: Dict[str, str],
-        on_found_service: Callable[[Dict[str, str]], None],
+        on_found_service: Callable[[Dict[str, object]], None],
     ):
         self.__broadcast_port = PropsUtils.get_prop_int(
             config_props,
             PropKeys.PROP_BROADCAST_PORT,
             UdpDetector.DEFAULT_BROADCAST_PORT,
         )
 
@@ -54,30 +55,34 @@
         )
 
         self.__receiver_sock = socket(AF_INET, SOCK_DGRAM)
         self.__receiver_sock.setsockopt(SOL_SOCKET, SO_BROADCAST, 1)
         self.__receiver_sock.bind(('', self.__broadcast_port))
         self.__is_keep_receiving = True
 
-        while self.__is_keep_receiving and self.__receiver_sock is not None:
-            self.__logger.debug(
-                f'Waiting for broadcast on port {self.__broadcast_port}')
-
-            data = self.__receiver_sock.recvfrom(UdpDetector.RECV_BUF_LEN)
-            if len(data[0]) == BROADCAST_MSG_HEADER_LEN:
-                broadcast_msg = BroadcastMsg()
-                broadcast_msg.from_bytes(data[0])
-                if broadcast_msg.flag == self.__flag:
-                    props = dict()
-                    props[PropKeys.PROP_SERVER_IP] \
-                        = str(ipaddress.IPv4Address(broadcast_msg.ip))
-                    props[PropKeys.PROP_SERVER_PORT] \
-                        = broadcast_msg.port
+        def receive_data():
+            while self.__is_keep_receiving and \
+                    self.__receiver_sock is not None:
+                self.__logger.debug(
+                    f'Waiting for broadcast on port {self.__broadcast_port}')
+
+                data = self.__receiver_sock.recvfrom(UdpDetector.RECV_BUF_LEN)
+                if len(data[0]) == BROADCAST_MSG_HEADER_LEN:
+                    broadcast_msg = BroadcastMsg()
+                    broadcast_msg.from_bytes(data[0])
+                    if broadcast_msg.flag == self.__flag:
+                        props = dict()
+                        props[PropKeys.PROP_SERVER_IP] \
+                            = str(ipaddress.IPv4Address(broadcast_msg.ip))
+                        props[PropKeys.PROP_SERVER_PORT] \
+                            = broadcast_msg.port
 
-                    on_found_service(props)
+                        on_found_service(props)
+
+        Thread(target=receive_data).start()
 
     def stop_discover(self):
         self.__is_keep_receiving = False
 
         try:
             if self.__receiver_sock is not None:
                 self.__receiver_sock.close()
```

## cconn/network/register/network_register.py

```diff
@@ -5,14 +5,14 @@
 from cconn.module import Module
 
 
 class NetworkRegister(Module):
     @abstractmethod
     def register(
         self,
-        config_props: Dict[str, str]
+        config_props: Dict[str, object]
     ):
         raise NotImplementedError
 
     @abstractmethod
     def unregister(self):
         raise NotImplementedError
```

## cconn/network/register/udp/udp_register.py

```diff
@@ -64,15 +64,15 @@
         self.__is_send_broadcast = True
 
         thread = Thread(target=self.__send_broadcast_task)
         thread.start()
 
     def register(
         self,
-        config_props: Dict[str, str]
+        config_props: Dict[str, object]
     ):
         self.__broadcast_port = PropsUtils.get_prop_int(
             config_props,
             PropKeys.PROP_BROADCAST_PORT,
             UdpRegister.DEFAULT_BROADCAST_PORT,
         )
         self.__broadcast_interval = PropsUtils.get_prop_int(
```

## cconn/utils/data_converter.py

```diff
@@ -6,9 +6,10 @@
 class DataConverter:
     ENCODEING_UTF8: Final = 'utf-8'
 
     @staticmethod
     def str_to_bytes(data: str) -> bytes:
         return data.encode(DataConverter.ENCODEING_UTF8)
 
+    @staticmethod
     def bytes_to_str(data: bytes) -> str:
         return data.decode(DataConverter.ENCODEING_UTF8)
```

## cconn/utils/msg_thread.py

```diff
@@ -32,17 +32,14 @@
                 self.__queue.append(msg)
 
             self.__set_key()
 
     def __msg_arrived(self, msg: any):
         self.__on_msg_arrived(msg)
 
-    def __reset_key(self):
-        self.__key = False
-
     def __wait_for_key(self):
         if not self.__key:
             self.__lock.acquire()
 
     def __reset_key(self):
         self.__key = False
```

## Comparing `cconn/comm/bus/cross_connection_bus.py` & `cconn/bus/cross_connection_bus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # coding: utf-8
 
 from dataclasses import dataclass
 from typing import Dict
+from cconn.definitions.types import ConnectionType
 from cconn.log.logger import Logger, DefaultLogger
-from cconn.module import Module
 from cconn.server import Server
-from cconn.comm.bus.bus import Bus
-from cconn.comm.bus.server_struct import ServerStruct
+from cconn.bus.bus import Bus
+from cconn.bus.server_struct import ServerStruct
 from cconn.comm.base.msg import Msg
-from cconn.connection_factory import (
-    ConnectionFactory,
-    ConnectionType,
-    NetworkDiscoveryType
-)
+from cconn.network.register.udp.udp_register import UdpRegister
 from cconn.comm.tcp.server.tcp_server import TcpServer
 from cconn.utils.msg_thread import MsgThread
 
 
 @dataclass
 class MsgObjPublish:
     msg: Msg = None
     exclude_server: Server = None
 
 
-class CrossConnectionBus(Bus, Module):
+class CrossConnectionBus(Bus):
     class ServerCallback(Server.Callback):
         def __init__(self, server: Server, bus: Bus):
             self.__server: Server = server
             self.__bus: Bus = bus
 
         def on_subscribe(self, full_topic: str):
             pass
@@ -35,52 +31,58 @@
         def on_unsubscribe(self, full_topic: str):
             pass
 
         def on_publish(self, msg: Msg):
             self.__bus.publish_msg_to_bus(msg, self.__server)
 
     def __init__(self):
-        self.__initialized = False
+        self.__is_initialized = False
         self.__server_dict: Dict[ConnectionType, ServerStruct] = dict()
         self.__msg_thread = None
         self.__logger = DefaultLogger()
-        self.__initialize()
 
     def set_logger(self, logger: Logger):
         self.__logger = logger
 
-    def __msg_handler(self, msg_obj: any):
+    def __msg_handler(self, msg_obj: object):
         if isinstance(msg_obj, MsgObjPublish):
             for server_struct in self.__server_dict.values():
                 if server_struct.server != msg_obj.exclude_server:
                     server_struct.server.handle_publish_message(msg_obj.msg)
 
-    def __initialize(self) -> bool:
-        if self.__initialized:
+    def initialize(self) -> bool:
+        if self.__is_initialized:
             return True
 
         self.__create_message_processing_thread()
 
         tcp_server = TcpServer()
         tcp_server.set_callback(self.__create_server_callback(tcp_server))
+        tcp_server.set_logger(self.__logger)
+
+        udp_register = UdpRegister()
+        udp_register.set_logger(self.__logger)
+
         self.__server_dict[ConnectionType.TCP] = \
             ServerStruct(
                 server=tcp_server,
-                register=ConnectionFactory.create_register(
-                    NetworkDiscoveryType.UDP)
+                register=udp_register,
         )
 
-        self.__initialized = True
-        return self.__initialized
+        self.__is_initialized = True
+        return self.__is_initialized
 
     def start(
             self,
             connection_type: ConnectionType,
-            server_config: Dict[str, str],
-            network_register_config: Dict[str, str]) -> bool:
+            server_config: Dict[str, object],
+            network_register_config: Dict[str, object]) -> bool:
+        if not self.__is_initialized:
+            return False
+
         if connection_type not in self.__server_dict:
             return False
 
         server_struct = self.__server_dict[connection_type]
         is_started = server_struct.server.start(server_config)
         if is_started:
             self.__logger.info(f'{connection_type.name} server started')
```

## Comparing `cross_connection-0.2.1.dist-info/LICENSE.md` & `cross_connection-0.2.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cross_connection-0.2.1.dist-info/RECORD` & `cross_connection-0.2.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 cconn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cconn/connection.py,sha256=BVSv14LxvZbmaOGANkdT4ATlVruluUTxoRKJyW7K5ww,1750
-cconn/connection_factory.py,sha256=FqwpuiJVQkZ5Q5LxmwD19GHvdGgfhBFiKzAsFZxdPao,1180
+cconn/connection.py,sha256=i5dXOIRC50QdwmXxjLyOEwVY93jSplR1A3R-PL6zE9g,1783
+cconn/connection_factory.py,sha256=g-k0vIcFWe9trcjGOPex-1aGK75r6tCkDIze3RoucHk,1509
 cconn/module.py,sha256=dA6RneH8_kWKNXOSsAdqjL9_ZfogjyVOX5tiaHIMbA8,206
-cconn/server.py,sha256=kgdRNit5Vsyr1a1tBu5RlEM4TWpE28kk_Aajrj9KEKk,908
+cconn/server.py,sha256=Mipw3KM1JFBmj3ev5EDE314Ck0RnD_3cXpatQgx3TFk,911
+cconn/bus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cconn/bus/bus.py,sha256=KH3d04UBEEURkWyVsELmyiZCM8iClJ_hd-sQkfx5EBo,771
+cconn/bus/cross_connection_bus.py,sha256=LT9aoPU-OOEqCxy4EbrCrzld46vqOQd58DMcf0z-qkw,3613
+cconn/bus/server_struct.py,sha256=tiBE75_JP8kuxIthrM_cES--OK-5sTNsHzC9rGAHaYI,233
 cconn/comm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/comm/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/comm/base/comm.py,sha256=O44AK74wfcQYrno221lpX9_hIfDLVnpYefzwftDTdbU,444
-cconn/comm/base/comm_handler.py,sha256=iSCDuDHmOpd11_dKD8KKJRkOCyoZ1F-5YPoznHAXtYQ,8700
+cconn/comm/base/comm_handler.py,sha256=nqIbFQ-FEOCm88zQg94Sps72odiqEvOIwvFukIpcFQo,8780
 cconn/comm/base/comm_server_wrapper.py,sha256=5mhRiQUNqsoknZ9qXs8uEdxanoNiy0wPh97f0Obo2yE,793
 cconn/comm/base/msg.py,sha256=4T0GfuBvuDEgqKraEwxLYcimAgdPzZrgzk8Jgqlf6Sg,4199
 cconn/comm/base/topic_mapper.py,sha256=lMpze2HsZOvPTlJOmqjtzFhiVkfAN3R6UOhYjWBhR1k,428
 cconn/comm/base/pubsub/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/comm/base/pubsub/client_comm_pubsub_manager.py,sha256=iwWdJ2EdDoKJeBkae8gLIG9VxgOzlT34nTBGwOmsMWI,1316
 cconn/comm/base/pubsub/server_comm_pubsub_manager.py,sha256=jekbL0mC18nF5AYokxtL1AH5GtM3wbxMl6hrrhxtVXo,2976
 cconn/comm/base/pubsub/subscription.py,sha256=pxF4LYZ1RFT5JhcKiKEWnsK243fD-BgXHFq9gsKB0lY,231
-cconn/comm/bus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cconn/comm/bus/bus.py,sha256=yyu5X-ogAEWhddvw2j16WUEzdNTPpRpuHUENtIdTinw,726
-cconn/comm/bus/cross_connection_bus.py,sha256=n8lG2xxVvhWmsENWPYhqrxOaDFaEbAvXj6vpFvl9YpQ,3538
-cconn/comm/bus/server_struct.py,sha256=tiBE75_JP8kuxIthrM_cES--OK-5sTNsHzC9rGAHaYI,233
 cconn/comm/tcp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/comm/tcp/tcp_comm.py,sha256=DgqtRsfUEB3KpF_qU2cEyX7uXt8lvE4F9PfqJLMbcEw,689
 cconn/comm/tcp/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cconn/comm/tcp/client/tcp_client.py,sha256=SEo1NHYZYsLpI7bjxIIFGcrRe3GGM0dhZ4K6GfmC2DY,12059
+cconn/comm/tcp/client/tcp_client.py,sha256=8UYkkN-v0Cyq-ZZsr5U-YXSRdTQoSLquYigAjffRlS8,12288
 cconn/comm/tcp/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/comm/tcp/server/tcp_server.py,sha256=DGDXIkshNX9zZ5FZAU2a6_2FJkTo2ikOhvnz8x1h7wA,4809
 cconn/definitions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/definitions/constants.py,sha256=o5H2Lh8mnV7YUAwWyqtbsY_QzVkCpGm5e3Gnq4dRg-8,141
 cconn/definitions/prop_keys.py,sha256=ZvYeSyO98uqlV7CkZ4_9Lr6LnVWRLMrrAaje5bdLUZM,575
+cconn/definitions/types.py,sha256=Z7Nrr6Q0XRqiGkb6Wl8X6mrm-leoJWfuK_Cq9gIKhfs,129
 cconn/log/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/log/logger.py,sha256=0jClOY7jURFSx-6P0nTLLFaWA33H-ZfR_qhj8eqMZRI,1501
 cconn/network/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/network/detect/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cconn/network/detect/network_detector.py,sha256=DITyu0P-4X8EvX9AXhdX-2eMlHPxaVCSfnhAWl0Pqz8,427
+cconn/network/detect/network_detector.py,sha256=Puoy42owMA4S9s2RlY9ZMUude8JxaC024w80fwNMBK0,433
 cconn/network/detect/udp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/network/detect/udp/broadcast_msg.py,sha256=dgAZTsDg6h1QIw1nrDZGi-ltYbYbZMPThdxJtbnEc3I,1133
-cconn/network/detect/udp/udp_detector.py,sha256=vliBWqS1G5qZXJVLPF4wXY8ewEwd-WbRNMIO5iwUCUE,2749
+cconn/network/detect/udp/udp_detector.py,sha256=l7mpDjrRCn_0TEuk1Rg1WB7PWWt-ImIEmTu9ivu3Y-4,2932
 cconn/network/register/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cconn/network/register/network_register.py,sha256=Blopo5w2iEOHHLD6HLIWveaM6E8zNWzsRCDwOD-n-Ko,348
+cconn/network/register/network_register.py,sha256=hRDlfSmiQVAa1Z3hYRHnjtvJil6i5ssmMGoV6cjy9I8,351
 cconn/network/register/udp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cconn/network/register/udp/udp_register.py,sha256=STWHrIxBIlwQFC2XR0PdOTx4CNHzGvpgI1Y5_a23uO8,3175
+cconn/network/register/udp/udp_register.py,sha256=NfIukfpC4WQEYOZF7Fzhrrp_XDb3sUrAuqfhYpaBFAc,3178
 cconn/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cconn/utils/address_utils.py,sha256=HF_D6Jff_mge5Kss4mYzf71hnc__li_5YPl-ib1r4sA,1077
-cconn/utils/data_converter.py,sha256=ldnf18Pd03j8io0r0iBViaNUy9Ea7pczn-dW8hFe_EQ,319
-cconn/utils/msg_thread.py,sha256=6NN4saZbHgIpcaQFOKDAffBsbWiK6qfaWWbagKHfHwA,2062
+cconn/utils/data_converter.py,sha256=uB4tvP3JMjJXDya3PfSF-Zxd2kJ1FeL9DpbbZimarH0,337
+cconn/utils/msg_thread.py,sha256=2XCFzuXvvvH01q58YNPcrMBs2ocZQjUzndGz2a3z9aw,2007
 cconn/utils/props.py,sha256=UyqQBD1_y7y9ZRocfL24cNiYpFNLUbxyYtSEFq9C0EU,1544
 cconn/utils/str.py,sha256=d4ufBNzP_Jblz_0kSu_XX5ubazjA6UQMwALzfVmATfo,102
 cconn/utils/time.py,sha256=vhm0iHUmDQTi_Yj0wCf9Ho5cXGVdL6y29_FWLEnsjJg,95
 cconn/utils/topic_utils.py,sha256=FBclPNIF3bW7YAoGdm13nFrKPGEDBhGxRgcyuOq2ieU,955
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_comm_handler.py,sha256=aCjsW4qIgljj7fezmS5TBqCairQBL-Ib1EyvK374X9M,10369
 tests/test_ip_utils.py,sha256=4uacrF936D6jQ8NvD1xa6tMFUkioqPpPEX6WEdOR0BA,294
 tests/test_msg.py,sha256=vNUv_PWTn5lrBI8ztThOyHsBOR8lMDz0yJCNPEFpoco,2452
 tests/test_msg_thread.py,sha256=F6MAOF5GyS9DWw1rzmYfyK6wbCZpK-GJt-RdIo6JLmc,448
 tests/test_topic_mapper.py,sha256=aqalzWTzo-iGZ4DIBoURuccDhAFMRnbXQHzE8tWT9b4,1896
 tests/test_topic_utils.py,sha256=0Q-hH8ZZT_ljNpmCU_7Df6z6AyqBsHR_xwZsQrFRTHY,1511
-cross_connection-0.2.1.dist-info/LICENSE.md,sha256=MHMVWN38TN7LC098YZmfN15sqOCrdf4Uq4nXHT5N_C8,10786
-cross_connection-0.2.1.dist-info/METADATA,sha256=ryGIjPCIOlHLGSfCzw8jHFdtBGGdI4KnR0rWwk_9bhI,196
-cross_connection-0.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-cross_connection-0.2.1.dist-info/top_level.txt,sha256=d188yxYHpDbzWdV6qP8A2Zcv5iM5TjWgSwYh65hBSzY,12
-cross_connection-0.2.1.dist-info/RECORD,,
+cross_connection-0.2.2.dist-info/LICENSE.md,sha256=MHMVWN38TN7LC098YZmfN15sqOCrdf4Uq4nXHT5N_C8,10786
+cross_connection-0.2.2.dist-info/METADATA,sha256=Yc8MjVR0SO7QKZCOzWVKEuj8e3KfGNmARESd_LVy_d4,196
+cross_connection-0.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+cross_connection-0.2.2.dist-info/top_level.txt,sha256=d188yxYHpDbzWdV6qP8A2Zcv5iM5TjWgSwYh65hBSzY,12
+cross_connection-0.2.2.dist-info/RECORD,,
```

