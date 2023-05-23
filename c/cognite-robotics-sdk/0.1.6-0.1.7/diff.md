# Comparing `tmp/cognite_robotics_sdk-0.1.6.tar.gz` & `tmp/cognite_robotics_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_robotics_sdk-0.1.6.tar", max compression
+gzip compressed data, was "cognite_robotics_sdk-0.1.7.tar", max compression
```

## Comparing `cognite_robotics_sdk-0.1.6.tar` & `cognite_robotics_sdk-0.1.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1252 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/README.md
--rw-r--r--   0        0        0       74 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/__init__.py
--rw-r--r--   0        0        0     1190 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/config/config.py
--rw-r--r--   0        0        0      255 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_classes.py
--rw-r--r--   0        0        0       67 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_classes.py
--rw-r--r--   0        0        0    11878 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader.py
--rw-r--r--   0        0        0     1662 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader_task.py
--rw-r--r--   0        0        0    11675 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/helpers.py
--rw-r--r--   0        0        0     9034 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/robot_interface_client.py
--rw-r--r--   0        0        0     1505 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/web_interface_client.py
--rw-r--r--   0        0        0       62 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/__init__.py
--rw-r--r--   0        0        0      821 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/bearer_token_auth.py
--rw-r--r--   0        0        0      826 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/channel.py
--rw-r--r--   0        0        0    10327 2023-05-10 08:49:07.565107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/messages.py
--rw-r--r--   0        0        0        0 2023-05-10 09:02:55.487861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/__init__.py
--rw-r--r--   0        0        0     1453 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.py
--rw-r--r--   0        0        0     1702 2023-05-10 09:02:55.469859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.pyi
--rw-r--r--   0        0        0     2519 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.py
--rw-r--r--   0        0        0     6430 2023-05-10 09:02:55.469859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.pyi
--rw-r--r--   0        0        0     3047 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.py
--rw-r--r--   0        0        0     7303 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.pyi
--rw-r--r--   0        0        0     2302 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.py
--rw-r--r--   0        0        0     4811 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.pyi
--rw-r--r--   0        0        0     3228 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.py
--rw-r--r--   0        0        0     8503 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.pyi
--rw-r--r--   0        0        0     1444 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.py
--rw-r--r--   0        0        0     1705 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.pyi
--rw-r--r--   0        0        0     2590 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.py
--rw-r--r--   0        0        0     5930 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.pyi
--rw-r--r--   0        0        0     1842 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.py
--rw-r--r--   0        0        0     2460 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.pyi
--rw-r--r--   0        0        0     2384 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.py
--rw-r--r--   0        0        0     5977 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.pyi
--rw-r--r--   0        0        0     1461 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.py
--rw-r--r--   0        0        0     1805 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.pyi
--rw-r--r--   0        0        0     8330 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.py
--rw-r--r--   0        0        0    23660 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.pyi
--rw-r--r--   0        0        0     2549 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.py
--rw-r--r--   0        0        0     4966 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.pyi
--rw-r--r--   0        0        0     4899 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.py
--rw-r--r--   0        0        0    12598 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.pyi
--rw-r--r--   0        0        0     4507 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.py
--rw-r--r--   0        0        0    15277 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.pyi
--rw-r--r--   0        0        0     1597 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.py
--rw-r--r--   0        0        0     2003 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.pyi
--rw-r--r--   0        0        0     2845 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2.pyi
--rw-r--r--   0        0        0    15062 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
--rw-r--r--   0        0        0     2853 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2.pyi
--rw-r--r--   0        0        0    14820 2023-05-10 09:02:55.493861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2_grpc.py
--rw-r--r--   0        0        0       60 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/__init__.py
--rw-r--r--   0        0        0      943 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/base_model.py
--rw-r--r--   0        0        0       64 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/client.py
--rw-r--r--   0        0        0    50682 2023-05-10 09:02:57.518000 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/models.py
--rw-r--r--   0        0        0       58 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/env_utils.py
--rw-r--r--   0        0        0     3016 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/token.py
--rw-r--r--   0        0        0     3153 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/utils.py
--rw-r--r--   0        0        0     1460 2023-05-10 08:49:07.568107 cognite_robotics_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1252 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0       74 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/__init__.py
+-rw-r--r--   0        0        0     1190 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/config/config.py
+-rw-r--r--   0        0        0      560 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_classes.py
+-rw-r--r--   0        0        0       67 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_classes.py
+-rw-r--r--   0        0        0    11878 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader.py
+-rw-r--r--   0        0        0     1662 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader_task.py
+-rw-r--r--   0        0        0    11669 2023-05-23 10:59:30.347036 cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/helpers.py
+-rw-r--r--   0        0        0     9034 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/robot_interface_client.py
+-rw-r--r--   0        0        0     1505 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/web_interface_client.py
+-rw-r--r--   0        0        0       62 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/__init__.py
+-rw-r--r--   0        0        0      821 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/bearer_token_auth.py
+-rw-r--r--   0        0        0      826 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/channel.py
+-rw-r--r--   0        0        0    10327 2023-05-23 10:59:30.348037 cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/messages.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:12:39.124992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-23 11:12:39.126992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.py
+-rw-r--r--   0        0        0     1702 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.pyi
+-rw-r--r--   0        0        0     2519 2023-05-23 11:12:39.126992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.py
+-rw-r--r--   0        0        0     6430 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.pyi
+-rw-r--r--   0        0        0     3047 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.py
+-rw-r--r--   0        0        0     7303 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.pyi
+-rw-r--r--   0        0        0     2302 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.py
+-rw-r--r--   0        0        0     4811 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.pyi
+-rw-r--r--   0        0        0     3228 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.py
+-rw-r--r--   0        0        0     8503 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.pyi
+-rw-r--r--   0        0        0     1444 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.py
+-rw-r--r--   0        0        0     1705 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.pyi
+-rw-r--r--   0        0        0     2590 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.py
+-rw-r--r--   0        0        0     5930 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.pyi
+-rw-r--r--   0        0        0     1842 2023-05-23 11:12:39.127992 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.py
+-rw-r--r--   0        0        0     2460 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.pyi
+-rw-r--r--   0        0        0     2384 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.py
+-rw-r--r--   0        0        0     5977 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.pyi
+-rw-r--r--   0        0        0     1461 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.py
+-rw-r--r--   0        0        0     1805 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.pyi
+-rw-r--r--   0        0        0     8330 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.py
+-rw-r--r--   0        0        0    23660 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.pyi
+-rw-r--r--   0        0        0     2549 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.py
+-rw-r--r--   0        0        0     4966 2023-05-23 11:12:39.106991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.pyi
+-rw-r--r--   0        0        0     4899 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.py
+-rw-r--r--   0        0        0    12598 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.pyi
+-rw-r--r--   0        0        0     4507 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.py
+-rw-r--r--   0        0        0    15277 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.pyi
+-rw-r--r--   0        0        0     1597 2023-05-23 11:12:39.128993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.py
+-rw-r--r--   0        0        0     2003 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.pyi
+-rw-r--r--   0        0        0     2845 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2.pyi
+-rw-r--r--   0        0        0    15062 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
+-rw-r--r--   0        0        0     2853 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-05-23 11:12:39.107991 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2.pyi
+-rw-r--r--   0        0        0    14820 2023-05-23 11:12:39.129993 cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2_grpc.py
+-rw-r--r--   0        0        0       60 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/__init__.py
+-rw-r--r--   0        0        0      943 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/base_model.py
+-rw-r--r--   0        0        0       64 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/client.py
+-rw-r--r--   0        0        0    50682 2023-05-23 11:12:41.111128 cognite_robotics_sdk-0.1.7/cognite_robotics/rest/models.py
+-rw-r--r--   0        0        0       58 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/env_utils.py
+-rw-r--r--   0        0        0     3016 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/token.py
+-rw-r--r--   0        0        0     3865 2023-05-23 10:59:30.350037 cognite_robotics_sdk-0.1.7/cognite_robotics/utils/utils.py
+-rw-r--r--   0        0        0     1462 2023-05-23 10:59:30.351037 cognite_robotics_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.7/PKG-INFO
```

### Comparing `cognite_robotics_sdk-0.1.6/README.md` & `cognite_robotics_sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/config/config.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/config/config.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_classes.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader_task.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/data_uploader_task.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/helpers.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/data_uploader/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             if not os.path.exists(file):
                 logger.debug(f"File `{file}` does not exist. Skipping removal.")
                 continue
             try:
                 os.remove(file)
                 logger.debug(f"Removed {file}.")
             except OSError as e:
