# Comparing `tmp/flwr_nightly-1.5.0.dev20230713.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230714.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230713.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230714.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230713.tar` & `flwr_nightly-1.5.0.dev20230714.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    11358 2023-07-13 23:00:54.358889 flwr_nightly-1.5.0.dev20230713/LICENSE
--rw-r--r--   0        0        0    10721 2023-07-13 23:00:54.358889 flwr_nightly-1.5.0.dev20230713/README.md
--rw-r--r--   0        0        0     5221 2023-07-13 23:01:18.254975 flwr_nightly-1.5.0.dev20230713/pyproject.toml
--rw-r--r--   0        0        0      952 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    14058 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4954 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     7345 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6380 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     4693 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     9050 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3459 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16315 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-07-13 23:00:54.666886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     7295 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     6182 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     7505 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2183 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26333 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     2546 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2876 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3686 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19294 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4654 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6995 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5893 2023-07-13 23:00:54.670886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7014 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11522 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9991 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8286 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2708 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5428 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7126 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     6026 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3519 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7079 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6343 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10154 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5478 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4940 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7762 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5471 2023-07-13 23:00:54.674886 flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12946 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230713/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:00:45.545738 flwr_nightly-1.5.0.dev20230714/LICENSE
+-rw-r--r--   0        0        0    10846 2023-07-14 23:00:45.545738 flwr_nightly-1.5.0.dev20230714/README.md
+-rw-r--r--   0        0        0     5400 2023-07-14 23:01:07.545839 flwr_nightly-1.5.0.dev20230714/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    14058 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4954 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     7345 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6380 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     4693 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     9050 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3459 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16315 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7295 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     6182 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     7505 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2183 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-07-14 23:00:45.845740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26333 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     2546 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2876 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3686 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19294 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-07-14 23:00:45.849740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5478 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4940 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7762 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5471 2023-07-14 23:00:45.853740 flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    13168 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230714/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230713/LICENSE` & `flwr_nightly-1.5.0.dev20230714/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/README.md` & `flwr_nightly-1.5.0.dev20230714/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |
     <a href="https://flower.dev/join-slack">Slack</a>
     <br /><br />
 </p>
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)
-![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)
+![Build](https://github.com/adap/flower/actions/workflows/framework.yml/badge.svg)
 ![Downloads](https://pepy.tech/badge/flwr)
 [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)
 
 Flower (`flwr`) is a framework for building federated learning systems. The
 design of Flower is based on a few guiding principles:
 
 * **Customizable**: Federated learning systems vary wildly from one use case to
@@ -73,43 +73,43 @@
 
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb))
 
 
 ## Documentation
 
 [Flower Docs](https://flower.dev/docs):
-* [Installation](https://flower.dev/docs/installation.html)
-* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
-* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)
-* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)
-* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)
-* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)
-* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)
-* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)
+* [Installation](https://flower.dev/docs/framework/installation.html)
+* [Quickstart (TensorFlow)](https://flower.dev/framework/docs/quickstart-tensorflow.html)
+* [Quickstart (PyTorch)](https://flower.dev/docs/framework/quickstart-pytorch.html)
+* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/framework/quickstart-huggingface.html)
+* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/framework/quickstart-pytorch-lightning.html)
+* [Quickstart (MXNet)](https://flower.dev/docs/framework/example-mxnet-walk-through.html)
+* [Quickstart (Pandas)](https://flower.dev/docs/framework/quickstart-pandas.html)
+* [Quickstart (fastai)](https://flower.dev/docs/framework/quickstart-fastai.html)
 * [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)
 * [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
 * [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)
-* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)
+* [Quickstart (iOS)](https://flower.dev/docs/framework/quickstart-ios.html)
 
 ## Flower Baselines
 
 Flower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:
 
 * [FedAvg](https://arxiv.org/abs/1602.05629):
-  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/fedavg_mnist)
 * [FedProx](https://arxiv.org/abs/1812.06127):
-  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/fedprox/)
 * [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):
-  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)
+  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/fedbn/convergence_rate)
 * [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):
-  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)
+  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/adaptive_federated_optimization)
 
-Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)
+Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/baselines/using-baselines.html)
 
