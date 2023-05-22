# Comparing `tmp/flwr_nightly-1.5.0.dev20230519.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230519.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230522.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230519.tar` & `flwr_nightly-1.5.0.dev20230522.tar`

### file list

```diff
@@ -1,111 +1,113 @@
--rw-r--r--   0        0        0    11358 2023-05-19 23:02:42.853466 flwr_nightly-1.5.0.dev20230519/LICENSE
--rw-r--r--   0        0        0    10297 2023-05-19 23:02:42.853466 flwr_nightly-1.5.0.dev20230519/README.md
--rw-r--r--   0        0        0     4268 2023-05-19 23:03:07.641859 flwr_nightly-1.5.0.dev20230519/pyproject.toml
--rw-r--r--   0        0        0      952 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    13514 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     6503 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3351 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4288 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      712 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1686 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5100 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8194 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1876 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1044 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1828 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1894 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3483 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3909 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4414 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5654 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     3217 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    23751 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5602 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4627 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11523 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6314 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1638 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3718 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4457 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15891 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6521 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19296 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4805 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1648 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6105 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4519 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4875 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5830 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6730 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7012 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11495 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9985 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8805 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     6321 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5393 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7708 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5924 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     7624 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7044 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6863 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10147 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5114 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4941 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7777 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5472 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12394 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230519/setup.py
--rw-r--r--   0        0        0    12772 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230519/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-22 23:02:50.109359 flwr_nightly-1.5.0.dev20230522/LICENSE
+-rw-r--r--   0        0        0    10297 2023-05-22 23:02:50.109359 flwr_nightly-1.5.0.dev20230522/README.md
+-rw-r--r--   0        0        0     4268 2023-05-22 23:03:27.637348 flwr_nightly-1.5.0.dev20230522/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    13838 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     6503 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4293 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     5476 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1686 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5100 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8336 2023-05-22 23:02:50.449360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1876 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1828 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1894 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3483 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16316 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3909 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4414 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5654 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3217 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4286 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26297 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     5941 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2228 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1058 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5602 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6416 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4627 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11523 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6314 2023-05-22 23:02:50.453360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     1858 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3718 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4457 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15963 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6521 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4805 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1648 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6100 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4519 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4875 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5830 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6730 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7012 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11495 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9985 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8252 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2674 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5393 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7065 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5924 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3368 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7044 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6310 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10147 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5114 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4941 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7777 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5472 2023-05-22 23:02:50.457360 flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12427 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230522/setup.py
+-rw-r--r--   0        0        0    12772 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230522/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230519/LICENSE` & `flwr_nightly-1.5.0.dev20230522/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/README.md` & `flwr_nightly-1.5.0.dev20230522/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/pyproject.toml` & `flwr_nightly-1.5.0.dev20230522/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230519"
+version = "1.5.0-dev20230522"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_BIDI,
+    TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPES,
 )
 from flwr.common.logger import log
 from flwr.common.typing import (
     Code,
     EvaluateIns,
@@ -47,14 +48,15 @@
     GetPropertiesRes,
     NDArrays,
     Status,
 )
 
 from .client import Client
 from .grpc_client.connection import grpc_connection
+from .grpc_rere_client.connection import grpc_request_response
 from .message_handler.message_handler import handle
 from .numpy_client import NumPyClient
 from .numpy_client import has_evaluate as numpyclient_has_evaluate
 from .numpy_client import has_fit as numpyclient_has_fit
 from .numpy_client import has_get_parameters as numpyclient_has_get_parameters
 from .numpy_client import has_get_properties as numpyclient_has_get_properties
 
@@ -83,15 +85,15 @@
     0.5, 10, {"accuracy": 0.95}
 
 """
 
 ClientLike = Union[Client, NumPyClient]
 
 
-# pylint: disable=import-outside-toplevel,too-many-locals
+# pylint: disable=import-outside-toplevel,too-many-locals,too-many-branches
 def start_client(
     *,
     server_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
     rest: bool = False,  # Deprecated in favor of `transport`
@@ -123,14 +125,15 @@
         DEPRECATED - USE 'transport' INSTEAD.
         Defines whether or not the client is interacting with the server using the
         experimental REST API. This feature is experimental, it might change
         considerably in future versions of Flower.
     transport : Optional[str] (default: None)
         Configure the transport layer. Allowed values:
         - 'grpc-bidi': gRPC, bidirectional streaming
+        - 'grpc-rere': gRPC, request-response (experimental)
         - 'rest': HTTP (experimental)
 
     Examples
     --------
     Starting a gRPC client with an insecure server connection:
 
     >>> start_client(
@@ -169,14 +172,16 @@
             sys.exit(MISSING_EXTRA_REST)
         if server_address[:4] != "http":
             sys.exit(
                 "When using the REST API, please provide `https://` or "
                 "`http://` before the server address (e.g. `http://127.0.0.1:8080`)"
             )
         connection = http_request_response