-                logger.error(f"Failed to remove `{file}`: {str(e)}")
+                logger.error(f"Failed to remove `{file}`: {e!s}")
 
     await asyncio.shield(to_thread(_remove_files))
 
 
 async def move_files(
     files: List[str],
     to_folder: str,
@@ -263,15 +263,15 @@
             if not os.path.exists(file):
                 logger.debug(f"File `{file}` does not exist. Skipping moving.")
                 continue
             try:
                 os.rename(file, os.path.join(to_folder, os.path.basename(file)))
                 logger.debug(f"Moved {file} to {to_folder}.")
             except Exception as e:
-                logger.error(f"Failed to move `{file}`: {str(e)}")
+                logger.error(f"Failed to move `{file}`: {e!s}")
 
     await asyncio.shield(to_thread(_move_files))
 
 
 async def cleanup_upload_data_folder(upload_data_path: str) -> None:
     """Clean up the upload data folder.
```

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/robot_interface_client.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/robot_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/web_interface_client.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/clients/web_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/bearer_token_auth.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/bearer_token_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/channel.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/channel.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/messages.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/grpc/helpers/messages.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/connectivity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/control_authority_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/geometry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/joint_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/mission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_registration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/robot_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.pyi` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/messages/web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/robot_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/protos/services/web_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/rest/base_model.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/rest/base_model.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/rest/models.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/rest/models.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/utils/env_utils.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/utils/token.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/utils/token.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.6/cognite_robotics/utils/utils.py` & `cognite_robotics_sdk-0.1.7/cognite_robotics/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # -*- coding: utf-8 -*-
 """Utils tests."""
 import asyncio
 import contextvars
 import functools
+import json
 import logging
 import typing
 from typing import Any, AsyncGenerator, List, Optional, TypeVar
 
 import grpc
-from cognite.client import CogniteClient
+from cognite.client import CogniteClient, global_config
 from cognite.client.config import ClientConfig
 from cognite.client.credentials import OAuthClientCredentials
 
 from cognite_robotics.utils.env_utils import get_env
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
+global_config.disable_gzip = True
+
 
 async def yield_from_queue(queue: "asyncio.Queue[T]") -> AsyncGenerator[T, None]:
     """Yield items from a queue.
 
     Args:
         queue (asyncio.Queue[T]): queue to yield items from
     Returns:
@@ -80,14 +83,33 @@
     token_scopes = [f"{base_url}/.default"]
 
     creds = OAuthClientCredentials(token_url=token_url, client_id=client_id, client_secret=client_secret, scopes=token_scopes)
     cnf = ClientConfig(client_name=client_name, base_url=base_url, project=str(project), credentials=creds)
     return CogniteClient(cnf)
 
 
+def get_robot_data_set_id(
+    cognite_client: CogniteClient,
+) -> Optional[int]:
+    """Get the robot's data set id.
+
+    The data set id is the data set of the only robot in CDF the service has access to.
+
+    Returns:
+        Optional[Any]: robot data set id (if available)
+    """
+    cognite_client.config.project
+    response = cognite_client.get(f"/api/v1/projects/{cognite_client.config.project}/robotics/robots")
+    robots = json.loads(response.content)["items"]
+    if len(robots) != 1:
+        logger.error("Found none or more than one robot for the robot's credentials.")
+        return None
+    return int(robots[0].get("dataSetId"))
+
+
 @typing.no_type_check
 async def to_thread(func, /, *args, **kwargs) -> Any:
     """Asyncio thread implementation for Python 3.8."""
     loop = asyncio.get_running_loop()
     ctx = contextvars.copy_context()
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
     return await loop.run_in_executor(None, func_call)
```

### Comparing `cognite_robotics_sdk-0.1.6/pyproject.toml` & `cognite_robotics_sdk-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 description = "Cognite Robotics SDK"
 name = "cognite-robotics-sdk"
 packages = [
     { include = "cognite_robotics", from = "." },
     { include = "protos", from = "cognite_robotics" },
 ]
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 aiofiles = ">=23.1.0"
 cognite-sdk = ">=6.0.0"
 grpcio = ">=1.54.0"
 protobuf = ">=4.22.3"
 pydantic = "1.10.7"
 python = "^3.8"
-python-dotenv = "0.21.1"
+python-dotenv = ">=0.21.1"
 
 [tool.poetry.dev-dependencies]
 black = "23.3.0"
-datamodel-code-generator = "0.18.0"
-mypy = "1.2.0"
-pre-commit = "3.3.1"
+datamodel-code-generator = "0.19.0"
+mypy = "1.3.0"
+pre-commit = "3.3.2"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 types-aiofiles = "23.1.0.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `cognite_robotics_sdk-0.1.6/PKG-INFO` & `cognite_robotics_sdk-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cognite-robotics-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Cognite Robotics SDK
 Author: Cognite Robotics
 Author-email: robotics-team@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0)
 Requires-Dist: cognite-sdk (>=6.0.0)
 Requires-Dist: grpcio (>=1.54.0)
 Requires-Dist: protobuf (>=4.22.3)
 Requires-Dist: pydantic (==1.10.7)
-Requires-Dist: python-dotenv (==0.21.1)
+Requires-Dist: python-dotenv (>=0.21.1)
 Description-Content-Type: text/markdown
 
 # Cognite Robotics SDK
 
 [![PyPI version](https://badge.fury.io/py/cognite-robotics-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
 [![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org)
 [![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
```