-The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)
+The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/baselines/contributing-baselines.html)
 
 ## Flower Usage Examples
 
 Several code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).
 
 Quickstart examples:
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
                                [Flower_Website]
                   Website | Blog | Docs | Conference | Slack
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
-actions/workflows/flower.yml/badge.svg) ![Downloads](https://pepy.tech/badge/
-flwr) [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://
+actions/workflows/framework.yml/badge.svg) ![Downloads](https://pepy.tech/
+badge/flwr) [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://
 flower.dev/join-slack) Flower (`flwr`) is a framework for building federated
 learning systems. The design of Flower is based on a few guiding principles: *
 **Customizable**: Federated learning systems vary wildly from one use case to
 another. Flower allows for a wide range of different configurations depending
 on the needs of each individual use case. * **Extendable**: Flower originated
 from a research project at the University of Oxford, so it was built with AI
 research in mind. Many components can be extended and overridden to build new
@@ -58,48 +58,50 @@
 tutorials are coming soon. Topics include **Privacy and Security in Federated
 Learning**, and **Scaling Federated Learning**. ## 30 Minute Federated Learning
 Tutorial [![Open in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/
 examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter
 Notebook](https://github.com/adap/flower/blob/main/examples/
 simulation_pytorch_colab/tutorial.ipynb)) ## Documentation [Flower Docs](https:
