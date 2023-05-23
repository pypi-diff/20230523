# Comparing `tmp/qwak_core-0.0.72.tar.gz` & `tmp/qwak_core-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.72.tar", max compression
+gzip compressed data, was "qwak_core-0.0.73.tar", max compression
```

## Comparing `qwak_core-0.0.72.tar` & `qwak_core-0.0.73.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-23 07:34:35.402304 qwak_core-0.0.72/README.md
--rw-r--r--   0        0        0        0 2023-05-23 07:37:07.468317 qwak_core-0.0.72/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-23 07:37:07.504317 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-23 07:36:37.343917 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.504317 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-23 07:37:07.496317 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-23 07:36:36.787909 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.500317 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-23 07:37:07.500317 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-23 07:36:37.071913 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.500317 qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-23 07:37:07.488317 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-23 07:36:35.951898 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-23 07:37:07.488317 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-23 07:37:07.492317 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-23 07:36:36.251902 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.492317 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-23 07:37:07.492317 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-23 07:36:36.519906 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.496317 qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-23 07:37:07.472317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-23 07:36:35.635894 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-23 07:37:07.472317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-23 07:37:07.472317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-23 07:36:37.615920 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.476317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-23 07:37:07.480317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-23 07:36:38.175928 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.480317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-23 07:37:07.484317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-23 07:36:38.455931 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-23 07:37:07.484317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-23 07:37:07.476317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-23 07:36:37.903924 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.476317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-23 07:37:07.484317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-23 07:36:38.723935 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.488317 qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-23 07:37:07.544318 qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-23 07:36:42.491985 qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.544318 qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-23 07:37:07.544318 qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-23 07:36:42.755988 qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-23 07:37:07.548318 qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-23 07:37:07.636319 qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-23 07:36:50.372089 qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.640319 qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-23 07:37:07.640319 qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-23 07:36:50.648093 qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-23 07:37:07.640319 qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-23 07:37:07.648319 qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-23 07:36:52.032112 qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-23 07:37:07.648319 qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-23 07:37:07.644319 qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-23 07:36:51.756108 qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.644319 qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-23 07:37:07.648319 qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-23 07:36:52.304115 qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.652319 qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-23 07:37:07.652319 qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-23 07:36:52.572119 qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-23 07:37:07.652319 qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-23 07:37:07.780321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-23 07:37:04.108272 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.780321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-23 07:37:07.776321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-23 07:37:03.564265 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.776321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-23 07:37:07.776321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-23 07:37:03.828268 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.780321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-23 07:37:07.768321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-23 07:37:03.024258 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-23 07:37:07.772321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-23 07:37:07.772321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-23 07:37:03.300261 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.772321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-23 07:37:07.788321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-23 07:37:04.944283 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.792321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-23 07:37:07.788321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-23 07:37:04.684280 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.788321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-23 07:37:07.784321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-23 07:37:04.404276 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.784321 qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-23 07:37:07.764320 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-23 07:37:02.736254 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.768321 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-23 07:37:07.760321 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-23 07:37:02.180246 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.760321 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-23 07:37:07.764320 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-23 07:37:02.468250 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-23 07:37:07.764320 qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-23 07:37:07.688320 qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-23 07:36:55.380156 qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-23 07:37:07.688320 qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-23 07:37:07.684320 qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-23 07:36:55.088152 qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.684320 qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-23 07:37:07.672319 qwak_core-0.0.72/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-23 07:36:54.520145 qwak_core-0.0.72/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.676319 qwak_core-0.0.72/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-23 07:37:07.676319 qwak_core-0.0.72/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-23 07:36:54.792148 qwak_core-0.0.72/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.676319 qwak_core-0.0.72/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-23 07:37:07.680319 qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-23 07:36:55.652160 qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-23 07:37:07.680319 qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-23 07:37:07.680319 qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-23 07:36:56.240167 qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-23 07:37:07.684320 qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-23 07:37:07.700320 qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-23 07:36:56.804175 qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.700320 qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-23 07:37:07.700320 qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-23 07:36:57.072179 qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-23 07:37:07.704320 qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-23 07:37:07.664319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-23 07:36:53.716134 qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.664319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-23 07:37:07.668319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-23 07:36:53.984138 qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-23 07:37:07.668319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-23 07:37:07.656319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-23 07:36:53.156127 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.660319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-23 07:37:07.656319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-23 07:36:52.868123 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.656319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-23 07:37:07.660319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-23 07:36:53.444131 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-23 07:37:07.664319 qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-23 07:37:07.528318 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-23 07:36:41.147967 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.528318 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-23 07:37:07.532317 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-23 07:36:41.415971 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.532317 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-23 07:37:07.536317 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-23 07:36:41.683974 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-23 07:37:07.536317 qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-23 07:37:07.612319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-23 07:36:48.712067 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.612319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-23 07:37:07.608318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-23 07:36:48.444064 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-23 07:37:07.612319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-23 07:37:07.584318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-23 07:36:46.032032 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.584318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-23 07:37:07.580318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-23 07:36:45.760028 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.580318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-23 07:37:07.572318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-23 07:36:44.928017 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.572318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-23 07:37:07.576318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-23 07:36:45.496025 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-23 07:37:07.580318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-23 07:37:07.584318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-23 07:36:46.304036 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.588318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-23 07:37:07.588318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-23 07:36:46.568039 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-23 07:37:07.588318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-23 07:37:07.572318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-23 07:36:45.212021 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.576318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-23 07:37:07.592318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-23 07:36:46.828042 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.592318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11224 2023-05-23 07:37:07.596318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    14819 2023-05-23 07:36:47.092046 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.596318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-23 07:37:07.616319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-23 07:37:06.840308 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.616319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-23 07:37:07.616319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-23 07:37:07.108312 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-23 07:37:07.620319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-23 07:37:07.620319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-23 07:36:49.556079 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.620319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-23 07:37:07.624319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-23 07:36:49.832082 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-23 07:37:07.624319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-23 07:37:07.628319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-23 07:36:50.100086 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.628319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-23 07:37:07.632319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-23 07:36:51.200101 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.632319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-23 07:37:07.628319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-23 07:36:50.924097 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-23 07:37:07.632319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-23 07:37:07.636319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-23 07:36:51.468104 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.636319 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-23 07:37:07.596318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-23 07:36:47.364050 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.600318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-23 07:37:07.600318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-23 07:36:47.636053 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.600318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-23 07:37:07.604318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-23 07:36:47.908057 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-23 07:37:07.604318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-23 07:37:07.604318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-23 07:36:48.180060 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.608318 qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-23 07:37:07.792321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-23 07:37:05.208287 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.792321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-23 07:37:07.796321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-23 07:37:05.484290 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-23 07:37:07.796321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-23 07:37:07.796321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-23 07:37:05.752294 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.800321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-23 07:37:07.800321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-23 07:37:06.032297 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-23 07:37:07.804321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-23 07:37:07.804321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-23 07:37:06.312301 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-23 07:37:07.804321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-23 07:37:07.808321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-23 07:37:06.576305 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.808321 qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-23 07:37:07.704320 qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-23 07:36:57.340182 qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.708320 qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-23 07:37:07.708320 qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-23 07:36:57.600186 qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-23 07:37:07.708320 qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-23 07:37:07.552318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-23 07:36:43.832003 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.552318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-23 07:37:07.556318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-23 07:36:44.096006 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.560318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-23 07:37:07.560318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-23 07:36:44.364010 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-23 07:37:07.564318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-23 07:37:07.568318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-23 07:36:44.636013 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.568318 qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-23 07:37:07.668319 qwak_core-0.0.72/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-23 07:36:54.252141 qwak_core-0.0.72/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-23 07:37:07.672319 qwak_core-0.0.72/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-23 07:37:07.712320 qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-23 07:36:57.864189 qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.712320 qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-23 07:37:07.716320 qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-23 07:36:58.128193 qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-23 07:37:07.716320 qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-23 07:37:07.732320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-23 07:36:59.724214 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.736320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-23 07:37:07.736320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-23 07:36:59.992217 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.736320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-23 07:37:07.740320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-23 07:37:00.272221 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.740320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-23 07:37:07.740320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-23 07:37:00.548225 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.744320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-23 07:37:07.744320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-23 07:37:00.828229 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.748320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-23 07:37:07.748320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-23 07:37:01.116232 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-23 07:37:07.748320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-23 07:37:07.752320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-23 07:37:01.384236 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.752320 qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-23 07:37:07.720320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-23 07:36:58.656200 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.724320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-23 07:37:07.728320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-23 07:36:59.456210 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.732320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-23 07:37:07.724320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-23 07:36:58.920203 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-23 07:37:07.724320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-23 07:37:07.728320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-23 07:36:59.192207 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.728320 qwak_core-0.0.72/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-23 07:37:07.696320 qwak_core-0.0.72/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-23 07:36:56.536172 qwak_core-0.0.72/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-23 07:37:07.696320 qwak_core-0.0.72/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-23 07:37:07.524317 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-23 07:36:43.291995 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-23 07:37:07.524317 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-23 07:37:07.520317 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-23 07:36:43.019992 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.520317 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-23 07:37:07.524317 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-23 07:36:43.563999 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-23 07:37:07.528318 qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-23 07:37:07.692320 qwak_core-0.0.72/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-23 07:36:55.940164 qwak_core-0.0.72/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-23 07:37:07.692320 qwak_core-0.0.72/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-23 07:37:07.716320 qwak_core-0.0.72/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-23 07:36:58.392196 qwak_core-0.0.72/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-23 07:37:07.720320 qwak_core-0.0.72/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-23 07:37:07.516317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-23 07:36:40.067953 qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.520317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-23 07:37:07.512317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-23 07:36:39.803949 qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-23 07:37:07.516317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-23 07:37:07.504317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-23 07:36:38.987939 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.508317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-23 07:37:07.508317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-23 07:36:39.255942 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.508317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-23 07:37:07.512317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-23 07:36:39.531946 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-23 07:37:07.512317 qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-23 07:37:07.756321 qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-23 07:37:01.912243 qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-23 07:37:07.760321 qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-23 07:37:07.752320 qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-23 07:37:01.652239 qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.756321 qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-23 07:37:07.536317 qwak_core-0.0.72/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-23 07:36:41.951978 qwak_core-0.0.72/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.540318 qwak_core-0.0.72/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-23 07:37:07.540318 qwak_core-0.0.72/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-23 07:36:42.219981 qwak_core-0.0.72/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 07:37:07.540318 qwak_core-0.0.72/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-23 07:37:11.132365 qwak_core-0.0.72/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-23 07:37:11.132365 qwak_core-0.0.72/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.406304 qwak_core-0.0.72/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.410304 qwak_core-0.0.72/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-23 07:34:35.414304 qwak_core-0.0.72/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-23 07:34:35.418304 qwak_core-0.0.72/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.72/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.72/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-23 08:09:11.257644 qwak_core-0.0.73/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:56.383821 qwak_core-0.0.73/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-23 08:11:56.415822 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-23 08:11:25.047408 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.419822 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-23 08:11:56.411821 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-23 08:11:24.495401 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.411821 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-23 08:11:56.415822 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-23 08:11:24.771405 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.415822 qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-23 08:11:56.403821 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-23 08:11:23.675390 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-23 08:11:56.403821 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-23 08:11:56.403821 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-23 08:11:23.947394 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.407822 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-23 08:11:56.407822 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-23 08:11:24.215397 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.411821 qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-23 08:11:56.383821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-23 08:11:23.399387 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-23 08:11:56.383821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-23 08:11:56.387821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-23 08:11:25.327412 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.387821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-23 08:11:56.391821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-23 08:11:25.899420 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.395821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-23 08:11:56.395821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-23 08:11:26.175423 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-23 08:11:56.395821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-23 08:11:56.387821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-23 08:11:25.619416 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.391821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-23 08:11:56.399821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-23 08:11:26.459427 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.399821 qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-23 08:11:56.463822 qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-23 08:11:30.227477 qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.463822 qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-23 08:11:56.467822 qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-23 08:11:30.503480 qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-23 08:11:56.467822 qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-23 08:11:56.563824 qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-23 08:11:38.299583 qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.563824 qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-23 08:11:56.567824 qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-23 08:11:38.567587 qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-23 08:11:56.567824 qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-23 08:11:56.571824 qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-23 08:11:39.927605 qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-23 08:11:56.575824 qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-23 08:11:56.571824 qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-23 08:11:39.655601 qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.571824 qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-23 08:11:56.575824 qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-23 08:11:40.199608 qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.575824 qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-23 08:11:56.579824 qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-23 08:11:40.471612 qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-23 08:11:56.579824 qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-23 08:11:56.711825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-23 08:11:52.447769 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.711825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-23 08:11:56.703825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-23 08:11:51.831761 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.703825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-23 08:11:56.707826 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-23 08:11:52.131765 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.707826 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-23 08:11:56.699825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-23 08:11:51.159752 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-23 08:11:56.699825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-23 08:11:56.699825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-23 08:11:51.519757 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.703825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-23 08:11:56.719826 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-23 08:11:53.395782 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.719826 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-23 08:11:56.715825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-23 08:11:53.055777 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.715825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-23 08:11:56.711825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-23 08:11:52.755773 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.715825 qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-23 08:11:56.695825 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-23 08:11:50.827748 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.695825 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-23 08:11:56.687825 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-23 08:11:50.187739 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.691825 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-23 08:11:56.691825 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-23 08:11:50.519744 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-23 08:11:56.691825 qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    19978 2023-05-23 08:11:56.615824 qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    16810 2023-05-23 08:11:43.243648 qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-23 08:11:56.619824 qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-23 08:11:56.611824 qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-23 08:11:42.971644 qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.615824 qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-23 08:11:56.599824 qwak_core-0.0.73/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-23 08:11:42.431637 qwak_core-0.0.73/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.603824 qwak_core-0.0.73/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-23 08:11:56.603824 qwak_core-0.0.73/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-23 08:11:42.699641 qwak_core-0.0.73/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.603824 qwak_core-0.0.73/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-23 08:11:56.607824 qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-23 08:11:43.515652 qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-23 08:11:56.607824 qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-23 08:11:56.611824 qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-23 08:11:44.099660 qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-23 08:11:56.611824 qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-23 08:11:56.627824 qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-23 08:11:44.671667 qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.627824 qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-23 08:11:56.631824 qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-23 08:11:44.935670 qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-23 08:11:56.631824 qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-23 08:11:56.591824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-23 08:11:41.607627 qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.591824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-23 08:11:56.595824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-23 08:11:41.883630 qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-23 08:11:56.595824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-23 08:11:56.583824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-23 08:11:41.043619 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.587824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-23 08:11:56.583824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-23 08:11:40.767616 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.583824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-23 08:11:56.587824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-23 08:11:41.335623 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-23 08:11:56.591824 qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-23 08:11:56.447822 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-23 08:11:28.875459 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.447822 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-23 08:11:56.451822 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-23 08:11:29.143463 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.451822 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-23 08:11:56.451822 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-23 08:11:29.415466 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-23 08:11:56.455822 qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-23 08:11:56.535823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-23 08:11:36.683562 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.535823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-23 08:11:56.531823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-23 08:11:36.415558 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-23 08:11:56.535823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-23 08:11:56.503823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-23 08:11:33.947526 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.503823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-23 08:11:56.499823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-23 08:11:33.675522 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.503823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-23 08:11:56.491823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-23 08:11:32.843511 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.491823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-23 08:11:56.495823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-23 08:11:33.407519 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-23 08:11:56.499823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-23 08:11:56.507823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-23 08:11:34.235530 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.507823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-23 08:11:56.507823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-23 08:11:34.507533 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-23 08:11:56.511823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-23 08:11:56.495823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-23 08:11:33.123515 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.495823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-23 08:11:56.511823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-23 08:11:34.783537 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.515823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11224 2023-05-23 08:11:56.515823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    14819 2023-05-23 08:11:35.051540 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.515823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-23 08:11:56.539823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-23 08:11:55.727812 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.539823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-23 08:11:56.539823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-23 08:11:56.003816 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-23 08:11:56.543823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-23 08:11:56.543823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-23 08:11:37.483572 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.547823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-23 08:11:56.547823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-23 08:11:37.759576 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-23 08:11:56.547823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-23 08:11:56.551823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-23 08:11:38.027579 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.551823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-23 08:11:56.559823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-23 08:11:39.115594 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.559823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-23 08:11:56.555823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-23 08:11:38.843590 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-23 08:11:56.555823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-23 08:11:56.559823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-23 08:11:39.383597 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.563824 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-23 08:11:56.519823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-23 08:11:35.331544 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.519823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-23 08:11:56.519823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-23 08:11:35.599547 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.523823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-23 08:11:56.527823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-23 08:11:35.871551 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-23 08:11:56.527823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-23 08:11:56.531823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-23 08:11:36.139555 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.531823 qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-23 08:11:56.719826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-23 08:11:53.723786 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.723826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-23 08:11:56.723826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-23 08:11:54.047790 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-23 08:11:56.727826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-23 08:11:56.727826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-23 08:11:54.355795 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.727826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-23 08:11:56.731826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-23 08:11:54.699799 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-23 08:11:56.731826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-23 08:11:56.731826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-23 08:11:55.031803 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-23 08:11:56.735826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-23 08:11:56.735826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-23 08:11:55.403808 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.735826 qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-23 08:11:56.631824 qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-23 08:11:45.199674 qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.635825 qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-23 08:11:56.635825 qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-23 08:11:45.475678 qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-23 08:11:56.639824 qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-23 08:11:56.471822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-23 08:11:31.767497 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.475822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-23 08:11:56.475822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-23 08:11:32.031500 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.479822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-23 08:11:56.479822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-23 08:11:32.299504 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-23 08:11:56.483822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-23 08:11:56.487822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-23 08:11:32.567508 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.487822 qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-23 08:11:56.595824 qwak_core-0.0.73/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-23 08:11:42.155634 qwak_core-0.0.73/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-23 08:11:56.599824 qwak_core-0.0.73/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-23 08:11:56.639824 qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-23 08:11:45.747681 qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.639824 qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-23 08:11:56.643825 qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-23 08:11:46.019685 qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-23 08:11:56.643825 qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-23 08:11:56.659825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-23 08:11:47.607706 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.663825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-23 08:11:56.663825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-23 08:11:47.875709 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.663825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-23 08:11:56.667825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-23 08:11:48.151713 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.667825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-23 08:11:56.671825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-23 08:11:48.427716 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.671825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-23 08:11:56.671825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-23 08:11:48.707720 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.675825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-23 08:11:56.675825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-23 08:11:48.999724 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-23 08:11:56.679825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-23 08:11:56.679825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-23 08:11:49.271727 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.679825 qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-23 08:11:56.647825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-23 08:11:46.551692 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.647825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-23 08:11:56.655825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-23 08:11:47.339702 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.659825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-23 08:11:56.651825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-23 08:11:46.815695 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-23 08:11:56.651825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-23 08:11:56.655825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-23 08:11:47.079699 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.655825 qwak_core-0.0.73/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-23 08:11:56.623824 qwak_core-0.0.73/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-23 08:11:44.399663 qwak_core-0.0.73/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-23 08:11:56.623824 qwak_core-0.0.73/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-23 08:11:56.439822 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-23 08:11:31.135489 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-23 08:11:56.439822 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-23 08:11:56.435822 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-23 08:11:30.807484 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.435822 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-23 08:11:56.443822 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-23 08:11:31.471493 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-23 08:11:56.443822 qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-23 08:11:56.619824 qwak_core-0.0.73/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-23 08:11:43.799656 qwak_core-0.0.73/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-23 08:11:56.619824 qwak_core-0.0.73/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-23 08:11:56.643825 qwak_core-0.0.73/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-23 08:11:46.283688 qwak_core-0.0.73/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-23 08:11:56.647825 qwak_core-0.0.73/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-23 08:11:56.431822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-23 08:11:27.811445 qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.435822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-23 08:11:56.427822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-23 08:11:27.535441 qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-23 08:11:56.431822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-23 08:11:56.419822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-23 08:11:26.723430 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.423822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-23 08:11:56.423822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-23 08:11:26.991434 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.423822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-23 08:11:56.427822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-23 08:11:27.259438 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-23 08:11:56.427822 qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-23 08:11:56.683825 qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-23 08:11:49.875735 qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-23 08:11:56.687825 qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-23 08:11:56.683825 qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-23 08:11:49.559731 qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.683825 qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-23 08:11:56.455822 qwak_core-0.0.73/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-23 08:11:29.687470 qwak_core-0.0.73/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.459822 qwak_core-0.0.73/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-23 08:11:56.459822 qwak_core-0.0.73/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-23 08:11:29.951473 qwak_core-0.0.73/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 08:11:56.459822 qwak_core-0.0.73/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-23 08:11:59.235859 qwak_core-0.0.73/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-23 08:11:59.235859 qwak_core-0.0.73/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-23 08:09:11.261644 qwak_core-0.0.73/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.265644 qwak_core-0.0.73/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.269644 qwak_core-0.0.73/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-23 08:09:11.273644 qwak_core-0.0.73/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.73/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.73/PKG-INFO
```

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.build.v1 import build_pb2 as qwak_dot_build_dot_v1_dot_build__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dqwak/build/v1/build_api.proto\x12\x11\x63om.qwak.build.v1\x1a\x19qwak/build/v1/build.proto\"|\n\x14RegisterBuildRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x10\n\x08\x63ommitId\x18\x02 \x01(\t\x12\x0f\n\x07modelId\x18\x03 \x01(\t\x12\x13\n\x0b\x62uildConfig\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12\r\n\x05steps\x18\x06 \x03(\t\"\x17\n\x15RegisterBuildResponse\"a\n\x18UpdateBuildStatusRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x34\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.BuildStatus\"\x1b\n\x19UpdateBuildStatusResponse\"\xba\x02\n!RegisterExperimentTrackingRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12P\n\x06params\x18\x02 \x03(\x0b\x32@.com.qwak.build.v1.RegisterExperimentTrackingRequest.ParamsEntry\x12R\n\x07metrics\x18\x03 \x03(\x0b\x32\x41.com.qwak.build.v1.RegisterExperimentTrackingRequest.MetricsEntry\x1a-\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"$\n\"RegisterExperimentTrackingResponse\"d\n\x1aRegisterModelSchemaRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x34\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.ModelSchema\"\x1d\n\x1bRegisterModelSchemaResponse\"#\n\x0fGetBuildRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\";\n\x10GetBuildResponse\x12\'\n\x05\x62uild\x18\x01 \x01(\x0b\x32\x18.com.qwak.build.v1.Build\"j\n\x11ListBuildsRequest\x12\x11\n\tbranch_id\x18\x01 \x01(\t\x12.\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.BuildFilter\x12\x12\n\nmodel_uuid\x18\x03 \x01(\t\"=\n\x12ListBuildsResponse\x12\'\n\x05\x62uild\x18\x01 \x03(\x0b\x32\x18.com.qwak.build.v1.Build\"5\n\x13RegisterTagsRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\"\x16\n\x14RegisterTagsResponse\"\x8e\x01\n\x15LogPhaseStatusRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x10\n\x08phase_id\x18\x02 \x01(\t\x12.\n\x06status\x18\x03 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x04 \x01(\x05\"\x18\n\x16LogPhaseStatusResponse\"+\n\x17GetPhaseStatusesRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\"\xb3\x01\n\x0ePhaseStatusLog\x12\x10\n\x08phase_id\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x03 \x01(\x05\x12<\n\x12pod_failure_reason\x18\x04 \x01(\x0e\x32 .com.qwak.build.v1.FailureReason\"O\n\x18GetPhaseStatusesResponse\x12\x33\n\x08statuses\x18\x01 \x03(\x0b\x32!.com.qwak.build.v1.PhaseStatusLog\"\'\n\x12\x44\x65leteBuildRequest\x12\x11\n\tbuild_ids\x18\x01 \x03(\t\"\x15\n\x13\x44\x65leteBuildResponse*\x97\x01\n\x0bPhaseStatus\x12\x18\n\x14PHASE_STATUS_INVALID\x10\x00\x12\x1c\n\x18PHASE_STATUS_IN_PROGRESS\x10\x01\x12\x1b\n\x17PHASE_STATUS_SUCCESSFUL\x10\x02\x12\x17\n\x13PHASE_STATUS_FAILED\x10\x03\x12\x1a\n\x16PHASE_STATUS_CANCELLED\x10\x04*w\n\rFailureReason\x12\x1e\n\x1a\x46\x41ILURE_REASON_UNSPECIFIED\x10\x00\x12$\n FAILURE_REASON_AVAILABLE_IN_LOGS\x10\x01\x12 \n\x1c\x46\x41ILURE_REASON_OUT_OF_MEMORY\x10\x02\x32\xa3\x08\n\x08\x42uildAPI\x12\x62\n\rRegisterBuild\x12\'.com.qwak.build.v1.RegisterBuildRequest\x1a(.com.qwak.build.v1.RegisterBuildResponse\x12n\n\x11UpdateBuildStatus\x12+.com.qwak.build.v1.UpdateBuildStatusRequest\x1a,.com.qwak.build.v1.UpdateBuildStatusResponse\x12\x89\x01\n\x1aRegisterExperimentTracking\x12\x34.com.qwak.build.v1.RegisterExperimentTrackingRequest\x1a\x35.com.qwak.build.v1.RegisterExperimentTrackingResponse\x12_\n\x0cRegisterTags\x12&.com.qwak.build.v1.RegisterTagsRequest\x1a\'.com.qwak.build.v1.RegisterTagsResponse\x12t\n\x13RegisterModelSchema\x12-.com.qwak.build.v1.RegisterModelSchemaRequest\x1a..com.qwak.build.v1.RegisterModelSchemaResponse\x12S\n\x08GetBuild\x12\".com.qwak.build.v1.GetBuildRequest\x1a#.com.qwak.build.v1.GetBuildResponse\x12Y\n\nListBuilds\x12$.com.qwak.build.v1.ListBuildsRequest\x1a%.com.qwak.build.v1.ListBuildsResponse\x12\\\n\x0b\x44\x65leteBuild\x12%.com.qwak.build.v1.DeleteBuildRequest\x1a&.com.qwak.build.v1.DeleteBuildResponse\x12\x65\n\x0eLogPhaseStatus\x12(.com.qwak.build.v1.LogPhaseStatusRequest\x1a).com.qwak.build.v1.LogPhaseStatusResponse\x12k\n\x10GetPhaseStatuses\x12*.com.qwak.build.v1.GetPhaseStatusesRequest\x1a+.com.qwak.build.v1.GetPhaseStatusesResponseB$\n\x11\x63om.qwak.build.v1B\rBuildApiProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dqwak/build/v1/build_api.proto\x12\x11\x63om.qwak.build.v1\x1a\x19qwak/build/v1/build.proto\"|\n\x14RegisterBuildRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x10\n\x08\x63ommitId\x18\x02 \x01(\t\x12\x0f\n\x07modelId\x18\x03 \x01(\t\x12\x13\n\x0b\x62uildConfig\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12\r\n\x05steps\x18\x06 \x03(\t\"\x17\n\x15RegisterBuildResponse\"a\n\x18UpdateBuildStatusRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x34\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.BuildStatus\"\x1b\n\x19UpdateBuildStatusResponse\"\xba\x02\n!RegisterExperimentTrackingRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12P\n\x06params\x18\x02 \x03(\x0b\x32@.com.qwak.build.v1.RegisterExperimentTrackingRequest.ParamsEntry\x12R\n\x07metrics\x18\x03 \x03(\x0b\x32\x41.com.qwak.build.v1.RegisterExperimentTrackingRequest.MetricsEntry\x1a-\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"$\n\"RegisterExperimentTrackingResponse\"d\n\x1aRegisterModelSchemaRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x34\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.ModelSchema\"\x1d\n\x1bRegisterModelSchemaResponse\"#\n\x0fGetBuildRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\";\n\x10GetBuildResponse\x12\'\n\x05\x62uild\x18\x01 \x01(\x0b\x32\x18.com.qwak.build.v1.Build\"j\n\x11ListBuildsRequest\x12\x11\n\tbranch_id\x18\x01 \x01(\t\x12.\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.BuildFilter\x12\x12\n\nmodel_uuid\x18\x03 \x01(\t\"=\n\x12ListBuildsResponse\x12\'\n\x05\x62uild\x18\x01 \x03(\x0b\x32\x18.com.qwak.build.v1.Build\"5\n\x13RegisterTagsRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\"\x16\n\x14RegisterTagsResponse\"\x8e\x01\n\x15LogPhaseStatusRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x10\n\x08phase_id\x18\x02 \x01(\t\x12.\n\x06status\x18\x03 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x04 \x01(\x05\"\x18\n\x16LogPhaseStatusResponse\"+\n\x17GetPhaseStatusesRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\"\xb3\x01\n\x0ePhaseStatusLog\x12\x10\n\x08phase_id\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x03 \x01(\x05\x12<\n\x12pod_failure_reason\x18\x04 \x01(\x0e\x32 .com.qwak.build.v1.FailureReason\"O\n\x18GetPhaseStatusesResponse\x12\x33\n\x08statuses\x18\x01 \x03(\x0b\x32!.com.qwak.build.v1.PhaseStatusLog\"\'\n\x12\x44\x65leteBuildRequest\x12\x11\n\tbuild_ids\x18\x01 \x03(\t\"\x15\n\x13\x44\x65leteBuildResponse\"a\n\x11GetTagPathRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x10\n\x08tag_name\x18\x04 \x01(\t\"&\n\x12GetTagPathResponse\x12\x10\n\x08key_path\x18\x01 \x01(\t*\x97\x01\n\x0bPhaseStatus\x12\x18\n\x14PHASE_STATUS_INVALID\x10\x00\x12\x1c\n\x18PHASE_STATUS_IN_PROGRESS\x10\x01\x12\x1b\n\x17PHASE_STATUS_SUCCESSFUL\x10\x02\x12\x17\n\x13PHASE_STATUS_FAILED\x10\x03\x12\x1a\n\x16PHASE_STATUS_CANCELLED\x10\x04*w\n\rFailureReason\x12\x1e\n\x1a\x46\x41ILURE_REASON_UNSPECIFIED\x10\x00\x12$\n FAILURE_REASON_AVAILABLE_IN_LOGS\x10\x01\x12 \n\x1c\x46\x41ILURE_REASON_OUT_OF_MEMORY\x10\x02\x32\xfe\x08\n\x08\x42uildAPI\x12\x62\n\rRegisterBuild\x12\'.com.qwak.build.v1.RegisterBuildRequest\x1a(.com.qwak.build.v1.RegisterBuildResponse\x12n\n\x11UpdateBuildStatus\x12+.com.qwak.build.v1.UpdateBuildStatusRequest\x1a,.com.qwak.build.v1.UpdateBuildStatusResponse\x12\x89\x01\n\x1aRegisterExperimentTracking\x12\x34.com.qwak.build.v1.RegisterExperimentTrackingRequest\x1a\x35.com.qwak.build.v1.RegisterExperimentTrackingResponse\x12_\n\x0cRegisterTags\x12&.com.qwak.build.v1.RegisterTagsRequest\x1a\'.com.qwak.build.v1.RegisterTagsResponse\x12t\n\x13RegisterModelSchema\x12-.com.qwak.build.v1.RegisterModelSchemaRequest\x1a..com.qwak.build.v1.RegisterModelSchemaResponse\x12S\n\x08GetBuild\x12\".com.qwak.build.v1.GetBuildRequest\x1a#.com.qwak.build.v1.GetBuildResponse\x12Y\n\nListBuilds\x12$.com.qwak.build.v1.ListBuildsRequest\x1a%.com.qwak.build.v1.ListBuildsResponse\x12\\\n\x0b\x44\x65leteBuild\x12%.com.qwak.build.v1.DeleteBuildRequest\x1a&.com.qwak.build.v1.DeleteBuildResponse\x12\x65\n\x0eLogPhaseStatus\x12(.com.qwak.build.v1.LogPhaseStatusRequest\x1a).com.qwak.build.v1.LogPhaseStatusResponse\x12k\n\x10GetPhaseStatuses\x12*.com.qwak.build.v1.GetPhaseStatusesRequest\x1a+.com.qwak.build.v1.GetPhaseStatusesResponse\x12Y\n\nGetTagPath\x12$.com.qwak.build.v1.GetTagPathRequest\x1a%.com.qwak.build.v1.GetTagPathResponseB$\n\x11\x63om.qwak.build.v1B\rBuildApiProtoP\x01\x62\x06proto3')
 
 _PHASESTATUS = DESCRIPTOR.enum_types_by_name['PhaseStatus']
 PhaseStatus = enum_type_wrapper.EnumTypeWrapper(_PHASESTATUS)
 _FAILUREREASON = DESCRIPTOR.enum_types_by_name['FailureReason']
 FailureReason = enum_type_wrapper.EnumTypeWrapper(_FAILUREREASON)
 PHASE_STATUS_INVALID = 0
 PHASE_STATUS_IN_PROGRESS = 1
@@ -51,14 +51,16 @@
 _LOGPHASESTATUSREQUEST = DESCRIPTOR.message_types_by_name['LogPhaseStatusRequest']
 _LOGPHASESTATUSRESPONSE = DESCRIPTOR.message_types_by_name['LogPhaseStatusResponse']
 _GETPHASESTATUSESREQUEST = DESCRIPTOR.message_types_by_name['GetPhaseStatusesRequest']
 _PHASESTATUSLOG = DESCRIPTOR.message_types_by_name['PhaseStatusLog']
 _GETPHASESTATUSESRESPONSE = DESCRIPTOR.message_types_by_name['GetPhaseStatusesResponse']
 _DELETEBUILDREQUEST = DESCRIPTOR.message_types_by_name['DeleteBuildRequest']
 _DELETEBUILDRESPONSE = DESCRIPTOR.message_types_by_name['DeleteBuildResponse']
+_GETTAGPATHREQUEST = DESCRIPTOR.message_types_by_name['GetTagPathRequest']
+_GETTAGPATHRESPONSE = DESCRIPTOR.message_types_by_name['GetTagPathResponse']
 RegisterBuildRequest = _reflection.GeneratedProtocolMessageType('RegisterBuildRequest', (_message.Message,), {
   'DESCRIPTOR' : _REGISTERBUILDREQUEST,
   '__module__' : 'qwak.build.v1.build_api_pb2'
   # @@protoc_insertion_point(class_scope:com.qwak.build.v1.RegisterBuildRequest)
   })
 _sym_db.RegisterMessage(RegisterBuildRequest)
 
@@ -214,27 +216,41 @@
 DeleteBuildResponse = _reflection.GeneratedProtocolMessageType('DeleteBuildResponse', (_message.Message,), {
   'DESCRIPTOR' : _DELETEBUILDRESPONSE,
   '__module__' : 'qwak.build.v1.build_api_pb2'
   # @@protoc_insertion_point(class_scope:com.qwak.build.v1.DeleteBuildResponse)
   })
 _sym_db.RegisterMessage(DeleteBuildResponse)
 
+GetTagPathRequest = _reflection.GeneratedProtocolMessageType('GetTagPathRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETTAGPATHREQUEST,
+  '__module__' : 'qwak.build.v1.build_api_pb2'
+  # @@protoc_insertion_point(class_scope:com.qwak.build.v1.GetTagPathRequest)
+  })
+_sym_db.RegisterMessage(GetTagPathRequest)
+
+GetTagPathResponse = _reflection.GeneratedProtocolMessageType('GetTagPathResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETTAGPATHRESPONSE,
+  '__module__' : 'qwak.build.v1.build_api_pb2'
+  # @@protoc_insertion_point(class_scope:com.qwak.build.v1.GetTagPathResponse)
+  })
+_sym_db.RegisterMessage(GetTagPathResponse)
+
 _BUILDAPI = DESCRIPTOR.services_by_name['BuildAPI']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.qwak.build.v1B\rBuildApiProtoP\001'
   _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._options = None
   _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._serialized_options = b'8\001'
   _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._options = None
   _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._serialized_options = b'8\001'
-  _PHASESTATUS._serialized_start=1738
-  _PHASESTATUS._serialized_end=1889
-  _FAILUREREASON._serialized_start=1891
-  _FAILUREREASON._serialized_end=2010
+  _PHASESTATUS._serialized_start=1877
+  _PHASESTATUS._serialized_end=2028
+  _FAILUREREASON._serialized_start=2030
+  _FAILUREREASON._serialized_end=2149
   _REGISTERBUILDREQUEST._serialized_start=79
   _REGISTERBUILDREQUEST._serialized_end=203
   _REGISTERBUILDRESPONSE._serialized_start=205
   _REGISTERBUILDRESPONSE._serialized_end=228
   _UPDATEBUILDSTATUSREQUEST._serialized_start=230
   _UPDATEBUILDSTATUSREQUEST._serialized_end=327
   _UPDATEBUILDSTATUSRESPONSE._serialized_start=329
@@ -273,10 +289,14 @@
   _PHASESTATUSLOG._serialized_end=1590
   _GETPHASESTATUSESRESPONSE._serialized_start=1592
   _GETPHASESTATUSESRESPONSE._serialized_end=1671
   _DELETEBUILDREQUEST._serialized_start=1673
   _DELETEBUILDREQUEST._serialized_end=1712
   _DELETEBUILDRESPONSE._serialized_start=1714
   _DELETEBUILDRESPONSE._serialized_end=1735
-  _BUILDAPI._serialized_start=2013
-  _BUILDAPI._serialized_end=3072
+  _GETTAGPATHREQUEST._serialized_start=1737
+  _GETTAGPATHREQUEST._serialized_end=1834
+  _GETTAGPATHRESPONSE._serialized_start=1836
+  _GETTAGPATHRESPONSE._serialized_end=1874
+  _BUILDAPI._serialized_start=2152
+  _BUILDAPI._serialized_end=3302
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -409,7 +409,44 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___DeleteBuildResponse = DeleteBuildResponse
+
+class GetTagPathRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
+    MODEL_ID_FIELD_NUMBER: builtins.int
+    BUILD_ID_FIELD_NUMBER: builtins.int
+    TAG_NAME_FIELD_NUMBER: builtins.int
+    environment_id: builtins.str
+    model_id: builtins.str
+    build_id: builtins.str
+    tag_name: builtins.str
+    def __init__(
+        self,
+        *,
+        environment_id: builtins.str = ...,
+        model_id: builtins.str = ...,
+        build_id: builtins.str = ...,
+        tag_name: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["build_id", b"build_id", "environment_id", b"environment_id", "model_id", b"model_id", "tag_name", b"tag_name"]) -> None: ...
+
+global___GetTagPathRequest = GetTagPathRequest
+
+class GetTagPathResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    KEY_PATH_FIELD_NUMBER: builtins.int
+    key_path: builtins.str
+    def __init__(
+        self,
+        *,
+        key_path: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["key_path", b"key_path"]) -> None: ...
+
+global___GetTagPathResponse = GetTagPathResponse
```

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,19 @@
                 response_deserializer=qwak_dot_build_dot_v1_dot_build__api__pb2.LogPhaseStatusResponse.FromString,
                 )
         self.GetPhaseStatuses = channel.unary_unary(
                 '/com.qwak.build.v1.BuildAPI/GetPhaseStatuses',
                 request_serializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetPhaseStatusesRequest.SerializeToString,
                 response_deserializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetPhaseStatusesResponse.FromString,
                 )
