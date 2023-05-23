# Comparing `tmp/opentera-1.2.1.tar.gz` & `tmp/opentera-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentera-1.2.1.tar", last modified: Wed Apr 19 13:15:57 2023, max compression
+gzip compressed data, was "opentera-1.2.2.tar", last modified: Tue May 23 18:48:14 2023, max compression
```

## Comparing `opentera-1.2.1.tar` & `opentera-1.2.2.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.833879 opentera-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 13:14:34.000000 opentera-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 13:14:34.000000 opentera-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-19 13:15:57.833879 opentera-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 13:14:34.000000 opentera-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 13:15:02.000000 opentera-1.2.1/opentera/OpenTeraServerVersion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/config/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/crypto/crypto_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera/db/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12396 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/SoftDeleteMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/SoftDeleteQueryRewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/SoftInsertMixin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.821878 opentera-1.2.1/opentera/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraAsset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceParticipant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceSubType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraDeviceType.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraParticipant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraParticipantGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServerSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraService.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceConfigSpecific.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceRole.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraServiceSite.py
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSession.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionParticipants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionType.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionTypeSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSessionUsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTestType.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTestTypeProject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraTestTypeSite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13864 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUserPreference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/TeraUserUserGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/db/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.821878 opentera-1.2.1/opentera/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.825878 opentera-1.2.1/opentera/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraDeviceForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraDeviceSubTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraDeviceTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraParticipantForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraParticipantGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraProjectForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraServiceConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraServiceForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSessionForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSessionTypeConfigForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSessionTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraSiteForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraTestTypeForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraUserForm.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraUserGroupForm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/TeraVersionsForm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.825878 opentera-1.2.1/opentera/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/logging/LoggingClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.825878 opentera-1.2.1/opentera/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:35.000000 opentera-1.2.1/opentera/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/messages/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/CreateSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/DatabaseEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/DeviceEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/JoinSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/JoinSessionReplyEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/LeaveSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/LogEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/LoginEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/ParticipantEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/RPCMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/Result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/ServerCommand_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/StopSessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/TeraEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/TeraMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-19 13:15:51.000000 opentera-1.2.1/opentera/messages/python/TeraModuleMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-19 13:15:51.000000 opentera-1.2.1/opentera/messages/python/UserEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-19 13:15:50.000000 opentera-1.2.1/opentera/messages/python/UserRegisterToEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-19 13:14:35.000000 opentera-1.2.1/opentera/messages/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/modules/BaseModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/redis/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisProtocolFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisRPCClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/RedisVars.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/services/
--rw-r--r--   0 runner    (1001) docker     (123)    38393 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/BaseWebRTCService.py
--rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceAccessManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceOpenTera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceOpenTeraWithAssets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/ServiceOpenTeraWithTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraDeviceClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraParticipantClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraServiceClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/TeraUserClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/services/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/modules/WebRTCModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/services/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/Metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/TeraVersions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/UserAgentParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.829878 opentera-1.2.1/opentera/utils/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/AssetFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/AssetVideoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/BaseAsset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:14:34.000000 opentera-1.2.1/opentera/utils/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.817878 opentera-1.2.1/opentera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 13:15:57.000000 opentera-1.2.1/opentera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:15:57.833879 opentera-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 13:14:34.000000 opentera-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.813878 opentera-1.2.1/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.813878 opentera-1.2.1/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.833879 opentera-1.2.1/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 13:15:53.000000 opentera-1.2.1/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    71383 2023-04-19 13:14:34.000000 opentera-1.2.1/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.813878 opentera-1.2.1/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:15:57.833879 opentera-1.2.1/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    37867 2023-04-19 13:15:53.000000 opentera-1.2.1/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    88110 2023-04-19 13:14:34.000000 opentera-1.2.1/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 18:46:51.000000 opentera-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 18:46:51.000000 opentera-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-23 18:48:14.655590 opentera-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 18:46:51.000000 opentera-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 18:47:25.000000 opentera-1.2.2/opentera/OpenTeraServerVersion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/config/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/crypto/crypto_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.643590 opentera-1.2.2/opentera/db/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12396 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/SoftDeleteMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/SoftDeleteQueryRewriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/SoftInsertMixin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraAsset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceSubType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraDeviceType.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17755 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraParticipant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraParticipantGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServerSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceConfigSpecific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceRole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraServiceSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionParticipants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionTypeSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSessionUsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTestType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTestTypeProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraTestTypeSite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17164 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUserPreference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/TeraUserUserGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/db/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraDeviceForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraDeviceSubTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraDeviceTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraParticipantForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraParticipantGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraProjectForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraServiceConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraServiceForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSessionForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSessionTypeConfigForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSessionTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraSiteForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraTestTypeForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraUserForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraUserGroupForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/TeraVersionsForm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/logging/LoggingClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.647590 opentera-1.2.2/opentera/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.651589 opentera-1.2.2/opentera/messages/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/CreateSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/DatabaseEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/DeviceEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/JoinSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/JoinSessionReplyEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/LeaveSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/LogEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/LoginEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/ParticipantEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/RPCMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/Result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/ServerCommand_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/StopSessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/TeraEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/TeraMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/TeraModuleMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-23 18:48:07.000000 opentera-1.2.2/opentera/messages/python/UserEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-23 18:48:06.000000 opentera-1.2.2/opentera/messages/python/UserRegisterToEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/messages/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.651589 opentera-1.2.2/opentera/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/modules/BaseModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.651589 opentera-1.2.2/opentera/redis/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5734 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2896 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisProtocolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisRPCClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/RedisVars.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/services/
+-rw-r--r--   0 runner    (1001) docker     (123)    38393 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/BaseWebRTCService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/DisabledTokenStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceAccessManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceOpenTera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceOpenTeraWithAssets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/ServiceOpenTeraWithTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraDeviceClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraParticipantClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraServiceClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/TeraUserClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/services/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/modules/WebRTCModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/services/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/TeraVersions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/UserAgentParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/opentera/utils/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/AssetFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/AssetVideoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/BaseAsset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:46:51.000000 opentera-1.2.2/opentera/utils/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/opentera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 18:48:14.000000 opentera-1.2.2/opentera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:48:14.655590 opentera-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 18:46:51.000000 opentera-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-23 18:48:10.000000 opentera-1.2.2/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    76833 2023-05-23 18:46:51.000000 opentera-1.2.2/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.639589 opentera-1.2.2/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:48:14.655590 opentera-1.2.2/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39138 2023-05-23 18:48:10.000000 opentera-1.2.2/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    94200 2023-05-23 18:46:51.000000 opentera-1.2.2/translations/fr/LC_MESSAGES/messages.po
```

### Comparing `opentera-1.2.1/LICENSE` & `opentera-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/PKG-INFO` & `opentera-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.1
+Version: 1.2.2
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opentera-1.2.1/README.md` & `opentera-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/config/ConfigManager.py` & `opentera-1.2.2/opentera/config/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/crypto/crypto_utils.py` & `opentera-1.2.2/opentera/crypto/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/Base.py` & `opentera-1.2.2/opentera/db/Base.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/SoftDeleteMixin.py` & `opentera-1.2.2/opentera/db/SoftDeleteMixin.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,36 +9,51 @@
 
 from sqlalchemy import Column, DateTime, text
 from sqlalchemy.inspection import inspect
 from sqlalchemy.sql.type_api import TypeEngine
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from sqlalchemy.event import listens_for
 from sqlalchemy.orm import ORMExecuteState, Session
+from sqlalchemy.engine import Engine, Connection
+from sqlalchemy.sql import Select
 
 from functools import cache
 
 from opentera.db.SoftDeleteQueryRewriter import SoftDeleteQueryRewriter
 
 
 @cache
 def activate_soft_delete_hook(deleted_field_name: str, disable_soft_delete_option_name: str):
     """Activate an event hook to rewrite the queries."""
     # Enable Soft Delete on all Relationship Loads which implement SoftDeleteMixin
-    @listens_for(Session, "do_orm_execute")
-    def soft_delete_execute(state: ORMExecuteState):
-        if not state.is_select:
-            return
-        if 'include_deleted' in state.session.info and len(state.session.info['include_deleted']) > 0:
+    # @listens_for(Session, "do_orm_execute")
+    # def soft_delete_execute(state: ORMExecuteState):
+    #     if not state.is_select:
+    #         return
+    #     if 'include_deleted' in state.session.info and len(state.session.info['include_deleted']) > 0:
+    #         print('test_include_deleted')
+    #         return
+    #
+    #     adapted = SoftDeleteQueryRewriter(deleted_field_name, disable_soft_delete_option_name).rewrite_statement(
+    #         state.statement
+    #     )
+    #     state.statement = adapted
+    @listens_for(Engine, "before_execute", retval=True)
+    def soft_delete_execute(conn: Connection, clauseelement, multiparams, params, execution_options):
+        if not isinstance(clauseelement, Select):
+            return clauseelement, multiparams, params
+
+        if disable_soft_delete_option_name in execution_options and execution_options[disable_soft_delete_option_name]:
             print('test_include_deleted')
-            return
+            return clauseelement, multiparams, params
 
         adapted = SoftDeleteQueryRewriter(deleted_field_name, disable_soft_delete_option_name).rewrite_statement(
-            state.statement
+            clauseelement
         )
-        state.statement = adapted
+        return adapted, multiparams, params
 
 
 def generate_soft_delete_mixin_class(
     deleted_field_name: str = "deleted_at",
     class_name: str = "_SoftDeleteMixin",
     deleted_field_type: TypeEngine = DateTime(timezone=True),
     disable_soft_delete_filtering_option_name: str = "include_deleted",
```

### Comparing `opentera-1.2.1/opentera/db/SoftDeleteQueryRewriter.py` & `opentera-1.2.2/opentera/db/SoftDeleteQueryRewriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,18 @@
         # Normal cases - Tables
         if isinstance(join_obj.left, Table):
             stmt = self.rewrite_from_table(stmt, join_obj.left)
 
         if isinstance(join_obj.right, Table):
             stmt = self.rewrite_from_table(stmt, join_obj.right)
 
+        # SB - This happened when managing "lazy-joined" relationship
+        # if isinstance(join_obj.right, Alias) and isinstance(join_obj.left, Subquery):  # Lazy joins
+        #     stmt = self.analyze_from(stmt, join_obj.right)
+
         return stmt
 
     def analyze_from(self, stmt: Select, from_obj):
         """Analyze the FROMS of a Select to determine possible soft-delete rewritable tables."""
         if isinstance(from_obj, Table):
             return self.rewrite_from_table(stmt, from_obj)
 
@@ -119,14 +123,19 @@
 
         if isinstance(from_obj, TableClause) or isinstance(from_obj, TextClause):
             # TableClause/TextClause objects are raw text SQL identifiers and as such, we cannot
             # introspect or do anything about this statement.
             return stmt
 
         if isinstance(from_obj, Alias):
+            # SB - This happened when managing "lazy-joined" relationship
+            # if isinstance(from_obj.element, Table):
+            #     return self.rewrite_from_table(from_obj.element.select(), from_obj)
+            #     # return self.rewrite_element(from_obj.element)
+
             if isinstance(from_obj.element, Subquery):
                 self.rewrite_element(from_obj.element)
                 return stmt
 
             raise NotImplementedError(
                 f"Unsupported object \"{(type(from_obj.element))}\" inside Alias in " f"statement.froms"
             )
```

### Comparing `opentera-1.2.1/opentera/db/SoftInsertMixin.py` & `opentera-1.2.2/opentera/db/SoftInsertMixin.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraAsset.py` & `opentera-1.2.2/opentera/db/models/TeraAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraDevice.py` & `opentera-1.2.2/opentera/db/models/TeraDevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     device_infos = Column(String, nullable=True)
     device_notes = Column(String, nullable=True)
     device_lastonline = Column(TIMESTAMP(timezone=True), nullable=True)
 
     device_sites = relationship("TeraSite", secondary='t_devices_sites', back_populates='site_devices')
     # device_projects = relationship('TeraDeviceProject', cascade='delete')
     device_projects = relationship("TeraProject", secondary="t_devices_projects",
-                                   back_populates="project_devices", lazy='joined')
+                                   back_populates="project_devices", lazy='selectin')
     # device_session_types = relationship("TeraSessionTypeDeviceType")
     device_participants = relationship("TeraParticipant",  secondary="t_devices_participants",
                                        back_populates="participant_devices", passive_deletes=True)
     device_sessions = relationship("TeraSession", secondary="t_sessions_devices", back_populates="session_devices",
                                    passive_deletes=True)
     device_type = relationship('TeraDeviceType')
     device_subtype = relationship('TeraDeviceSubType')
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraDeviceParticipant.py` & `opentera-1.2.2/opentera/db/models/TeraDeviceParticipant.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraDeviceProject.py` & `opentera-1.2.2/opentera/db/models/TeraDeviceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraDeviceSite.py` & `opentera-1.2.2/opentera/db/models/TeraDeviceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraDeviceSubType.py` & `opentera-1.2.2/opentera/db/models/TeraDeviceSubType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraDeviceType.py` & `opentera-1.2.2/opentera/db/models/TeraDeviceType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraParticipant.py` & `opentera-1.2.2/opentera/db/models/TeraParticipant.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from sqlalchemy.exc import IntegrityError
 from opentera.db.models.TeraParticipantGroup import TeraParticipantGroup
 from opentera.db.models.TeraServerSettings import TeraServerSettings
 from opentera.db.models.TeraSessionParticipants import TeraSessionParticipants
 from opentera.db.models.TeraSession import TeraSession
 from opentera.db.models.TeraAsset import TeraAsset
 from opentera.db.models.TeraTest import TeraTest
+from opentera.db.models.TeraProject import TeraProject
 
 import uuid
 import jwt
 import datetime
 from passlib.hash import bcrypt
 
 
@@ -51,15 +52,15 @@
 
     participant_sessions = relationship("TeraSession", secondary="t_sessions_participants",
                                         back_populates="session_participants", passive_deletes=True)
 
     participant_participant_group = relationship("TeraParticipantGroup",
                                                  back_populates='participant_group_participants')
 
-    participant_project = relationship("TeraProject", back_populates='project_participants', lazy='joined')
+    participant_project = relationship("TeraProject", back_populates='project_participants', lazy='selectin')
 
     participant_created_sessions = relationship("TeraSession", cascade='delete',
                                                 back_populates='session_creator_participant', passive_deletes=True)
 
     participant_service_config = relationship("TeraServiceConfig", cascade='delete', passive_deletes=True)
 
     participant_assets = relationship("TeraAsset", cascade='delete', back_populates='asset_participant',
@@ -125,15 +126,18 @@
                               'participant_project', 'participant_participant_group', 'fullAccess',
                               'participant_created_sessions', 'participant_service_config'
                               ])
         if minimal:
             ignore_fields.extend(['participant_username', 'participant_lastonline',
                                   'participant_login_enabled', 'participant_token'])
 
-        return super().to_json(ignore_fields=ignore_fields)
+        participant_json = super().to_json(ignore_fields=ignore_fields)
+        if self.participant_project and not minimal:
+            participant_json['participant_project_enabled'] = self.participant_project.project_enabled
+        return participant_json
 
     def to_json_create_event(self):
         return self.to_json(minimal=True)
 
     def to_json_update_event(self):
         return self.to_json(minimal=True)
 
@@ -317,14 +321,20 @@
             # Create token with added participants, since we need to have the id_participant field set
             participant1.create_token()
             participant2.create_token()
             TeraParticipant.db().session.commit()
 
     @classmethod
     def update(cls, update_id: int, values: dict):
+        update_participant = TeraParticipant.get_participant_by_id(update_id)
+        # Check if participant is an enabled project
+        if 'participant_enabled' in values and values['participant_enabled'] and \
+                not update_participant.participant_project.project_enabled:
+            raise IntegrityError('Participant project disabled - no update allowed', update_id, 't_projects')
+
         # Check if username is available
         if 'participant_username' in values:
             if not TeraParticipant.is_participant_username_available(values['participant_username']):
                 raise NameError('Participant username already in use.')
 
         # Prevent changes on UUID
         if 'participant_uuid' in values:
@@ -336,15 +346,14 @@
                 del values['participant_password']
             else:
                 # Forcing password to string
                 values['participant_password'] = TeraParticipant.encrypt_password(str(values['participant_password']))
 
         # Check if we need to generate or delete tokens
         if 'participant_token_enabled' in values:
-            update_participant = TeraParticipant.get_participant_by_id(update_id)
             if values['participant_token_enabled'] != update_participant.participant_token_enabled:
                 if 'participant_enabled' in values:
                     participant_enabled = values['participant_enabled']
                 else:
                     participant_enabled = update_participant.participant_enabled
                 # Value changed
                 if not values['participant_token_enabled'] or not participant_enabled:
@@ -370,14 +379,19 @@
         if not TeraParticipant.is_participant_username_available(participant.participant_username):
             raise NameError('Participant username already in use.')
         super().insert(participant)
 
         # Token must be created after being inserted, since we need to have a valid ID participant into it
         if participant.participant_token_enabled and participant.participant_enabled:
             participant.create_token()
+
+        # Check if participant project is enabled
+        project = TeraProject.get_project_by_id(participant.id_project)
+        if not project or not project.project_enabled:
+            raise IntegrityError('Participant project disabled - no insert allowed', -1, 't_projects')
         TeraParticipant.db().session.commit()
 
     def delete_check_integrity(self) -> IntegrityError | None:
         # Safety check - can't delete participants with sessions
         if TeraSessionParticipants.get_session_count_for_participant(self.id_participant) > 0:
             return IntegrityError('Participant still has sessions', self.id_participant, 't_sessions_participants')
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraParticipantGroup.py` & `opentera-1.2.2/opentera/db/models/TeraParticipantGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraProject.py` & `opentera-1.2.2/opentera/db/models/TeraProject.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from opentera.db.Base import BaseModel
 from opentera.db.SoftDeleteMixin import SoftDeleteMixin
-from sqlalchemy import Column, ForeignKey, Integer, String, Sequence
+from sqlalchemy import Column, ForeignKey, Integer, String, Sequence, Boolean
 from sqlalchemy.orm import relationship
 from sqlalchemy.exc import IntegrityError
 
 
 class TeraProject(BaseModel, SoftDeleteMixin):
     __tablename__ = 't_projects'
     id_project = Column(Integer, Sequence('id_project_sequence'), primary_key=True, autoincrement=True)
     id_site = Column(Integer, ForeignKey('t_sites.id_site', ondelete='cascade'), nullable=False)
     project_name = Column(String, nullable=False, unique=False)