+    elif transport == TRANSPORT_TYPE_GRPC_RERE:
+        connection = grpc_request_response
     elif transport == TRANSPORT_TYPE_GRPC_BIDI:
         connection = grpc_connection
     else:
         raise ValueError(
             f"Unknown transport type: {transport} (possible: {TRANSPORT_TYPES})"
         )
 
@@ -248,14 +253,15 @@
         DEPRECATED - USE 'transport' INSTEAD.
         Defines whether or not the client is interacting with the server using the
         experimental REST API. This feature is experimental, it might change
         considerably in future versions of Flower.
     transport : Optional[str] (default: None)
         Configure the transport layer. Allowed values:
         - 'grpc-bidi': gRPC, bidirectional streaming
+        - 'grpc-rere': gRPC, request-response (experimental)
         - 'rest': HTTP (experimental)
 
     Examples
     --------
     Starting a client with an insecure server connection:
 
     >>> start_client(
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/grpc_client/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Contextmanager managing a gRPC channel to the Flower server."""
+"""Contextmanager for a gRPC streaming channel to the Flower server."""
 
 
 from contextlib import contextmanager
 from logging import DEBUG
 from pathlib import Path
 from queue import Queue
 from typing import Callable, Iterator, Optional, Tuple, Union
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/client/rest_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Contextmanager managing a REST-based channel to the Flower server."""
+"""Contextmanager for a REST request-response channel to the Flower server."""
 
 
 import sys
 from contextlib import contextmanager
 from logging import ERROR, INFO, WARN
-from typing import Callable, Dict, Iterator, Optional, Tuple, Union
+from typing import Callable, Dict, Iterator, Optional, Tuple, Union, cast
 
 from flwr.client.message_handler.task_handler import get_server_message
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.common.logger import log
 from flwr.proto.fleet_pb2 import (
     PullTaskInsRequest,
@@ -36,14 +36,17 @@
 
 try:
     import requests
 except ModuleNotFoundError:
     sys.exit(MISSING_EXTRA_REST)
 
 
+KEY_TASK_INS = "current_task_ins"
+
+
 PATH_PULL_TASK_INS: str = "api/v0/fleet/pull-task-ins"
 PATH_PUSH_TASK_RES: str = "api/v0/fleet/push-task-res"
 
 
 @contextmanager
 def http_request_response(
     server_address: str,
@@ -98,15 +101,15 @@
         log(
             ERROR,
             "For the REST API, the root certificates "
             "must be provided as a string path to the client.",
         )
 
     # Necessary state to link TaskRes to TaskIns
-    state: Dict[str, Optional[TaskIns]] = {"current_task_ins": None}
+    state: Dict[str, Optional[TaskIns]] = {KEY_TASK_INS: None}
 
     ###########################################################################
     # receive/send functions
     ###########################################################################
 
     def receive() -> Optional[ServerMessage]:
         """Receive next task from server."""
@@ -149,41 +152,45 @@
         # Deserialize ProtoBuf from bytes
         pull_task_ins_response_proto = PullTaskInsResponse()
         pull_task_ins_response_proto.ParseFromString(res.content)
 
         # Remember the current TaskIns
         task_ins_server_message_tuple = get_server_message(pull_task_ins_response_proto)
         if task_ins_server_message_tuple is None:
-            state["current_task_ins"] = None
+            state[KEY_TASK_INS] = None
             return None
 
         task_ins, server_message = task_ins_server_message_tuple
 
         # Remember `task_ins` until `task_res` is available
-        state["current_task_ins"] = task_ins
+        state[KEY_TASK_INS] = task_ins
 
         # Return the ServerMessage
         log(INFO, "[Node] POST /%s: success", PATH_PULL_TASK_INS)
         return server_message
 
     def send(client_message_proto: ClientMessage) -> None:
         """Send task result back to server."""
 
-        if state["current_task_ins"] is None:
+        if state[KEY_TASK_INS] is None:
             log(ERROR, "No current TaskIns")
             return
 
+        task_ins: TaskIns = cast(TaskIns, state[KEY_TASK_INS])
+
         # Wrap ClientMessage in TaskRes
         task_res = TaskRes(
             task_id="",  # This will be generated by the server
+            group_id=task_ins.group_id,
+            workload_id=task_ins.workload_id,
             task=Task(
                 producer=Node(node_id=0, anonymous=True),
-                consumer=Node(node_id=0, anonymous=True),
+                consumer=task_ins.task.producer,
                 legacy_client_message=client_message_proto,
-                ancestry=[state["current_task_ins"].task_id],
+                ancestry=[task_ins.task_id],
             ),
         )
 
         # Serialize ProtoBuf to bytes
         push_task_res_request_proto = PushTaskResRequest(task_res_list=[task_res])
         push_task_res_request_bytes: bytes = (
             push_task_res_request_proto.SerializeToString()
@@ -196,15 +203,15 @@
                 "Accept": "application/protobuf",
                 "Content-Type": "application/protobuf",
             },
             data=push_task_res_request_bytes,
             verify=verify,
         )
 
-        state["current_task_ins"] = None
+        state[KEY_TASK_INS] = None
 
         # Check status code and headers
         if res.status_code != 200:
             return
         if "content-type" not in res.headers:
             log(
                 WARN,
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/constant.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 
 To use the REST API, install `flwr` with the `rest` extra:
 
     `pip install flwr[rest]`.
 """
 
 TRANSPORT_TYPE_GRPC_BIDI = "grpc-bido"
+TRANSPORT_TYPE_GRPC_RERE = "grpc-rere"
 TRANSPORT_TYPE_REST = "rest"
 TRANSPORT_TYPES = [
     TRANSPORT_TYPE_GRPC_BIDI,
+    TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
 ]
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,30 @@
 import grpc
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_BIDI,
+    TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
 )
 from flwr.common.logger import log
 from flwr.proto.driver_pb2_grpc import add_DriverServicer_to_server
+from flwr.proto.fleet_pb2_grpc import add_FleetServicer_to_server
 from flwr.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
 from flwr.server.client_manager import ClientManager, SimpleClientManager
 from flwr.server.driver.driver_servicer import DriverServicer
 from flwr.server.fleet.grpc_bidi.driver_client_manager import DriverClientManager
 from flwr.server.fleet.grpc_bidi.flower_service_servicer import FlowerServiceServicer
 from flwr.server.fleet.grpc_bidi.grpc_server import (
     generic_create_grpc_server,
     start_grpc_server,
 )
+from flwr.server.fleet.grpc_rere.fleet_servicer import FleetServicer
 from flwr.server.history import History
 from flwr.server.server import Server
 from flwr.server.state import StateFactory
 from flwr.server.strategy import FedAvg, Strategy
 
 ADDRESS_DRIVER_API = "0.0.0.0:9091"
 ADDRESS_FLEET_API_GRPC_RERE = "0.0.0.0:9092"
@@ -313,14 +316,26 @@
         host, port, is_v6 = parsed_address
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_bidi(
             address=address,
             state_factory=state_factory,
         )
         grpc_servers.append(fleet_server)
+    elif args.fleet_api_type == TRANSPORT_TYPE_GRPC_RERE:
+        address_arg = args.grpc_rere_fleet_api_address
+        parsed_address = parse_address(address_arg)
+        if not parsed_address:
+            sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
+        host, port, is_v6 = parsed_address
+        address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+        fleet_server = _run_fleet_api_grpc_rere(
+            address=address,
+            state_factory=state_factory,
+        )
+        grpc_servers.append(fleet_server)
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
     _register_exit_handlers(
         grpc_servers=grpc_servers,
         bckg_threads=bckg_threads,
@@ -330,14 +345,15 @@
     # Block
     if len(grpc_servers) > 0:
         grpc_servers[0].wait_for_termination()
     elif len(bckg_threads) > 0:
         bckg_threads[0].join()
 
 
+# pylint: disable=too-many-branches
 def run_server() -> None:
     """Run Flower server (Driver API and Fleet API)."""
 
     log(INFO, "Starting Flower server")
     event(EventType.RUN_SERVER_ENTER)
     args = _parse_args_server().parse_args()
 
@@ -384,25 +400,37 @@
                 state_factory,
                 args.rest_fleet_api_workers,
             ),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
     elif args.fleet_api_type == TRANSPORT_TYPE_GRPC_BIDI:
-        address_arg = args.grpc_fleet_api_address
+        address_arg = args.grpc_bidi_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
             sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
         host, port, is_v6 = parsed_address
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_bidi(
             address=address,
             state_factory=state_factory,
         )
         grpc_servers.append(fleet_server)
+    elif args.fleet_api_type == TRANSPORT_TYPE_GRPC_RERE:
+        address_arg = args.grpc_rere_fleet_api_address
+        parsed_address = parse_address(address_arg)
+        if not parsed_address:
+            sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
+        host, port, is_v6 = parsed_address
+        address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+        fleet_server = _run_fleet_api_grpc_rere(
+            address=address,
+            state_factory=state_factory,
+        )
+        grpc_servers.append(fleet_server)
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
     _register_exit_handlers(
         grpc_servers=grpc_servers,
         bckg_threads=bckg_threads,
@@ -514,14 +542,38 @@
 
     log(INFO, "Flower ECE: Starting Fleet API (gRPC-bidi) on %s", address)
     fleet_grpc_server.start()
 
     return fleet_grpc_server
 
 
+def _run_fleet_api_grpc_rere(
+    address: str,
+    state_factory: StateFactory,
+) -> grpc.Server:
+    """Run Fleet API (gRPC, request-response)."""
+
+    # Create Fleet API gRPC server
+    fleet_servicer = FleetServicer(
+        state=state_factory.state(),
+    )
+    fleet_add_servicer_to_server_fn = add_FleetServicer_to_server
+    fleet_grpc_server = generic_create_grpc_server(
+        servicer_and_add_fn=(fleet_servicer, fleet_add_servicer_to_server_fn),
+        server_address=address,
+        max_message_length=GRPC_MAX_MESSAGE_LENGTH,
+        certificates=None,
+    )
+
+    log(INFO, "Flower ECE: Starting Fleet API (gRPC-rere) on %s", address)
+    fleet_grpc_server.start()
+
+    return fleet_grpc_server
+
+
 # pylint: disable=import-outside-toplevel,too-many-arguments
 def _run_fleet_api_rest(
     host: str,
     port: int,
     ssl_keyfile: Optional[str],
     ssl_certfile: Optional[str],
     state_factory: StateFactory,
@@ -668,14 +720,21 @@
         action="store_const",
         dest="fleet_api_type",
         const=TRANSPORT_TYPE_GRPC_BIDI,
         default=TRANSPORT_TYPE_GRPC_BIDI,
         help="Start a Fleet API server (gRPC-bidi)",
     )
     ex_group.add_argument(
+        "--grpc-rere",
+        action="store_const",
+        dest="fleet_api_type",
+        const=TRANSPORT_TYPE_GRPC_RERE,
+        help="Start a Fleet API server (gRPC-rere)",
+    )
+    ex_group.add_argument(
         "--rest",
         action="store_const",
         dest="fleet_api_type",
         const=TRANSPORT_TYPE_REST,
         help="Start a Fleet API server (REST, experimental)",
     )
 
@@ -685,14 +744,23 @@
     )
     grpc_bidi_group.add_argument(
         "--grpc-bidi-fleet-api-address",
         help="Fleet API (gRPC-bidi) server address (IPv4, IPv6, or a domain name)",
         default=ADDRESS_FLEET_API_GRPC_RERE,
     )
 
+    # Fleet API gRPC-rere options
+    grpc_rere_group = parser.add_argument_group(
+        "Fleet API (gRPC-rere) server options", ""
+    )
+    grpc_rere_group.add_argument(
+        "--grpc-rere-fleet-api-address",
+        help="Fleet API (gRPC-rere) server address (IPv4, IPv6, or a domain name)",
+    )
+
     # Fleet API REST options
     rest_group = parser.add_argument_group("Fleet API (REST) server options", "")
     rest_group.add_argument(
         "--rest-fleet-api-address",
         help="Fleet API (REST) server address (IPv4, IPv6, or a domain name)",
         default=ADDRESS_FLEET_API_REST,
     )
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,46 +8,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Fleet API servicer."""
+"""Fleet API gRPC request-response servicer."""
 
 
 from logging import INFO
 
 import grpc
 
 from flwr.common.logger import log
 from flwr.proto import fleet_pb2_grpc
 from flwr.proto.fleet_pb2 import (
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
+from flwr.server.fleet.message_handler import message_handler
 from flwr.server.state import State
 
 
 class FleetServicer(fleet_pb2_grpc.FleetServicer):
     """Fleet API servicer."""
 
     def __init__(self, state: State) -> None:
         self.state = state
 
     def PullTaskIns(
         self, request: PullTaskInsRequest, context: grpc.ServicerContext
     ) -> PullTaskInsResponse:
-        """."""
+        """Pull TaskIns."""
         log(INFO, "FleetServicer.PullTaskIns")
-
-        return PullTaskInsResponse(task_ins_list=[])
+        return message_handler.pull_task_ins(
+            request=request,
+            state=self.state,
+        )
 
     def PushTaskRes(
         self, request: PushTaskResRequest, context: grpc.ServicerContext
     ) -> PushTaskResResponse:
-        """."""
+        """Push TaskRes."""
         log(INFO, "FleetServicer.PushTaskRes")
-
-        return PushTaskResResponse(reconnect=None, results={})
+        return message_handler.push_task_res(
+            request=request,
+            state=self.state,
+        )
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,18 @@
 ]
 
 
 class Server:
     """Flower server."""
 
     def __init__(
-        self, *, client_manager: ClientManager, strategy: Optional[Strategy] = None
+        self,
+        *,
+        client_manager: ClientManager,
+        strategy: Optional[Strategy] = None,
     ) -> None:
         self._client_manager: ClientManager = client_manager
         self.parameters: Parameters = Parameters(
             tensors=[], tensor_type="numpy.ndarray"
         )
         self.strategy: Strategy = strategy if strategy is not None else FedAvg()
         self.max_workers: Optional[int] = None
@@ -99,15 +102,18 @@
 
         # Run federated learning for num_rounds
         log(INFO, "FL starting")
         start_time = timeit.default_timer()
 
         for current_round in range(1, num_rounds + 1):
             # Train model and replace previous global model
-            res_fit = self.fit_round(server_round=current_round, timeout=timeout)
+            res_fit = self.fit_round(
+                server_round=current_round,
+                timeout=timeout,
+            )
             if res_fit is not None:
                 parameters_prime, fit_metrics, _ = res_fit  # fit_metrics_aggregated
                 if parameters_prime:
                     self.parameters = parameters_prime
                 history.add_metrics_distributed_fit(
                     server_round=current_round, metrics=fit_metrics
                 )
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     if to_keep > 0:
         # Choose to_keep clients and return their average (MultiKrum)
         best_indices = np.argsort(scores)[::-1][len(scores) - to_keep :]  # noqa: E203
         best_results = [results[i] for i in best_indices]
         return aggregate(best_results)
 
-    # Return the index of the client which minimizes the score (Krum)
+    # Return the model parameters that minimize the score (Krum)
     return weights[np.argmin(scores)]
 
 
 def weighted_loss_avg(results: List[Tuple[int, float]]) -> float:
     """Aggregate evaluation results obtained from multiple clients."""
     num_total_evaluation_examples = sum([num_examples for num_examples, _ in results])
     weighted_losses = [num_examples * loss for num_examples, loss in results]
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedavgm.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,14 @@
 from flwr.common.logger import log
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate
 from .fedavg import FedAvg
 
-WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
-Setting `min_available_clients` lower than `min_fit_clients` or
-`min_evaluate_clients` can cause the server to fail when there are too few clients
-connected to the server. `min_available_clients` must be set to a value larger
-than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
-"""
-
 
 # flake8: noqa: E501
 class FedAvgM(FedAvg):
     """Configurable FedAvg with Momentum strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
@@ -102,20 +95,14 @@
         server_learning_rate: float
             Server-side learning rate used in server-side optimization.
             Defaults to 1.0.
         server_momentum: float
             Server-side momentum factor used for FedAvgM. Defaults to 0.0.
         """
 
-        if (
-            min_fit_clients > min_available_clients
-            or min_evaluate_clients > min_available_clients
-        ):
-            log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/krum.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated Median (FedMedian) [Yin et al., 2018] strategy.
+"""Machine Learning with Adversaries: Byzantine Tolerant Gradient Descent.
 
-Paper: https://arxiv.org/pdf/1803.01498v1.pdf
+[Blanchard et al., 2017].
+
+Paper: https://proceedings.neurips.cc/paper/2017/file/f4b9ec30ad9f68f89b29639786cb62ef-Paper.pdf
 """
 
 
 from logging import WARNING
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from flwr.common import (
@@ -29,124 +31,119 @@
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
-from .aggregate import aggregate_median
+from .aggregate import aggregate_krum
 from .fedavg import FedAvg
 
-WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
-Setting `min_available_clients` lower than `min_fit_clients` or
-`min_evaluate_clients` can cause the server to fail when there are too few clients
-connected to the server. `min_available_clients` must be set to a value larger
-than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
-"""
-
 
 # flake8: noqa: E501
-class FedMedian(FedAvg):
-    """Configurable FedAvg with Momentum strategy implementation."""
+class Krum(FedAvg):
+    """Configurable Krum strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        num_malicious_clients: int = 0,
+        num_clients_to_keep: int = 0,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
-        """Configurable FedMedian strategy.
-
-        Implementation based on https://arxiv.org/pdf/1803.01498v1.pdf
+        """Configurable Krum strategy.
 
         Parameters
         ----------
         fraction_fit : float, optional
             Fraction of clients used during training. Defaults to 0.1.
         fraction_evaluate : float, optional
             Fraction of clients used during validation. Defaults to 0.1.
         min_fit_clients : int, optional
             Minimum number of clients used during training. Defaults to 2.
         min_evaluate_clients : int, optional
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : int, optional
             Minimum number of total clients in the system. Defaults to 2.
+        num_malicious_clients : int, optional
+            Number of malicious clients in the system. Defaults to 0.
+        num_clients_to_keep : int, optional
+            Number of clients to keep before averaging (MultiKrum). Defaults to 0, in that case classical Krum is applied.
         evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
         initial_parameters : Parameters, optional
             Initial global model parameters.
         """
 
-        if (
-            min_fit_clients > min_available_clients
-            or min_evaluate_clients > min_available_clients
-        ):
-            log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
         )
+        self.num_malicious_clients = num_malicious_clients
+        self.num_clients_to_keep = num_clients_to_keep
 
     def __repr__(self) -> str:
-        rep = f"FedMedian(accept_failures={self.accept_failures})"
+        rep = f"Krum(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
     ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
-        """Aggregate fit results using median."""
+        """Aggregate fit results using Krum."""
         if not results:
             return None, {}
         # Do not aggregate if there are failures and failures are not accepted
         if not self.accept_failures and failures:
             return None, {}
 
         # Convert results
         weights_results = [
             (parameters_to_ndarrays(fit_res.parameters), fit_res.num_examples)
             for _, fit_res in results
         ]
         parameters_aggregated = ndarrays_to_parameters(
-            aggregate_median(weights_results)
+            aggregate_krum(
+                weights_results, self.num_malicious_clients, self.num_clients_to_keep
+            )
         )
 
         # Aggregate custom metrics if aggregation fn was provided
         metrics_aggregated = {}
         if self.fit_metrics_aggregation_fn:
             fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedprox.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,31 +14,22 @@
 # ==============================================================================
 """Federated Optimization (FedProx) [Li et al., 2018] strategy.
 
 Paper: https://arxiv.org/abs/1812.06127
 """
 
 
-from logging import WARNING
 from typing import Callable, Dict, List, Optional, Tuple
 
 from flwr.common import FitIns, MetricsAggregationFn, NDArrays, Parameters, Scalar
-from flwr.common.logger import log
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
 from .fedavg import FedAvg
 
-WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
-Setting `min_available_clients` lower than `min_fit_clients` or
-`min_evaluate_clients` can cause the server to fail when there are too few clients
-connected to the server. `min_available_clients` must be set to a value larger
-than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
-"""
-
 
 # flake8: noqa: E501
 class FedProx(FedAvg):
     """Configurable FedProx strategy implementation."""
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
     def __init__(
@@ -128,21 +119,14 @@
             Metrics aggregation function, optional.
         proximal_mu : float
             The weight of the proximal term used in the optimization. 0.0 makes
             this strategy equivalent to FedAvg, and the higher the coefficient, the more
             regularization will be used (that is, the client parameters will need to be
             closer to the server parameters during training).
         """
-        super().__init__()
-
-        if (
-            min_fit_clients > min_available_clients
-            or min_evaluate_clients > min_available_clients
-        ):
-            log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
 
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/fedyogi.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,52 +8,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated XGBoost in the horizontal setting based on building Neural Network
-and averaging on prediction outcomes [Ma et al., 2023].
+"""Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020]
+strategy.
 
-Paper: Coming
+Paper: https://arxiv.org/abs/2003.00295
 """
 
 
-from logging import WARNING
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
+
+import numpy as np
 
 from flwr.common import (
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
-from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
-from .aggregate import aggregate
-from .fedavg import FedAvg
-
-WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW = """
-Setting `min_available_clients` lower than `min_fit_clients` or
-`min_evaluate_clients` can cause the server to fail when there are too few clients
-connected to the server. `min_available_clients` must be set to a value larger
-than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
-"""
+from .fedopt import FedOpt
 
 
 # flake8: noqa: E501
-class FedXgbNnAvg(FedAvg):
-    """Configurable FedXgbNnAvg strategy implementation."""
+class FedYogi(FedOpt):
+    """Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al.,
+    2020] strategy.
+
+    Paper: https://arxiv.org/abs/2003.00295
+    """
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals,line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -63,120 +59,126 @@
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
-        initial_parameters: Optional[Parameters] = None,
+        initial_parameters: Parameters,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
+        eta: float = 1e-2,
+        eta_l: float = 0.0316,
+        beta_1: float = 0.9,
+        beta_2: float = 0.99,
+        tau: float = 1e-3,
     ) -> None:
-        """Federated XGBoost based on building Neural Network and averaging on
-        prediction outcomes strategy.
+        """Federated learning strategy using Yogi on server-side.
+
+        Implementation based on https://arxiv.org/abs/2003.00295v5
 
         Parameters
         ----------
         fraction_fit : float, optional
-            Fraction of clients used during training. In case `min_fit_clients`
-            is larger than `fraction_fit * available_clients`, `min_fit_clients`
-            will still be sampled. Defaults to 1.0.
+            Fraction of clients used during training. Defaults to 1.0.
         fraction_evaluate : float, optional
-            Fraction of clients used during validation. In case `min_evaluate_clients`
-            is larger than `fraction_evaluate * available_clients`, `min_evaluate_clients`
-            will still be sampled. Defaults to 1.0.
+            Fraction of clients used during validation. Defaults to 1.0.
         min_fit_clients : int, optional
             Minimum number of clients used during training. Defaults to 2.
         min_evaluate_clients : int, optional
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : int, optional
             Minimum number of total clients in the system. Defaults to 2.
         evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
-        initial_parameters : Parameters, optional
+        initial_parameters : Parameters
             Initial global model parameters.
         fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
-        evaluate_metrics_aggregation_fn : Optional[MetricsAggregationFn]
+        evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
             Metrics aggregation function, optional.
+        eta : float, optional
+            Server-side learning rate. Defaults to 1e-1.
+        eta_l : float, optional
+            Client-side learning rate. Defaults to 1e-1.
+        beta_1 : float, optional
+            Momentum parameter. Defaults to 0.9.
+        beta_2 : float, optional
+            Second moment parameter. Defaults to 0.99.
+        tau : float, optional
+            Controls the algorithm's degree of adaptability.
+            Defaults to 1e-9.
         """
-        super().__init__()
-
-        if (
-            min_fit_clients > min_available_clients
-            or min_evaluate_clients > min_available_clients
-        ):
-            log(WARNING, WARNING_MIN_AVAILABLE_CLIENTS_TOO_LOW)
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
+            eta=eta,
+            eta_l=eta_l,
+            beta_1=beta_1,
+            beta_2=beta_2,
+            tau=tau,
         )
 
     def __repr__(self) -> str:
-        rep = f"FedXgbNnAvg(accept_failures={self.accept_failures})"
+        rep = f"FedYogi(accept_failures={self.accept_failures})"
         return rep
 
-    def evaluate(
-        self, server_round: int, parameters: Any
-    ) -> Optional[Tuple[float, Dict[str, Scalar]]]:
-        """Evaluate model parameters using an evaluation function."""
-        if self.evaluate_fn is None:
-            # No evaluation function provided
-            return None
-        eval_res = self.evaluate_fn(server_round, parameters, {})
-        if eval_res is None:
-            return None
-        loss, metrics = eval_res
-        return loss, metrics
-
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
-    ) -> Tuple[Optional[Any], Dict[str, Scalar],]:
+    ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
         """Aggregate fit results using weighted average."""
-        if not results:
-            return None, {}
-        # Do not aggregate if there are failures and failures are not accepted
-        if not self.accept_failures and failures:
+        fedavg_parameters_aggregated, metrics_aggregated = super().aggregate_fit(
+            server_round=server_round, results=results, failures=failures
+        )
+        if fedavg_parameters_aggregated is None:
             return None, {}
 
-        # Convert results
-        weights_results = [
-            (
-                parameters_to_ndarrays(fit_res.parameters[0].parameters),  # type: ignore
-                fit_res.num_examples,
-            )
-            for _, fit_res in results
+        fedavg_weights_aggregate = parameters_to_ndarrays(fedavg_parameters_aggregated)
+
+        # Yogi
+        delta_t: NDArrays = [
+            x - y for x, y in zip(fedavg_weights_aggregate, self.current_weights)
+        ]
+
+        # m_t
+        if not self.m_t:
+            self.m_t = [np.zeros_like(x) for x in delta_t]
+        self.m_t = [
+            np.multiply(self.beta_1, x) + (1 - self.beta_1) * y
+            for x, y in zip(self.m_t, delta_t)
+        ]
+
+        # v_t
+        if not self.v_t:
+            self.v_t = [np.zeros_like(x) for x in delta_t]
+        self.v_t = [
+            x - (1.0 - self.beta_2) * np.multiply(y, y) * np.sign(x - np.multiply(y, y))
+            for x, y in zip(self.v_t, delta_t)
         ]
-        parameters_aggregated = ndarrays_to_parameters(aggregate(weights_results))
 
-        # Aggregate XGBoost trees from all clients
-        trees_aggregated = [fit_res.parameters[1] for _, fit_res in results]  # type: ignore
+        new_weights = [
+            x + self.eta * y / (np.sqrt(z) + self.tau)
+            for x, y, z in zip(self.current_weights, self.m_t, self.v_t)
+        ]
 
-        # Aggregate custom metrics if aggregation fn was provided
-        metrics_aggregated = {}
-        if self.fit_metrics_aggregation_fn:
-            fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
-            metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
-        elif server_round == 1:  # Only log this warning once
-            log(WARNING, "No fit_metrics_aggregation_fn provided")
+        self.current_weights = new_weights
 
-        return [parameters_aggregated, trees_aggregated], metrics_aggregated
+        return ndarrays_to_parameters(self.current_weights), metrics_aggregated
```

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230522/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230519/setup.py` & `flwr_nightly-1.5.0.dev20230522/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 package_dir = \
 {'': 'src/py'}
 
 packages = \
 ['flwr',
  'flwr.client',
  'flwr.client.grpc_client',
+ 'flwr.client.grpc_rere_client',
  'flwr.client.message_handler',
  'flwr.client.rest_client',
  'flwr.common',
  'flwr.driver',
  'flwr.proto',
  'flwr.server',
  'flwr.server.driver',
@@ -47,15 +48,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.5.0.dev20230519',
+    'version': '1.5.0.dev20230522',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': 'src/
 py'} packages = \ ['flwr', 'flwr.client', 'flwr.client.grpc_client',
-'flwr.client.message_handler', 'flwr.client.rest_client', 'flwr.common',
-'flwr.driver', 'flwr.proto', 'flwr.server', 'flwr.server.driver',
-'flwr.server.fleet', 'flwr.server.fleet.grpc_bidi',
-'flwr.server.fleet.grpc_rere', 'flwr.server.fleet.message_handler',
-'flwr.server.fleet.rest_rere', 'flwr.server.state', 'flwr.server.strategy',
-'flwr.server.utils', 'flwr.simulation', 'flwr.simulation.ray_transport']
-package_data = \ {'': ['*']} install_requires = \
-['grpcio>=1.48.2,<2.0.0,!=1.52.0', 'iterators>=0.0.2,<0.0.3',
-'numpy>=1.21.0,<2.0.0', 'protobuf>=3.19.0,<4.0.0'] extras_require = \ {':
-python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'], 'rest':
-['requests>=2.28.2,<3.0.0', 'fastapi>=0.95.0,<0.96.0',
-'starlette>=0.26.1,<0.27.0', 'uvicorn[standard]>=0.21.1,<0.22.0'],
-'simulation': ['ray[default]>=2.4.0,<3.0.0']} entry_points = \
-{'console_scripts': ['flower-client = flwr.client:run_client', 'flower-driver-
-api = flwr.server:run_driver_api', 'flower-fleet-api = flwr.server:
-run_fleet_api', 'flower-server = flwr.server:run_server']} setup_kwargs =
-{ 'name': 'flwr-nightly', 'version': '1.5.0.dev20230519', 'description':
-'Flower: A Friendly Federated Learning Framework', 'long_description': '#
-Flower: A Friendly Federated Learning Framework\n\n
+'flwr.client.grpc_rere_client', 'flwr.client.message_handler',
+'flwr.client.rest_client', 'flwr.common', 'flwr.driver', 'flwr.proto',
+'flwr.server', 'flwr.server.driver', 'flwr.server.fleet',
+'flwr.server.fleet.grpc_bidi', 'flwr.server.fleet.grpc_rere',
+'flwr.server.fleet.message_handler', 'flwr.server.fleet.rest_rere',
+'flwr.server.state', 'flwr.server.strategy', 'flwr.server.utils',
+'flwr.simulation', 'flwr.simulation.ray_transport'] package_data = \ {'':
+['*']} install_requires = \ ['grpcio>=1.48.2,<2.0.0,!=1.52.0',
+'iterators>=0.0.2,<0.0.3', 'numpy>=1.21.0,<2.0.0', 'protobuf>=3.19.0,<4.0.0']
+extras_require = \ {':python_version < "3.8"': ['importlib-
+metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
+'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
+[standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.4.0,<3.0.0']}
+entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
+'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
+flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
+setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230522',
+'description': 'Flower: A Friendly Federated Learning Framework',
+'long_description': '# Flower: A Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
 \n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)]
 (https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://
```

### Comparing `flwr_nightly-1.5.0.dev20230519/PKG-INFO` & `flwr_nightly-1.5.0.dev20230522/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230519
+Version: 1.5.0.dev20230522
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230519 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230522 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