+        self.GetTagPath = channel.unary_unary(
+                '/com.qwak.build.v1.BuildAPI/GetTagPath',
+                request_serializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetTagPathRequest.SerializeToString,
+                response_deserializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetTagPathResponse.FromString,
+                )
 
 
 class BuildAPIServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def RegisterBuild(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -125,14 +130,20 @@
 
     def GetPhaseStatuses(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetTagPath(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_BuildAPIServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'RegisterBuild': grpc.unary_unary_rpc_method_handler(
                     servicer.RegisterBuild,
                     request_deserializer=qwak_dot_build_dot_v1_dot_build__api__pb2.RegisterBuildRequest.FromString,
                     response_serializer=qwak_dot_build_dot_v1_dot_build__api__pb2.RegisterBuildResponse.SerializeToString,
@@ -178,14 +189,19 @@
                     response_serializer=qwak_dot_build_dot_v1_dot_build__api__pb2.LogPhaseStatusResponse.SerializeToString,
             ),
             'GetPhaseStatuses': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPhaseStatuses,
                     request_deserializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetPhaseStatusesRequest.FromString,
                     response_serializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetPhaseStatusesResponse.SerializeToString,
             ),
+            'GetTagPath': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetTagPath,
+                    request_deserializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetTagPathRequest.FromString,
+                    response_serializer=qwak_dot_build_dot_v1_dot_build__api__pb2.GetTagPathResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.qwak.build.v1.BuildAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -357,7 +373,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.qwak.build.v1.BuildAPI/GetPhaseStatuses',
             qwak_dot_build_dot_v1_dot_build__api__pb2.GetPhaseStatusesRequest.SerializeToString,
             qwak_dot_build_dot_v1_dot_build__api__pb2.GetPhaseStatusesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetTagPath(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/com.qwak.build.v1.BuildAPI/GetTagPath',
+            qwak_dot_build_dot_v1_dot_build__api__pb2.GetTagPathRequest.SerializeToString,
+            qwak_dot_build_dot_v1_dot_build__api__pb2.GetTagPathResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.73/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.73/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/pyproject.toml` & `qwak_core-0.0.73/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.72"
+version = "0.0.73"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.72/qwak/automations/__init__.py` & `qwak_core-0.0.73/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/automations/automation_executions.py` & `qwak_core-0.0.73/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/automations/automations.py` & `qwak_core-0.0.73/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.73/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.73/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/automations/common.py` & `qwak_core-0.0.73/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.73/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.73/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.73/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.73/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.73/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/alert_management/client.py` & `qwak_core-0.0.73/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/analytics/client.py` & `qwak_core-0.0.73/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/audience/client.py` & `qwak_core-0.0.73/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/automation_management/client.py` & `qwak_core-0.0.73/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.73/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.73/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.73/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.73/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/build_management/client.py` & `qwak_core-0.0.73/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.73/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.73/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/deployment/client.py` & `qwak_core-0.0.73/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.73/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.73/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.73/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.73/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/instance_template/client.py` & `qwak_core-0.0.73/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.73/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/logging_client/client.py` & `qwak_core-0.0.73/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/model_management/client.py` & `qwak_core-0.0.73/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/project/client.py` & `qwak_core-0.0.73/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/secret_service/client.py` & `qwak_core-0.0.73/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.73/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.73/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.73/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.73/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.73/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.73/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.73/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.73/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.73/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.73/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.73/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.73/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.73/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.73/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.73/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/offline/client.py` & `qwak_core-0.0.73/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/feature_store/online/client.py` & `qwak_core-0.0.73/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/const.py` & `qwak_core-0.0.73/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.73/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.73/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.73/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.73/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/singleton_meta.py` & `qwak_core-0.0.73/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/tool/auth.py` & `qwak_core-0.0.73/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.73/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.73/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.73/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.73/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/adapters/__init__.py` & `qwak_core-0.0.73/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.73/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.73/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.73/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.73/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.73/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/base.py` & `qwak_core-0.0.73/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/decorators/api.py` & `qwak_core-0.0.73/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.73/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/experiment_tracking.py` & `qwak_core-0.0.73/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/schema.py` & `qwak_core-0.0.73/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/schema_entities.py` & `qwak_core-0.0.73/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.73/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.73/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.73/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.73/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.73/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.73/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.73/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.73/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/client.py` & `qwak_core-0.0.73/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.73/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/models/model.py` & `qwak_core-0.0.73/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.73/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.73/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/tools/logger/logger.py` & `qwak_core-0.0.73/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak/tools/logger/logging.yml` & `qwak_core-0.0.73/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.73/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/qwak_services_mock/services_mock.py` & `qwak_core-0.0.73/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.72/setup.py` & `qwak_core-0.0.73/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.72',
+    'version': '0.0.73',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.72/PKG-INFO` & `qwak_core-0.0.73/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.72
+Version: 0.0.73
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