+    project_enabled = Column(Boolean, nullable=False, default=True)
+    project_description = Column(String, nullable=True)
 
     project_site = relationship("TeraSite", back_populates='site_projects')
     project_participants = relationship("TeraParticipant", cascade='delete', back_populates='participant_project',
                                         passive_deletes=True)
     project_participants_groups = relationship("TeraParticipantGroup", cascade='delete', passive_deletes=True)
     project_devices = relationship("TeraDevice", secondary="t_devices_projects", back_populates="device_projects")
     project_session_types = relationship("TeraSessionType", secondary="t_sessions_types_projects",
@@ -62,32 +64,32 @@
         return users_ids
 
     def get_users_in_project(self, include_superadmins=False, include_site_access=False, with_deleted: bool = False):
         import modules.Globals as Globals
         from opentera.db.models.TeraServiceAccess import TeraServiceAccess
         from opentera.db.models.TeraUser import TeraUser
         # Get all users who have a role in the project
-        project_access = TeraServiceAccess.get_service_access_for_project(id_service=Globals.opentera_service_id,
-                                                                          id_project=self.id_project,
-                                                                          with_deleted=with_deleted)
+        project_access = TeraServiceAccess.get_service_access(id_service=Globals.opentera_service_id,
+                                                              id_project=self.id_project,
+                                                              with_deleted=with_deleted)
 
         users = []
         for access in project_access:
             # Get all users in the related group
             if access.service_access_user_group:
                 access_users = access.service_access_user_group.user_group_users
                 for user in access_users:
                     if user not in users:
                         users.append(user)
 
         # Also appends users with site access but no direct access to project
         if include_site_access:
-            site_access = TeraServiceAccess.get_service_access_for_site(id_service=Globals.opentera_service_id,
-                                                                        id_site=self.id_site,
-                                                                        with_deleted=with_deleted)
+            site_access = TeraServiceAccess.get_service_access(id_service=Globals.opentera_service_id,
+                                                               id_site=self.id_site,
+                                                               with_deleted=with_deleted)
             for access in site_access:
                 if access.service_access_role.service_role_name == 'admin':
                     if access.service_access_user_group:
                         access_users = access.service_access_user_group.user_group_users
                         for user in access_users:
                             if user not in users:
                                 users.append(user)
@@ -117,40 +119,56 @@
             secret_project = TeraProject()
             secret_project.project_name = "Secret Project #1"
             secret_project.id_site = TeraSite.get_site_by_sitename('Top Secret Site').id_site
             TeraProject.insert(secret_project)
 
     @staticmethod
     def get_project_by_projectname(projectname, with_deleted: bool = False):
-        return TeraProject.query.execution_options(include_deleted=with_deleted)\
+        return TeraProject.query.execution_options(include_deleted=with_deleted) \
             .filter_by(project_name=projectname).first()
 
     @staticmethod
     def get_project_by_id(project_id, with_deleted: bool = False):
-        return TeraProject.query.execution_options(include_deleted=with_deleted)\
+        return TeraProject.query.execution_options(include_deleted=with_deleted) \
             .filter_by(id_project=project_id).first()
 
-    @staticmethod
-    def query_data(filter_args, with_deleted: bool = False):
-        if isinstance(filter_args, tuple):
-            return TeraProject.query.execution_options(include_deleted=with_deleted)\
-                .filter_by(*filter_args).all()
-        if isinstance(filter_args, dict):
-            return TeraProject.query.execution_options(include_deleted=with_deleted)\
-                .filter_by(**filter_args).all()
-        return None
+    # @staticmethod
+    # def query_data(filter_args, with_deleted: bool = False):
+    #     if isinstance(filter_args, tuple):
+    #         return TeraProject.query.execution_options(include_deleted=with_deleted)\
+    #             .filter_by(*filter_args).all()
+    #     if isinstance(filter_args, dict):
+    #         return TeraProject.query.execution_options(include_deleted=with_deleted)\
+    #             .filter_by(**filter_args).all()
+    #     return None
 
     def delete_check_integrity(self) -> IntegrityError | None:
         for participant in self.project_participants:
             cannot_be_deleted_exception = participant.delete_check_integrity()
             if cannot_be_deleted_exception:
                 return IntegrityError('Still have participants with session', self.id_project, 't_participants')
         return None
 
     @classmethod
+    def update(cls, update_id: int, values: dict):
+        # Update general infos
+        super().update(update_id, values)
+
+        # If project is inactive, disable all participants from that project
+        if 'project_enabled' in values and not values['project_enabled']:
+            from opentera.db.models.TeraDeviceParticipant import TeraDeviceParticipant
+            project = TeraProject.get_project_by_id(update_id)
+            for participant in project.project_participants:
+                participant.participant_enabled = False  # Set participant inactive
+                devices = TeraDeviceParticipant.query_devices_for_participant(participant.id_participant)
+                for device in devices:
+                    TeraDeviceParticipant.delete(device.id_device_participant)
+            cls.db().session.commit()
+
+    @classmethod
     def insert(cls, project):
         # Creates admin and user roles for that project
         super().insert(project)
 
         from opentera.db.models.TeraServiceRole import TeraServiceRole
         from opentera.db.models.TeraService import TeraService
         opentera_service_id = TeraService.get_openteraserver_service().id_service
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraServerSettings.py` & `opentera-1.2.2/opentera/db/models/TeraServerSettings.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraService.py` & `opentera-1.2.2/opentera/db/models/TeraService.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,30 +206,40 @@
         new_service.service_port = 4080
         new_service.service_endpoint = '/'
         new_service.service_clientendpoint = '/robot'
         new_service.service_enabled = True
         TeraService.db().session.add(new_service)
         TeraService.db().session.commit()
 
+    def to_json_create_event(self):
+        return self.to_json(minimal=False)
+
+    def to_json_update_event(self):
+        return self.to_json(minimal=False)
+
+    def to_json_delete_event(self):
+        # Minimal information, delete can not be filtered
+        return {'id_service': self.id_service, 'service_key': self.service_key}
+
     @classmethod
     def insert(cls, service):
         service.service_uuid = str(uuid.uuid4())
         super().insert(service)
 
         # Create default admin-user role for each service
-        from opentera.db.models.TeraServiceRole import TeraServiceRole
-        new_role = TeraServiceRole()
-        new_role.id_service = service.id_service
-        new_role.service_role_name = 'admin'
-        TeraServiceRole.insert(new_role)
-
-        new_role = TeraServiceRole()
-        new_role.id_service = service.id_service
-        new_role.service_role_name = 'user'
-        TeraServiceRole.insert(new_role)
+        # from opentera.db.models.TeraServiceRole import TeraServiceRole
+        # new_role = TeraServiceRole()
+        # new_role.id_service = service.id_service
+        # new_role.service_role_name = 'admin'
+        # TeraServiceRole.insert(new_role)
+        #
+        # new_role = TeraServiceRole()
+        # new_role.id_service = service.id_service
+        # new_role.service_role_name = 'user'
+        # TeraServiceRole.insert(new_role)
 
     def delete_check_integrity(self) -> IntegrityError | None:
         for service_site in self.service_sites:
             if service_site.delete_check_integrity():
                 return IntegrityError('Have sessions, assets or tests using that service', self.id_service,
                                       't_sessions')
         return None
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraServiceAccess.py` & `opentera-1.2.2/opentera/db/models/TeraServiceAccess.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from opentera.db.Base import BaseModel
 from opentera.db.SoftDeleteMixin import SoftDeleteMixin
 from opentera.db.SoftInsertMixin import SoftInsertMixin
-from sqlalchemy import Column, ForeignKey, Integer, String, Sequence, Boolean, TIMESTAMP
+from sqlalchemy import Column, ForeignKey, Integer, Sequence
 from sqlalchemy.orm import relationship
 from opentera.db.models.TeraServiceRole import TeraServiceRole
+import modules.Globals as Globals
 
 
 class TeraServiceAccess(BaseModel, SoftDeleteMixin, SoftInsertMixin):
     __tablename__ = 't_services_access'
     id_service_access = Column(Integer, Sequence('id_service_project_role_sequence'), primary_key=True,
                                autoincrement=True)
     id_user_group = Column(Integer, ForeignKey('t_users_groups.id_user_group', ondelete='cascade'),
@@ -50,14 +51,17 @@
         if not json_val['id_user_group']:
             del json_val['id_user_group']
 
         # Complete information if not minimal
         if not minimal:
             if self.service_access_role:
                 json_val['service_name'] = self.service_access_role.service_role_service.service_name
+                json_val['service_key'] = self.service_access_role.service_role_service.service_key
+                json_val['id_service'] = self.service_access_role.service_role_service.id_service
+                json_val['service_access_role_name'] = self.service_access_role.service_role_name
             # else:
             #     # This happens on transient objects
             #     from opentera.db.models.TeraService import TeraService
             #     service = TeraService.get_service_by_id(self.id_service)
             #     if service:
             #         json_val['service_name'] = service.service_name
             if self.id_user_group:
@@ -77,101 +81,99 @@
 
     @staticmethod
     def get_service_access_by_id(service_access_id: int, with_deleted: bool = False):
         return TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
             .filter_by(id_service_access=service_access_id).first()
 
     @staticmethod
-    def update_service_access_for_user_group_for_site(id_service: int, id_user_group: int, id_service_role: int,
-                                                      id_site: int):
+    def update_service_access_for_user_group(id_service: int, id_user_group: int, id_service_role: int,
+                                             id_site: int | None = None, id_project: int | None = None):
         # Check if access already exists
-        # access = TeraServiceAccess.get_specific_access_for_user_group(id_service=id_service,
-        #                                                               id_user_group=id_user_group,
-        #                                                               id_service_role=id_service_role)
-
-        access = TeraServiceAccess.get_service_access_for_user_group_for_site(id_service=id_service,
-                                                                              id_user_group=id_user_group,
-                                                                              id_site=id_site)
+        access = TeraServiceAccess.get_service_access_for_user_group(id_service=id_service,
+                                                                     id_user_group=id_user_group,
+                                                                     id_site=id_site,
+                                                                     id_project=id_project,
+                                                                     id_service_role=id_service_role)
 
-        if access is None:
+        if not access:
             # No access already present for that user group - create new one
             access = TeraServiceAccess()
             access.id_user_group = id_user_group
             access.id_service_role = id_service_role
             TeraServiceAccess.insert(access)
+            return access
         else:
             # Update it
-            access.id_service_role = id_service_role
-
+            access[0].id_service_role = id_service_role
             TeraServiceAccess.db().session.commit()
-        return access
+            return access[0]
 
     @staticmethod
-    def update_service_access_for_user_group_for_project(id_service: int, id_user_group: int, id_service_role: int,
-                                                         id_project: int):
-        # Check if access already exists
-        access = TeraServiceAccess.get_service_access_for_user_group_for_project(id_service=id_service,
-                                                                                 id_user_group=id_user_group,
-                                                                                 id_project=id_project)
+    def get_service_access_for_user_group(id_user_group: int, id_service: int, id_project: int | None = None,
+                                          id_site: int | None = None, id_service_role: int | None = None,
+                                          with_deleted: bool = False):
+        query = TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
+            .filter_by(id_user_group=id_user_group).join(TeraServiceRole).filter_by(id_service=id_service)
 
-        if access is None:
-            # No access already present for that user - create new one
-            access = TeraServiceAccess()
-            access.id_user_group = id_user_group
-            access.id_service_role = id_service_role
-            TeraServiceAccess.insert(access)
-        else:
-            # Update it
-            access.id_service_role = id_service_role
+        if id_project:
+            query = query.filter_by(id_project=id_project)
 
-            TeraServiceAccess.db().session.commit()
-        return access
+        if id_site:
+            query = query.filter_by(id_site=id_site)
 
-    @staticmethod
-    def get_service_access_for_user_group(id_service: int, id_user_group: int, with_deleted: bool = False):
-        return TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
-            .filter_by(id_user_group=id_user_group).join(TeraServiceRole)\
-            .filter_by(id_service=id_service).all()
+        if id_service_role and not id_site and not id_project:  # We search with id_service_role only if no project/site
+            query = query.filter_by(id_service_role=id_service_role)
 
-    @staticmethod
-    def get_service_access_for_project(id_service: int, id_project: int, with_deleted: bool = False):
-        return TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
-            .join(TeraServiceRole).filter_by(id_service=id_service, id_project=id_project).all()
+        return query.all()
 
     @staticmethod
-    def get_service_access_for_site(id_service: int, id_site: int, with_deleted: bool = False):
-        return TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
-            .join(TeraServiceRole).filter_by(id_service=id_service, id_site=id_site).all()
+    # Returns all access related to a service
+    def get_service_access(id_service: int, id_project: int | None = None, id_site: int | None = None,
+                           with_deleted: bool = False):
+        query = TeraServiceAccess.query.execution_options(include_deleted=with_deleted) \
+            .join(TeraServiceRole).filter_by(id_service=id_service)\
 
-    @staticmethod
-    def get_service_access_for_user_group_for_site(id_service: int, id_user_group: int, id_site: int,
-                                                   with_deleted: bool = False):
-        return TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
-            .join(TeraServiceRole).filter_by(id_service=id_service, id_site=id_site).filter(
-            TeraServiceAccess.id_user_group == id_user_group).first()
+        if id_site:
+            query = query.filter_by(id_site=id_site)
+        if id_project:
+            query = query.filter_by(id_project=id_project)
+
+        return query.all()
 
     @staticmethod
-    def get_service_access_for_user_group_for_project(id_service: int, id_user_group: int, id_project: int,
-                                                      with_deleted: bool = False):
-        return TeraServiceAccess.query.execution_options(include_deleted=with_deleted)\
-            .join(TeraServiceRole).filter_by(id_service=id_service, id_project=id_project).filter(
-            TeraServiceAccess.id_user_group == id_user_group).first()
+    def delete_service_access_for_user_group(id_service: int, id_user_group: int, id_site: int | None = None,
+                                             id_project: int | None = None, id_service_role: int | None = None):
+
+        for service_access in TeraServiceAccess.get_service_access_for_user_group(id_service=id_service,
+                                                                                  id_user_group=id_user_group,
+                                                                                  id_site=id_site,
+                                                                                  id_project=id_project):
+            if id_service_role and service_access.id_service_role == id_service_role:
+                TeraServiceAccess.delete(service_access.id_service_access)
+                return
+
+            if id_site and service_access.service_access_role.id_site == id_site:
+                TeraServiceAccess.delete(service_access.id_service_access)
+                return
+
+            if id_project and service_access.service_access_role.id_project == id_project:
+                TeraServiceAccess.delete(service_access.id_service_access)
+                return
 
+    # TODO: Delete those methods (replaced by the generic one)
     @staticmethod
     def delete_service_access_for_user_group_for_site(id_site: int, id_user_group: int):
-        import modules.Globals as Globals
         for service_access in TeraServiceAccess.get_service_access_for_user_group(
                 id_service=Globals.opentera_service_id, id_user_group=id_user_group):
             if service_access.service_access_role.id_site == id_site:
                 TeraServiceAccess.delete(service_access.id_service_access)
                 break
 
     @staticmethod
     def delete_service_access_for_user_group_for_project(id_project: int, id_user_group: int):
-        import modules.Globals as Globals
         for service_access in TeraServiceAccess.get_service_access_for_user_group(
                 id_service=Globals.opentera_service_id, id_user_group=id_user_group):
             if service_access.service_access_role.id_project == id_project:
                 TeraServiceAccess.delete(service_access.id_service_access)
                 break
 
     @staticmethod
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraServiceConfig.py` & `opentera-1.2.2/opentera/db/models/TeraServiceConfig.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraServiceConfigSpecific.py` & `opentera-1.2.2/opentera/db/models/TeraServiceConfigSpecific.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraServiceProject.py` & `opentera-1.2.2/opentera/db/models/TeraServiceProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraServiceRole.py` & `opentera-1.2.2/opentera/db/models/TeraServiceRole.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     service_role_name = Column(String(100), nullable=False)
 
     service_role_service = relationship("TeraService", viewonly=True)
     service_role_project = relationship('TeraProject', viewonly=True)
     service_role_site = relationship('TeraSite', viewonly=True)
 
     service_role_user_groups = relationship("TeraUserGroup", secondary="t_services_access",
-                                            back_populates="user_group_services_roles",  lazy='joined')
+                                            back_populates="user_group_services_roles",  lazy='selectin')
 
     def __init__(self):
         pass
 
     def __str__(self):
         return '<TeraServiceRole Service = ' + str(self.service_role_service.service_name) + ', Role = ' + \
                str(self.service_role_name) + ' >'
@@ -42,54 +42,68 @@
             ignore_fields.extend([])
 
         json_val = super().to_json(ignore_fields=ignore_fields)
 
         # Remove null values
         if not json_val['id_project']:
             del json_val['id_project']
+        else:
+            if not minimal:
+                json_val['project_name'] = self.service_role_project.project_name
+
         if not json_val['id_site']:
             del json_val['id_site']
         else:
             if not minimal:
                 json_val['site_name'] = self.service_role_site.site_name
 
+        if not minimal:
+            json_val['service_name'] = self.service_role_service.service_name
         return json_val
 
     @staticmethod
-    def get_service_roles(service_id: int, with_deleted: bool = False):
-        return TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
-            .filter_by(id_service=service_id).all()
+    def get_service_roles(service_id: int, globals_only: bool = False, with_deleted: bool = False):
+        query = TeraServiceRole.query.execution_options(include_deleted=with_deleted).filter_by(id_service=service_id)
+
+        if globals_only:
+            query = query.filter_by(id_site=None).filter_by(id_project=None)
+
+        return query.all()
 
     @staticmethod
     def get_service_roles_for_site(service_id: int, site_id: int, with_deleted: bool = False):
         return TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
             .filter_by(id_service=service_id, id_site=site_id).all()
 
     @staticmethod
-    def get_specific_service_role_for_site(service_id: int, site_id: int, rolename: str, with_deleted: bool = False):
-        return TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
-            .filter_by(id_service=service_id, id_site=site_id, service_role_name=rolename).first()
-
-    @staticmethod
     def get_service_roles_for_project(service_id: int, project_id: int, with_deleted: bool = False):
         return TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
             .filter_by(id_service=service_id, id_project=project_id).all()
 
     @staticmethod
-    def get_specific_service_role_for_project(service_id: int, project_id: int, rolename: str,
-                                              with_deleted: bool = False):
-        return TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
-            .filter_by(id_service=service_id, id_project=project_id, service_role_name=rolename).first()
-
-    @staticmethod
     def get_service_role_by_id(role_id: int, with_deleted: bool = False):
         return TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
             .filter_by(id_service_role=role_id).first()
 
     @staticmethod
+    def get_service_role_by_name(service_id: int, rolename: str, site_id: int | None = None,
+                                 project_id: int | None = None, with_deleted: bool = False):
+
+        query = TeraServiceRole.query.execution_options(include_deleted=with_deleted)\
+            .filter_by(id_service=service_id, service_role_name=rolename)
+
+        if site_id:
+            query = query.filter_by(id_site=site_id)
+
+        if project_id:
+            query = query.filter_by(id_project=project_id)
+
+        return query.first()
+
+    @staticmethod
     def create_defaults(test=False):
         from opentera.db.models.TeraService import TeraService
 
         for service in TeraService.query.all():
             if service.service_key != 'OpenTeraServer':  # Don't add global roles for TeraServer
                 new_role = TeraServiceRole()
                 new_role.id_service = service.id_service
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraServiceSite.py` & `opentera-1.2.2/opentera/db/models/TeraServiceSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSession.py` & `opentera-1.2.2/opentera/db/models/TeraSession.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,29 +33,29 @@
     session_start_datetime = Column(TIMESTAMP(timezone=True), nullable=False)
     session_duration = Column(Integer, nullable=False, default=0)
     session_status = Column(Integer, nullable=False)
     session_comments = Column(String, nullable=True)
     session_parameters = Column(String, nullable=True)
 
     session_participants = relationship("TeraParticipant", secondary="t_sessions_participants",
-                                        back_populates="participant_sessions", lazy="joined")
+                                        back_populates="participant_sessions", lazy="selectin")
     session_users = relationship("TeraUser", secondary="t_sessions_users", back_populates="user_sessions",
-                                 lazy="joined")
+                                 lazy="selectin")
     session_devices = relationship("TeraDevice", secondary="t_sessions_devices",
-                                   back_populates="device_sessions", lazy="joined")
+                                   back_populates="device_sessions", lazy="selectin")
 
     session_creator_user = relationship('TeraUser')
     session_creator_device = relationship('TeraDevice')
     session_creator_participant = relationship('TeraParticipant')
     session_creator_service = relationship('TeraService')
 
-    session_session_type = relationship('TeraSessionType', back_populates='session_type_sessions', lazy='joined')
+    session_session_type = relationship('TeraSessionType', back_populates='session_type_sessions', lazy='selectin')
     session_events = relationship('TeraSessionEvent', cascade="delete", back_populates='session_event_session')
-    session_assets = relationship('TeraAsset', cascade='delete', back_populates='asset_session')
-    session_tests = relationship('TeraTest', cascade='delete', back_populates='test_session')
+    session_assets = relationship('TeraAsset', cascade='delete', back_populates='asset_session', lazy='selectin')
+    session_tests = relationship('TeraTest', cascade='delete', back_populates='test_session', lazy='selectin')
 
     def to_json(self, ignore_fields=None, minimal=False):
         if ignore_fields is None:
             ignore_fields = []
 
         ignore_fields.extend(['session_participants', 'session_creator_user', 'session_creator_device',
                               'session_creator_participant', 'session_creator_service', 'session_session_type',
@@ -106,17 +106,19 @@
             rval['session_creator_participant_uuid'] = self.session_creator_participant.participant_uuid
         if self.session_creator_service:
             rval['session_creator_service'] = self.session_creator_service.service_name
             rval['session_creator_service_uuid'] = self.session_creator_service.service_uuid
 
         # Append session stats
         from opentera.db.models.TeraAsset import TeraAsset
-        from opentera.db.models.TeraTest import TeraTest
-        rval['session_assets_count'] = TeraAsset.get_count({'id_session': self.id_session})
-        rval['session_tests_count'] = TeraTest.get_count({'id_session': self.id_session})
+        # from opentera.db.models.TeraTest import TeraTest
+        # rval['session_assets_count'] = TeraAsset.get_count({'id_session': self.id_session})
+        rval['session_assets_count'] = len(self.session_assets)
+        # rval['session_tests_count'] = TeraTest.get_count({'id_session': self.id_session})
+        rval['session_tests_count'] = len(self.session_tests)
         return rval
 
     def to_json_create_event(self):
         return self.to_json(minimal=True)
 
     def to_json_update_event(self):
         return self.to_json(minimal=True)
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionDevices.py` & `opentera-1.2.2/opentera/db/models/TeraSessionDevices.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionEvent.py` & `opentera-1.2.2/opentera/db/models/TeraSessionEvent.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         CUSTOM_EVENT6 = 105
         CUSTOM_EVENT7 = 106
         CUSTOM_EVENT8 = 107
         CUSTOM_EVENT9 = 108
         CUSTOM_EVENT10 = 109
 
     __tablename__ = 't_sessions_events'
-    id_session_event = Column(Integer, Sequence('id_session_events_sequence'), primary_key=True,
-                                 autoincrement=True)
+    id_session_event = Column(Integer, Sequence('id_session_events_sequence'), primary_key=True, autoincrement=True)
     id_session = Column(Integer, ForeignKey('t_sessions.id_session', ondelete='cascade'), nullable=False)
     id_session_event_type = Column(Integer, nullable=False)
     session_event_datetime = Column(TIMESTAMP(timezone=True), nullable=False)
     session_event_text = Column(String, nullable=True)
     session_event_context = Column(String, nullable=True)
 
     session_event_session = relationship('TeraSession', back_populates='session_events')
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionParticipants.py` & `opentera-1.2.2/opentera/db/models/TeraSessionParticipants.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionType.py` & `opentera-1.2.2/opentera/db/models/TeraSessionType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionTypeProject.py` & `opentera-1.2.2/opentera/db/models/TeraSessionTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionTypeSite.py` & `opentera-1.2.2/opentera/db/models/TeraSessionTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSessionUsers.py` & `opentera-1.2.2/opentera/db/models/TeraSessionUsers.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraSite.py` & `opentera-1.2.2/opentera/db/models/TeraSite.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class TeraSite(BaseModel, SoftDeleteMixin):
     __tablename__ = 't_sites'
     id_site = Column(Integer, Sequence('id_site_sequence'), primary_key=True, autoincrement=True)
     site_name = Column(String, nullable=False)
 
     site_devices = relationship("TeraDevice", secondary="t_devices_sites", back_populates="device_sites")
     site_projects = relationship("TeraProject", cascade="delete", passive_deletes=True,
-                                 back_populates='project_site', lazy='joined')
+                                 back_populates='project_site', lazy='selectin')
 
     site_services_roles = relationship("TeraServiceRole", cascade='delete', passive_deletes=True)
 
     site_services = relationship("TeraService", secondary="t_services_sites", viewonly=True)
 
     site_sessions_types = relationship("TeraSessionType", secondary="t_sessions_types_sites", viewonly=True)
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraTest.py` & `opentera-1.2.2/opentera/db/models/TeraTest.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraTestType.py` & `opentera-1.2.2/opentera/db/models/TeraTestType.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraTestTypeProject.py` & `opentera-1.2.2/opentera/db/models/TeraTestTypeProject.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraTestTypeSite.py` & `opentera-1.2.2/opentera/db/models/TeraTestTypeSite.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraUser.py` & `opentera-1.2.2/opentera/db/models/TeraUser.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 from sqlalchemy.exc import IntegrityError
 from opentera.db.models.TeraSite import TeraSite
 from opentera.db.models.TeraProject import TeraProject
 from opentera.db.models.TeraSessionUsers import TeraSessionUsers
 from opentera.db.models.TeraSession import TeraSession
 from opentera.db.models.TeraTest import TeraTest
 from opentera.db.models.TeraAsset import TeraAsset
+from opentera.db.models.TeraServiceRole import TeraServiceRole
 
 
 from passlib.hash import bcrypt
 import uuid
 import datetime
 import json
+import time
+import jwt
 
 
 # Generator for jti
 def infinite_jti_sequence():
     num = 0
     while True:
         yield num
@@ -43,15 +46,15 @@
     user_notes = Column(String, nullable=True)
     user_lastonline = Column(TIMESTAMP(timezone=True), nullable=True)
     user_superadmin = Column(Boolean, nullable=False, default=False)
 
     # user_sites_access = relationship('TeraSiteAccess', cascade="all,delete")
     # user_projects_access = relationship("TeraProjectAccess", cascade="all,delete")
     user_user_groups = relationship("TeraUserGroup", secondary="t_users_users_groups",
-                                    back_populates="user_group_users", lazy='joined')
+                                    back_populates="user_group_users", passive_deletes=True)
     user_sessions = relationship("TeraSession", secondary="t_sessions_users", back_populates="session_users",
                                  passive_deletes=True)
 
     user_created_sessions = relationship("TeraSession", cascade='delete', back_populates='session_creator_user',
                                          passive_deletes=True)
 
     user_service_config = relationship("TeraServiceConfig", cascade='delete', passive_deletes=True)
@@ -79,34 +82,70 @@
     def to_json_update_event(self):
         return self.to_json(minimal=True)
 
     def to_json_delete_event(self):
         # Minimal information, delete can not be filtered
         return {'id_user': self.id_user, 'user_uuid': self.user_uuid}
 
-    def get_token(self, token_key: str, expiration=3600):
-        import time
-        import jwt
+    def get_token(self, token_key: str, expiration: int = 3600):
+        """
+        Generates a token for the user. The token will contain the following information:
+        - issue time (iat)
+        - expiration time (exp)
+        - issuer (iss)
+        - token id (jti)
+        - user_uuid (string, user's uuid)
+        - id_user (int, user's id)
+        - user_fullname (string, user's fullname)
+        - user_superadmin (boolean, true if user is superadmin)
+        - service_access dict containing all global services access in a dict of the form:
+            {'service_access': {'service_key': ['access1', 'access2']}}
+
+        :param token_key: Key to use to generate the token
+        :param expiration: Expiration time in seconds
+        """
 
         # Creating token with user info
         now = time.time()
 
         payload = {
             'iat': int(now),
             'exp': int(now) + expiration,
             'iss': 'TeraServer',
             'jti': next(user_jti_generator),
             'user_uuid': self.user_uuid,
             'id_user': self.id_user,
             'user_fullname': self.get_fullname(),
-            'user_superadmin': self.user_superadmin
+            'user_superadmin': self.user_superadmin,
+            'service_access': self.get_service_access_dict()
         }
 
         return jwt.encode(payload, token_key, algorithm='HS256')
 