-//flower.dev/docs): * [Installation](https://flower.dev/docs/installation.html)
-* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
-* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html) *
-[Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-
-huggingface.html) * [Quickstart (PyTorch Lightning [code example])](https://
-flower.dev/docs/quickstart-pytorch-lightning.html) * [Quickstart (MXNet)]
-(https://flower.dev/docs/example-mxnet-walk-through.html) * [Quickstart
-(Pandas)](https://flower.dev/docs/quickstart-pandas.html) * [Quickstart
-(fastai)](https://flower.dev/docs/quickstart-fastai.html) * [Quickstart (JAX)]
-(https://github.com/adap/flower/tree/main/examples/quickstart_jax) *
-[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
-sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code example])](https:/
-/github.com/adap/flower/tree/main/examples/android) * [Quickstart (iOS)](https:
-//flower.dev/docs/quickstart-ios.html) ## Flower Baselines Flower Baselines is
-a collection of community-contributed experiments that reproduce the
-experiments performed in popular federated learning publications. Researchers
-can build on Flower Baselines to quickly evaluate new ideas: * [FedAvg](https:/
-/arxiv.org/abs/1602.05629): * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedavg_mnist) * [FedProx](https://
-arxiv.org/abs/1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedprox_mnist) * [FedBN: Federated
-Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/
-abs/2102.07623): * [Convergence Rate](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedbn/convergence_rate) * [Adaptive
-Federated Optimization](https://arxiv.org/abs/2003.00295): * [CIFAR-10/100]
+//flower.dev/docs): * [Installation](https://flower.dev/docs/framework/
+installation.html) * [Quickstart (TensorFlow)](https://flower.dev/framework/
+docs/quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/
+docs/framework/quickstart-pytorch.html) * [Quickstart (Hugging Face [code
+example])](https://flower.dev/docs/framework/quickstart-huggingface.html) *
+[Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/
+framework/quickstart-pytorch-lightning.html) * [Quickstart (MXNet)](https://
+flower.dev/docs/framework/example-mxnet-walk-through.html) * [Quickstart
+(Pandas)](https://flower.dev/docs/framework/quickstart-pandas.html) *
+[Quickstart (fastai)](https://flower.dev/docs/framework/quickstart-fastai.html)
+* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
+quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
+tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
+example])](https://github.com/adap/flower/tree/main/examples/android) *
+[Quickstart (iOS)](https://flower.dev/docs/framework/quickstart-ios.html) ##
+Flower Baselines Flower Baselines is a collection of community-contributed
+experiments that reproduce the experiments performed in popular federated
+learning publications. Researchers can build on Flower Baselines to quickly
+evaluate new ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST]
 (https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-publications/adaptive_federated_optimization) Check the Flower documentation to
-learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html) The
+flwr_baselines/publications/fedavg_mnist) * [FedProx](https://arxiv.org/abs/
+1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/baselines/
+fedprox/) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/
+publications/fedbn/convergence_rate) * [Adaptive Federated Optimization](https:
+//arxiv.org/abs/2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/
+tree/main/baselines/flwr_baselines/flwr_baselines/publications/
+adaptive_federated_optimization) Check the Flower documentation to learn more:
+[Using Baselines](https://flower.dev/docs/baselines/using-baselines.html) The
 Flower community loves contributions! Make your work more visible and enable
 others to build on it by contributing it as a baseline: [Contributing
-Baselines](https://flower.dev/docs/contributing-baselines.html) ## Flower Usage
-Examples Several code examples show different usage scenarios of Flower (in
-combination with popular machine learning frameworks such as PyTorch or
-TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
+Baselines](https://flower.dev/docs/baselines/contributing-baselines.html) ##
+Flower Usage Examples Several code examples show different usage scenarios of
+Flower (in combination with popular machine learning frameworks such as PyTorch
+or TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
 github.com/adap/flower/tree/main/examples/quickstart_tensorflow) * [Quickstart
 (PyTorch)](https://github.com/adap/flower/tree/main/examples/
 quickstart_pytorch) * [Quickstart (Hugging Face)](https://github.com/adap/
 flower/tree/main/examples/quickstart_huggingface) * [Quickstart (PyTorch
 Lightning)](https://github.com/adap/flower/tree/main/examples/
 quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
 flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
```

### Comparing `flwr_nightly-1.5.0.dev20230713/pyproject.toml` & `flwr_nightly-1.5.0.dev20230714/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230713"
+version = "1.5.0-dev20230714"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
+keywords = [
+    "flower",
+    "fl",
+    "federated learning",
+    "federated analytics",
+    "federated evaluation",
+    "machine learning",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
@@ -76,15 +84,15 @@
 types-requests = "==2.28.11.17"
 types-setuptools = "==67.7.0.1"
 clang-format = "==16.0.3"
 isort = "==5.11.5"
 black = { version = "==23.3.0", extras = ["jupyter"] }
 docformatter = "==1.7.1"
 mypy = "==1.4.0"
-pylint = "==2.13.8"
+pylint = "==2.13.9"
 flake8 = "==3.9.2"
 pytest = "==7.1.2"
 pytest-cov = "==3.0.0"
 pytest-watch = "==4.2.0"
 grpcio-tools = "==1.48.2"
 mypy-protobuf = "==3.2.0"
 jupyterlab = "==3.6.3"
@@ -102,14 +110,16 @@
 ruff = "==0.0.277"
 sphinx-argparse = "==0.4.0"
 pipreqs = "==0.4.13"
 mdformat-gfm = "==0.3.5"
 mdformat-frontmatter = "==2.0.1"
 mdformat-beautysh = "==0.1.1"
 mdformat-myst = "==0.1.5"
+twine = "==4.0.2"
+pyroma = "==4.2"
 
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
```

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230714/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230713/PKG-INFO` & `flwr_nightly-1.5.0.dev20230714/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230713
+Version: 1.5.0.dev20230714
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
+Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -60,15 +61,15 @@
     <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |
     <a href="https://flower.dev/join-slack">Slack</a>
     <br /><br />
 </p>
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)
-![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)
+![Build](https://github.com/adap/flower/actions/workflows/framework.yml/badge.svg)
 ![Downloads](https://pepy.tech/badge/flwr)
 [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)
 
 Flower (`flwr`) is a framework for building federated learning systems. The
 design of Flower is based on a few guiding principles:
 
 * **Customizable**: Federated learning systems vary wildly from one use case to
@@ -121,43 +122,43 @@
 
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb))
 
 
 ## Documentation
 
 [Flower Docs](https://flower.dev/docs):
-* [Installation](https://flower.dev/docs/installation.html)
-* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
-* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)
-* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)
-* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)
-* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)
-* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)
-* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)
+* [Installation](https://flower.dev/docs/framework/installation.html)
+* [Quickstart (TensorFlow)](https://flower.dev/framework/docs/quickstart-tensorflow.html)
+* [Quickstart (PyTorch)](https://flower.dev/docs/framework/quickstart-pytorch.html)
+* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/framework/quickstart-huggingface.html)
+* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/framework/quickstart-pytorch-lightning.html)
+* [Quickstart (MXNet)](https://flower.dev/docs/framework/example-mxnet-walk-through.html)
+* [Quickstart (Pandas)](https://flower.dev/docs/framework/quickstart-pandas.html)
+* [Quickstart (fastai)](https://flower.dev/docs/framework/quickstart-fastai.html)
 * [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)
 * [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
 * [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)
-* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)
+* [Quickstart (iOS)](https://flower.dev/docs/framework/quickstart-ios.html)
 
 ## Flower Baselines
 
 Flower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:
 
 * [FedAvg](https://arxiv.org/abs/1602.05629):
-  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/fedavg_mnist)
 * [FedProx](https://arxiv.org/abs/1812.06127):
-  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/fedprox/)
 * [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):
-  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)
+  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/fedbn/convergence_rate)
 * [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):
-  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)
+  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/adaptive_federated_optimization)
 
-Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)
+Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/baselines/using-baselines.html)
 
-The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)
+The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/baselines/contributing-baselines.html)
 
 ## Flower Usage Examples
 
 Several code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).
 
 Quickstart examples:
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230713 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230714 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
-License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
-Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Topic ::
-Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
-Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Typing :: Typed Provides-Extra: rest
-Provides-Extra: simulation Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra ==
-"rest" Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist:
-importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8" Requires-Dist:
-iterators (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
-Dist: protobuf (>=3.19.0,<4.0.0) Requires-Dist: pydantic (<2.0.0) ; extra ==
-"simulation" Requires-Dist: ray[default] (==2.5.1) ; extra == "simulation"
-Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest" Requires-Dist:
-starlette (>=0.27.0,<0.28.0) ; extra == "rest" Requires-Dist: uvicorn[standard]
-(>=0.21.1,<0.22.0) ; extra == "rest" Project-URL: Documentation, https://
-flower.dev Project-URL: Repository, https://github.com/adap/flower Description-
-Content-Type: text/markdown # Flower: A Friendly Federated Learning Framework
+License: Apache-2.0 Keywords: flower,fl,federated learning,federated
+analytics,federated evaluation,machine learning Author: The Flower Authors
+Author-email: hello@flower.dev Requires-Python: >=3.7,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: MacOS :: MacOS X Classifier: Operating System :: POSIX :: Linux Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
+Engineering :: Mathematics Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Provides-Extra: rest Provides-Extra: simulation Requires-Dist: fastapi
+(>=0.95.0,<0.96.0) ; extra == "rest" Requires-Dist: grpcio
+(>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ;
+python_version < "3.8" Requires-Dist: iterators (>=0.0.2,<0.0.3) Requires-Dist:
+numpy (>=1.21.0,<2.0.0) Requires-Dist: protobuf (>=3.19.0,<4.0.0) Requires-
+Dist: pydantic (<2.0.0) ; extra == "simulation" Requires-Dist: ray[default]
+(==2.5.1) ; extra == "simulation" Requires-Dist: requests (>=2.28.2,<3.0.0) ;
+extra == "rest" Requires-Dist: starlette (>=0.27.0,<0.28.0) ; extra == "rest"
+Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest" Project-
+URL: Documentation, https://flower.dev Project-URL: Repository, https://
+github.com/adap/flower Description-Content-Type: text/markdown # Flower: A
+Friendly Federated Learning Framework
                                [Flower_Website]
                   Website | Blog | Docs | Conference | Slack
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
-actions/workflows/flower.yml/badge.svg) ![Downloads](https://pepy.tech/badge/
-flwr) [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://
+actions/workflows/framework.yml/badge.svg) ![Downloads](https://pepy.tech/
+badge/flwr) [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://
 flower.dev/join-slack) Flower (`flwr`) is a framework for building federated
 learning systems. The design of Flower is based on a few guiding principles: *
 **Customizable**: Federated learning systems vary wildly from one use case to
 another. Flower allows for a wide range of different configurations depending
 on the needs of each individual use case. * **Extendable**: Flower originated
 from a research project at the University of Oxford, so it was built with AI
 research in mind. Many components can be extended and overridden to build new
@@ -87,48 +89,50 @@
 tutorials are coming soon. Topics include **Privacy and Security in Federated
 Learning**, and **Scaling Federated Learning**. ## 30 Minute Federated Learning
 Tutorial [![Open in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/
 examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter
 Notebook](https://github.com/adap/flower/blob/main/examples/
 simulation_pytorch_colab/tutorial.ipynb)) ## Documentation [Flower Docs](https:
-//flower.dev/docs): * [Installation](https://flower.dev/docs/installation.html)
-* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
-* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html) *
-[Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-
-huggingface.html) * [Quickstart (PyTorch Lightning [code example])](https://
-flower.dev/docs/quickstart-pytorch-lightning.html) * [Quickstart (MXNet)]
-(https://flower.dev/docs/example-mxnet-walk-through.html) * [Quickstart
-(Pandas)](https://flower.dev/docs/quickstart-pandas.html) * [Quickstart
-(fastai)](https://flower.dev/docs/quickstart-fastai.html) * [Quickstart (JAX)]
-(https://github.com/adap/flower/tree/main/examples/quickstart_jax) *
-[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
-sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code example])](https:/
-/github.com/adap/flower/tree/main/examples/android) * [Quickstart (iOS)](https:
-//flower.dev/docs/quickstart-ios.html) ## Flower Baselines Flower Baselines is
-a collection of community-contributed experiments that reproduce the
-experiments performed in popular federated learning publications. Researchers
-can build on Flower Baselines to quickly evaluate new ideas: * [FedAvg](https:/
-/arxiv.org/abs/1602.05629): * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedavg_mnist) * [FedProx](https://
-arxiv.org/abs/1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedprox_mnist) * [FedBN: Federated
-Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/
-abs/2102.07623): * [Convergence Rate](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedbn/convergence_rate) * [Adaptive
-Federated Optimization](https://arxiv.org/abs/2003.00295): * [CIFAR-10/100]
+//flower.dev/docs): * [Installation](https://flower.dev/docs/framework/
+installation.html) * [Quickstart (TensorFlow)](https://flower.dev/framework/
+docs/quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/
+docs/framework/quickstart-pytorch.html) * [Quickstart (Hugging Face [code
+example])](https://flower.dev/docs/framework/quickstart-huggingface.html) *
+[Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/
+framework/quickstart-pytorch-lightning.html) * [Quickstart (MXNet)](https://
+flower.dev/docs/framework/example-mxnet-walk-through.html) * [Quickstart
+(Pandas)](https://flower.dev/docs/framework/quickstart-pandas.html) *
+[Quickstart (fastai)](https://flower.dev/docs/framework/quickstart-fastai.html)
+* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
+quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
+tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
+example])](https://github.com/adap/flower/tree/main/examples/android) *
+[Quickstart (iOS)](https://flower.dev/docs/framework/quickstart-ios.html) ##
+Flower Baselines Flower Baselines is a collection of community-contributed
+experiments that reproduce the experiments performed in popular federated
+learning publications. Researchers can build on Flower Baselines to quickly
+evaluate new ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST]
 (https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-publications/adaptive_federated_optimization) Check the Flower documentation to
-learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html) The
+flwr_baselines/publications/fedavg_mnist) * [FedProx](https://arxiv.org/abs/
+1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/baselines/
+fedprox/) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/
+publications/fedbn/convergence_rate) * [Adaptive Federated Optimization](https:
+//arxiv.org/abs/2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/
+tree/main/baselines/flwr_baselines/flwr_baselines/publications/
+adaptive_federated_optimization) Check the Flower documentation to learn more:
+[Using Baselines](https://flower.dev/docs/baselines/using-baselines.html) The
 Flower community loves contributions! Make your work more visible and enable
 others to build on it by contributing it as a baseline: [Contributing
-Baselines](https://flower.dev/docs/contributing-baselines.html) ## Flower Usage
-Examples Several code examples show different usage scenarios of Flower (in
-combination with popular machine learning frameworks such as PyTorch or
-TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
+Baselines](https://flower.dev/docs/baselines/contributing-baselines.html) ##
+Flower Usage Examples Several code examples show different usage scenarios of
+Flower (in combination with popular machine learning frameworks such as PyTorch
+or TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
 github.com/adap/flower/tree/main/examples/quickstart_tensorflow) * [Quickstart
 (PyTorch)](https://github.com/adap/flower/tree/main/examples/
 quickstart_pytorch) * [Quickstart (Hugging Face)](https://github.com/adap/
 flower/tree/main/examples/quickstart_huggingface) * [Quickstart (PyTorch
 Lightning)](https://github.com/adap/flower/tree/main/examples/
 quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
 flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
```

