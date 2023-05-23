# Comparing `tmp/qwak_core-0.0.74.tar.gz` & `tmp/qwak_core-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.74.tar", max compression
+gzip compressed data, was "qwak_core-0.0.75.tar", max compression
```

## Comparing `qwak_core-0.0.74.tar` & `qwak_core-0.0.75.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-23 12:09:12.882221 qwak_core-0.0.74/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:11:44.276186 qwak_core-0.0.74/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-23 12:11:44.320186 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-23 12:11:13.691789 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.324186 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-23 12:11:44.316186 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-23 12:11:13.155782 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.316186 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-23 12:11:44.320186 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-23 12:11:13.419786 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.320186 qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-23 12:11:44.304186 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-23 12:11:12.359772 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-23 12:11:44.308186 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-23 12:11:44.308186 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-23 12:11:12.627775 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.312186 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-23 12:11:44.312186 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-23 12:11:12.891779 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.316186 qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-23 12:11:44.280186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-23 12:11:12.091768 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-23 12:11:44.280186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-23 12:11:44.288186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-23 12:11:13.963793 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.292186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-23 12:11:44.296186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-23 12:11:14.495800 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.296186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-23 12:11:44.300186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-23 12:11:14.763803 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-23 12:11:44.300186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-23 12:11:44.292186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-23 12:11:14.227796 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.296186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-23 12:11:44.304186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-23 12:11:15.031807 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.304186 qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-23 12:11:44.380187 qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-23 12:11:18.855856 qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.384187 qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-23 12:11:44.388187 qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-23 12:11:19.159860 qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-23 12:11:44.388187 qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-23 12:11:44.504189 qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-23 12:11:26.851960 qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.508189 qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-23 12:11:44.508189 qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-23 12:11:27.119963 qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-23 12:11:44.512189 qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-23 12:11:44.516189 qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-23 12:11:28.475981 qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-23 12:11:44.516189 qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-23 12:11:44.512189 qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-23 12:11:28.207977 qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.512189 qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-23 12:11:44.516189 qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-23 12:11:28.743984 qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.520189 qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-23 12:11:44.520189 qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-23 12:11:29.011988 qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-23 12:11:44.524189 qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-23 12:11:44.680191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-23 12:11:40.660139 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.684191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-23 12:11:44.664191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-23 12:11:40.112132 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.672191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-23 12:11:44.676191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-23 12:11:40.380135 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.676191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-23 12:11:44.660191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-23 12:11:39.568125 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-23 12:11:44.660191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-23 12:11:44.660191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-23 12:11:39.844128 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.664191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-23 12:11:44.692191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-23 12:11:41.480149 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.696191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-23 12:11:44.692191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-23 12:11:41.208146 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.692191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-23 12:11:44.684191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-23 12:11:40.932142 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.688191 qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-23 12:11:44.656191 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-23 12:11:39.284121 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.656191 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-23 12:11:44.648191 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-23 12:11:38.724114 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.652191 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-23 12:11:44.652191 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-23 12:11:39.016117 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-23 12:11:44.652191 qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    19978 2023-05-23 12:11:44.560189 qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    16810 2023-05-23 12:11:31.844024 qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-23 12:11:44.560189 qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-23 12:11:44.556189 qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-23 12:11:31.572021 qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.556189 qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-23 12:11:44.544189 qwak_core-0.0.74/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-23 12:11:31.020014 qwak_core-0.0.74/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.544189 qwak_core-0.0.74/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-23 12:11:44.548189 qwak_core-0.0.74/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-23 12:11:31.284017 qwak_core-0.0.74/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.548189 qwak_core-0.0.74/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-23 12:11:44.548189 qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-23 12:11:32.116028 qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-23 12:11:44.552189 qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-23 12:11:44.552189 qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-23 12:11:32.708036 qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-23 12:11:44.556189 qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-23 12:11:44.584190 qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-23 12:11:33.272043 qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.588190 qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-23 12:11:44.588190 qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-23 12:11:33.540046 qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-23 12:11:44.592190 qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-23 12:11:44.532189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-23 12:11:30.208003 qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.536189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-23 12:11:44.536189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-23 12:11:30.480007 qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-23 12:11:44.540189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-23 12:11:44.528189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-23 12:11:29.627996 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.528189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-23 12:11:44.524189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-23 12:11:29.307991 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.524189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-23 12:11:44.532189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-23 12:11:29.932000 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-23 12:11:44.532189 qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-23 12:11:44.352187 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-23 12:11:17.495838 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.352187 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-23 12:11:44.352187 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-23 12:11:17.771842 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.356187 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-23 12:11:44.356187 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-23 12:11:18.047845 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-23 12:11:44.356187 qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-23 12:11:44.460188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-23 12:11:25.223939 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.460188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-23 12:11:44.456188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-23 12:11:24.955935 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-23 12:11:44.456188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-23 12:11:44.428188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-23 12:11:22.507903 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.432188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-23 12:11:44.424188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-23 12:11:22.227900 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.428188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-23 12:11:44.416188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-23 12:11:21.371888 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.416188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-23 12:11:44.424188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-23 12:11:21.955896 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-23 12:11:44.424188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-23 12:11:44.432188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-23 12:11:22.787907 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.432188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-23 12:11:44.436188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-23 12:11:23.055910 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-23 12:11:44.436188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-23 12:11:44.420188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-23 12:11:21.659892 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.420188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-23 12:11:44.440188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-23 12:11:23.323914 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.440188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11224 2023-05-23 12:11:44.440188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    14819 2023-05-23 12:11:23.591917 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.444188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-23 12:11:44.464188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-23 12:11:43.512176 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.464188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-23 12:11:44.480188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-23 12:11:43.816180 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-23 12:11:44.484188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-23 12:11:44.484188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-23 12:11:26.035949 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.488188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-23 12:11:44.488188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-23 12:11:26.307953 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-23 12:11:44.492189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-23 12:11:44.492189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-23 12:11:26.579956 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.496188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-23 12:11:44.500189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-23 12:11:27.671970 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.500189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-23 12:11:44.496188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-23 12:11:27.395967 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-23 12:11:44.500189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-23 12:11:44.504189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-23 12:11:27.939974 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.504189 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-23 12:11:44.444188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-23 12:11:23.867921 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.444188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-23 12:11:44.448188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-23 12:11:24.143925 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.448188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-23 12:11:44.452188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-23 12:11:24.415928 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-23 12:11:44.452188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-23 12:11:44.452188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-23 12:11:24.683931 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.456188 qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-23 12:11:44.696191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-23 12:11:41.748153 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.700191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-23 12:11:44.700191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-23 12:11:42.012156 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-23 12:11:44.704191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-23 12:11:44.704191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-23 12:11:42.276160 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.704191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-23 12:11:44.708191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-23 12:11:42.552163 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-23 12:11:44.708191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-23 12:11:44.712191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-23 12:11:42.868167 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-23 12:11:44.712191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-23 12:11:44.712191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-23 12:11:43.196172 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.716191 qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-23 12:11:44.592190 qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-23 12:11:33.820050 qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.596190 qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-23 12:11:44.596190 qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-23 12:11:34.096053 qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-23 12:11:44.596190 qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-23 12:11:44.396187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-23 12:11:20.275874 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.396187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-23 12:11:44.400187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-23 12:11:20.543878 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.404187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-23 12:11:44.404187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-23 12:11:20.819882 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-23 12:11:44.408187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-23 12:11:44.412187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-23 12:11:21.091885 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.412187 qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-23 12:11:44.540189 qwak_core-0.0.74/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-23 12:11:30.748010 qwak_core-0.0.74/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-23 12:11:44.540189 qwak_core-0.0.74/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-23 12:11:44.600190 qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-23 12:11:34.368057 qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.600190 qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-23 12:11:44.604190 qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-23 12:11:34.644061 qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-23 12:11:44.604190 qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-23 12:11:44.620190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-23 12:11:36.268082 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.624190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-23 12:11:44.624190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-23 12:11:36.532085 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.624190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-23 12:11:44.628190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-23 12:11:36.804089 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.628190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-23 12:11:44.628190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-23 12:11:37.072092 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.632190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-23 12:11:44.632190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-23 12:11:37.352096 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.636190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-23 12:11:44.636190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-23 12:11:37.648100 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-23 12:11:44.640190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-23 12:11:44.640190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-23 12:11:37.916103 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.640190 qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-23 12:11:44.608190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-23 12:11:35.200068 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.608190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-23 12:11:44.616190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-23 12:11:35.996078 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.620190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-23 12:11:44.612190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-23 12:11:35.468071 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-23 12:11:44.612190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-23 12:11:44.616190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-23 12:11:35.732075 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.616190 qwak_core-0.0.74/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-23 12:11:44.576190 qwak_core-0.0.74/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-23 12:11:33.004039 qwak_core-0.0.74/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-23 12:11:44.584190 qwak_core-0.0.74/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-23 12:11:44.344187 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-23 12:11:19.727867 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-23 12:11:44.344187 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-23 12:11:44.340186 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-23 12:11:19.455864 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.344187 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-23 12:11:44.348187 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-23 12:11:20.003871 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-23 12:11:44.348187 qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-23 12:11:44.564190 qwak_core-0.0.74/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-23 12:11:32.404032 qwak_core-0.0.74/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-23 12:11:44.564190 qwak_core-0.0.74/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-23 12:11:44.604190 qwak_core-0.0.74/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-23 12:11:34.932064 qwak_core-0.0.74/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-23 12:11:44.608190 qwak_core-0.0.74/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-23 12:11:44.336187 qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-23 12:11:16.411824 qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.340186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-23 12:11:44.336187 qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-23 12:11:16.143821 qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-23 12:11:44.336187 qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-23 12:11:44.324186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-23 12:11:15.315810 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.328186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-23 12:11:44.328186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-23 12:11:15.599814 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.328186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-23 12:11:44.332186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-23 12:11:15.871817 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-23 12:11:44.332186 qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-23 12:11:44.644190 qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-23 12:11:38.460110 qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-23 12:11:44.648191 qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-23 12:11:44.644190 qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-23 12:11:38.188107 qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.644190 qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-23 12:11:44.360187 qwak_core-0.0.74/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-23 12:11:18.319849 qwak_core-0.0.74/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.360187 qwak_core-0.0.74/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-23 12:11:44.364187 qwak_core-0.0.74/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-23 12:11:18.587853 qwak_core-0.0.74/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-23 12:11:44.364187 qwak_core-0.0.74/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-23 12:11:47.380226 qwak_core-0.0.74/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-23 12:11:47.380226 qwak_core-0.0.74/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-23 12:09:12.882221 qwak_core-0.0.74/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-23 12:09:12.886222 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-23 12:09:12.890221 qwak_core-0.0.74/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-23 12:09:12.894221 qwak_core-0.0.74/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-23 12:09:12.898222 qwak_core-0.0.74/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.74/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.74/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-23 19:04:00.882871 qwak_core-0.0.75/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 19:05:51.651655 qwak_core-0.0.75/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-23 19:05:51.679655 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-23 19:05:29.411498 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.683655 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-23 19:05:51.675655 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-23 19:05:28.991495 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.679655 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-23 19:05:51.679655 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-23 19:05:29.211496 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.679655 qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-23 19:05:51.671655 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-23 19:05:28.311490 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-23 19:05:51.671655 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-23 19:05:51.671655 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-23 19:05:28.527492 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.671655 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-23 19:05:51.675655 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-23 19:05:28.775493 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.675655 qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-23 19:05:51.655655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-23 19:05:28.095489 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-23 19:05:51.655655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-23 19:05:51.655655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-23 19:05:29.623499 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.659655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-23 19:05:51.663655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-23 19:05:30.015502 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.663655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-23 19:05:51.663655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-23 19:05:30.211504 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-23 19:05:51.667655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-23 19:05:51.659655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-23 19:05:29.819501 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.663655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-23 19:05:51.667655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-23 19:05:30.399505 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.667655 qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-23 19:05:51.711655 qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-23 19:05:33.195525 qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.715655 qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-23 19:05:51.715655 qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-23 19:05:33.395526 qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-23 19:05:51.715655 qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-23 19:05:51.879657 qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-23 19:05:38.951566 qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.879657 qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-23 19:05:51.879657 qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-23 19:05:39.143567 qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-23 19:05:51.883657 qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-23 19:05:51.887657 qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-23 19:05:40.147574 qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-23 19:05:51.887657 qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-23 19:05:51.883657 qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-23 19:05:39.951573 qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.883657 qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-23 19:05:51.887657 qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-23 19:05:40.351575 qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.887657 qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-23 19:05:51.891657 qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-23 19:05:40.543577 qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-23 19:05:51.891657 qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-23 19:05:51.995658 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-23 19:05:49.027637 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.995658 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-23 19:05:51.991657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-23 19:05:48.639634 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.991657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-23 19:05:51.991657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-23 19:05:48.827635 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.995658 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-23 19:05:51.987657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-23 19:05:48.243631 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-23 19:05:51.987657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-23 19:05:51.987657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-23 19:05:48.443632 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.991657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-23 19:05:52.003657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-23 19:05:49.623641 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:52.007658 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-23 19:05:51.999657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-23 19:05:49.407639 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.999657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-23 19:05:51.999657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-23 19:05:49.215638 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.999657 qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-23 19:05:51.983657 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-23 19:05:48.039630 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.983657 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-23 19:05:51.979657 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-23 19:05:47.643627 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.979657 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-23 19:05:51.979657 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-23 19:05:47.847628 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-23 19:05:51.983657 qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-23 19:05:51.919657 qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-23 19:05:42.567591 qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-23 19:05:51.919657 qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-23 19:05:51.915657 qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-23 19:05:42.351590 qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.915657 qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-23 19:05:51.907657 qwak_core-0.0.75/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-23 19:05:41.963587 qwak_core-0.0.75/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.907657 qwak_core-0.0.75/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-23 19:05:51.907657 qwak_core-0.0.75/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-23 19:05:42.155588 qwak_core-0.0.75/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.911657 qwak_core-0.0.75/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-23 19:05:51.911657 qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-23 19:05:42.771593 qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-23 19:05:51.911657 qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-23 19:05:51.915657 qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-23 19:05:43.199596 qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-23 19:05:51.915657 qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-23 19:05:51.923657 qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-23 19:05:43.615599 qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.927657 qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-23 19:05:51.927657 qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-23 19:05:43.811600 qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-23 19:05:51.927657 qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-23 19:05:51.899657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-23 19:05:41.359583 qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.899657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-23 19:05:51.903657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-23 19:05:41.555584 qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-23 19:05:51.903657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-23 19:05:51.895657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-23 19:05:40.959580 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.895657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-23 19:05:51.891657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-23 19:05:40.763579 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.895657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-23 19:05:51.895657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-23 19:05:41.159581 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-23 19:05:51.899657 qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-23 19:05:51.703655 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-23 19:05:32.195518 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.703655 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-23 19:05:51.703655 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-23 19:05:32.395519 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.703655 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-23 19:05:51.707656 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-23 19:05:32.595521 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-23 19:05:51.707656 qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-23 19:05:51.859656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-23 19:05:37.763557 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.859656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-23 19:05:51.855656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-23 19:05:37.571556 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-23 19:05:51.855656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-23 19:05:51.831656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-23 19:05:35.735543 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.831656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-23 19:05:51.827656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-23 19:05:35.543542 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.827656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-23 19:05:51.819656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-23 19:05:34.939537 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.819656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-23 19:05:51.823656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-23 19:05:35.343540 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-23 19:05:51.827656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-23 19:05:51.831656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-23 19:05:35.931544 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.831656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-23 19:05:51.835656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-23 19:05:36.151546 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-23 19:05:51.835656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-23 19:05:51.823656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-23 19:05:35.139539 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.823656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-23 19:05:51.835656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-23 19:05:36.347547 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.839656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11224 2023-05-23 19:05:51.839656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    14819 2023-05-23 19:05:36.547549 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.839656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-23 19:05:51.859656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-23 19:05:51.003651 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.863657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-23 19:05:51.863657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-23 19:05:51.231652 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-23 19:05:51.863657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-23 19:05:51.863657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-23 19:05:38.363561 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.867657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-23 19:05:51.867657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-23 19:05:38.559563 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-23 19:05:51.867657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-23 19:05:51.871657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-23 19:05:38.751564 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.871657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-23 19:05:51.875657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-23 19:05:39.539570 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.875657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-23 19:05:51.871657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-23 19:05:39.339568 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-23 19:05:51.871657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-23 19:05:51.875657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-23 19:05:39.747571 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.879657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-23 19:05:51.839656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-23 19:05:36.763550 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.843656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-23 19:05:51.843656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-23 19:05:36.967552 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.843656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-23 19:05:51.847656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-23 19:05:37.167553 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-23 19:05:51.851657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-23 19:05:51.851657 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-23 19:05:37.371554 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.855656 qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-23 19:05:52.007658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-23 19:05:49.815642 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:52.007658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-23 19:05:52.007658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-23 19:05:50.007644 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-23 19:05:52.011658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-23 19:05:52.011658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-23 19:05:50.203645 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:52.011658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-23 19:05:52.015658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-23 19:05:50.395646 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-23 19:05:52.015658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-23 19:05:52.015658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-23 19:05:50.595648 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-23 19:05:52.019658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-23 19:05:52.019658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-23 19:05:50.787649 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:52.019658 qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-23 19:05:51.931657 qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-23 19:05:44.011601 qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.931657 qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-23 19:05:51.931657 qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-23 19:05:44.211603 qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-23 19:05:51.931657 qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-23 19:05:51.739656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-23 19:05:34.175532 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.751656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-23 19:05:51.763656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-23 19:05:34.359533 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.771656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-23 19:05:51.783656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-23 19:05:34.547534 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-23 19:05:51.795656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-23 19:05:51.807656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-23 19:05:34.739536 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.819656 qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-23 19:05:51.903657 qwak_core-0.0.75/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-23 19:05:41.747585 qwak_core-0.0.75/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-23 19:05:51.903657 qwak_core-0.0.75/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-23 19:05:51.935657 qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-23 19:05:44.411604 qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.935657 qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-23 19:05:51.935657 qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-23 19:05:44.619606 qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-23 19:05:51.939657 qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-23 19:05:51.951657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-23 19:05:45.855614 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.955657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-23 19:05:51.955657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-23 19:05:46.047616 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.959657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-23 19:05:51.959657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-23 19:05:46.243617 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.959657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-23 19:05:51.963657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-23 19:05:46.459618 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.963657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-23 19:05:51.963657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-23 19:05:46.659620 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.967657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-23 19:05:51.967657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-23 19:05:46.883622 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-23 19:05:51.967657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-23 19:05:51.971657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-23 19:05:47.075623 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.971657 qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-23 19:05:51.939657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-23 19:05:45.051609 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.943657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-23 19:05:51.951657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-23 19:05:45.655613 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.951657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-23 19:05:51.943657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-23 19:05:45.259610 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-23 19:05:51.943657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-23 19:05:51.947657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-23 19:05:45.463611 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.947657 qwak_core-0.0.75/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-23 19:05:51.923657 qwak_core-0.0.75/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-23 19:05:43.415597 qwak_core-0.0.75/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-23 19:05:51.923657 qwak_core-0.0.75/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-23 19:05:51.695655 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-23 19:05:33.787529 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-23 19:05:51.699655 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-23 19:05:51.695655 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-23 19:05:33.591528 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.695655 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-23 19:05:51.699655 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-23 19:05:33.983530 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-23 19:05:51.699655 qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-23 19:05:51.919657 qwak_core-0.0.75/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-23 19:05:42.975594 qwak_core-0.0.75/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-23 19:05:51.923657 qwak_core-0.0.75/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-23 19:05:51.939657 qwak_core-0.0.75/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-23 19:05:44.855607 qwak_core-0.0.75/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-23 19:05:51.939657 qwak_core-0.0.75/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-23 19:05:51.691655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-23 19:05:31.399512 qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.695655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-23 19:05:51.691655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-23 19:05:31.203511 qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-23 19:05:51.691655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-23 19:05:51.683655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-23 19:05:30.615507 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.683655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-23 19:05:51.687655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-23 19:05:30.811508 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.687655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-23 19:05:51.687655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-23 19:05:31.007509 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-23 19:05:51.687655 qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-23 19:05:51.975657 qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-23 19:05:47.455626 qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-23 19:05:51.979657 qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-23 19:05:51.975657 qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-23 19:05:47.267624 qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.975657 qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-23 19:05:51.707656 qwak_core-0.0.75/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-23 19:05:32.787522 qwak_core-0.0.75/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.711655 qwak_core-0.0.75/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-23 19:05:51.711655 qwak_core-0.0.75/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-23 19:05:32.979523 qwak_core-0.0.75/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-23 19:05:51.711655 qwak_core-0.0.75/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-23 19:05:56.735691 qwak_core-0.0.75/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-23 19:05:56.735691 qwak_core-0.0.75/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-23 19:04:00.886871 qwak_core-0.0.75/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-23 19:04:00.890871 qwak_core-0.0.75/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-23 19:04:00.894871 qwak_core-0.0.75/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.75/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.75/PKG-INFO
```

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.build.v1 import build_pb2 as qwak_dot_build_dot_v1_dot_build__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dqwak/build/v1/build_api.proto\x12\x11\x63om.qwak.build.v1\x1a\x19qwak/build/v1/build.proto\"|\n\x14RegisterBuildRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x10\n\x08\x63ommitId\x18\x02 \x01(\t\x12\x0f\n\x07modelId\x18\x03 \x01(\t\x12\x13\n\x0b\x62uildConfig\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12\r\n\x05steps\x18\x06 \x03(\t\"\x17\n\x15RegisterBuildResponse\"a\n\x18UpdateBuildStatusRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x34\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.BuildStatus\"\x1b\n\x19UpdateBuildStatusResponse\"\xba\x02\n!RegisterExperimentTrackingRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12P\n\x06params\x18\x02 \x03(\x0b\x32@.com.qwak.build.v1.RegisterExperimentTrackingRequest.ParamsEntry\x12R\n\x07metrics\x18\x03 \x03(\x0b\x32\x41.com.qwak.build.v1.RegisterExperimentTrackingRequest.MetricsEntry\x1a-\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"$\n\"RegisterExperimentTrackingResponse\"d\n\x1aRegisterModelSchemaRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x34\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.ModelSchema\"\x1d\n\x1bRegisterModelSchemaResponse\"#\n\x0fGetBuildRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\";\n\x10GetBuildResponse\x12\'\n\x05\x62uild\x18\x01 \x01(\x0b\x32\x18.com.qwak.build.v1.Build\"j\n\x11ListBuildsRequest\x12\x11\n\tbranch_id\x18\x01 \x01(\t\x12.\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.BuildFilter\x12\x12\n\nmodel_uuid\x18\x03 \x01(\t\"=\n\x12ListBuildsResponse\x12\'\n\x05\x62uild\x18\x01 \x03(\x0b\x32\x18.com.qwak.build.v1.Build\"5\n\x13RegisterTagsRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\"\x16\n\x14RegisterTagsResponse\"\x8e\x01\n\x15LogPhaseStatusRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x10\n\x08phase_id\x18\x02 \x01(\t\x12.\n\x06status\x18\x03 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x04 \x01(\x05\"\x18\n\x16LogPhaseStatusResponse\"+\n\x17GetPhaseStatusesRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\"\xb3\x01\n\x0ePhaseStatusLog\x12\x10\n\x08phase_id\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x03 \x01(\x05\x12<\n\x12pod_failure_reason\x18\x04 \x01(\x0e\x32 .com.qwak.build.v1.FailureReason\"O\n\x18GetPhaseStatusesResponse\x12\x33\n\x08statuses\x18\x01 \x03(\x0b\x32!.com.qwak.build.v1.PhaseStatusLog\"\'\n\x12\x44\x65leteBuildRequest\x12\x11\n\tbuild_ids\x18\x01 \x03(\t\"\x15\n\x13\x44\x65leteBuildResponse\"a\n\x11GetTagPathRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x10\n\x08tag_name\x18\x04 \x01(\t\"&\n\x12GetTagPathResponse\x12\x10\n\x08key_path\x18\x01 \x01(\t*\x97\x01\n\x0bPhaseStatus\x12\x18\n\x14PHASE_STATUS_INVALID\x10\x00\x12\x1c\n\x18PHASE_STATUS_IN_PROGRESS\x10\x01\x12\x1b\n\x17PHASE_STATUS_SUCCESSFUL\x10\x02\x12\x17\n\x13PHASE_STATUS_FAILED\x10\x03\x12\x1a\n\x16PHASE_STATUS_CANCELLED\x10\x04*w\n\rFailureReason\x12\x1e\n\x1a\x46\x41ILURE_REASON_UNSPECIFIED\x10\x00\x12$\n FAILURE_REASON_AVAILABLE_IN_LOGS\x10\x01\x12 \n\x1c\x46\x41ILURE_REASON_OUT_OF_MEMORY\x10\x02\x32\xfe\x08\n\x08\x42uildAPI\x12\x62\n\rRegisterBuild\x12\'.com.qwak.build.v1.RegisterBuildRequest\x1a(.com.qwak.build.v1.RegisterBuildResponse\x12n\n\x11UpdateBuildStatus\x12+.com.qwak.build.v1.UpdateBuildStatusRequest\x1a,.com.qwak.build.v1.UpdateBuildStatusResponse\x12\x89\x01\n\x1aRegisterExperimentTracking\x12\x34.com.qwak.build.v1.RegisterExperimentTrackingRequest\x1a\x35.com.qwak.build.v1.RegisterExperimentTrackingResponse\x12_\n\x0cRegisterTags\x12&.com.qwak.build.v1.RegisterTagsRequest\x1a\'.com.qwak.build.v1.RegisterTagsResponse\x12t\n\x13RegisterModelSchema\x12-.com.qwak.build.v1.RegisterModelSchemaRequest\x1a..com.qwak.build.v1.RegisterModelSchemaResponse\x12S\n\x08GetBuild\x12\".com.qwak.build.v1.GetBuildRequest\x1a#.com.qwak.build.v1.GetBuildResponse\x12Y\n\nListBuilds\x12$.com.qwak.build.v1.ListBuildsRequest\x1a%.com.qwak.build.v1.ListBuildsResponse\x12\\\n\x0b\x44\x65leteBuild\x12%.com.qwak.build.v1.DeleteBuildRequest\x1a&.com.qwak.build.v1.DeleteBuildResponse\x12\x65\n\x0eLogPhaseStatus\x12(.com.qwak.build.v1.LogPhaseStatusRequest\x1a).com.qwak.build.v1.LogPhaseStatusResponse\x12k\n\x10GetPhaseStatuses\x12*.com.qwak.build.v1.GetPhaseStatusesRequest\x1a+.com.qwak.build.v1.GetPhaseStatusesResponse\x12Y\n\nGetTagPath\x12$.com.qwak.build.v1.GetTagPathRequest\x1a%.com.qwak.build.v1.GetTagPathResponseB$\n\x11\x63om.qwak.build.v1B\rBuildApiProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dqwak/build/v1/build_api.proto\x12\x11\x63om.qwak.build.v1\x1a\x19qwak/build/v1/build.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"|\n\x14RegisterBuildRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x10\n\x08\x63ommitId\x18\x02 \x01(\t\x12\x0f\n\x07modelId\x18\x03 \x01(\t\x12\x13\n\x0b\x62uildConfig\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12\r\n\x05steps\x18\x06 \x03(\t\"\x17\n\x15RegisterBuildResponse\"a\n\x18UpdateBuildStatusRequest\x12\x0f\n\x07\x62uildId\x18\x01 \x01(\t\x12\x34\n\x0c\x62uild_status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.BuildStatus\"\x1b\n\x19UpdateBuildStatusResponse\"\xba\x02\n!RegisterExperimentTrackingRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12P\n\x06params\x18\x02 \x03(\x0b\x32@.com.qwak.build.v1.RegisterExperimentTrackingRequest.ParamsEntry\x12R\n\x07metrics\x18\x03 \x03(\x0b\x32\x41.com.qwak.build.v1.RegisterExperimentTrackingRequest.MetricsEntry\x1a-\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"$\n\"RegisterExperimentTrackingResponse\"d\n\x1aRegisterModelSchemaRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x34\n\x0cmodel_schema\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.ModelSchema\"\x1d\n\x1bRegisterModelSchemaResponse\"#\n\x0fGetBuildRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\";\n\x10GetBuildResponse\x12\'\n\x05\x62uild\x18\x01 \x01(\x0b\x32\x18.com.qwak.build.v1.Build\"j\n\x11ListBuildsRequest\x12\x11\n\tbranch_id\x18\x01 \x01(\t\x12.\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x1e.com.qwak.build.v1.BuildFilter\x12\x12\n\nmodel_uuid\x18\x03 \x01(\t\"=\n\x12ListBuildsResponse\x12\'\n\x05\x62uild\x18\x01 \x03(\x0b\x32\x18.com.qwak.build.v1.Build\"5\n\x13RegisterTagsRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\"\x16\n\x14RegisterTagsResponse\"\x8e\x01\n\x15LogPhaseStatusRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x10\n\x08phase_id\x18\x02 \x01(\t\x12.\n\x06status\x18\x03 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x04 \x01(\x05\"\x18\n\x16LogPhaseStatusResponse\"+\n\x17GetPhaseStatusesRequest\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\"\x99\x02\n\x0ePhaseStatusLog\x12\x10\n\x08phase_id\x18\x01 \x01(\t\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.com.qwak.build.v1.PhaseStatus\x12!\n\x19phase_duration_in_seconds\x18\x03 \x01(\x05\x12<\n\x12pod_failure_reason\x18\x04 \x01(\x0e\x32 .com.qwak.build.v1.FailureReason\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10last_modified_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"O\n\x18GetPhaseStatusesResponse\x12\x33\n\x08statuses\x18\x01 \x03(\x0b\x32!.com.qwak.build.v1.PhaseStatusLog\"\'\n\x12\x44\x65leteBuildRequest\x12\x11\n\tbuild_ids\x18\x01 \x03(\t\"\x15\n\x13\x44\x65leteBuildResponse\"a\n\x11GetTagPathRequest\x12\x16\n\x0e\x65nvironment_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\x12\x10\n\x08tag_name\x18\x04 \x01(\t\"&\n\x12GetTagPathResponse\x12\x10\n\x08key_path\x18\x01 \x01(\t*\x97\x01\n\x0bPhaseStatus\x12\x18\n\x14PHASE_STATUS_INVALID\x10\x00\x12\x1c\n\x18PHASE_STATUS_IN_PROGRESS\x10\x01\x12\x1b\n\x17PHASE_STATUS_SUCCESSFUL\x10\x02\x12\x17\n\x13PHASE_STATUS_FAILED\x10\x03\x12\x1a\n\x16PHASE_STATUS_CANCELLED\x10\x04*w\n\rFailureReason\x12\x1e\n\x1a\x46\x41ILURE_REASON_UNSPECIFIED\x10\x00\x12$\n FAILURE_REASON_AVAILABLE_IN_LOGS\x10\x01\x12 \n\x1c\x46\x41ILURE_REASON_OUT_OF_MEMORY\x10\x02\x32\xfe\x08\n\x08\x42uildAPI\x12\x62\n\rRegisterBuild\x12\'.com.qwak.build.v1.RegisterBuildRequest\x1a(.com.qwak.build.v1.RegisterBuildResponse\x12n\n\x11UpdateBuildStatus\x12+.com.qwak.build.v1.UpdateBuildStatusRequest\x1a,.com.qwak.build.v1.UpdateBuildStatusResponse\x12\x89\x01\n\x1aRegisterExperimentTracking\x12\x34.com.qwak.build.v1.RegisterExperimentTrackingRequest\x1a\x35.com.qwak.build.v1.RegisterExperimentTrackingResponse\x12_\n\x0cRegisterTags\x12&.com.qwak.build.v1.RegisterTagsRequest\x1a\'.com.qwak.build.v1.RegisterTagsResponse\x12t\n\x13RegisterModelSchema\x12-.com.qwak.build.v1.RegisterModelSchemaRequest\x1a..com.qwak.build.v1.RegisterModelSchemaResponse\x12S\n\x08GetBuild\x12\".com.qwak.build.v1.GetBuildRequest\x1a#.com.qwak.build.v1.GetBuildResponse\x12Y\n\nListBuilds\x12$.com.qwak.build.v1.ListBuildsRequest\x1a%.com.qwak.build.v1.ListBuildsResponse\x12\\\n\x0b\x44\x65leteBuild\x12%.com.qwak.build.v1.DeleteBuildRequest\x1a&.com.qwak.build.v1.DeleteBuildResponse\x12\x65\n\x0eLogPhaseStatus\x12(.com.qwak.build.v1.LogPhaseStatusRequest\x1a).com.qwak.build.v1.LogPhaseStatusResponse\x12k\n\x10GetPhaseStatuses\x12*.com.qwak.build.v1.GetPhaseStatusesRequest\x1a+.com.qwak.build.v1.GetPhaseStatusesResponse\x12Y\n\nGetTagPath\x12$.com.qwak.build.v1.GetTagPathRequest\x1a%.com.qwak.build.v1.GetTagPathResponseB$\n\x11\x63om.qwak.build.v1B\rBuildApiProtoP\x01\x62\x06proto3')
 
 _PHASESTATUS = DESCRIPTOR.enum_types_by_name['PhaseStatus']
 PhaseStatus = enum_type_wrapper.EnumTypeWrapper(_PHASESTATUS)
 _FAILUREREASON = DESCRIPTOR.enum_types_by_name['FailureReason']
 FailureReason = enum_type_wrapper.EnumTypeWrapper(_FAILUREREASON)
 PHASE_STATUS_INVALID = 0
 PHASE_STATUS_IN_PROGRESS = 1
@@ -239,64 +240,64 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\021com.qwak.build.v1B\rBuildApiProtoP\001'
   _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._options = None
   _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._serialized_options = b'8\001'
   _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._options = None
   _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._serialized_options = b'8\001'
-  _PHASESTATUS._serialized_start=1877
-  _PHASESTATUS._serialized_end=2028
-  _FAILUREREASON._serialized_start=2030
-  _FAILUREREASON._serialized_end=2149
-  _REGISTERBUILDREQUEST._serialized_start=79
-  _REGISTERBUILDREQUEST._serialized_end=203
-  _REGISTERBUILDRESPONSE._serialized_start=205
-  _REGISTERBUILDRESPONSE._serialized_end=228
-  _UPDATEBUILDSTATUSREQUEST._serialized_start=230
-  _UPDATEBUILDSTATUSREQUEST._serialized_end=327
-  _UPDATEBUILDSTATUSRESPONSE._serialized_start=329
-  _UPDATEBUILDSTATUSRESPONSE._serialized_end=356
-  _REGISTEREXPERIMENTTRACKINGREQUEST._serialized_start=359
-  _REGISTEREXPERIMENTTRACKINGREQUEST._serialized_end=673
-  _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._serialized_start=580
-  _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._serialized_end=625
-  _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._serialized_start=627
-  _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._serialized_end=673
-  _REGISTEREXPERIMENTTRACKINGRESPONSE._serialized_start=675
-  _REGISTEREXPERIMENTTRACKINGRESPONSE._serialized_end=711
-  _REGISTERMODELSCHEMAREQUEST._serialized_start=713
-  _REGISTERMODELSCHEMAREQUEST._serialized_end=813
-  _REGISTERMODELSCHEMARESPONSE._serialized_start=815
-  _REGISTERMODELSCHEMARESPONSE._serialized_end=844
-  _GETBUILDREQUEST._serialized_start=846
-  _GETBUILDREQUEST._serialized_end=881
-  _GETBUILDRESPONSE._serialized_start=883
-  _GETBUILDRESPONSE._serialized_end=942
-  _LISTBUILDSREQUEST._serialized_start=944
-  _LISTBUILDSREQUEST._serialized_end=1050
-  _LISTBUILDSRESPONSE._serialized_start=1052
-  _LISTBUILDSRESPONSE._serialized_end=1113
-  _REGISTERTAGSREQUEST._serialized_start=1115
-  _REGISTERTAGSREQUEST._serialized_end=1168
-  _REGISTERTAGSRESPONSE._serialized_start=1170
-  _REGISTERTAGSRESPONSE._serialized_end=1192
-  _LOGPHASESTATUSREQUEST._serialized_start=1195
-  _LOGPHASESTATUSREQUEST._serialized_end=1337
-  _LOGPHASESTATUSRESPONSE._serialized_start=1339
-  _LOGPHASESTATUSRESPONSE._serialized_end=1363
-  _GETPHASESTATUSESREQUEST._serialized_start=1365
-  _GETPHASESTATUSESREQUEST._serialized_end=1408
-  _PHASESTATUSLOG._serialized_start=1411
-  _PHASESTATUSLOG._serialized_end=1590
-  _GETPHASESTATUSESRESPONSE._serialized_start=1592
-  _GETPHASESTATUSESRESPONSE._serialized_end=1671
-  _DELETEBUILDREQUEST._serialized_start=1673
-  _DELETEBUILDREQUEST._serialized_end=1712
-  _DELETEBUILDRESPONSE._serialized_start=1714
-  _DELETEBUILDRESPONSE._serialized_end=1735
-  _GETTAGPATHREQUEST._serialized_start=1737
-  _GETTAGPATHREQUEST._serialized_end=1834
-  _GETTAGPATHRESPONSE._serialized_start=1836
-  _GETTAGPATHRESPONSE._serialized_end=1874
-  _BUILDAPI._serialized_start=2152
-  _BUILDAPI._serialized_end=3302
+  _PHASESTATUS._serialized_start=2012
+  _PHASESTATUS._serialized_end=2163
+  _FAILUREREASON._serialized_start=2165
+  _FAILUREREASON._serialized_end=2284
+  _REGISTERBUILDREQUEST._serialized_start=112
+  _REGISTERBUILDREQUEST._serialized_end=236
+  _REGISTERBUILDRESPONSE._serialized_start=238
+  _REGISTERBUILDRESPONSE._serialized_end=261
+  _UPDATEBUILDSTATUSREQUEST._serialized_start=263
+  _UPDATEBUILDSTATUSREQUEST._serialized_end=360
+  _UPDATEBUILDSTATUSRESPONSE._serialized_start=362
+  _UPDATEBUILDSTATUSRESPONSE._serialized_end=389
+  _REGISTEREXPERIMENTTRACKINGREQUEST._serialized_start=392
+  _REGISTEREXPERIMENTTRACKINGREQUEST._serialized_end=706
+  _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._serialized_start=613
+  _REGISTEREXPERIMENTTRACKINGREQUEST_PARAMSENTRY._serialized_end=658
+  _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._serialized_start=660
+  _REGISTEREXPERIMENTTRACKINGREQUEST_METRICSENTRY._serialized_end=706
+  _REGISTEREXPERIMENTTRACKINGRESPONSE._serialized_start=708
+  _REGISTEREXPERIMENTTRACKINGRESPONSE._serialized_end=744
+  _REGISTERMODELSCHEMAREQUEST._serialized_start=746
+  _REGISTERMODELSCHEMAREQUEST._serialized_end=846
+  _REGISTERMODELSCHEMARESPONSE._serialized_start=848
+  _REGISTERMODELSCHEMARESPONSE._serialized_end=877
+  _GETBUILDREQUEST._serialized_start=879
+  _GETBUILDREQUEST._serialized_end=914
+  _GETBUILDRESPONSE._serialized_start=916
+  _GETBUILDRESPONSE._serialized_end=975
+  _LISTBUILDSREQUEST._serialized_start=977
+  _LISTBUILDSREQUEST._serialized_end=1083
+  _LISTBUILDSRESPONSE._serialized_start=1085
+  _LISTBUILDSRESPONSE._serialized_end=1146
+  _REGISTERTAGSREQUEST._serialized_start=1148
+  _REGISTERTAGSREQUEST._serialized_end=1201
+  _REGISTERTAGSRESPONSE._serialized_start=1203
+  _REGISTERTAGSRESPONSE._serialized_end=1225
+  _LOGPHASESTATUSREQUEST._serialized_start=1228
+  _LOGPHASESTATUSREQUEST._serialized_end=1370
+  _LOGPHASESTATUSRESPONSE._serialized_start=1372
+  _LOGPHASESTATUSRESPONSE._serialized_end=1396
+  _GETPHASESTATUSESREQUEST._serialized_start=1398
+  _GETPHASESTATUSESREQUEST._serialized_end=1441
+  _PHASESTATUSLOG._serialized_start=1444
+  _PHASESTATUSLOG._serialized_end=1725
+  _GETPHASESTATUSESRESPONSE._serialized_start=1727
+  _GETPHASESTATUSESRESPONSE._serialized_end=1806
+  _DELETEBUILDREQUEST._serialized_start=1808
+  _DELETEBUILDREQUEST._serialized_end=1847
+  _DELETEBUILDRESPONSE._serialized_start=1849
+  _DELETEBUILDRESPONSE._serialized_end=1870
+  _GETTAGPATHREQUEST._serialized_start=1872
+  _GETTAGPATHREQUEST._serialized_end=1969
+  _GETTAGPATHRESPONSE._serialized_start=1971
+  _GETTAGPATHRESPONSE._serialized_end=2009
+  _BUILDAPI._serialized_start=2287
+  _BUILDAPI._serialized_end=3437
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import google.protobuf.timestamp_pb2
 import qwak.build.v1.build_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
@@ -355,27 +356,36 @@
 class PhaseStatusLog(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PHASE_ID_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     PHASE_DURATION_IN_SECONDS_FIELD_NUMBER: builtins.int
     POD_FAILURE_REASON_FIELD_NUMBER: builtins.int
+    CREATED_AT_FIELD_NUMBER: builtins.int
+    LAST_MODIFIED_AT_FIELD_NUMBER: builtins.int
     phase_id: builtins.str
     status: global___PhaseStatus.ValueType
     phase_duration_in_seconds: builtins.int
     pod_failure_reason: global___FailureReason.ValueType
+    @property
+    def created_at(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def last_modified_at(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     def __init__(
         self,
         *,
         phase_id: builtins.str = ...,
         status: global___PhaseStatus.ValueType = ...,
         phase_duration_in_seconds: builtins.int = ...,
         pod_failure_reason: global___FailureReason.ValueType = ...,
+        created_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        last_modified_at: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["phase_duration_in_seconds", b"phase_duration_in_seconds", "phase_id", b"phase_id", "pod_failure_reason", b"pod_failure_reason", "status", b"status"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "last_modified_at", b"last_modified_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["created_at", b"created_at", "last_modified_at", b"last_modified_at", "phase_duration_in_seconds", b"phase_duration_in_seconds", "phase_id", b"phase_id", "pod_failure_reason", b"pod_failure_reason", "status", b"status"]) -> None: ...
 
 global___PhaseStatusLog = PhaseStatusLog
 
 class GetPhaseStatusesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUSES_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.75/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.75/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/pyproject.toml` & `qwak_core-0.0.75/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.74"
+version = "0.0.75"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.74/qwak/automations/__init__.py` & `qwak_core-0.0.75/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/automations/automation_executions.py` & `qwak_core-0.0.75/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/automations/automations.py` & `qwak_core-0.0.75/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.75/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.75/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/automations/common.py` & `qwak_core-0.0.75/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.75/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.75/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.75/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.75/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.75/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/alert_management/client.py` & `qwak_core-0.0.75/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/analytics/client.py` & `qwak_core-0.0.75/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/audience/client.py` & `qwak_core-0.0.75/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/automation_management/client.py` & `qwak_core-0.0.75/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.75/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.75/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.75/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.75/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/build_management/client.py` & `qwak_core-0.0.75/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.75/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.75/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/deployment/client.py` & `qwak_core-0.0.75/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.75/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.75/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.75/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.75/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/instance_template/client.py` & `qwak_core-0.0.75/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.75/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/logging_client/client.py` & `qwak_core-0.0.75/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/model_management/client.py` & `qwak_core-0.0.75/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/project/client.py` & `qwak_core-0.0.75/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/secret_service/client.py` & `qwak_core-0.0.75/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.75/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.75/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.75/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.75/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.75/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.75/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.75/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.75/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.75/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.75/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.75/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.75/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.75/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.75/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.75/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/offline/client.py` & `qwak_core-0.0.75/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/feature_store/online/client.py` & `qwak_core-0.0.75/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/const.py` & `qwak_core-0.0.75/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.75/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.75/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.75/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.75/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/singleton_meta.py` & `qwak_core-0.0.75/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/tool/auth.py` & `qwak_core-0.0.75/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.75/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.75/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.75/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.75/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/adapters/__init__.py` & `qwak_core-0.0.75/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.75/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.75/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.75/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.75/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.75/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/base.py` & `qwak_core-0.0.75/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/decorators/api.py` & `qwak_core-0.0.75/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.75/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/experiment_tracking.py` & `qwak_core-0.0.75/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/schema.py` & `qwak_core-0.0.75/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/schema_entities.py` & `qwak_core-0.0.75/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.75/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.75/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.75/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.75/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.75/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.75/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.75/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.75/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/client.py` & `qwak_core-0.0.75/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.75/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/models/model.py` & `qwak_core-0.0.75/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.75/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.75/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/tools/logger/logger.py` & `qwak_core-0.0.75/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak/tools/logger/logging.yml` & `qwak_core-0.0.75/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.75/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/qwak_services_mock/services_mock.py` & `qwak_core-0.0.75/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.74/setup.py` & `qwak_core-0.0.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.74',
+    'version': '0.0.75',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.74/PKG-INFO` & `qwak_core-0.0.75/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.74
+Version: 0.0.75
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