+    def get_service_access_dict(self):
+        service_access = {'service_access': {}}
+
+        # Service access are defined in user groups, not needed for superadmin
+        if not self.user_superadmin:
+            for user_group in self.user_user_groups:
+                for service_role in user_group.user_group_services_roles:
+                    service = service_role.service_role_service
+                    role_name = service_role.service_role_name
+                    service_key = service.service_key
+
+                    if service_role.id_site is None and service_role.id_project is None:
+                        # Global access
+                        # Create entry if not exists
+                        if service_key not in service_access['service_access']:
+                            service_access['service_access'][service_key] = []
+                        # Add role to service
+                        service_access['service_access'][service_key].append(role_name)
+
+        return service_access
+
     def get_fullname(self):
         return self.user_firstname + ' ' + self.user_lastname
 
     def is_authenticated(self):
         return self.authenticated
 
     def is_anonymous(self):
@@ -124,62 +163,96 @@
 
     def __str__(self):
         return '<TeraUser ' + str(self.user_username) + ', ' + str(self.user_email) + ' >'
 
     def __repr__(self):
         return self.__str__()
 
-    def get_sites_roles(self) -> dict:
+    def get_sites_roles(self, id_service: int | None = None) -> dict:
         sites_roles = {}
 
         if self.user_superadmin:
             # Super admin - admin role in all sites
-            sites = TeraSite.query.all()
+            if not id_service:
+                sites = TeraSite.query.all()
+            else:
+                all_roles = TeraServiceRole.get_service_roles(service_id=id_service)
+                sites = []
+                for role in all_roles:
+                    if role.id_site:
+                        sites.append(role.service_role_site)
+
             for site in sites:
                 sites_roles[site] = {'site_role': 'admin', 'inherited': True}
             return sites_roles
 
         # Browse all user groups to get roles for those sites
         for user_group in self.user_user_groups:
-            user_group_roles = user_group.get_sites_roles()
+            user_group_roles = user_group.get_sites_roles(service_id=id_service)
             for site, site_role in user_group_roles.items():
                 if site not in sites_roles:
                     # Site not already present
                     sites_roles[site] = site_role
                 else:
                     # Site present - check if we have an "admin" role to overwrite an "user" role
                     if site_role['site_role'] == 'admin':
                         sites_roles[site] = site_role
 
         return sites_roles
 
-    def get_projects_roles(self) -> dict:
+    def get_projects_roles(self, id_service: int | None = None) -> dict:
         projects_roles = {}
 
         if self.user_superadmin:
             # Super admin - admin role in all projects
-            projects = TeraProject.query.all()
+            if not id_service:
+                projects = TeraProject.query.all()
+            else:
+                all_roles = TeraServiceRole.get_service_roles(service_id=id_service)
+                projects = []
+                for role in all_roles:
+                    if role.id_project:
+                        projects.append(role.service_role_project)
+
             for project in projects:
                 projects_roles[project] = {'project_role': 'admin', 'inherited': True}
             return projects_roles
 
         # Browse all user groups to get roles for those projects
         for user_group in self.user_user_groups:
-            user_group_roles = user_group.get_projects_roles()
+            user_group_roles = user_group.get_projects_roles(service_id=id_service)
             for project, project_role in user_group_roles.items():
                 if project not in projects_roles:
                     # Project not already present
                     projects_roles[project] = project_role
                 else:
                     # Project present - check if we have an "admin" role to overwrite an "user" role
                     if project_role['project_role'] == 'admin':
                         projects_roles[project] = project_role
 
         return projects_roles
 
+    def get_service_roles(self, id_service: int) -> list:
+        service_roles = []
+
+        if self.user_superadmin:
+            # Super admin - has all service roles
+            all_roles = TeraServiceRole.get_service_roles(service_id=id_service, globals_only=True)
+            for role in all_roles:
+                service_roles.append(role.service_role_name)
+        else:
+            # Browse all user groups to get roles
+            for user_group in self.user_user_groups:
+                user_group_roles = user_group.get_global_roles(service_id=id_service)
+                for role in user_group_roles:
+                    if role not in service_roles:
+                        service_roles.append(role)
+
+        return service_roles
+
     @staticmethod
     def encrypt_password(password):
         return bcrypt.hash(password)
 
     @staticmethod
     def verify_password(username, password, user=None):
         # Query User with that username
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraUserGroup.py` & `opentera-1.2.2/opentera/db/models/TeraUserGroup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,50 +38,70 @@
     def to_json_update_event(self):
         return self.to_json(minimal=True)
 
     def to_json_delete_event(self):
         # Minimal information, delete can not be filtered
         return {'id_user_group': self.id_user_group}
 
-    def get_projects_roles(self, no_inheritance: bool = False) -> dict:
+    def get_projects_roles(self,  service_id: int | None = None, no_inheritance: bool = False) -> dict:
         projects_roles = {}
 
         # Projects
         for service_role in self.user_group_services_roles:
+            if service_id and service_role.id_service != service_id:
+                # Need to limit to a specific service and this is not one for that
+                continue
             if service_role.id_project:
                 projects_roles[service_role.service_role_project] = \
                     {'project_role': service_role.service_role_name, 'inherited': False}
 
         # Sites - if we are admin in a site, we are automatically admin in all its project
         if not no_inheritance:
             for service_role in self.user_group_services_roles:
+                if service_id and service_role.id_service != service_id:
+                    # Need to limit to a specific service and this is not one for that
+                    continue
                 if service_role.id_site:
                     if service_role.service_role_name == 'admin':
                         for project in service_role.service_role_site.site_projects:
                             projects_roles[project] = {'project_role': 'admin', 'inherited': True}
 
         return projects_roles
 
-    def get_sites_roles(self) -> dict:
+    def get_sites_roles(self, service_id: int | None = None) -> dict:
         sites_roles = {}
         # Sites
         for service_role in self.user_group_services_roles:
+            if service_id and service_role.id_service != service_id:
+                # Need to limit to a specific service and this is not one for that
+                continue
             if service_role.id_site:
                 sites_roles[service_role.service_role_site] = \
                     {'site_role': service_role.service_role_name, 'inherited': False}
 
         # Projects - each project's site also provides a "user" access for that site
         for service_role in self.user_group_services_roles:
+            if service_id and service_role.id_service != service_id:
+                # Need to limit to a specific service and this is not one for that
+                continue
             if service_role.id_project:
                 project_site = service_role.service_role_project.project_site
                 if project_site not in sites_roles:
                     sites_roles[project_site] = {'site_role': 'user', 'inherited': True}
 
         return sites_roles
 
+    def get_global_roles(self, service_id: int) -> list:
+        global_roles = []
+
+        for service_role in self.user_group_services_roles:
+            if not service_role.id_site and not service_role.id_project and service_role.id_service == service_id:
+                global_roles.append(service_role.service_role_name)
+        return global_roles
+
     @staticmethod
     def get_user_group_by_group_name(name: str, with_deleted: bool = False):
         return TeraUserGroup.query.execution_options(include_deleted=with_deleted)\
             .filter_by(user_group_name=name).first()
 
     @staticmethod
     def get_user_group_by_id(group_id: int, with_deleted: bool = False):
@@ -121,50 +141,49 @@
 
             TeraUserGroup.db().session.commit()
 
             id_user_group = TeraUserGroup.get_user_group_by_group_name('Users - Projects 1 & 2').id_user_group
             access = TeraServiceAccess()
             access.id_user_group = id_user_group
             id_project = TeraProject.get_project_by_projectname('Default Project #1').id_project
-            user_role = TeraServiceRole.get_specific_service_role_for_project(service_id=opentera_service_id,
-                                                                              project_id=id_project, rolename='user')
+            user_role = TeraServiceRole.get_service_role_by_name(service_id=opentera_service_id, project_id=id_project,
+                                                                 rolename='user')
             access.id_service_role = user_role.id_service_role
             TeraUserGroup.db().session.add(access)
 
             access = TeraServiceAccess()
             access.id_user_group = id_user_group
             id_project = TeraProject.get_project_by_projectname('Default Project #2').id_project
-            user_role = TeraServiceRole.get_specific_service_role_for_project(service_id=opentera_service_id,
-                                                                              project_id=id_project, rolename='user')
+            user_role = TeraServiceRole.get_service_role_by_name(service_id=opentera_service_id, project_id=id_project,
+                                                                 rolename='user')
             access.id_service_role = user_role.id_service_role
             TeraUserGroup.db().session.add(access)
 
             admin_access = TeraServiceAccess()
-            admin_role = TeraServiceRole.get_specific_service_role_for_site(service_id=opentera_service_id,
-                                                                            site_id=TeraSite
-                                                                            .get_site_by_sitename('Default Site')
-                                                                            .id_site,
-                                                                            rolename='admin')
+            admin_role = TeraServiceRole.get_service_role_by_name(service_id=opentera_service_id,
+                                                                  site_id=TeraSite.get_site_by_sitename('Default Site')
+                                                                  .id_site,
+                                                                  rolename='admin')
             admin_access.id_service_role = admin_role.id_service_role
             admin_access.id_user_group = \
                 TeraUserGroup.get_user_group_by_group_name('Admins - Default Site').id_user_group
             TeraUserGroup.db().session.add(admin_access)
 
             access = TeraServiceAccess()
             access.id_user_group = TeraUserGroup.get_user_group_by_group_name('Admins - Project 1').id_user_group
             id_project = TeraProject.get_project_by_projectname('Default Project #1').id_project
-            admin_role = TeraServiceRole.get_specific_service_role_for_project(service_id=opentera_service_id,
-                                                                               project_id=id_project, rolename='admin')
+            admin_role = TeraServiceRole.get_service_role_by_name(service_id=opentera_service_id, project_id=id_project,
+                                                                  rolename='admin')
             access.id_service_role = admin_role.id_service_role
             TeraUserGroup.db().session.add(access)
 
             access = TeraServiceAccess()
             access.id_user_group = TeraUserGroup.get_user_group_by_group_name('Users - Project 1').id_user_group
-            user_role = TeraServiceRole.get_specific_service_role_for_project(service_id=opentera_service_id,
-                                                                              project_id=id_project, rolename='user')
+            user_role = TeraServiceRole.get_service_role_by_name(service_id=opentera_service_id, project_id=id_project,
+                                                                 rolename='user')
             access.id_service_role = user_role.id_service_role
             TeraUserGroup.db().session.add(access)
 
             TeraUserGroup.db().session.commit()
 
     def delete_check_integrity(self) -> IntegrityError | None:
         if len(self.user_group_users) > 0:
```

### Comparing `opentera-1.2.1/opentera/db/models/TeraUserPreference.py` & `opentera-1.2.2/opentera/db/models/TeraUserPreference.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/TeraUserUserGroup.py` & `opentera-1.2.2/opentera/db/models/TeraUserUserGroup.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/db/models/__init__.py` & `opentera-1.2.2/opentera/db/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     TeraProject.get_model_name(): TeraProject,
     TeraSession.get_model_name(): TeraSession,
     TeraSessionType.get_model_name(): TeraSessionType,
     TeraSite.get_model_name(): TeraSite,
     TeraUser.get_model_name(): TeraUser,
     TeraUserGroup.get_model_name(): TeraUserGroup,
     TeraTestType.get_model_name(): TeraTestType,
-    TeraTest.get_model_name(): TeraTest
+    TeraTest.get_model_name(): TeraTest,
+    TeraService.get_model_name(): TeraService
 }
 
 # All exported symbols
 __all__ = ['TeraAsset',
            'TeraDevice',
            'TeraDeviceParticipant',
            'TeraDeviceProject',
```

### Comparing `opentera-1.2.1/opentera/forms/TeraDeviceForm.py` & `opentera-1.2.2/opentera/forms/TeraDeviceForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         section.add_item(TeraFormItem("device_uuid", gettext("Device UUID"), "hidden", item_required=True))
         section.add_item(TeraFormItem("device_name", gettext("Device Name"), "text", item_required=True))
         section.add_item(TeraFormItem("id_device_type", gettext("Device Type ID"), "array", item_required=True,
                                       item_values=device_types_list))
         section.add_item(TeraFormItem("id_device_subtype", gettext("Device Sub-Type"), "array", item_required=False,
                                       item_condition=TeraFormItemCondition("id_device_type", "=", "changed",
                                                                            "/api/user/devicesubtypes?id_device_type=")))
-        section.add_item(TeraFormItem("device_token", gettext("Access Token"), "label",
+        section.add_item(TeraFormItem("device_token", gettext("Access Token"), "longlabel",
                                       item_options={"readonly": False}))
         section.add_item(TeraFormItem("device_certificate", gettext("Certificate"), "hidden",
                                       item_options={"readonly": True}))
         section.add_item(TeraFormItem("device_enabled", gettext("Device Enabled?"), "boolean", item_required=True))
         section.add_item(TeraFormItem("device_onlineable", gettext("Device Onlineable?"), "boolean",
                                       item_required=True))
```

### Comparing `opentera-1.2.1/opentera/forms/TeraDeviceSubTypeForm.py` & `opentera-1.2.2/opentera/forms/TeraDeviceSubTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraDeviceTypeForm.py` & `opentera-1.2.2/opentera/forms/TeraDeviceTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraForm.py` & `opentera-1.2.2/opentera/forms/TeraForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraParticipantForm.py` & `opentera-1.2.2/opentera/forms/TeraParticipantForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraParticipantGroupForm.py` & `opentera-1.2.2/opentera/forms/TeraParticipantGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraProjectForm.py` & `opentera-1.2.2/opentera/forms/TeraProjectForm.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,21 @@
             sites_list.append(TeraFormValue(value_id=site.id_site, value=site.site_name))
 
         # Sections
         section = TeraFormSection("informations", gettext("Information"))
         form.add_section(section)
 
         # Items
-        section.add_item(TeraFormItem("id_project", gettext("Project ID"), "hidden", True))
-        section.add_item(TeraFormItem("project_name", gettext("Project Name"), "text", True))
-        section.add_item(TeraFormItem("id_site", gettext("Site"), "array", True, item_values=sites_list))
+        section.add_item(TeraFormItem("id_project", gettext("Project ID"), "hidden", item_required=True))
+        section.add_item(TeraFormItem("project_name", gettext("Project Name"), "text", item_required=True))
+        section.add_item(TeraFormItem("project_enabled", gettext("Enabled"), "boolean", item_required=True,
+                                      item_default=True))
+        section.add_item(TeraFormItem("id_site", gettext("Site"), "array", item_required=True, item_values=sites_list))
         section.add_item(TeraFormItem("project_role", gettext("Role"), "hidden"))
         section.add_item(TeraFormItem("site_name", gettext("Site Name"), "hidden"))
 
+        desc_section = TeraFormSection("description", gettext("Description"))
+        form.add_section(desc_section)
+        desc_section.add_item(TeraFormItem("project_description", gettext("Description"), "longtext",
+                                           item_required=False))
+
         return form.to_dict()
```

### Comparing `opentera-1.2.1/opentera/forms/TeraServiceConfigForm.py` & `opentera-1.2.2/opentera/forms/TeraServiceConfigForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraServiceForm.py` & `opentera-1.2.2/opentera/forms/TeraServiceForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraSessionForm.py` & `opentera-1.2.2/opentera/forms/TeraSessionForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         for st in ses_types:
             st_list.append(TeraFormValue(value_id=st.id_session_type, value=st.session_type_name))
 
         # Users
         if not project_info:
             users = user_access.get_accessible_users()
         else:
-            users = project_info.get_users_in_project(include_site_access=True)
+            users = project_info.get_users_in_project(include_superadmins=True, include_site_access=True)
 
         users_list = []
         users_ids = []
         for user in users:
             users_list.append(TeraFormValue(value_id=user.id_user, value=user.get_fullname()))
             users_ids.append(user.id_user)
```

### Comparing `opentera-1.2.1/opentera/forms/TeraSessionTypeForm.py` & `opentera-1.2.2/opentera/forms/TeraSessionTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraSiteForm.py` & `opentera-1.2.2/opentera/forms/TeraSiteForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraTestTypeForm.py` & `opentera-1.2.2/opentera/forms/TeraTestTypeForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraUserForm.py` & `opentera-1.2.2/opentera/forms/TeraUserForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraUserGroupForm.py` & `opentera-1.2.2/opentera/forms/TeraUserGroupForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/forms/TeraVersionsForm.py` & `opentera-1.2.2/opentera/forms/TeraVersionsForm.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/logging/LoggingClient.py` & `opentera-1.2.2/opentera/logging/LoggingClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/CreateSession_pb2.py` & `opentera-1.2.2/opentera/messages/python/CreateSession_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/DatabaseEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/DatabaseEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/DeviceEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/DeviceEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/JoinSessionEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/JoinSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/JoinSessionReplyEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/JoinSessionReplyEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/LeaveSessionEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/LeaveSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/LogEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/LogEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/LoginEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/LoginEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/ParticipantEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/ParticipantEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/RPCMessage_pb2.py` & `opentera-1.2.2/opentera/messages/python/RPCMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/Result_pb2.py` & `opentera-1.2.2/opentera/messages/python/Result_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/ServerCommand_pb2.py` & `opentera-1.2.2/opentera/messages/python/ServerCommand_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/StopSessionEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/StopSessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/TeraEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/TeraEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/TeraMessage_pb2.py` & `opentera-1.2.2/opentera/messages/python/TeraMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/TeraModuleMessage_pb2.py` & `opentera-1.2.2/opentera/messages/python/TeraModuleMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/UserEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/UserEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/UserRegisterToEvent_pb2.py` & `opentera-1.2.2/opentera/messages/python/UserRegisterToEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/messages/python/__init__.py` & `opentera-1.2.2/opentera/messages/python/__init__.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/modules/BaseModule.py` & `opentera-1.2.2/opentera/modules/BaseModule.py`

 * *Files 16% similar despite different names*

```diff
@@ -190,8 +190,27 @@
         module_message.head.source = src
         module_message.head.dest = dest
         return module_message
 
     def source_name(self):
         return "module." + self.module_name + ".messages"
 
+    def _send_disconnect_module_message(self, uuid: str):
+        module_message = self.create_module_message(
+            src='module.' + self.module_name + '.messages',
+            dest=create_module_event_topic_from_name(ModuleNames.TWISTED_MODULE_NAME, uuid)
+        )
+        server_command = messages.ServerCommand()
+        server_command.type = messages.ServerCommand.CMD_CLIENT_DISCONNECT
+        command_message = messages.Any()
+        command_message.Pack(server_command)
+        module_message.data.extend([command_message])
+        self.send_module_message(module_message)
 
+    def send_user_disconnect_module_message(self, user_uuid: str):
+        self._send_disconnect_module_message(user_uuid)
+
+    def send_participant_disconnect_module_message(self, participant_uuid: str):
+        self._send_disconnect_module_message(participant_uuid)
+
+    def send_device_disconnect_module_message(self, device_uuid: str):
+        self._send_disconnect_module_message(device_uuid)
```

### Comparing `opentera-1.2.1/opentera/redis/RedisClient.py` & `opentera-1.2.2/opentera/redis/RedisClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/redis/RedisProtocolFactory.py` & `opentera-1.2.2/opentera/redis/RedisProtocolFactory.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/redis/RedisRPCClient.py` & `opentera-1.2.2/opentera/redis/RedisRPCClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/redis/RedisVars.py` & `opentera-1.2.2/opentera/redis/RedisVars.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/services/BaseWebRTCService.py` & `opentera-1.2.2/opentera/services/BaseWebRTCService.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/services/ServiceAccessManager.py` & `opentera-1.2.2/opentera/services/ServiceAccessManager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from werkzeug.local import LocalProxy
 from functools import wraps
 from flask import _request_ctx_stack, request
 from flask_restx import reqparse
-
+from typing import List
 from enum import Enum
-
+from flask_babel import gettext
 import jwt
 
 from opentera.services.TeraUserClient import TeraUserClient
 from opentera.services.TeraDeviceClient import TeraDeviceClient
 from opentera.services.TeraParticipantClient import TeraParticipantClient
 from opentera.services.TeraServiceClient import TeraServiceClient
+from opentera.services.DisabledTokenStorage import DisabledTokenStorage
 from opentera.utils.UserAgentParser import UserAgentParser
+from opentera.redis.RedisVars import RedisVars
 import opentera.messages.python as messages
 
 # Current client identity, stacked
 current_user_client = LocalProxy(lambda: getattr(_request_ctx_stack.top, 'current_user_client', None))
 current_device_client = LocalProxy(lambda: getattr(_request_ctx_stack.top, 'current_device_client', None))
 current_participant_client = LocalProxy(lambda: getattr(_request_ctx_stack.top, 'current_participant_client', None))
 current_service_client = LocalProxy(lambda: getattr(_request_ctx_stack.top, 'current_service_client', None))
-
-
 current_login_type = LocalProxy(lambda: getattr(_request_ctx_stack.top, 'current_login_type', LoginType.UNKNOWN_LOGIN))
 
 
 class LoginType(Enum):
     UNKNOWN_LOGIN = 0,
     USER_LOGIN = 1,
     DEVICE_LOGIN = 2,
@@ -39,14 +39,59 @@
     api_participant_static_token_key = None
     api_device_token_key = None
     api_device_static_token_key = None
     api_service_token_key = None
     token_cookie_name = 'OpenTera'
     service = None
 
+    # Only user & participant tokens expire (for now)
+    __user_disabled_token_storage = DisabledTokenStorage(redis_key='user_disabled_tokens')
+    __participant_disabled_token_storage = DisabledTokenStorage(redis_key='participant_disabled_tokens')
+
+    @staticmethod
+    def init_access_manager(service):
+        # Set service
+        ServiceAccessManager.service = service
+
+        # Update Service Access information
+        ServiceAccessManager.api_user_token_key = \
+            service.redisGet(RedisVars.RedisVar_UserTokenAPIKey)
+        ServiceAccessManager.api_participant_token_key = \
+            service.redisGet(RedisVars.RedisVar_ParticipantTokenAPIKey)
+        ServiceAccessManager.api_participant_static_token_key = \
+            service.redisGet(RedisVars.RedisVar_ParticipantStaticTokenAPIKey)
+        ServiceAccessManager.api_device_token_key = \
+            service.redisGet(RedisVars.RedisVar_DeviceTokenAPIKey)
+        ServiceAccessManager.api_device_static_token_key = \
+            service.redisGet(RedisVars.RedisVar_DeviceStaticTokenAPIKey)
+        ServiceAccessManager.api_service_token_key = \
+            service.redisGet(RedisVars.RedisVar_ServiceTokenAPIKey)
+
+        # Update Token Storage information
+        ServiceAccessManager.__user_disabled_token_storage.config(
+            service.config_man, ServiceAccessManager.api_user_token_key)
+        ServiceAccessManager.__participant_disabled_token_storage.config(
+            service.config_man, ServiceAccessManager.api_participant_token_key)
+
+    @staticmethod
+    def user_add_disabled_token(token):
+        return ServiceAccessManager.__user_disabled_token_storage.add_disabled_token(token)
+
+    @staticmethod
+    def is_user_token_disabled(token):
+        return ServiceAccessManager.__user_disabled_token_storage.is_disabled_token(token)
+
+    @staticmethod
+    def participant_add_disabled_token(token):
+        return ServiceAccessManager.__participant_disabled_token_storage.add_disabled_token(token)
+
+    @staticmethod
+    def is_participant_token_disabled(token):
+        return ServiceAccessManager.__participant_disabled_token_storage.is_disabled_token(token)
+
     @staticmethod
     def token_required(allow_dynamic_tokens=True, allow_static_tokens=False):
         def wrap(f):
             def decorated(*args, **kwargs):
                 # We support 3 authentication scheme: token in url, cookie and authorization header
                 token = None
                 login_infos = UserAgentParser.parse_request_for_login_infos(request)
@@ -64,15 +109,15 @@
                             level=messages.LogEvent.LOGLEVEL_ERROR,
                             login_type=messages.LoginEvent.LOGIN_TYPE_TOKEN,
                             login_status=messages.LoginEvent.LOGIN_STATUS_FAILED_WITH_INVALID_TOKEN,
                             client_name=login_infos['client_name'], client_version=login_infos['client_version'],
                             client_ip=login_infos['client_ip'], os_name=login_infos['os_name'],
                             os_version=login_infos['os_version'], server_endpoint=login_infos['server_endpoint'],
                             service_uuid=ServiceAccessManager.service.service_uuid)
-                        return 'Forbidden', 403
+                        return gettext('Forbidden'), 403
 
                     # Verify scheme and token
                     if scheme == 'OpenTera':
                         token = atoken
                 if token is None:
                     #################
                     # TOKEN PARAMETER ?
@@ -90,15 +135,15 @@
                     # COOKIE TOKEN
                     if ServiceAccessManager.token_cookie_name in request.cookies:
                         token = request.cookies[ServiceAccessManager.token_cookie_name]
 
                 #########################
                 # Verify token from redis
                 # USER TOKEN MANAGEMENT
-                if allow_dynamic_tokens: # User only use dynamic tokens, don't validate otherwise
+                if allow_dynamic_tokens:  # User only use dynamic tokens, don't validate otherwise
                     if ServiceAccessManager.validate_user_token(token=token):
                         return f(*args, **kwargs)
 
                 # DEVICE TOKEN MANAGEMENT
                 if ServiceAccessManager.validate_device_token(token=token, allow_dynamic_tokens=allow_dynamic_tokens,
                                                               allow_static_tokens=allow_static_tokens):
                     return f(*args, **kwargs)
@@ -114,15 +159,15 @@
                     level=messages.LogEvent.LOGLEVEL_ERROR,
                     login_type=messages.LoginEvent.LOGIN_TYPE_TOKEN,
                     login_status=messages.LoginEvent.LOGIN_STATUS_FAILED_WITH_INVALID_TOKEN,
                     client_name=login_infos['client_name'], client_version=login_infos['client_version'],
                     client_ip=login_infos['client_ip'], os_name=login_infos['os_name'],
                     os_version=login_infos['os_version'], server_endpoint=login_infos['server_endpoint'],
                     service_uuid=ServiceAccessManager.service.service_uuid)
-                return 'Forbidden', 403
+                return gettext('Forbidden'), 403
 
             return decorated
         return wrap
 
     @staticmethod
     def service_token_required(f):
         @wraps(f)
@@ -143,15 +188,15 @@
                         level=messages.LogEvent.LOGLEVEL_ERROR,
                         login_type=messages.LoginEvent.LOGIN_TYPE_TOKEN,
                         login_status=messages.LoginEvent.LOGIN_STATUS_FAILED_WITH_INVALID_TOKEN,
                         client_name=login_infos['client_name'], client_version=login_infos['client_version'],
                         client_ip=login_infos['client_ip'], os_name=login_infos['os_name'],
                         os_version=login_infos['os_version'], server_endpoint=login_infos['server_endpoint'],
                         service_uuid=ServiceAccessManager.service.service_uuid)
-                    return 'Forbidden', 403
+                    return gettext('Forbidden'), 403
 
                 # Verify scheme and token
                 if scheme == 'OpenTera':
                     token = atoken
 
             # Verify token from with service api key
             if ServiceAccessManager.validate_service_token(token=token):
@@ -162,15 +207,15 @@
                 level=messages.LogEvent.LOGLEVEL_ERROR,
                 login_type=messages.LoginEvent.LOGIN_TYPE_TOKEN,
                 login_status=messages.LoginEvent.LOGIN_STATUS_FAILED_WITH_INVALID_TOKEN,
                 client_name=login_infos['client_name'], client_version=login_infos['client_version'],
                 client_ip=login_infos['client_ip'], os_name=login_infos['os_name'],
                 os_version=login_infos['os_version'], server_endpoint=login_infos['server_endpoint'],
                 service_uuid=ServiceAccessManager.service.service_uuid)
-            return 'Forbidden', 403
+            return gettext('Forbidden'), 403
 
         return decorated
 
     @staticmethod
     def service_or_others_token_required(allow_dynamic_tokens=True, allow_static_tokens=False):
         def wrap(f):
             def decorated(*args, **kwargs):
@@ -190,15 +235,15 @@
                             level=messages.LogEvent.LOGLEVEL_ERROR,
                             login_type=messages.LoginEvent.LOGIN_TYPE_TOKEN,
                             login_status=messages.LoginEvent.LOGIN_STATUS_FAILED_WITH_INVALID_TOKEN,
                             client_name=login_infos['client_name'], client_version=login_infos['client_version'],
                             client_ip=login_infos['client_ip'], os_name=login_infos['os_name'],
                             os_version=login_infos['os_version'], server_endpoint=login_infos['server_endpoint'],
                             service_uuid=ServiceAccessManager.service.service_uuid)
-                        return 'Forbidden', 403
+                        return gettext('Forbidden'), 403
 
                     # Verify scheme and token
                     if scheme == 'OpenTera':
                         token = atoken
 
                         # Service tokens only allowed in authorization header - check here
                         if ServiceAccessManager.validate_service_token(token=token):
@@ -245,29 +290,33 @@
                     level=messages.LogEvent.LOGLEVEL_ERROR,
                     login_type=messages.LoginEvent.LOGIN_TYPE_TOKEN,
                     login_status=messages.LoginEvent.LOGIN_STATUS_FAILED_WITH_INVALID_TOKEN,
                     client_name=login_infos['client_name'], client_version=login_infos['client_version'],
                     client_ip=login_infos['client_ip'], os_name=login_infos['os_name'],
                     os_version=login_infos['os_version'], server_endpoint=login_infos['server_endpoint'],
                     service_uuid=ServiceAccessManager.service.service_uuid)
-                return 'Forbidden', 403
+                return gettext('Forbidden'), 403
 
             return decorated
 
         return wrap
 
     @staticmethod
     def validate_user_token(token: str) -> bool:
         try:
             token_dict = jwt.decode(token, ServiceAccessManager.api_user_token_key, algorithms='HS256')
         except jwt.PyJWTError as e:
             # Not a user, or invalid token, will continue...
             pass
         else:
-            # User token
+            # Check if token is disabled
+            if ServiceAccessManager.is_user_token_disabled(token):
+                return False
+
+            # User token is valid and not disabled
             _request_ctx_stack.top.current_user_client = \
                 TeraUserClient(token_dict, token, ServiceAccessManager.service.config_man)
             _request_ctx_stack.top.current_login_type = LoginType.USER_LOGIN
             return True
 
     @staticmethod
     def validate_device_token(token: str, allow_dynamic_tokens: bool, allow_static_tokens: bool) -> bool:
@@ -304,15 +353,19 @@
         if allow_dynamic_tokens:  # Check for dynamic participant token
             try:
                 token_dict = jwt.decode(token, ServiceAccessManager.api_participant_token_key, algorithms='HS256')
             except jwt.PyJWTError as e:
                 # Not a participant, or invalid token, will continue...
                 pass
             else:
-                # Participant token
+                # Look for disabled tokens, token was decoded successfully
+                if ServiceAccessManager.is_participant_token_disabled(token):
+                    return False
+
+                # Participant token is not disabled, everything is ok
                 _request_ctx_stack.top.current_participant_client = \
                     TeraParticipantClient(token_dict, token, ServiceAccessManager.service.config_man)
                 _request_ctx_stack.top.current_login_type = LoginType.PARTICIPANT_LOGIN
                 return True
 
         if allow_static_tokens:  # Check for static participant token
             try:
@@ -327,22 +380,54 @@
                     TeraParticipantClient(token_dict, token, ServiceAccessManager.service.config_man)
                 _request_ctx_stack.top.current_login_type = LoginType.PARTICIPANT_LOGIN
                 return True
 
         return False
 
     @staticmethod
-    def validate_service_token(token:str) -> bool:
+    def validate_service_token(token: str) -> bool:
         try:
             token_dict = jwt.decode(token, ServiceAccessManager.api_service_token_key, algorithms='HS256')
         except jwt.PyJWTError as e:
             # Not a device, or invalid token, will continue...
             pass
         else:
             # Service token
             _request_ctx_stack.top.current_service_client = \
                 TeraServiceClient(token_dict, token, ServiceAccessManager.service.config_man)
             _request_ctx_stack.top.current_login_type = LoginType.SERVICE_LOGIN
             return True
 
         return False
 
+    @staticmethod
+    def service_user_roles_required(roles: List[str]):
+        def wrap(f):
+            @wraps(f)
+            def decorated(*args, **kwargs):
+
+                # Check if service is initialized
+                if ServiceAccessManager.service is None or 'service_key' \
+                        not in ServiceAccessManager.service.service_info:
+                    return gettext('Forbidden'), 403
+
+                service_key = ServiceAccessManager.service.service_info['service_key']
+
+                # Check if user is logged in, watch out not None object but LocalProxy cannot use is None...
+                if not current_user_client:
+                    return gettext('Forbidden'), 403
+
+                # Super admin pass through
+                if current_user_client.user_superadmin:
+                    return f(*args, **kwargs)
+
+                # Check if user has the required role (global roles are stored in token)
+                user_roles_from_token = current_user_client.get_roles_for_service(service_key)
+
+                # Check if user has the required roles
+                if not all(role in user_roles_from_token for role in roles):
+                    return gettext('Forbidden'), 403
+
+                # Everything ok, continue
+                return f(*args, **kwargs)
+            return decorated
+        return wrap
```

### Comparing `opentera-1.2.1/opentera/services/ServiceConfigManager.py` & `opentera-1.2.2/opentera/services/ServiceConfigManager.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/services/ServiceOpenTera.py` & `opentera-1.2.2/opentera/services/ServiceOpenTera.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,32 +33,20 @@
 
         # Take values from config_man
         # Values are checked when config is loaded...
         self.backend_hostname = config_man.backend_config['hostname']
         self.backend_port = config_man.backend_config['port']
         self.service_uuid = config_man.service_config['ServiceUUID']
 
-        # Update Service Access information
-        ServiceAccessManager.api_user_token_key = \
-            self.redisGet(RedisVars.RedisVar_UserTokenAPIKey)
-        ServiceAccessManager.api_participant_token_key = \
-            self.redisGet(RedisVars.RedisVar_ParticipantTokenAPIKey)
-        ServiceAccessManager.api_participant_static_token_key = \
-            self.redisGet(RedisVars.RedisVar_ParticipantStaticTokenAPIKey)
-        ServiceAccessManager.api_device_token_key = \
-            self.redisGet(RedisVars.RedisVar_DeviceTokenAPIKey)
-        ServiceAccessManager.api_device_static_token_key = \
-            self.redisGet(RedisVars.RedisVar_DeviceStaticTokenAPIKey)
-        ServiceAccessManager.api_service_token_key = \
-            self.redisGet(RedisVars.RedisVar_ServiceTokenAPIKey)
-        ServiceAccessManager.service = self
-
         # Create service token for service api requests
         self.service_token = self.service_generate_token()
 
+        # Init service access manager
+        ServiceAccessManager.init_access_manager(service=self)
+
     def redisConnectionMade(self):
         print('*** ServiceOpenTera.redisConnectionMade for', self.config['name'])
 
         # Build RPC interface
         self.setup_rpc_interface()
 
         # Build standard interface
```

### Comparing `opentera-1.2.1/opentera/services/ServiceOpenTeraWithAssets.py` & `opentera-1.2.2/opentera/services/ServiceOpenTeraWithAssets.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/services/ServiceOpenTeraWithTests.py` & `opentera-1.2.2/opentera/services/ServiceOpenTeraWithTests.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/services/TeraDeviceClient.py` & `opentera-1.2.2/opentera/services/TeraDeviceClient.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/services/TeraServiceClient.py` & `opentera-1.2.2/opentera/services/TeraServiceClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,24 +6,17 @@
 
 class TeraServiceClient:
 
     def __init__(self, token_dict: dict, token: str, config_man):
         self.__service_uuid = token_dict['service_uuid']
         self.__service_token = token
 
-        # A little trick here to get the right URL for the server if we are using a proxy
         backend_hostname = config_man.backend_config["hostname"]
         backend_port = str(config_man.backend_config["port"])
 
-        #if 'X-Externalhost' in request.headers:
-        #    backend_hostname = request.headers['X-Externalhost']
-
-        #if 'X-Externalport' in request.headers:
-        #    backend_port = request.headers['X-Externalport']
-
         self.__backend_url = 'https://' + backend_hostname + ':' + backend_port
 
     @property
     def service_uuid(self):
         return self.__service_uuid
 
     @service_uuid.setter
```

### Comparing `opentera-1.2.1/opentera/services/modules/WebRTCModule.py` & `opentera-1.2.2/opentera/services/modules/WebRTCModule.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/utils/Metrics.py` & `opentera-1.2.2/opentera/utils/Metrics.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/utils/TeraVersions.py` & `opentera-1.2.2/opentera/utils/TeraVersions.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/utils/UserAgentParser.py` & `opentera-1.2.2/opentera/utils/UserAgentParser.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera/utils/assets/BaseAsset.py` & `opentera-1.2.2/opentera/utils/assets/BaseAsset.py`

 * *Files identical despite different names*

### Comparing `opentera-1.2.1/opentera.egg-info/PKG-INFO` & `opentera-1.2.2/opentera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentera
-Version: 1.2.1
+Version: 1.2.2
 Summary: OpenTera base package
 Home-page: https://github.com/introlab/opentera
 Author: Dominic Létourneau, Simon Brière
 Author-email: dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opentera-1.2.1/opentera.egg-info/SOURCES.txt` & `opentera-1.2.2/opentera.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 opentera/modules/__init__.py
 opentera/redis/RedisClient.py
 opentera/redis/RedisProtocolFactory.py
 opentera/redis/RedisRPCClient.py
 opentera/redis/RedisVars.py
 opentera/redis/__init__.py
 opentera/services/BaseWebRTCService.py
+opentera/services/DisabledTokenStorage.py
 opentera/services/ServiceAccessManager.py
 opentera/services/ServiceConfigManager.py
 opentera/services/ServiceOpenTera.py
 opentera/services/ServiceOpenTeraWithAssets.py
 opentera/services/ServiceOpenTeraWithTests.py
 opentera/services/TeraDeviceClient.py
 opentera/services/TeraParticipantClient.py
```

### Comparing `opentera-1.2.1/opentera.egg-info/requires.txt` & `opentera-1.2.2/opentera.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Twisted==22.10.0
 treq==22.2.0
-cryptography==39.0.1
+cryptography==40.0.2
 autobahn==23.1.2
-SQLAlchemy==1.4.46
+SQLAlchemy==1.4.48
 sqlalchemy-schemadisplay==1.3
 pydot==1.4.2
-psycopg2-binary==2.9.5
-Flask==2.2.3
+psycopg2-binary==2.9.6
+Flask==2.3.2
 Flask-SQLAlchemy==3.0.3
 Flask-Login==0.6.2
 Flask-Login-Multi==0.1.2
-Flask-HTTPAuth==4.7.0
-Flask-SocketIO==5.3.2
-Flask-Session==0.4.0
-flask-restx==1.0.6
+Flask-HTTPAuth==4.8.0
+Flask-SocketIO==5.3.4
+Flask-Session==0.5.0
+flask-restx==1.1.0
 Flask-Security==3.0.0
-Flask-Babel==3.0.1
+Flask-Babel==3.1.0
 Flask-BabelEx==0.9.4
 Flask-Migrate==4.0.4
 flask-swagger-ui==4.11.1
-Flask-Limiter==3.2.0
+Flask-Limiter==3.3.1
 Flask-Mail==0.9.1
 Flask-Principal==0.4.0
-redis==4.5.1
-txredisapi==1.4.7
+redis==4.5.5
+txredisapi==1.4.9
 passlib==1.7.4
 bcrypt==4.0.1
 WTForms==3.0.1
-pyOpenSSL==23.0.0
+pyOpenSSL==23.1.1
 service-identity==21.1.0
-PyJWT==2.6.0
+PyJWT==2.7.0
 pylzma==0.5.0
 bz2file==0.98
-python-slugify==8.0.0
-websocket-client==1.5.1
-pytest==7.2.1
+python-slugify==8.0.1
+websocket-client==1.5.2
+pytest==7.3.1
 jsonschema==4.17.3
 Jinja2==3.1.2
 ua-parser==0.16.1
 protobuf==3.20.3
 
 [:sys_platform == "win32"]
 pypiwin32==223
```

### Comparing `opentera-1.2.1/setup.py` & `opentera-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("env/requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.readlines()
     requirements.append('protobuf==3.20.3')
 
 setuptools.setup(
     name="opentera",
-    version="1.2.1",
+    version="1.2.2",
     author="Dominic Létourneau, Simon Brière",
     author_email="dominic.letourneau@usherbrooke.ca, simon.briere@usherbrooke.ca",
     description="OpenTera base package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/introlab/opentera",
     packages=setuptools.find_packages(),
```

### Comparing `opentera-1.2.1/translations/en/LC_MESSAGES/messages.po` & `opentera-1.2.2/translations/en/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-21 09:06-0400\n"
+"POT-Creation-Date: 2023-05-23 14:24-0400\n"
 "PO-Revision-Date: 2021-01-25 13:01-0500\n"
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -45,23 +45,35 @@
 #: modules/FlaskModule/API/device/DeviceQueryDevices.py:82
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:49
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:55
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:62
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:68
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:74
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:80
-#: modules/FlaskModule/API/service/ServiceQueryProjects.py:41
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:52
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:57
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:99
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:106
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:158
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:112
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:100
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:104
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:108
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:116
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:194
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:86
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:91
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:66
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:72
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:76
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:84
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:90
 #: modules/FlaskModule/API/service/ServiceQuerySites.py:36
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:96
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:197
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:301
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:122
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:257
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:112
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:166
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:105
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:191
@@ -72,53 +84,55 @@
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:60
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:66
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:72
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:78
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:84
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:107
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:159
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:350
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:353
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:198
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:269
-#: modules/FlaskModule/API/user/UserQueryProjects.py:145
-#: modules/FlaskModule/API/user/UserQueryProjects.py:150
-#: modules/FlaskModule/API/user/UserQueryProjects.py:258
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:112
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:363
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:366
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:204
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:275
+#: modules/FlaskModule/API/user/UserQueryProjects.py:151
+#: modules/FlaskModule/API/user/UserQueryProjects.py:156
+#: modules/FlaskModule/API/user/UserQueryProjects.py:264
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:117
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:121
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:129
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:208
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:212
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:216
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:220
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:122
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:126
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:134
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:213
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:217
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:221
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:225
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:151
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:155
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:159
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:165
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:240
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:245
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:249
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:253
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:79
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:136
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:129
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:259
 #: modules/FlaskModule/API/user/UserQueryServices.py:121
 #: modules/FlaskModule/API/user/UserQueryServices.py:134
 #: modules/FlaskModule/API/user/UserQueryServices.py:231
 #: modules/FlaskModule/API/user/UserQueryServices.py:239
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:91
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:144
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:204
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:203
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:267
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:55
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:107
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:138
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:183
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:266
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:187
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:270
 #: modules/FlaskModule/API/user/UserQuerySites.py:124
 #: modules/FlaskModule/API/user/UserQuerySites.py:127
 #: modules/FlaskModule/API/user/UserQuerySites.py:176
 #: modules/FlaskModule/API/user/UserQueryStats.py:51
 #: modules/FlaskModule/API/user/UserQueryStats.py:56
 #: modules/FlaskModule/API/user/UserQueryStats.py:61
 #: modules/FlaskModule/API/user/UserQueryStats.py:67
@@ -134,31 +148,53 @@
 #: modules/FlaskModule/API/user/UserQueryTests.py:140
 #: modules/FlaskModule/API/user/UserQueryUserGroups.py:147
 #: modules/FlaskModule/API/user/UserQueryUserPreferences.py:47
 #: modules/FlaskModule/API/user/UserQueryUserPreferences.py:96
 #: modules/FlaskModule/API/user/UserQueryUsers.py:214
 #: modules/FlaskModule/API/user/UserQueryUsers.py:219
 #: modules/FlaskModule/API/user/UserQueryUsers.py:348
+#: opentera/services/ServiceAccessManager.py:116
+#: opentera/services/ServiceAccessManager.py:166
+#: opentera/services/ServiceAccessManager.py:195
+#: opentera/services/ServiceAccessManager.py:214
+#: opentera/services/ServiceAccessManager.py:242
+#: opentera/services/ServiceAccessManager.py:297
+#: opentera/services/ServiceAccessManager.py:411
+#: opentera/services/ServiceAccessManager.py:417
+#: opentera/services/ServiceAccessManager.py:428
 msgid "Forbidden"
 msgstr ""
 
 #: modules/FlaskModule/API/device/DeviceQueryDevices.py:93
 #: modules/FlaskModule/API/device/DeviceQuerySessionEvents.py:74
 #: modules/FlaskModule/API/device/DeviceQuerySessionEvents.py:89
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:156
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:233
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:247
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:284
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:116
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:138
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:176
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:73
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:94
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:123
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:138
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:150
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:172
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:205
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:104
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:119
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:185
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:218
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:234
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:245
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:280
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:141
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:158
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:215
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:180
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:221
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:276
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:331
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:232
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:268
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:130
@@ -169,27 +205,30 @@
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:189
 #: modules/FlaskModule/API/user/UserQueryDevices.py:328
 #: modules/FlaskModule/API/user/UserQueryDevices.py:343
 #: modules/FlaskModule/API/user/UserQueryDevices.py:460
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:120
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:135
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:178
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:239
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:280
-#: modules/FlaskModule/API/user/UserQueryProjects.py:190
-#: modules/FlaskModule/API/user/UserQueryProjects.py:205
-#: modules/FlaskModule/API/user/UserQueryProjects.py:276
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:151
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:163
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:185
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:231
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:245
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:286
+#: modules/FlaskModule/API/user/UserQueryProjects.py:196
+#: modules/FlaskModule/API/user/UserQueryProjects.py:211
+#: modules/FlaskModule/API/user/UserQueryProjects.py:282
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:156
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:168
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:190
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:236
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:208
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:264
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:287
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:322
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:98
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:119
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:147
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:244
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:286
 #: modules/FlaskModule/API/user/UserQueryServices.py:162
 #: modules/FlaskModule/API/user/UserQueryServices.py:182
 #: modules/FlaskModule/API/user/UserQueryServices.py:259
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:104
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:119
@@ -200,16 +239,16 @@
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:286
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:197
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:212
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:342
 #: modules/FlaskModule/API/user/UserQuerySessions.py:179
 #: modules/FlaskModule/API/user/UserQuerySessions.py:194
 #: modules/FlaskModule/API/user/UserQuerySessions.py:272
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:237
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:277
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:241
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:281
 #: modules/FlaskModule/API/user/UserQuerySites.py:140
 #: modules/FlaskModule/API/user/UserQuerySites.py:155
 #: modules/FlaskModule/API/user/UserQuerySites.py:194
 #: modules/FlaskModule/API/user/UserQueryTestType.py:216
 #: modules/FlaskModule/API/user/UserQueryTestType.py:231
 #: modules/FlaskModule/API/user/UserQueryTestType.py:345
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:252
@@ -229,23 +268,25 @@
 #: modules/FlaskModule/API/user/UserQueryUsers.py:272
 #: modules/FlaskModule/API/user/UserQueryUsers.py:385
 msgid "Database error"
 msgstr ""
 
 #: modules/FlaskModule/API/device/DeviceQueryParticipants.py:41
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:82
-#: modules/FlaskModule/API/service/ServiceQueryProjects.py:56
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:72
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:67
 #: modules/FlaskModule/API/service/ServiceQueryServices.py:76
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:62
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:122
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:109
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:86
-#: modules/FlaskModule/API/user/UserQueryProjects.py:110
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:80
+#: modules/FlaskModule/API/user/UserQueryProjects.py:116
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:84
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:123
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:67
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:112
 #: modules/FlaskModule/API/user/UserQueryServices.py:104
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:62
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:101
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:79
 #: modules/FlaskModule/API/user/UserQuerySessions.py:103
 #: modules/FlaskModule/API/user/UserQuerySites.py:97
@@ -268,28 +309,29 @@
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:95
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:99
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:104
 #: modules/FlaskModule/API/device/DeviceQueryStatus.py:48
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:270
 #: modules/FlaskModule/API/service/ServiceQueryDevices.py:73
 #: modules/FlaskModule/API/service/ServiceQueryDevices.py:87
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:68
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:83
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:69
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:84
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:49
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:46
 #: modules/FlaskModule/API/service/ServiceQuerySiteProjectAccessRoles.py:43
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:266
 #: modules/FlaskModule/API/service/ServiceQueryUsers.py:38
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:70
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:65
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:61
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:157
-#: modules/FlaskModule/API/user/UserQueryForms.py:82
+#: modules/FlaskModule/API/user/UserQueryForms.py:85
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:76
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:81
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:52
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:53
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:63
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:60
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:46
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:62
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:59
 #: modules/FlaskModule/API/user/UserQuerySessions.py:59
 #: modules/FlaskModule/API/user/UserQuerySiteAccess.py:80
@@ -297,19 +339,19 @@
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:60
 msgid "Missing arguments"
 msgstr ""
 
 #: modules/FlaskModule/API/device/DeviceQuerySessionEvents.py:61
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:114
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:137
-#: modules/LoginModule/LoginModule.py:595
-#: modules/LoginModule/LoginModule.py:695
-#: modules/LoginModule/LoginModule.py:762
-#: modules/LoginModule/LoginModule.py:789
-#: modules/LoginModule/LoginModule.py:808
+#: modules/LoginModule/LoginModule.py:587
+#: modules/LoginModule/LoginModule.py:687
+#: modules/LoginModule/LoginModule.py:753
+#: modules/LoginModule/LoginModule.py:780
+#: modules/LoginModule/LoginModule.py:799
 msgid "Unauthorized"
 msgstr ""
 
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:119
 msgid "Missing argument 'session name'"
 msgstr ""
 
@@ -341,19 +383,19 @@
 msgid "Participant already logged in."
 msgstr ""
 
 #: modules/FlaskModule/API/participant/ParticipantLogin.py:126
 msgid "Missing current_participant"
 msgstr ""
 
-#: modules/FlaskModule/API/participant/ParticipantLogout.py:33
+#: modules/FlaskModule/API/participant/ParticipantLogout.py:41
 msgid "Participant logged out."
 msgstr ""
 
-#: modules/FlaskModule/API/participant/ParticipantLogout.py:35
+#: modules/FlaskModule/API/participant/ParticipantLogout.py:43
 msgid "Participant not logged in"
 msgstr ""
 
 #: modules/FlaskModule/API/participant/ParticipantQueryParticipants.py:55
 #: modules/FlaskModule/API/participant/ParticipantQuerySessions.py:73
 msgid "Not implemented"
 msgstr ""
@@ -481,28 +523,117 @@
 msgstr ""
 
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:84
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:88
 msgid "Success"
 msgstr ""
 
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:89
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:90
 msgid "Unknown project"
 msgstr ""
 
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:92
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:93
 msgid "Invalid participant name"
 msgstr ""
 
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:95
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:96
 msgid "Invalid participant email"
 msgstr ""
 
-#: modules/FlaskModule/API/service/ServiceQueryProjects.py:37
-msgid "Missing project id"
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:120
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:312
+msgid "Can't insert participant: participant's project is disabled or invalid."
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:130
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:285
+msgid "Can't update participant: participant's project is disabled."
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:48
+msgid "Missing parameter"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:87
+#: modules/FlaskModule/API/user/UserQueryProjects.py:132
+msgid "Missing project"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:93
+#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:180
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:198
+#: modules/FlaskModule/API/user/UserQueryProjects.py:138
+#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:179
+msgid "Missing id_project"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:96
+#: modules/FlaskModule/API/user/UserQueryProjects.py:140
+msgid "Missing id_site arguments"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:169
+#: modules/FlaskModule/API/user/UserQueryProjects.py:275
+msgid ""
+"Can't delete project: please delete all participants with sessions before"
+" deleting."
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:52
+msgid "Missing service_role field"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:58
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:154
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:172
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:85
+msgid "Missing id_service_role"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:81
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:106
+msgid "Missing fields"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:87
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:104
+msgid "Missing service_access"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:91
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:108
+msgid "Missing id_service_access"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:95
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:112
+msgid "Can't combine id_user_group, id_participant_group and id_device in request"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:114
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:132
+msgid "Bad id_service_role"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:158
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:176
+#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:192
+msgid "Missing at least one id field"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:191
+#: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:203
+#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:296
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:209
+#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:63
+#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:308
+#: modules/FlaskModule/API/user/UserQueryServiceSites.py:266
+#: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:270
+#: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:271
+msgid "Not found"
 msgstr ""
 
 #: modules/FlaskModule/API/service/ServiceQueryServices.py:38
 msgid "Missing service key, id or uuid"
 msgstr ""
 
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:76
@@ -568,14 +699,58 @@
 msgid "Service can't create tests for that session"
 msgstr ""
 
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:269
 msgid "Service can't delete tests for that session"
 msgstr ""
 
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:71
+#: modules/FlaskModule/API/user/UserQueryUserGroups.py:132
+msgid "Missing user_group"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:78
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:196
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:179
+#: modules/FlaskModule/API/user/UserQueryUserGroups.py:139
+#: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:102
+msgid "Missing id_user_group"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:90
+msgid "Missing service role name or id_service_role"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:103
+msgid "Can't set access to service other than self"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:109
+msgid "No access for at a least one project in the list"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:115
+msgid "No access for at a least one site in the list"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:127
+msgid "Bad role name for service"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:145
+msgid "A new usergroup must have at least one service access"
+msgstr ""
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:207
+#: modules/FlaskModule/API/user/UserQueryUserGroups.py:300
+msgid ""
+"Can't delete user group: please delete all users part of that user group "
+"before deleting."
+msgstr ""
+
 #: modules/FlaskModule/API/service/ServiceSessionManager.py:116
 #: modules/FlaskModule/API/user/UserSessionManager.py:107
 msgid "Missing action"
 msgstr ""
 
 #: modules/FlaskModule/API/service/ServiceSessionManager.py:131
 #: modules/FlaskModule/API/user/UserSessionManager.py:121
@@ -628,19 +803,19 @@
 msgid "Invalid client name :"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserLogin.py:143
 msgid "Invalid client version handler"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserLogout.py:27
+#: modules/FlaskModule/API/user/UserLogout.py:34
 msgid "User logged out."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserLogout.py:29
+#: modules/FlaskModule/API/user/UserLogout.py:36
 msgid "User not logged in"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryAssets.py:79
 msgid "Service access denied"
 msgstr ""
 
@@ -666,25 +841,14 @@
 msgid "Access denied to device"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:149
 msgid "Device not assigned to project or participant"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:203
-#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:296
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:204
-#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:63
-#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:308
-#: modules/FlaskModule/API/user/UserQueryServiceSites.py:266
-#: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:270
-#: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:271
-msgid "Not found"
-msgstr ""
-
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:141
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:127
 #: modules/FlaskModule/API/user/UserQueryDevices.py:259
 msgid "Missing id_device"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:143
@@ -718,21 +882,14 @@
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:321
 msgid ""
 "Can't delete device from project. Please remove all participants "
 "associated with the device or all sessions in the project referring to "
 "the device before deleting."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:180
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:192
-#: modules/FlaskModule/API/user/UserQueryProjects.py:132
-#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:179
-msgid "Missing id_project"
-msgstr ""
-
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:182
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:157
 msgid "Missing devices"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:238
 msgid ""
@@ -829,15 +986,15 @@
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:60
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:65
 msgid "Unexisting ID/Forbidden access"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:79
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:387
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:400
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:182
 msgid "Database Error"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:95
 msgid "Missing device type"
 msgstr ""
@@ -933,27 +1090,31 @@
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:49
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:57
 msgid "Use Logout instead to disconnect current user"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:79
+#: modules/FlaskModule/API/user/UserQueryForms.py:82
 msgid "Missing type"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:134
+#: modules/FlaskModule/API/user/UserQueryForms.py:137
 msgid "Missing session type id"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:167
+#: modules/FlaskModule/API/user/UserQueryForms.py:148
+msgid "No reply from service while querying session type config"
+msgstr ""
+
+#: modules/FlaskModule/API/user/UserQueryForms.py:182
 msgid "Invalid service specified"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:180
+#: modules/FlaskModule/API/user/UserQueryForms.py:195
 msgid "Unknown form type: "
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryOnlineDevices.py:60
 #: modules/FlaskModule/API/user/UserQueryOnlineParticipants.py:59
 #: modules/FlaskModule/API/user/UserQueryOnlineUsers.py:57
 msgid "Internal server error when making RPC call."
@@ -997,103 +1158,69 @@
 msgid "Participant group not found."
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:266
 msgid "Mismatch between id_project and group's project"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:370
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:383
 msgid "Can't delete participant: please remove all related sessions beforehand."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:372
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:385
 msgid ""
 "Can't delete participant: please remove all sessions created by this "
 "participant beforehand."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:375
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:388
 msgid "Can't delete participant: please remove all related assets beforehand."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:377
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:390
 msgid "Can't delete participant: please remove all related tests beforehand."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:379
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:392
 msgid ""
 "Can't delete participant: please remove all related sessions, assets and "
 "tests before deleting."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:190
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:175
-#: modules/FlaskModule/API/user/UserQueryUserGroups.py:139
-#: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:102
-msgid "Missing id_user_group"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:194
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:179
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:200
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:183
 msgid "Missing role name or id"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:223
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:229
 msgid "Invalid role name or id for that project"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:265
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:271
 msgid "No project access to delete."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:126
-msgid "Missing project"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryProjects.py:134
-msgid "Missing id_site arguments"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryProjects.py:163
+#: modules/FlaskModule/API/user/UserQueryProjects.py:169
 msgid "No access to a session type for at least one of it"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:175
+#: modules/FlaskModule/API/user/UserQueryProjects.py:181
 msgid "At least one session type is not associated to the project site"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:269
-msgid ""
-"Can't delete project: please delete all participants with sessions before"
-" deleting."
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:99
-msgid "Missing service_access"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:103
-msgid "Missing id_service_access"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:107
-msgid "Can't combine id_user_group, id_participant_group and id_device in request"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:127
-msgid "Bad id_service_role"
-msgstr ""
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:167
-msgid "Missing id_service_role"
+#: modules/FlaskModule/API/user/UserQueryServiceAccessToken.py:35
+#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:189
+#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:142
+#: modules/FlaskModule/API/user/UserQueryServiceSites.py:134
+#: modules/FlaskModule/API/user/UserQueryServices.py:128
+msgid "Missing id_service"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:171
-#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:192
-msgid "Missing at least one id field"
+#: modules/FlaskModule/API/user/UserQueryServiceAccessToken.py:38
+msgid "No access to specified service"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:72
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:146
 msgid "Can't combine id_user, id_participant and id_device in request"
 msgstr ""
 
@@ -1102,21 +1229,14 @@
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:175
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:198
 msgid "Invalid config format provided"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:189
-#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:142
-#: modules/FlaskModule/API/user/UserQueryServiceSites.py:134
-#: modules/FlaskModule/API/user/UserQueryServices.py:128
-msgid "Missing id_service"
-msgstr ""
-
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:170
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:211
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:339
 msgid ""
 "Can't delete service-project: please remove all related sessions, assets "
 "and tests before deleting."
 msgstr ""
@@ -1295,23 +1415,23 @@
 msgid "User doesn't have access to at least one device of that session."
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQuerySessions.py:261
 msgid "Session is in progress: can't delete that session."
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:177
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:181
 msgid "Missing id_site"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:221
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:225
 msgid "Invalid role name or id for that site"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:262
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:266
 msgid "No site access to delete"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQuerySites.py:112
 msgid "Missing site"
 msgstr ""
 
@@ -1408,28 +1528,18 @@
 msgid "Item can't be undeleted"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryUndelete.py:52
 msgid "Item isn't deleted"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryUserGroups.py:132
-msgid "Missing user_group"
-msgstr ""
-
 #: modules/FlaskModule/API/user/UserQueryUserGroups.py:142
 msgid "Missing user group name"
 msgstr ""
 
-#: modules/FlaskModule/API/user/UserQueryUserGroups.py:300
-msgid ""
-"Can't delete user group: please delete all users part of that user group "
-"before deleting."
-msgstr ""
-
 #: modules/FlaskModule/API/user/UserQueryUserPreferences.py:89
 msgid "Missing app tag"
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:57
 msgid "At least one id must be specified"
 msgstr ""
@@ -1550,24 +1660,24 @@
 msgstr ""
 
 #: modules/FlaskModule/API/user/UserSessionManager.py:181
 #: modules/FlaskModule/API/user/UserSessionManager.py:184
 msgid "Invalid reply code"
 msgstr ""
 
-#: modules/LoginModule/LoginModule.py:630
-#: modules/LoginModule/LoginModule.py:663
+#: modules/LoginModule/LoginModule.py:622
+#: modules/LoginModule/LoginModule.py:655
 msgid "Disabled device"
 msgstr ""
 
-#: modules/LoginModule/LoginModule.py:640
+#: modules/LoginModule/LoginModule.py:632
 msgid "Invalid token"
 msgstr ""
 
-#: modules/LoginModule/LoginModule.py:740
+#: modules/LoginModule/LoginModule.py:732
 msgid "Invalid Token"
 msgstr ""
 
 #: opentera/db/models/TeraSessionType.py:149
 #: opentera/forms/TeraSessionForm.py:105
 msgid "Unknown"
 msgstr ""
@@ -1756,25 +1866,34 @@
 msgstr ""
 
 #: opentera/forms/TeraProjectForm.py:22
 msgid "Project ID"
 msgstr ""
 
 #: opentera/forms/TeraProjectForm.py:24
+msgid "Enabled"
+msgstr ""
+
+#: opentera/forms/TeraProjectForm.py:26
 msgid "Site"
 msgstr ""
 
-#: opentera/forms/TeraProjectForm.py:25
+#: opentera/forms/TeraProjectForm.py:27
 msgid "Role"
 msgstr ""
 
-#: opentera/forms/TeraProjectForm.py:26 opentera/forms/TeraSiteForm.py:17
+#: opentera/forms/TeraProjectForm.py:28 opentera/forms/TeraSiteForm.py:17
 msgid "Site Name"
 msgstr ""
 
+#: opentera/forms/TeraProjectForm.py:30 opentera/forms/TeraProjectForm.py:32
+#: opentera/forms/TeraTestTypeForm.py:32
+msgid "Description"
+msgstr ""
+
 #: opentera/forms/TeraServiceConfigForm.py:25
 #: opentera/forms/TeraServiceForm.py:25
 msgid "Service ID"
 msgstr ""
 
 #: opentera/forms/TeraServiceConfigForm.py:26
 msgid "Service Config ID"
@@ -1968,22 +2087,14 @@
 msgid "Comments"
 msgstr ""
 
 #: opentera/forms/TeraSessionForm.py:167
 msgid "Session Has Device Data"
 msgstr ""
 
-#: opentera/forms/TeraSessionTypeConfigForm.py:19
-msgid "General configuration"
-msgstr ""
-
-#: opentera/forms/TeraSessionTypeConfigForm.py:22
-msgid "Allow session recording"
-msgstr ""
-
 #: opentera/forms/TeraSessionTypeForm.py:29
 msgid "Session Type ID"
 msgstr ""
 
 #: opentera/forms/TeraSessionTypeForm.py:30
 msgid "Session Type Name"
 msgstr ""
@@ -2040,18 +2151,14 @@
 msgid "Expose Web interface"
 msgstr ""
 
 #: opentera/forms/TeraTestTypeForm.py:31
 msgid "Expose Web editor"
 msgstr ""
 
-#: opentera/forms/TeraTestTypeForm.py:32
-msgid "Description"
-msgstr ""
-
 #: opentera/forms/TeraUserForm.py:18
 msgid "User UUID"
 msgstr ""
 
 #: opentera/forms/TeraUserForm.py:19
 msgid "User Full Name"
 msgstr ""
@@ -2137,87 +2244,87 @@
 msgid "Client linux version"
 msgstr ""
 
 #: opentera/services/BaseWebRTCService.py:52
 msgid "Join me!"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:382
+#: opentera/services/BaseWebRTCService.py:383
 msgid "Cannot create session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:422
+#: opentera/services/BaseWebRTCService.py:423
 msgid "Cannot create process"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:436
+#: opentera/services/BaseWebRTCService.py:437
 msgid "Cannot create session"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:459
+#: opentera/services/BaseWebRTCService.py:460
 msgid "Cannot create STOP session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:516
+#: opentera/services/BaseWebRTCService.py:517
 msgid "Error stopping session - check server logs"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:518
+#: opentera/services/BaseWebRTCService.py:519
 msgid "No matching session to stop"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:542
-#: opentera/services/BaseWebRTCService.py:619
-#: opentera/services/BaseWebRTCService.py:706
+#: opentera/services/BaseWebRTCService.py:543
+#: opentera/services/BaseWebRTCService.py:620
+#: opentera/services/BaseWebRTCService.py:707
 msgid "User"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:544
+#: opentera/services/BaseWebRTCService.py:545
 msgid "Error creating user invited session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:556
-#: opentera/services/BaseWebRTCService.py:634
-#: opentera/services/BaseWebRTCService.py:721
+#: opentera/services/BaseWebRTCService.py:557
+#: opentera/services/BaseWebRTCService.py:635
+#: opentera/services/BaseWebRTCService.py:722
 msgid "Participant"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:558
+#: opentera/services/BaseWebRTCService.py:559
 msgid "Error creating participant invited session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:571
-#: opentera/services/BaseWebRTCService.py:650
-#: opentera/services/BaseWebRTCService.py:736
+#: opentera/services/BaseWebRTCService.py:572
+#: opentera/services/BaseWebRTCService.py:651
+#: opentera/services/BaseWebRTCService.py:737
 msgid "Device"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:573
+#: opentera/services/BaseWebRTCService.py:574
 msgid "Error creating device invited session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:589
+#: opentera/services/BaseWebRTCService.py:590
 msgid "Error updating session"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:621
+#: opentera/services/BaseWebRTCService.py:622
 msgid "Error creating user left session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:636
+#: opentera/services/BaseWebRTCService.py:637
 msgid "Error creating participant left session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:652
+#: opentera/services/BaseWebRTCService.py:653
 msgid "Error creating device left session event"
 msgstr ""
 
-#: opentera/services/BaseWebRTCService.py:709
-#: opentera/services/BaseWebRTCService.py:724
-#: opentera/services/BaseWebRTCService.py:739
+#: opentera/services/BaseWebRTCService.py:710
+#: opentera/services/BaseWebRTCService.py:725
+#: opentera/services/BaseWebRTCService.py:740
 msgid "Cannot create refused session event"
 msgstr ""
 
 #: templates/about.html:33
 msgid "Downloads"
 msgstr ""
 
@@ -2249,7 +2356,16 @@
 
 #~ msgid ""
 #~ "Can't delete service from site: please"
 #~ " delete all sessions using that "
 #~ "service in the site before deleting."
 #~ msgstr ""
 
+#~ msgid "Missing project id"
+#~ msgstr ""
+
+#~ msgid "General configuration"
+#~ msgstr ""
+
+#~ msgid "Allow session recording"
+#~ msgstr ""
+
```

### Comparing `opentera-1.2.1/translations/fr/LC_MESSAGES/messages.mo` & `opentera-1.2.2/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,37 +1,38 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-21 09:06-0400\n"
-"PO-Revision-Date: 2023-03-07 08:35-0500\n"
+"POT-Creation-Date: 2023-05-23 14:24-0400\n"
+"PO-Revision-Date: 2023-05-23 14:28-0400\n"
 "Last-Translator: \n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
+msgid "A new usergroup must have at least one service access"
+msgstr ""
+"Un nouveau groupe utilisateur doit avoir au moins un accès à un service"
+
 msgid "Access Token"
 msgstr "Jeton d'accès"
 
 msgid "Access denied"
 msgstr "Accès refusé"
 
 msgid "Access denied to at least one project"
 msgstr "Accès refusé pour au moins un projet"
 
 msgid "Access denied to device"
 msgstr "Aucun accès à l’appareil"
 
-msgid "Allow session recording"
-msgstr "Autoriser l'enregistrement des séances"
-
 msgid ""
 "Asset information deletion must be done directly into a service (such as "
 "Filetransfer service)"
 msgstr ""
 "La suppression d'information sur les ressources doivent être fait "
 "directement dans un service (comme le service de transfert de fichiers - "
 "FileTransfer)"
@@ -77,14 +78,17 @@
 
 msgid "Bad id_service_role"
 msgstr "Mauvais id_service_role"
 
 msgid "Bad parameter"
 msgstr "Mauvais Paramètre(s)"
 
+msgid "Bad role name for service"
+msgstr "Nom de rôle invalide pour le service"
+
 msgid "Badly formatted request"
 msgstr "Requête mal formée"
 
 msgid "Camera"
 msgstr "Caméra"
 
 msgid "Can't combine id_user, id_participant and id_device in request"
@@ -365,14 +369,27 @@
 msgid ""
 "Can't delete user: please remove all tests created by this user before "
 "deleting."
 msgstr ""
 "Impossible de supprimer l'utilisateur: veuillez supprimer tous les tests "
 "créés par cet utilisateur au préalable."
 
+msgid "Can't insert participant: participant's project is disabled or invalid."
+msgstr ""
+"Impossible d'ajouter le participant: le projet du participant est désactivé "
+"ou invalide."
+
+msgid "Can't set access to service other than self"
+msgstr "Impossible d'ajuster les accès à un service autre que soi-même."
+
+msgid "Can't update participant: participant's project is disabled."
+msgstr ""
+"Impossible de mettre à jour le participant: le projet du participant est "
+"désactivé."
+
 msgid "Cancelled"
 msgstr "Annulée"
 
 msgid "Cannot create STOP session event"
 msgstr "Impossible de créer l'événement de séance \"Arrêt de séance\""
 
 msgid "Cannot create process"
@@ -539,14 +556,17 @@
 
 msgid "Duration"
 msgstr "Durée"
 
 msgid "Email"
 msgstr "Courriel"
 
+msgid "Enabled"
+msgstr "Activé"
+
 msgid "Error creating device invited session event"
 msgstr "Erreur lors de la création de l'événement de séance 'Appareil invité\""
 
 msgid "Error creating device left session event"
 msgstr ""
 "Erreur lors de la création de l'événement de séance 'Appareil a quitté la "
 "séance\""
@@ -593,17 +613,14 @@
 
 msgid "Forbidden"
 msgstr "Accès refusé"
 
 msgid "Forbidden for security reasons"
 msgstr "Accès interdit pour raison de sécurité"
 
-msgid "General configuration"
-msgstr "Configuration générale"
-
 msgid "In progess"
 msgstr "En cours"
 
 msgid "Information"
 msgstr "Information"
 
 msgid "Internal server error when making RPC call."
@@ -788,14 +805,17 @@
 
 msgid "Missing device_subtype"
 msgstr "Champ device_subtype manquant"
 
 msgid "Missing devices"
 msgstr "Appareils manquants"
 
+msgid "Missing fields"
+msgstr "Champs manquants"
+
 msgid "Missing group"
 msgstr "Groupe manquant"
 
 msgid "Missing id argument"
 msgstr "Champ id manquant"
 
 msgid "Missing id_asset field"
@@ -863,29 +883,29 @@
 
 msgid "Missing id_user"
 msgstr "Champ id_user manquant"
 
 msgid "Missing id_user_group"
 msgstr "Champ id_user_group manquant"
 
+msgid "Missing parameter"
+msgstr "Paramètre manquant"
+
 msgid "Missing parameters"
 msgstr "Paramètres manquants"
 
 msgid "Missing participant"
 msgstr "Participant manquant"
 
 msgid "Missing project"
 msgstr "Projet manquant"
 
 msgid "Missing project ID"
 msgstr "ID de projet manquant"
 
-msgid "Missing project id"
-msgstr "ID de projet manquant"
-
 msgid "Missing project(s) to associate that test type to"
 msgstr "Projet(s) manquant(s) pour l'association avec ce type de test"
 
 msgid "Missing projects"
 msgstr "Projets manquants"
 
 msgid "Missing reply code in parameters"
@@ -899,23 +919,29 @@
 
 msgid "Missing role name or id"
 msgstr "Nom du rôle ou ID manquant"
 
 msgid "Missing service key, id or uuid"
 msgstr "Clé, ID ou UUID de service manquant"
 
+msgid "Missing service role name or id_service_role"
+msgstr "Nom du rôle ou id_service_role manquant"
+
 msgid "Missing service_access"
 msgstr "Accès Service manquant (service_access)"
 
 msgid "Missing service_config"
 msgstr "Champ service_config manquant"
 
 msgid "Missing service_key"
 msgstr "Clé du service manquante"
 
+msgid "Missing service_role field"
+msgstr "Champ iservice_role manquant"
+
 msgid "Missing services"
 msgstr "Services manquants"
 
 msgid "Missing session"
 msgstr "Champ session manquant"
 
 msgid "Missing session participants and users"
@@ -974,14 +1000,20 @@
 
 msgid "Name"
 msgstr "Nom"
 
 msgid "Network Address"
 msgstr "Adresse Réseau"
 
+msgid "No access for at a least one project in the list"
+msgstr "Aucun accès pour au moins un projet dans la liste"
+
+msgid "No access for at a least one site in the list"
+msgstr "Aucun accès pour au moins un site dans la liste"
+
 msgid "No access for at a least one user group in the list"
 msgstr "Aucun accès pour au moins un groupe d'utilisateurs dans la liste"
 
 msgid "No access to a session type for at least one of it"
 msgstr "Pas d'accès à ce type de session pour au moins un projet"
 
 msgid "No access to device subtype"
@@ -995,14 +1027,17 @@
 
 msgid "No access to relationship's user group"
 msgstr "Aucun accès au groupe"
 
 msgid "No access to session."
 msgstr "Aucun accès à la séance."
 
+msgid "No access to specified service"
+msgstr "Aucun accès au service spécifié"
+
 msgid "No access to specified user"
 msgstr "Aucun accès à l'utilisateur"
 
 msgid "No access to specified user group"
 msgstr "Aucun accès au groupe utilisateurs"
 
 msgid "No access to this API"
@@ -1025,14 +1060,19 @@
 
 msgid "No project access to delete."
 msgstr "Aucun accès au projet pour supprimer."
 
 msgid "No project admin access for at a least one project in the list"
 msgstr "Pas administrateur pour au moins un projet da la liste"
 
+msgid "No reply from service while querying session type config"
+msgstr ""
+"Aucune réponse du service lors de la requête de la configuration du type de "
+"séance."
+
 msgid "No site access to delete"
 msgstr "Pas d'accès à effacer"
 
 msgid "No site admin access for at a least one project in the list"
 msgstr "Aucun accès administrateur pour au moins un projet dans la liste"
 
 msgid "No site admin access for at a least one site in the list"
```

### Comparing `opentera-1.2.1/translations/fr/LC_MESSAGES/messages.po` & `opentera-1.2.2/translations/fr/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-03-21 09:06-0400\n"
-"PO-Revision-Date: 2023-03-07 08:35-0500\n"
+"POT-Creation-Date: 2023-05-23 14:24-0400\n"
+"PO-Revision-Date: 2023-05-23 14:28-0400\n"
 "Last-Translator: \n"
-"Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "Generated-By: Babel 2.12.1\n"
+"X-Generator: Poedit 3.3.1\n"
 
 #: modules/FlaskModule/API/device/DeviceLogin.py:82
 msgid "Unable to get online devices."
 msgstr "Impossible d'obtenir les appareils connectés."
 
 #: modules/FlaskModule/API/device/DeviceLogin.py:98
 msgid "Device already logged in."
@@ -45,23 +46,35 @@
 #: modules/FlaskModule/API/device/DeviceQueryDevices.py:82
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:49
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:55
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:62
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:68
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:74
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:80
-#: modules/FlaskModule/API/service/ServiceQueryProjects.py:41
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:52
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:57
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:99
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:106
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:158
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:112
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:100
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:104
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:108
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:116
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:194
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:86
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:91
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:66
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:72
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:76
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:84
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:90
 #: modules/FlaskModule/API/service/ServiceQuerySites.py:36
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:96
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:197
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:301
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:122
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:257
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:112
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:166
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:105
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:191
@@ -72,53 +85,55 @@
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:60
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:66
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:72
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:78
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:84
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:107
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:159
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:350
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:353
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:198
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:269
-#: modules/FlaskModule/API/user/UserQueryProjects.py:145
-#: modules/FlaskModule/API/user/UserQueryProjects.py:150
-#: modules/FlaskModule/API/user/UserQueryProjects.py:258
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:112
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:363
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:366
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:204
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:275
+#: modules/FlaskModule/API/user/UserQueryProjects.py:151
+#: modules/FlaskModule/API/user/UserQueryProjects.py:156
+#: modules/FlaskModule/API/user/UserQueryProjects.py:264
 #: modules/FlaskModule/API/user/UserQueryServiceAccess.py:117
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:121
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:129
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:208
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:212
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:216
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:220
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:122
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:126
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:134
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:213
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:217
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:221
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:225
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:151
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:155
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:159
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:165
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:240
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:245
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:249
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:253
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:79
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:136
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:129
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:259
 #: modules/FlaskModule/API/user/UserQueryServices.py:121
 #: modules/FlaskModule/API/user/UserQueryServices.py:134
 #: modules/FlaskModule/API/user/UserQueryServices.py:231
 #: modules/FlaskModule/API/user/UserQueryServices.py:239
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:91
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:144
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:204
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:203
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:267
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:55
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:107
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:138
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:183
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:266
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:187
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:270
 #: modules/FlaskModule/API/user/UserQuerySites.py:124
 #: modules/FlaskModule/API/user/UserQuerySites.py:127
 #: modules/FlaskModule/API/user/UserQuerySites.py:176
 #: modules/FlaskModule/API/user/UserQueryStats.py:51
 #: modules/FlaskModule/API/user/UserQueryStats.py:56
 #: modules/FlaskModule/API/user/UserQueryStats.py:61
 #: modules/FlaskModule/API/user/UserQueryStats.py:67
@@ -134,31 +149,53 @@
 #: modules/FlaskModule/API/user/UserQueryTests.py:140
 #: modules/FlaskModule/API/user/UserQueryUserGroups.py:147
 #: modules/FlaskModule/API/user/UserQueryUserPreferences.py:47
 #: modules/FlaskModule/API/user/UserQueryUserPreferences.py:96
 #: modules/FlaskModule/API/user/UserQueryUsers.py:214
 #: modules/FlaskModule/API/user/UserQueryUsers.py:219
 #: modules/FlaskModule/API/user/UserQueryUsers.py:348
+#: opentera/services/ServiceAccessManager.py:116
+#: opentera/services/ServiceAccessManager.py:166
+#: opentera/services/ServiceAccessManager.py:195
+#: opentera/services/ServiceAccessManager.py:214
+#: opentera/services/ServiceAccessManager.py:242
+#: opentera/services/ServiceAccessManager.py:297
+#: opentera/services/ServiceAccessManager.py:411
+#: opentera/services/ServiceAccessManager.py:417
+#: opentera/services/ServiceAccessManager.py:428
 msgid "Forbidden"
 msgstr "Accès refusé"
 
 #: modules/FlaskModule/API/device/DeviceQueryDevices.py:93
 #: modules/FlaskModule/API/device/DeviceQuerySessionEvents.py:74
 #: modules/FlaskModule/API/device/DeviceQuerySessionEvents.py:89
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:156
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:233
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:247
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:284
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:116
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:138
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:176
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:73
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:94
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:123
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:138
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:150
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:172
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:205
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:104
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:119
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:185
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:218
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:234
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:245
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:280
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:141
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:158
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:215
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:180
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:221
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:276
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:331
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:232
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:268
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:130
@@ -169,27 +206,30 @@
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:189
 #: modules/FlaskModule/API/user/UserQueryDevices.py:328
 #: modules/FlaskModule/API/user/UserQueryDevices.py:343
 #: modules/FlaskModule/API/user/UserQueryDevices.py:460
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:120
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:135
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:178
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:239
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:280
-#: modules/FlaskModule/API/user/UserQueryProjects.py:190
-#: modules/FlaskModule/API/user/UserQueryProjects.py:205
-#: modules/FlaskModule/API/user/UserQueryProjects.py:276
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:151
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:163
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:185
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:231
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:245
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:286
+#: modules/FlaskModule/API/user/UserQueryProjects.py:196
+#: modules/FlaskModule/API/user/UserQueryProjects.py:211
+#: modules/FlaskModule/API/user/UserQueryProjects.py:282
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:156
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:168
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:190
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:236
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:208
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:264
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:287
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:322
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:98
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:119
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:147
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:244
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:286
 #: modules/FlaskModule/API/user/UserQueryServices.py:162
 #: modules/FlaskModule/API/user/UserQueryServices.py:182
 #: modules/FlaskModule/API/user/UserQueryServices.py:259
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:104
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:119
@@ -200,16 +240,16 @@
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:286
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:197
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:212
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:342
 #: modules/FlaskModule/API/user/UserQuerySessions.py:179
 #: modules/FlaskModule/API/user/UserQuerySessions.py:194
 #: modules/FlaskModule/API/user/UserQuerySessions.py:272
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:237
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:277
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:241
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:281
 #: modules/FlaskModule/API/user/UserQuerySites.py:140
 #: modules/FlaskModule/API/user/UserQuerySites.py:155
 #: modules/FlaskModule/API/user/UserQuerySites.py:194
 #: modules/FlaskModule/API/user/UserQueryTestType.py:216
 #: modules/FlaskModule/API/user/UserQueryTestType.py:231
 #: modules/FlaskModule/API/user/UserQueryTestType.py:345
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:252
@@ -229,23 +269,25 @@
 #: modules/FlaskModule/API/user/UserQueryUsers.py:272
 #: modules/FlaskModule/API/user/UserQueryUsers.py:385
 msgid "Database error"
 msgstr "Erreur de base de données"
 
 #: modules/FlaskModule/API/device/DeviceQueryParticipants.py:41
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:82
-#: modules/FlaskModule/API/service/ServiceQueryProjects.py:56
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:72
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:67
 #: modules/FlaskModule/API/service/ServiceQueryServices.py:76
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:62
 #: modules/FlaskModule/API/service/ServiceQuerySessions.py:122
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:109
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:86
-#: modules/FlaskModule/API/user/UserQueryProjects.py:110
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:80
+#: modules/FlaskModule/API/user/UserQueryProjects.py:116
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:84
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:123
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:67
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:112
 #: modules/FlaskModule/API/user/UserQueryServices.py:104
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:62
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:101
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:79
 #: modules/FlaskModule/API/user/UserQuerySessions.py:103
 #: modules/FlaskModule/API/user/UserQuerySites.py:97
@@ -268,28 +310,29 @@
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:95
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:99
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:104
 #: modules/FlaskModule/API/device/DeviceQueryStatus.py:48
 #: modules/FlaskModule/API/service/ServiceQueryAssets.py:270
 #: modules/FlaskModule/API/service/ServiceQueryDevices.py:73
 #: modules/FlaskModule/API/service/ServiceQueryDevices.py:87
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:68
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:83
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:69
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:84
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:49
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:46
 #: modules/FlaskModule/API/service/ServiceQuerySiteProjectAccessRoles.py:43
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:266
 #: modules/FlaskModule/API/service/ServiceQueryUsers.py:38
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:70
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:65
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:61
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:157
-#: modules/FlaskModule/API/user/UserQueryForms.py:82
+#: modules/FlaskModule/API/user/UserQueryForms.py:85
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:76
 #: modules/FlaskModule/API/user/UserQueryProjectAccess.py:81
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:52
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:53
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:63
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:60
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:46
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:62
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:59
 #: modules/FlaskModule/API/user/UserQuerySessions.py:59
 #: modules/FlaskModule/API/user/UserQuerySiteAccess.py:80
@@ -297,19 +340,17 @@
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:60
 msgid "Missing arguments"
 msgstr "Arguments manquants"
 
 #: modules/FlaskModule/API/device/DeviceQuerySessionEvents.py:61
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:114
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:137
-#: modules/LoginModule/LoginModule.py:595
-#: modules/LoginModule/LoginModule.py:695
-#: modules/LoginModule/LoginModule.py:762
-#: modules/LoginModule/LoginModule.py:789
-#: modules/LoginModule/LoginModule.py:808
+#: modules/LoginModule/LoginModule.py:587 modules/LoginModule/LoginModule.py:687
+#: modules/LoginModule/LoginModule.py:753 modules/LoginModule/LoginModule.py:780
+#: modules/LoginModule/LoginModule.py:799
 msgid "Unauthorized"
 msgstr "Non autorisé"
 
 #: modules/FlaskModule/API/device/DeviceQuerySessions.py:119
 msgid "Missing argument 'session name'"
 msgstr "Paramètre 'session name' manquant"
 
@@ -341,19 +382,19 @@
 msgid "Participant already logged in."
 msgstr "Le participant est déjà connecté."
 
 #: modules/FlaskModule/API/participant/ParticipantLogin.py:126
 msgid "Missing current_participant"
 msgstr "Champ current_participant manquant"
 
-#: modules/FlaskModule/API/participant/ParticipantLogout.py:33
+#: modules/FlaskModule/API/participant/ParticipantLogout.py:41
 msgid "Participant logged out."
 msgstr "Participant hors ligne."
 
-#: modules/FlaskModule/API/participant/ParticipantLogout.py:35
+#: modules/FlaskModule/API/participant/ParticipantLogout.py:43
 msgid "Participant not logged in"
 msgstr "Le participant n'est pas connecté"
 
 #: modules/FlaskModule/API/participant/ParticipantQueryParticipants.py:55
 #: modules/FlaskModule/API/participant/ParticipantQuerySessions.py:73
 msgid "Not implemented"
 msgstr "Non implémenté"
@@ -481,29 +522,125 @@
 msgstr "Sous-type d'appareil inconnu"
 
 #: modules/FlaskModule/API/service/ServiceQueryDisconnect.py:84
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:88
 msgid "Success"
 msgstr "Succès"
 
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:89
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:90
 msgid "Unknown project"
 msgstr "Projet inconnu"
 
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:92
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:93
 msgid "Invalid participant name"
 msgstr "Nom de participant incorrect"
 
-#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:95
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:96
 msgid "Invalid participant email"
 msgstr "Courriel de participant incorrect"
 
-#: modules/FlaskModule/API/service/ServiceQueryProjects.py:37
-msgid "Missing project id"
-msgstr "ID de projet manquant"
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:120
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:312
+msgid "Can't insert participant: participant's project is disabled or invalid."
+msgstr ""
+"Impossible d'ajouter le participant: le projet du participant est désactivé ou "
+"invalide."
+
+#: modules/FlaskModule/API/service/ServiceQueryParticipants.py:130
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:285
+msgid "Can't update participant: participant's project is disabled."
+msgstr ""
+"Impossible de mettre à jour le participant: le projet du participant est "
+"désactivé."
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:48
+msgid "Missing parameter"
+msgstr "Paramètre manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:87
+#: modules/FlaskModule/API/user/UserQueryProjects.py:132
+msgid "Missing project"
+msgstr "Projet manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:93
+#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:180
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:198
+#: modules/FlaskModule/API/user/UserQueryProjects.py:138
+#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:179
+msgid "Missing id_project"
+msgstr "Champ manquant : id_project"
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:96
+#: modules/FlaskModule/API/user/UserQueryProjects.py:140
+msgid "Missing id_site arguments"
+msgstr "Champ id_site manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryProjects.py:169
+#: modules/FlaskModule/API/user/UserQueryProjects.py:275
+msgid ""
+"Can't delete project: please delete all participants with sessions before "
+"deleting."
+msgstr ""
+"Impossible de supprimer le projet: veuillez supprimer tous les participants "
+"ayant des séances au préalable."
+
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:52
+msgid "Missing service_role field"
+msgstr "Champ iservice_role manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:58
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:154
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:172
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:85
+msgid "Missing id_service_role"
+msgstr "Champ id_service_role manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryRoles.py:81
+#: modules/FlaskModule/API/user/UserQueryServiceRoles.py:106
+msgid "Missing fields"
+msgstr "Champs manquants"
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:87
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:104
+msgid "Missing service_access"
+msgstr "Accès Service manquant (service_access)"
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:91
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:108
+msgid "Missing id_service_access"
+msgstr "Champ manquant: id_service_access"
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:95
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:112
+msgid "Can't combine id_user_group, id_participant_group and id_device in request"
+msgstr ""
+"Ne peut pas combiner id_user_group, id_participant et id_device dans  la requête"
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:114
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:132
+msgid "Bad id_service_role"
+msgstr "Mauvais id_service_role"
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:158
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:176
+#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:192
+msgid "Missing at least one id field"
+msgstr "Au moins un champ id manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryServiceAccess.py:191
+#: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:203
+#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:296
+#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:209
+#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:63
+#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:308
+#: modules/FlaskModule/API/user/UserQueryServiceSites.py:266
+#: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:270
+#: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:271
+msgid "Not found"
+msgstr "Non trouvé"
 
 #: modules/FlaskModule/API/service/ServiceQueryServices.py:38
 msgid "Missing service key, id or uuid"
 msgstr "Clé, ID ou UUID de service manquant"
 
 #: modules/FlaskModule/API/service/ServiceQuerySessionEvents.py:76
 #: modules/FlaskModule/API/user/UserQuerySessionEvents.py:77
@@ -568,14 +705,60 @@
 msgid "Service can't create tests for that session"
 msgstr "Le service ne peut pas créer de tests pour cette séance"
 
 #: modules/FlaskModule/API/service/ServiceQueryTests.py:269
 msgid "Service can't delete tests for that session"
 msgstr "Le service ne peut pas effacer les tests de cette séance"
 
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:71
+#: modules/FlaskModule/API/user/UserQueryUserGroups.py:132
+msgid "Missing user_group"
+msgstr "Champ user_group manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:78
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:196
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:179
+#: modules/FlaskModule/API/user/UserQueryUserGroups.py:139
+#: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:102
+msgid "Missing id_user_group"
+msgstr "Champ id_user_group manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:90
+msgid "Missing service role name or id_service_role"
+msgstr "Nom du rôle ou id_service_role manquant"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:103
+msgid "Can't set access to service other than self"
+msgstr "Impossible d'ajuster les accès à un service autre que soi-même."
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:109
+msgid "No access for at a least one project in the list"
+msgstr "Aucun accès pour au moins un projet dans la liste"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:115
+msgid "No access for at a least one site in the list"
+msgstr "Aucun accès pour au moins un site dans la liste"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:127
+msgid "Bad role name for service"
+msgstr "Nom de rôle invalide pour le service"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:145
+msgid "A new usergroup must have at least one service access"
+msgstr "Un nouveau groupe utilisateur doit avoir au moins un accès à un service"
+
+#: modules/FlaskModule/API/service/ServiceQueryUserGroups.py:207
+#: modules/FlaskModule/API/user/UserQueryUserGroups.py:300
+msgid ""
+"Can't delete user group: please delete all users part of that user group before "
+"deleting."
+msgstr ""
+"Impossible de supprimer le groupe d'utilisateurs: veuillez retirer tous les "
+"utilisateurs de ce groupe au préalable."
+
 #: modules/FlaskModule/API/service/ServiceSessionManager.py:116
 #: modules/FlaskModule/API/user/UserSessionManager.py:107
 msgid "Missing action"
 msgstr "Action manquante"
 
 #: modules/FlaskModule/API/service/ServiceSessionManager.py:131
 #: modules/FlaskModule/API/user/UserSessionManager.py:121
@@ -628,43 +811,42 @@
 msgid "Invalid client name :"
 msgstr "Nom du client invalide :"
 
 #: modules/FlaskModule/API/user/UserLogin.py:143
 msgid "Invalid client version handler"
 msgstr "Mauvaise version du client"
 
-#: modules/FlaskModule/API/user/UserLogout.py:27
+#: modules/FlaskModule/API/user/UserLogout.py:34
 msgid "User logged out."
 msgstr "Utilisateur déconnecté."
 
-#: modules/FlaskModule/API/user/UserLogout.py:29
+#: modules/FlaskModule/API/user/UserLogout.py:36
 msgid "User not logged in"
 msgstr "L'utilisateur n'est pas connecté"
 
 #: modules/FlaskModule/API/user/UserQueryAssets.py:79
 msgid "Service access denied"
 msgstr "Accès au service refusé"
 
 #: modules/FlaskModule/API/user/UserQueryAssets.py:174
 msgid ""
-"Asset information update and creation must be done directly into a "
-"service (such as Filetransfer service)"
+"Asset information update and creation must be done directly into a service (such "
+"as Filetransfer service)"
 msgstr ""
-"La création et la mise à jour d'information sur les ressources doivent "
-"être fait directement dans un service (comme le service de transfert de "
-"fichiers - FileTransfer)"
+"La création et la mise à jour d'information sur les ressources doivent être fait "
+"directement dans un service (comme le service de transfert de fichiers - "
+"FileTransfer)"
 
 #: modules/FlaskModule/API/user/UserQueryAssets.py:182
 msgid ""
 "Asset information deletion must be done directly into a service (such as "
 "Filetransfer service)"
 msgstr ""
-"La suppression d'information sur les ressources doivent être fait "
-"directement dans un service (comme le service de transfert de fichiers - "
-"FileTransfer)"
+"La suppression d'information sur les ressources doivent être fait directement "
+"dans un service (comme le service de transfert de fichiers - FileTransfer)"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:128
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:207
 msgid "User is not admin of the participant's project"
 msgstr "L’utilisateur n’est pas administrateur du projet du participant"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:131
@@ -672,25 +854,14 @@
 msgid "Access denied to device"
 msgstr "Aucun accès à l’appareil"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:149
 msgid "Device not assigned to project or participant"
 msgstr "Appareil non assigné à un projet ou un participant"
 
-#: modules/FlaskModule/API/user/UserQueryDeviceParticipants.py:203
-#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:296
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:204
-#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:63
-#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:308
-#: modules/FlaskModule/API/user/UserQueryServiceSites.py:266
-#: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:270
-#: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:271
-msgid "Not found"
-msgstr "Non trouvé"
-
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:141
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:127
 #: modules/FlaskModule/API/user/UserQueryDevices.py:259
 msgid "Missing id_device"
 msgstr "Champ manquant : id_device"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:143
@@ -719,73 +890,63 @@
 msgid "Access denied"
 msgstr "Accès refusé"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:172
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:208
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:321
 msgid ""
-"Can't delete device from project. Please remove all participants "
-"associated with the device or all sessions in the project referring to "
-"the device before deleting."
+"Can't delete device from project. Please remove all participants associated with "
+"the device or all sessions in the project referring to the device before "
+"deleting."
 msgstr ""
 "Impossible de retirer l'appareil du projet: veuillez retirer tous les "
-"participants associés à cet appareil et/ou toutes les séances de ce "
-"projet impliquant cet appareil."
-
-#: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:180
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:192
-#: modules/FlaskModule/API/user/UserQueryProjects.py:132
-#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:179
-msgid "Missing id_project"
-msgstr "Champ manquant : id_project"
+"participants associés à cet appareil et/ou toutes les séances de ce projet "
+"impliquant cet appareil."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:182
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:157
 msgid "Missing devices"
 msgstr "Appareils manquants"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:238
-msgid ""
-"At least one device is not part of the allowed device for that project "
-"site"
+msgid "At least one device is not part of the allowed device for that project site"
 msgstr "Au moins un appareil n'est pas admissible pour ce projet pour ce site"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:314
 msgid ""
-"Can't delete device from project: please remove all participants with "
-"device before deleting."
+"Can't delete device from project: please remove all participants with device "
+"before deleting."
 msgstr ""
-"Impossible de retirer l'appareil du projet: veuillez désassocier tous les"
-" participants liés à cet appareil dans ce projet au préalable."
+"Impossible de retirer l'appareil du projet: veuillez désassocier tous les "
+"participants liés à cet appareil dans ce projet au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceProjects.py:317
 msgid ""
-"Can't delete device from project: please remove all sessions in this "
-"project referring to that device before deleting."
+"Can't delete device from project: please remove all sessions in this project "
+"referring to that device before deleting."
 msgstr ""
-"Impossible de retirer l'appareil du projet: veuillez retirer toutes les "
-"séances impliquant cet appareil dans ce projet au préalable."
+"Impossible de retirer l'appareil du projet: veuillez retirer toutes les séances "
+"impliquant cet appareil dans ce projet au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:129
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:136
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:123
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:121
 msgid "Missing sites"
 msgstr "Sites manquants"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:148
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:175
 msgid ""
-"Can't delete device from site. Please remove all participants associated "
-"with the device or all sessions in the site referring to the device "
-"before deleting."
+"Can't delete device from site. Please remove all participants associated with "
+"the device or all sessions in the site referring to the device before deleting."
 msgstr ""
-"Impossible de retirer l'appareil du site: veuillez retirer tous les "
-"participants associés à cet appareil dans ce site et/ou toutes les "
-"séances de ce site impliquant cet appareil."
+"Impossible de retirer l'appareil du site: veuillez retirer tous les participants "
+"associés à cet appareil dans ce site et/ou toutes les séances de ce site "
+"impliquant cet appareil."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceSites.py:155
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:164
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:158
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:150
 msgid "Missing site ID"
 msgstr "Champ id_site manquant"
@@ -831,31 +992,31 @@
 
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:170
 msgid "Device subtype not found"
 msgstr "Sous-type d'appareil non trouvé"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:180
 msgid ""
-"Can't delete device subtype: please delete all devices of that subtype "
-"before deleting."
+"Can't delete device subtype: please delete all devices of that subtype before "
+"deleting."
 msgstr ""
-"Impossible de supprimer le sous-type d'appareil: veuillez supprimer ou "
-"modifier tous les appareils utilisant ce sous-type au préalable."
+"Impossible de supprimer le sous-type d'appareil: veuillez supprimer ou modifier "
+"tous les appareils utilisant ce sous-type au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceSubTypes.py:190
 msgid "Device subtype successfully deleted"
 msgstr "Sous-type d'appareil supprimé avec succès"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:60
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:65
 msgid "Unexisting ID/Forbidden access"
 msgstr "ID inexistant/Accès interdit"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:79
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:387
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:400
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:182
 msgid "Database Error"
 msgstr "Erreur de bases de données"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:95
 msgid "Missing device type"
 msgstr "Champ device_type manquant"
@@ -875,16 +1036,15 @@
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:168
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:171
 msgid "Device type not found"
 msgstr "Type d'appareil non trouvé"
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:181
 msgid ""
-"Can't delete device type: please delete all associated devices before "
-"deleting."
+"Can't delete device type: please delete all associated devices before deleting."
 msgstr ""
 "Impossible de supprimer le type d'appareil: veuillez supprimer tous les "
 "appareils associés au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDeviceTypes.py:193
 msgid "Device type successfully deleted"
 msgstr "Type d'appareil supprimé avec succès"
@@ -910,82 +1070,87 @@
 #: modules/FlaskModule/API/user/UserQueryDevices.py:412
 #: modules/FlaskModule/API/user/UserQueryUsers.py:343
 msgid "Invalid id"
 msgstr "ID invalide"
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:436
 msgid ""
-"Can't delete device: please delete all participants association before "
-"deleting."
+"Can't delete device: please delete all participants association before deleting."
 msgstr ""
-"Impossible de supprimer l'appareil: veuillez supprimer ou retirer tous "
-"les participants associés au préalable."
+"Impossible de supprimer l'appareil: veuillez supprimer ou retirer tous les "
+"participants associés au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:439
 msgid ""
-"Can't delete device: please remove all sessions referring to that device "
-"before deleting."
+"Can't delete device: please remove all sessions referring to that device before "
+"deleting."
 msgstr ""
 "Impossible de supprimer l'appareil: veuillez retirer toutes les séances "
 "impliquant cet appareil."
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:442
 msgid ""
-"Can't delete device: please remove all sessions created by that device "
-"before deleting."
+"Can't delete device: please remove all sessions created by that device before "
+"deleting."
 msgstr ""
-"Impossible de supprimer l'appareil: veuillez retirer toutes les séances "
-"créées par cet appareil au préalable."
+"Impossible de supprimer l'appareil: veuillez retirer toutes les séances créées "
+"par cet appareil au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:445
 msgid ""
-"Can't delete device: please delete all assets created by that device "
-"before deleting."
+"Can't delete device: please delete all assets created by that device before "
+"deleting."
 msgstr ""
-"Impossible de supprimer l'appareil: veuillez supprimer toutes les "
-"ressources crées par cet appareil au préalable."
+"Impossible de supprimer l'appareil: veuillez supprimer toutes les ressources "
+"crées par cet appareil au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:448
 msgid ""
-"Can't delete device: please delete all tests created by that device "
-"before deleting."
+"Can't delete device: please delete all tests created by that device before "
+"deleting."
 msgstr ""
-"Impossible de supprimer l'appareil: veuillez supprimer tous les tests "
-"créés par cet appareil au préalable."
+"Impossible de supprimer l'appareil: veuillez supprimer tous les tests créés par "
+"cet appareil au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:451
 msgid ""
-"Can't delete device: please remove all related sessions, assets and tests"
-" before deleting."
+"Can't delete device: please remove all related sessions, assets and tests before "
+"deleting."
 msgstr ""
 "Impossible de supprimer l'appareil: veuillez retirer toutes les séances, "
 "ressources et tests associés au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryDevices.py:469
 msgid "Device successfully deleted"
 msgstr "Appareil supprimé avec succès"
 
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:49
 #: modules/FlaskModule/API/user/UserQueryDisconnect.py:57
 msgid "Use Logout instead to disconnect current user"
 msgstr "Utilisez l'API de Logout pour déconnecter l'utilisateur actuel"
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:79
+#: modules/FlaskModule/API/user/UserQueryForms.py:82
 msgid "Missing type"
 msgstr "Champ type manquant"
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:134
+#: modules/FlaskModule/API/user/UserQueryForms.py:137
 msgid "Missing session type id"
 msgstr "Champ id_session_type manquant"
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:167
+#: modules/FlaskModule/API/user/UserQueryForms.py:148
+msgid "No reply from service while querying session type config"
+msgstr ""
+"Aucune réponse du service lors de la requête de la configuration du type de "
+"séance."
+
+#: modules/FlaskModule/API/user/UserQueryForms.py:182
 msgid "Invalid service specified"
 msgstr "Service non valide"
 
-#: modules/FlaskModule/API/user/UserQueryForms.py:180
+#: modules/FlaskModule/API/user/UserQueryForms.py:195
 msgid "Unknown form type: "
 msgstr "Formulaire inconnu: "
 
 #: modules/FlaskModule/API/user/UserQueryOnlineDevices.py:60
 #: modules/FlaskModule/API/user/UserQueryOnlineParticipants.py:59
 #: modules/FlaskModule/API/user/UserQueryOnlineUsers.py:57
 msgid "Internal server error when making RPC call."
@@ -997,19 +1162,19 @@
 
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:102
 msgid "Missing id_participant_group or id_project"
 msgstr "Champs id_participant_group ou id_project manquants"
 
 #: modules/FlaskModule/API/user/UserQueryParticipantGroup.py:170
 msgid ""
-"Can't delete participant group: please delete all sessions from all "
-"participants before deleting."
+"Can't delete participant group: please delete all sessions from all participants "
+"before deleting."
 msgstr ""
-"Impossible de supprimer le groupe: veuillez supprimer toutes les séances "
-"de tous les participants du groupe au préalable."
+"Impossible de supprimer le groupe: veuillez supprimer toutes les séances de tous "
+"les participants du groupe au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:220
 msgid "Missing participant"
 msgstr "Participant manquant"
 
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:226
 msgid "Missing id_participant"
@@ -1031,118 +1196,80 @@
 msgid "Participant group not found."
 msgstr "Le groupe participant n'existe pas."
 
 #: modules/FlaskModule/API/user/UserQueryParticipants.py:266
 msgid "Mismatch between id_project and group's project"
 msgstr "Aucune correspondance entre id_project et le projet"
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:370
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:383
 msgid "Can't delete participant: please remove all related sessions beforehand."
 msgstr ""
-"Impossible de supprimer le participant: veuillez supprimer toutes les "
-"séances de ce participant au préalable."
+"Impossible de supprimer le participant: veuillez supprimer toutes les séances de "
+"ce participant au préalable."
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:372
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:385
 msgid ""
-"Can't delete participant: please remove all sessions created by this "
-"participant beforehand."
+"Can't delete participant: please remove all sessions created by this participant "
+"beforehand."
 msgstr ""
-"Impossible de supprimer le participant: veuillez supprimer toutes les "
-"séances créées par ce participant au préalable."
+"Impossible de supprimer le participant: veuillez supprimer toutes les séances "
+"créées par ce participant au préalable."
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:375
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:388
 msgid "Can't delete participant: please remove all related assets beforehand."
 msgstr ""
-"Impossible de supprimer le participant: veuillez supprimer toutes les "
-"ressources de ce participant au préalable."
+"Impossible de supprimer le participant: veuillez supprimer toutes les ressources "
+"de ce participant au préalable."
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:377
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:390
 msgid "Can't delete participant: please remove all related tests beforehand."
 msgstr ""
-"Impossible de supprimer le participant: veuillez supprimer tous les tests"
-" associés à ce participant au préalable."
+"Impossible de supprimer le participant: veuillez supprimer tous les tests "
+"associés à ce participant au préalable."
 
-#: modules/FlaskModule/API/user/UserQueryParticipants.py:379
+#: modules/FlaskModule/API/user/UserQueryParticipants.py:392
 msgid ""
-"Can't delete participant: please remove all related sessions, assets and "
-"tests before deleting."
+"Can't delete participant: please remove all related sessions, assets and tests "
+"before deleting."
 msgstr ""
-"Impossible de supprimer le participant: veuillez retirer toutes les "
-"séances, ressources et tests associés à ce participant au préalable."
+"Impossible de supprimer le participant: veuillez retirer toutes les séances, "
+"ressources et tests associés à ce participant au préalable."
 
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:190
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:175
-#: modules/FlaskModule/API/user/UserQueryUserGroups.py:139
-#: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:102
-msgid "Missing id_user_group"
-msgstr "Champ id_user_group manquant"
-
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:194
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:179
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:200
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:183
 msgid "Missing role name or id"
 msgstr "Nom du rôle ou ID manquant"
 
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:223
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:229
 msgid "Invalid role name or id for that project"
 msgstr "Nom du rôle ou ID invalide pour ce projet"
 
-#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:265
+#: modules/FlaskModule/API/user/UserQueryProjectAccess.py:271
 msgid "No project access to delete."
 msgstr "Aucun accès au projet pour supprimer."
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:126
-msgid "Missing project"
-msgstr "Projet manquant"
-
-#: modules/FlaskModule/API/user/UserQueryProjects.py:134
-msgid "Missing id_site arguments"
-msgstr "Champ id_site manquant"
-
-#: modules/FlaskModule/API/user/UserQueryProjects.py:163
+#: modules/FlaskModule/API/user/UserQueryProjects.py:169
 msgid "No access to a session type for at least one of it"
 msgstr "Pas d'accès à ce type de session pour au moins un projet"
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:175
+#: modules/FlaskModule/API/user/UserQueryProjects.py:181
 msgid "At least one session type is not associated to the project site"
 msgstr "Au moins un type de séance n’est pas associé au site du projet"
 
-#: modules/FlaskModule/API/user/UserQueryProjects.py:269
-msgid ""
-"Can't delete project: please delete all participants with sessions before"
-" deleting."
-msgstr ""
-"Impossible de supprimer le projet: veuillez supprimer tous les "
-"participants ayant des séances au préalable."
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:99
-msgid "Missing service_access"
-msgstr "Accès Service manquant (service_access)"
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:103
-msgid "Missing id_service_access"
-msgstr "Champ manquant: id_service_access"
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:107
-msgid "Can't combine id_user_group, id_participant_group and id_device in request"
-msgstr ""
-"Ne peut pas combiner id_user_group, id_participant et id_device dans  la "
-"requête"
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:127
-msgid "Bad id_service_role"
-msgstr "Mauvais id_service_role"
-
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:167
-msgid "Missing id_service_role"
-msgstr "Champ id_service_role manquant"
+#: modules/FlaskModule/API/user/UserQueryServiceAccessToken.py:35
+#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:189
+#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:142
+#: modules/FlaskModule/API/user/UserQueryServiceSites.py:134
+#: modules/FlaskModule/API/user/UserQueryServices.py:128
+msgid "Missing id_service"
+msgstr "Champ id_service manquant"
 
-#: modules/FlaskModule/API/user/UserQueryServiceAccess.py:171
-#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:192
-msgid "Missing at least one id field"
-msgstr "Au moins un champ id manquant"
+#: modules/FlaskModule/API/user/UserQueryServiceAccessToken.py:38
+msgid "No access to specified service"
+msgstr "Aucun accès au service spécifié"
 
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:72
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:146
 msgid "Can't combine id_user, id_participant and id_device in request"
 msgstr "Ne peut pas combiner id_user, id_participant et id_device dans la requête"
 
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:121
@@ -1150,77 +1277,67 @@
 msgstr "Champ service_config manquant"
 
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:175
 #: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:198
 msgid "Invalid config format provided"
 msgstr "Le format de la configuration est invalide"
 
-#: modules/FlaskModule/API/user/UserQueryServiceConfigs.py:189
-#: modules/FlaskModule/API/user/UserQueryServiceProjects.py:142
-#: modules/FlaskModule/API/user/UserQueryServiceSites.py:134
-#: modules/FlaskModule/API/user/UserQueryServices.py:128
-msgid "Missing id_service"
-msgstr "Champ id_service manquant"
-
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:170
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:211
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:339
 msgid ""
-"Can't delete service-project: please remove all related sessions, assets "
-"and tests before deleting."
+"Can't delete service-project: please remove all related sessions, assets and "
+"tests before deleting."
 msgstr ""
-"Impossible de retirer ce service de ce projet: veuillez supprimer toutes "
-"les séances, ressources et tests en lien avec ce service au préalable."
+"Impossible de retirer ce service de ce projet: veuillez supprimer toutes les "
+"séances, ressources et tests en lien avec ce service au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:181
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:166
 msgid "Missing services"
 msgstr "Services manquants"
 
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:249
 msgid ""
-"At least one service is not part of the allowed service for that project "
-"site"
+"At least one service is not part of the allowed service for that project site"
 msgstr "Au moins un service n'est pas permis pour ce projet pour ce site"
 
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:311
 msgid "Operation not completed"
 msgstr "Opération non complétée"
 
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:332
 msgid ""
-"Can't delete service-project: please remove all sessions involving a "
-"session type using this project beforehand."
+"Can't delete service-project: please remove all sessions involving a session "
+"type using this project beforehand."
 msgstr ""
-"Impossible de retirer ce service de ce projet: veuillez supprimer toutes "
-"les séances impliquant un type de séance en lien avec ce service au "
-"préalable."
+"Impossible de retirer ce service de ce projet: veuillez supprimer toutes les "
+"séances impliquant un type de séance en lien avec ce service au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:335
 msgid "Can't delete service-project: please remove all related assets beforehand."
 msgstr ""
-"Impossible de retirer ce service de ce projet: veuillez supprimer toutes "
-"les ressources associées au préalable."
+"Impossible de retirer ce service de ce projet: veuillez supprimer toutes les "
+"ressources associées au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryServiceProjects.py:337
 msgid "Can't delete service-project: please remove all related tests beforehand."
 msgstr ""
-"Impossible de retirer ce service de ce projet: veuillez supprimer tous "
-"les tests associés à ce service au préalable."
+"Impossible de retirer ce service de ce projet: veuillez supprimer tous les tests "
+"associés à ce service au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:155
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:185
 #: modules/FlaskModule/API/user/UserQueryServiceSites.py:278
 msgid ""
-"Can't delete service from site: please delete all sessions, assets and "
-"tests related to that service beforehand."
+"Can't delete service from site: please delete all sessions, assets and tests "
+"related to that service beforehand."
 msgstr ""
-"Impossible de retirer le service de ce site: veuillez supprimer toutes "
-"les séances, ressources et tests reliés à ce service dans ce site au "
-"préalable."
+"Impossible de retirer le service de ce site: veuillez supprimer toutes les "
+"séances, ressources et tests reliés à ce service dans ce site au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryServices.py:150
 msgid "OpenTera service can't be updated using this API"
 msgstr "Les services ne peuvent pas être mis-à-jour par cet API"
 
 #: modules/FlaskModule/API/user/UserQueryServices.py:164
 #: modules/FlaskModule/API/user/UserQueryServices.py:184
@@ -1233,28 +1350,28 @@
 
 #: modules/FlaskModule/API/user/UserQueryServices.py:236
 msgid "Invalid service"
 msgstr "Service invalide"
 
 #: modules/FlaskModule/API/user/UserQueryServices.py:251
 msgid ""
-"Can't delete service: please delete all sessions, assets and tests "
-"related to that service beforehand."
+"Can't delete service: please delete all sessions, assets and tests related to "
+"that service beforehand."
 msgstr ""
-"Impossible de supprimer le service: veuillez supprimer toutes les "
-"séances, ressources et tests reliés à ce service au préalable."
+"Impossible de supprimer le service: veuillez supprimer toutes les séances, "
+"ressources et tests reliés à ce service au préalable."
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:154
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:186
 msgid ""
-"Can't delete session type from project: please delete all sessions using "
-"that type in that project before deleting."
+"Can't delete session type from project: please delete all sessions using that "
+"type in that project before deleting."
 msgstr ""
-"Impossible de retirer le type de séance du projet: veuillez supprimer "
-"toutes les séances de ce type dans ce projet avant de supprimer."
+"Impossible de retirer le type de séance du projet: veuillez supprimer toutes les "
+"séances de ce type dans ce projet avant de supprimer."
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:161
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:164
 msgid "Missing project ID"
 msgstr "ID de projet manquant"
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:163
@@ -1269,29 +1386,29 @@
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:212
 msgid "At least one session type is not associated to the site of its project"
 msgstr "Au moins un type de session n'est pas associé au site de ce projet"
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypeProjects.py:283
 msgid ""
-"Can't delete session type from project: please delete all sessions of "
-"that type in the project before deleting."
+"Can't delete session type from project: please delete all sessions of that type "
+"in the project before deleting."
 msgstr ""
-"Impossible de retirer le type de séance du projet: veuillez supprimer "
-"toutes les séances de ce type dans ce projet avant de supprimer."
+"Impossible de retirer le type de séance du projet: veuillez supprimer toutes les "
+"séances de ce type dans ce projet avant de supprimer."
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:150
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:185
 #: modules/FlaskModule/API/user/UserQuerySessionTypeSites.py:278
 msgid ""
-"Can't delete session type from site: please delete all sessions of that "
-"type in the site before deleting."
+"Can't delete session type from site: please delete all sessions of that type in "
+"the site before deleting."
 msgstr ""
-"Impossible de retirer le type de séance du site: veuillez supprimer "
-"toutes les séances de ce type dans ce site au préalable."
+"Impossible de retirer le type de séance du site: veuillez supprimer toutes les "
+"séances de ce type dans ce site au préalable."
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:95
 msgid "Missing session_type"
 msgstr "Champ session_type manquant"
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:111
 msgid "Missing site(s) to associate that session type to"
@@ -1319,36 +1436,35 @@
 #: modules/FlaskModule/API/user/UserQueryTestType.py:280
 msgid "Session type not associated to project site"
 msgstr "Type de séance non associé au site du projet"
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:292
 msgid "Session type has a a service not associated to its site"
 msgstr ""
-"Tentative d'association avec un type de séance qui a un service non "
-"associé à son site"
+"Tentative d'association avec un type de séance qui a un service non associé à "
+"son site"
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:316
 #: modules/FlaskModule/API/user/UserQueryTestType.py:324
 msgid "Cannot delete because you are not admin in all projects."
 msgstr ""
-"Impossible de supprimer: vous n'êtes pas administrateur dans tous les "
-"projets."
+"Impossible de supprimer: vous n'êtes pas administrateur dans tous les projets."
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:321
 #: modules/FlaskModule/API/user/UserQueryTestType.py:328
 msgid "Unable to delete - not admin in at least one project"
 msgstr "Impossible de supprimer - pas administrateur dans au moins un projet"
 
 #: modules/FlaskModule/API/user/UserQuerySessionTypes.py:334
 msgid ""
-"Can't delete session type: please delete all sessions with that type "
-"before deleting."
+"Can't delete session type: please delete all sessions with that type before "
+"deleting."
 msgstr ""
-"Impossible de supprimer le type de séance: veuillez supprimer toutes les "
-"séances de ce type au préalable."
+"Impossible de supprimer le type de séance: veuillez supprimer toutes les séances "
+"de ce type au préalable."
 
 #: modules/FlaskModule/API/user/UserQuerySessions.py:135
 msgid "Missing session participants and users"
 msgstr "Usagers ou participants manquants pour la session"
 
 #: modules/FlaskModule/API/user/UserQuerySessions.py:141
 msgid "No access to session."
@@ -1369,41 +1485,40 @@
 msgid "User doesn't have access to at least one device of that session."
 msgstr "L'utilisateur n'a pas accès à au moins un appareil de la séance."
 
 #: modules/FlaskModule/API/user/UserQuerySessions.py:261
 msgid "Session is in progress: can't delete that session."
 msgstr "La séance est en cours: impossible de supprimer."
 
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:177
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:181
 msgid "Missing id_site"
 msgstr "Champ id_site manquant"
 
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:221
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:225
 msgid "Invalid role name or id for that site"
 msgstr "Nom de rôle ou id invalide(s) pour ce site"
 
-#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:262
+#: modules/FlaskModule/API/user/UserQuerySiteAccess.py:266
 msgid "No site access to delete"
 msgstr "Pas d'accès à effacer"
 
 #: modules/FlaskModule/API/user/UserQuerySites.py:112
 msgid "Missing site"
 msgstr "Site manquant"
 
 #: modules/FlaskModule/API/user/UserQuerySites.py:119
 msgid "Missing id_site field"
 msgstr "Champ id_site manquant"
 
 #: modules/FlaskModule/API/user/UserQuerySites.py:187
 msgid ""
-"Can't delete site: please delete all participants with sessions before "
-"deleting."
+"Can't delete site: please delete all participants with sessions before deleting."
 msgstr ""
-"Impossible de supprimer le site: veuillez supprimer tous les participants"
-" au préalable."
+"Impossible de supprimer le site: veuillez supprimer tous les participants au "
+"préalable."
 
 #: modules/FlaskModule/API/user/UserQueryStats.py:93
 msgid "Missing id argument"
 msgstr "Champ id manquant"
 
 #: modules/FlaskModule/API/user/UserQueryTestType.py:128
 msgid "Missing test_type"
@@ -1426,65 +1541,64 @@
 #: modules/FlaskModule/API/user/UserQueryTestType.py:186
 msgid "At least one site isn't associated with the service of that test type"
 msgstr "Au moins un site n'est pas associé avec le service de ce type de test"
 
 #: modules/FlaskModule/API/user/UserQueryTestType.py:300
 msgid "Test type has a a service not associated to its site"
 msgstr ""
-"Tentative d'association avec un type de test qui a un service non associé"
-" à son site"
+"Tentative d'association avec un type de test qui a un service non associé à son "
+"site"
 
 #: modules/FlaskModule/API/user/UserQueryTestType.py:338
 msgid ""
-"Can't delete test type: please delete all tests of that type before "
-"deleting."
+"Can't delete test type: please delete all tests of that type before deleting."
 msgstr ""
-"Impossible de supprimer le type de test: veuillez supprimer tous les "
-"tests de ce type au préalable."
+"Impossible de supprimer le type de test: veuillez supprimer tous les tests de ce "
+"type au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:141
 msgid "Access denied to at least one project"
 msgstr "Accès refusé pour au moins un projet"
 
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:157
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:188
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:285
 msgid ""
-"Can't delete test type from project: please delete all tests of that type"
-" in the project before deleting."
+"Can't delete test type from project: please delete all tests of that type in the "
+"project before deleting."
 msgstr ""
-"Impossible de supprimer le type de test: veuillez supprimer tous les "
-"tests de ce type au préalable."
+"Impossible de supprimer le type de test: veuillez supprimer tous les tests de ce "
+"type au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:166
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:152
 msgid "Missing test types"
 msgstr "Types de test manquants"
 
 #: modules/FlaskModule/API/user/UserQueryTestTypeProjects.py:213
 msgid "At least one test type is not associated to the site of its project"
 msgstr "Au moins un type de test n'est pas associé au site de ce projet"
 
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:143
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:176
 #: modules/FlaskModule/API/user/UserQueryTestTypeSites.py:266
 msgid ""
-"Can't delete test type from site: please delete all tests of that type in"
-" the site before deleting."
+"Can't delete test type from site: please delete all tests of that type in the "
+"site before deleting."
 msgstr ""
-"Impossible de retirer ce type de test du site: veuillez supprimer tous "
-"les tests de ce type dans ce site au préalable."
+"Impossible de retirer ce type de test du site: veuillez supprimer tous les tests "
+"de ce type dans ce site au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryTests.py:123
 msgid ""
-"Test information update and creation must be done directly into a service"
-" (such as Test service)"
+"Test information update and creation must be done directly into a service (such "
+"as Test service)"
 msgstr ""
-"La création et la mise à jour d'information sur les tests doivent être "
-"fait directement dans un service"
+"La création et la mise à jour d'information sur les tests doivent être fait "
+"directement dans un service"
 
 #: modules/FlaskModule/API/user/UserQueryUndelete.py:30
 msgid "No access to this API"
 msgstr "Aucun accès à cet API"
 
 #: modules/FlaskModule/API/user/UserQueryUndelete.py:46
 msgid "Item to undelete not found"
@@ -1494,30 +1608,18 @@
 msgid "Item can't be undeleted"
 msgstr "L'élément ne peut pas être restauré"
 
 #: modules/FlaskModule/API/user/UserQueryUndelete.py:52
 msgid "Item isn't deleted"
 msgstr "L'élément n'est pas supprimé"
 
-#: modules/FlaskModule/API/user/UserQueryUserGroups.py:132
-msgid "Missing user_group"
-msgstr "Champ user_group manquant"
-
 #: modules/FlaskModule/API/user/UserQueryUserGroups.py:142
 msgid "Missing user group name"
 msgstr "Nom du groupe utilisateur manquant"
 
-#: modules/FlaskModule/API/user/UserQueryUserGroups.py:300
-msgid ""
-"Can't delete user group: please delete all users part of that user group "
-"before deleting."
-msgstr ""
-"Impossible de supprimer le groupe d'utilisateurs: veuillez retirer tous "
-"les utilisateurs de ce groupe au préalable."
-
 #: modules/FlaskModule/API/user/UserQueryUserPreferences.py:89
 msgid "Missing app tag"
 msgstr "Champ App Tag manquant"
 
 #: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:57
 msgid "At least one id must be specified"
 msgstr "Au moins un ID doit être spécifié"
@@ -1538,16 +1640,15 @@
 #: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:108
 msgid "No access to specified user group"
 msgstr "Aucun accès au groupe utilisateurs"
 
 #: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:113
 msgid "Super admins can't be associated to an user group"
 msgstr ""
-"Les super administrateurs ne peuvent pas être associés à un groupe "
-"d'utilisateurs"
+"Les super administrateurs ne peuvent pas être associés à un groupe d'utilisateurs"
 
 #: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:158
 msgid "Can't delete specified relationship"
 msgstr "Impossible de supprimer cette relation"
 
 #: modules/FlaskModule/API/user/UserQueryUserUserGroups.py:161
 msgid "No access to relationship's user"
@@ -1583,51 +1684,48 @@
 
 #: modules/FlaskModule/API/user/UserQueryUsers.py:336
 msgid "Sorry, you can't delete yourself!"
 msgstr "Désolé, vous ne pouvez pas vous supprimer!"
 
 #: modules/FlaskModule/API/user/UserQueryUsers.py:366
 msgid ""
-"Can't delete user: please remove all sessions that this user is part of "
-"before deleting."
+"Can't delete user: please remove all sessions that this user is part of before "
+"deleting."
 msgstr ""
-"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les "
-"séances dont cet utilisateur fait partie au préalable."
+"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les séances "
+"dont cet utilisateur fait partie au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryUsers.py:369
 msgid ""
-"Can't delete user: please remove all sessions created by this user before"
-" deleting."
+"Can't delete user: please remove all sessions created by this user before "
+"deleting."
 msgstr ""
-"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les "
-"séances créées par cet utilisateur au préalable."
+"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les séances "
+"créées par cet utilisateur au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryUsers.py:372
 msgid ""
-"Can't delete user: please remove all tests created by this user before "
-"deleting."
+"Can't delete user: please remove all tests created by this user before deleting."
 msgstr ""
-"Impossible de supprimer l'utilisateur: veuillez supprimer tous les tests "
-"créés par cet utilisateur au préalable."
+"Impossible de supprimer l'utilisateur: veuillez supprimer tous les tests créés "
+"par cet utilisateur au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryUsers.py:375
 msgid ""
-"Can't delete user: please remove all assets created by this user before "
-"deleting."
+"Can't delete user: please remove all assets created by this user before deleting."
 msgstr ""
-"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les "
-"ressources créées par cet utilisateur au préalable."
+"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les ressources "
+"créées par cet utilisateur au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryUsers.py:378
 msgid ""
-"Can't delete user: please delete all assets created by this user before "
-"deleting."
+"Can't delete user: please delete all assets created by this user before deleting."
 msgstr ""
-"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les "
-"ressources créées par cet utilisateur au préalable."
+"Impossible de supprimer l'utilisateur: veuillez supprimer toutes les ressources "
+"créées par cet utilisateur au préalable."
 
 #: modules/FlaskModule/API/user/UserQueryVersions.py:69
 msgid "Wrong ClientVersions"
 msgstr "Mauvais version du client (ClientVersions)"
 
 #: modules/FlaskModule/API/user/UserQueryVersions.py:75
 msgid "Not authorized"
@@ -1650,35 +1748,32 @@
 msgstr "Manque le reply code dans les paramètres"
 
 #: modules/FlaskModule/API/user/UserSessionManager.py:181
 #: modules/FlaskModule/API/user/UserSessionManager.py:184
 msgid "Invalid reply code"
 msgstr "Le champ reply code est invalide"
 
-#: modules/LoginModule/LoginModule.py:630
-#: modules/LoginModule/LoginModule.py:663
+#: modules/LoginModule/LoginModule.py:622 modules/LoginModule/LoginModule.py:655
 msgid "Disabled device"
 msgstr "Appareil désactivé"
 
-#: modules/LoginModule/LoginModule.py:640
+#: modules/LoginModule/LoginModule.py:632
 msgid "Invalid token"
 msgstr "Jeton invalide"
 
-#: modules/LoginModule/LoginModule.py:740
+#: modules/LoginModule/LoginModule.py:732
 msgid "Invalid Token"
 msgstr "Jeton invalide"
 
-#: opentera/db/models/TeraSessionType.py:149
-#: opentera/forms/TeraSessionForm.py:105
+#: opentera/db/models/TeraSessionType.py:149 opentera/forms/TeraSessionForm.py:105
 msgid "Unknown"
 msgstr "Inconnue"
 
 #: opentera/db/models/TeraSessionType.py:151
-#: opentera/forms/TeraSessionTypeForm.py:35
-#: opentera/forms/TeraTestTypeForm.py:24
+#: opentera/forms/TeraSessionTypeForm.py:35 opentera/forms/TeraTestTypeForm.py:24
 msgid "Service"
 msgstr "Service"
 
 #: opentera/db/models/TeraSessionType.py:153
 msgid "File Transfer"
 msgstr "Transfert de fichiers"
 
@@ -1690,29 +1785,27 @@
 msgid "Protocol"
 msgstr "Protocole"
 
 #: opentera/forms/TeraDeviceForm.py:24 opentera/forms/TeraSessionForm.py:160
 msgid "Parameters"
 msgstr "Paramètres"
 
-#: opentera/forms/TeraDeviceForm.py:28
-#: opentera/forms/TeraServiceConfigForm.py:28
+#: opentera/forms/TeraDeviceForm.py:28 opentera/forms/TeraServiceConfigForm.py:28
 msgid "Device ID"
 msgstr "ID Appareil"
 
 #: opentera/forms/TeraDeviceForm.py:29
 msgid "Device UUID"
 msgstr "UUID Appareil"
 
 #: opentera/forms/TeraDeviceForm.py:30
 msgid "Device Name"
 msgstr "Nom Appareil"
 
-#: opentera/forms/TeraDeviceForm.py:31
-#: opentera/forms/TeraDeviceSubTypeForm.py:32
+#: opentera/forms/TeraDeviceForm.py:31 opentera/forms/TeraDeviceSubTypeForm.py:32
 #: opentera/forms/TeraDeviceTypeForm.py:21
 msgid "Device Type ID"
 msgstr "Type d'appareil"
 
 #: opentera/forms/TeraDeviceForm.py:33
 msgid "Device Sub-Type"
 msgstr "Sous-type d'appareil"
@@ -1734,21 +1827,18 @@
 msgstr "Se met en ligne?"
 
 #: opentera/forms/TeraDeviceForm.py:44 opentera/forms/TeraParticipantForm.py:50
 #: opentera/forms/TeraUserForm.py:30
 msgid "Last Connection"
 msgstr "Dernière connexion"
 
-#: opentera/forms/TeraDeviceForm.py:47
-#: opentera/forms/TeraDeviceSubTypeForm.py:24
-#: opentera/forms/TeraDeviceTypeForm.py:17
-#: opentera/forms/TeraParticipantForm.py:24
+#: opentera/forms/TeraDeviceForm.py:47 opentera/forms/TeraDeviceSubTypeForm.py:24
+#: opentera/forms/TeraDeviceTypeForm.py:17 opentera/forms/TeraParticipantForm.py:24
 #: opentera/forms/TeraParticipantGroupForm.py:18
-#: opentera/forms/TeraProjectForm.py:18
-#: opentera/forms/TeraServiceConfigForm.py:18
+#: opentera/forms/TeraProjectForm.py:18 opentera/forms/TeraServiceConfigForm.py:18
 #: opentera/forms/TeraServiceForm.py:18 opentera/forms/TeraSessionForm.py:120
 #: opentera/forms/TeraSessionTypeForm.py:25 opentera/forms/TeraSiteForm.py:12
 #: opentera/forms/TeraUserForm.py:13 opentera/forms/TeraUserGroupForm.py:18
 #: opentera/forms/TeraVersionsForm.py:18
 msgid "Information"
 msgstr "Information"
 
@@ -1856,27 +1946,35 @@
 msgstr "Nom Projet"
 
 #: opentera/forms/TeraProjectForm.py:22
 msgid "Project ID"
 msgstr "ID Projet"
 
 #: opentera/forms/TeraProjectForm.py:24
+msgid "Enabled"
+msgstr "Activé"
+
+#: opentera/forms/TeraProjectForm.py:26
 msgid "Site"
 msgstr "Site"
 
-#: opentera/forms/TeraProjectForm.py:25
+#: opentera/forms/TeraProjectForm.py:27
 msgid "Role"
 msgstr "Rôle"
 
-#: opentera/forms/TeraProjectForm.py:26 opentera/forms/TeraSiteForm.py:17
+#: opentera/forms/TeraProjectForm.py:28 opentera/forms/TeraSiteForm.py:17
 msgid "Site Name"
 msgstr "Nom Site"
 
-#: opentera/forms/TeraServiceConfigForm.py:25
-#: opentera/forms/TeraServiceForm.py:25
+#: opentera/forms/TeraProjectForm.py:30 opentera/forms/TeraProjectForm.py:32
+#: opentera/forms/TeraTestTypeForm.py:32
+msgid "Description"
+msgstr "Description"
+
+#: opentera/forms/TeraServiceConfigForm.py:25 opentera/forms/TeraServiceForm.py:25
 msgid "Service ID"
 msgstr "ID Service"
 
 #: opentera/forms/TeraServiceConfigForm.py:26
 msgid "Service Config ID"
 msgstr "ID Configuration Service"
 
@@ -2068,22 +2166,14 @@
 msgid "Comments"
 msgstr "Commentaires"
 
 #: opentera/forms/TeraSessionForm.py:167
 msgid "Session Has Device Data"
 msgstr "La Séance contient des données"
 
-#: opentera/forms/TeraSessionTypeConfigForm.py:19
-msgid "General configuration"
-msgstr "Configuration générale"
-
-#: opentera/forms/TeraSessionTypeConfigForm.py:22
-msgid "Allow session recording"
-msgstr "Autoriser l'enregistrement des séances"
-
 #: opentera/forms/TeraSessionTypeForm.py:29
 msgid "Session Type ID"
 msgstr "ID Type Séance"
 
 #: opentera/forms/TeraSessionTypeForm.py:30
 msgid "Session Type Name"
 msgstr "Nom Type Séance"
@@ -2140,18 +2230,14 @@
 msgid "Expose Web interface"
 msgstr "A une interface web"
 
 #: opentera/forms/TeraTestTypeForm.py:31
 msgid "Expose Web editor"
 msgstr "A un éditeur web"
 
-#: opentera/forms/TeraTestTypeForm.py:32
-msgid "Description"
-msgstr "Description"
-
 #: opentera/forms/TeraUserForm.py:18
 msgid "User UUID"
 msgstr "UUID Utilisateur"
 
 #: opentera/forms/TeraUserForm.py:19
 msgid "User Full Name"
 msgstr "Nom complet Utilisateur"
@@ -2237,95 +2323,94 @@
 msgid "Client linux version"
 msgstr "Version Linux du Client"
 
 #: opentera/services/BaseWebRTCService.py:52
 msgid "Join me!"
 msgstr "Joins-toi à moi!"
 
-#: opentera/services/BaseWebRTCService.py:382
+#: opentera/services/BaseWebRTCService.py:383
 msgid "Cannot create session event"
 msgstr "Impossible de créer l'événement de séance"
 
-#: opentera/services/BaseWebRTCService.py:422
+#: opentera/services/BaseWebRTCService.py:423
 msgid "Cannot create process"
 msgstr "Impossible de démarrer le processus"
 
-#: opentera/services/BaseWebRTCService.py:436
+#: opentera/services/BaseWebRTCService.py:437
 msgid "Cannot create session"
 msgstr "Impossible de créer la séance"
 
-#: opentera/services/BaseWebRTCService.py:459
+#: opentera/services/BaseWebRTCService.py:460
 msgid "Cannot create STOP session event"
 msgstr "Impossible de créer l'événement de séance \"Arrêt de séance\""
 
-#: opentera/services/BaseWebRTCService.py:516
+#: opentera/services/BaseWebRTCService.py:517
 msgid "Error stopping session - check server logs"
 msgstr ""
-"Erreur lors de l'arrêt de la séance - veuillez vérifier les journaux "
-"système"
+"Erreur lors de l'arrêt de la séance - veuillez vérifier les journaux système"
 
-#: opentera/services/BaseWebRTCService.py:518
+#: opentera/services/BaseWebRTCService.py:519
 msgid "No matching session to stop"
 msgstr "Aucune séance correspondante n'a pu être arrêtée"
 
-#: opentera/services/BaseWebRTCService.py:542
-#: opentera/services/BaseWebRTCService.py:619
-#: opentera/services/BaseWebRTCService.py:706
+#: opentera/services/BaseWebRTCService.py:543
+#: opentera/services/BaseWebRTCService.py:620
+#: opentera/services/BaseWebRTCService.py:707
 msgid "User"
 msgstr "Utilisateur"
 
-#: opentera/services/BaseWebRTCService.py:544
+#: opentera/services/BaseWebRTCService.py:545
 msgid "Error creating user invited session event"
 msgstr "Erreur lors de la création de l'événement de séance 'Utilisateur invité\""
 
-#: opentera/services/BaseWebRTCService.py:556
-#: opentera/services/BaseWebRTCService.py:634
-#: opentera/services/BaseWebRTCService.py:721
+#: opentera/services/BaseWebRTCService.py:557
+#: opentera/services/BaseWebRTCService.py:635
+#: opentera/services/BaseWebRTCService.py:722
 msgid "Participant"
 msgstr "Participant"
 
-#: opentera/services/BaseWebRTCService.py:558
+#: opentera/services/BaseWebRTCService.py:559
 msgid "Error creating participant invited session event"
 msgstr "Erreur lors de la création de l'événement de séance 'Participant invité\""
 
-#: opentera/services/BaseWebRTCService.py:571
-#: opentera/services/BaseWebRTCService.py:650
-#: opentera/services/BaseWebRTCService.py:736
+#: opentera/services/BaseWebRTCService.py:572
+#: opentera/services/BaseWebRTCService.py:651
+#: opentera/services/BaseWebRTCService.py:737
 msgid "Device"
 msgstr "Appareil"
 
-#: opentera/services/BaseWebRTCService.py:573
+#: opentera/services/BaseWebRTCService.py:574
 msgid "Error creating device invited session event"
 msgstr "Erreur lors de la création de l'événement de séance 'Appareil invité\""
 
-#: opentera/services/BaseWebRTCService.py:589
+#: opentera/services/BaseWebRTCService.py:590
 msgid "Error updating session"
 msgstr "Erreur de mise à jour de la séance"
 
-#: opentera/services/BaseWebRTCService.py:621
+#: opentera/services/BaseWebRTCService.py:622
 msgid "Error creating user left session event"
 msgstr ""
-"Erreur lors de la création de l'événement de séance 'Utilisateur a quitté"
-" la séance\""
+"Erreur lors de la création de l'événement de séance 'Utilisateur a quitté la "
+"séance\""
 
-#: opentera/services/BaseWebRTCService.py:636
+#: opentera/services/BaseWebRTCService.py:637
 msgid "Error creating participant left session event"
 msgstr ""
-"Erreur lors de la création de l'événement de séance 'Participant a quitté"
-" la séance\""
+"Erreur lors de la création de l'événement de séance 'Participant a quitté la "
+"séance\""
 
-#: opentera/services/BaseWebRTCService.py:652
+#: opentera/services/BaseWebRTCService.py:653
 msgid "Error creating device left session event"
 msgstr ""
-"Erreur lors de la création de l'événement de séance 'Appareil a quitté la"
-" séance\""
+"Erreur lors de la création de l'événement de séance 'Appareil a quitté la "
+"séance\""
 
-#: opentera/services/BaseWebRTCService.py:709
-#: opentera/services/BaseWebRTCService.py:724
-#: opentera/services/BaseWebRTCService.py:739
+#: opentera/services/BaseWebRTCService.py:710
+#: opentera/services/BaseWebRTCService.py:725
+#: opentera/services/BaseWebRTCService.py:740
 msgid "Cannot create refused session event"
 msgstr "Erreur lors de la création de l'événement de séance 'Invitation refusée\""
 
 #: templates/about.html:33
 msgid "Downloads"
 msgstr "Téléchargements"
 
@@ -2348,7 +2433,15 @@
 #: templates/disabled_doc.html:48
 msgid "Documentation is disabled!"
 msgstr "La documentation d’API est désactivée!"
 
 #~ msgid "Missing id_project or id_site arguments"
 #~ msgstr "Champs : id_projet oou id_site manquants"
 
+#~ msgid "Missing project id"
+#~ msgstr "ID de projet manquant"
+
+#~ msgid "General configuration"
+#~ msgstr "Configuration générale"
+
+#~ msgid "Allow session recording"
+#~ msgstr "Autoriser l'enregistrement des séances"
```

