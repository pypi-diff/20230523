# Comparing `tmp/assemblyline-4.4.1.dev85.tar.gz` & `tmp/assemblyline-4.4.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-4.4.1.dev85.tar", last modified: Tue May 23 11:59:01 2023, max compression
+gzip compressed data, was "assemblyline-4.4.1.dev9.tar", last modified: Fri Mar 24 16:14:12 2023, max compression
```

## Comparing `assemblyline-4.4.1.dev85.tar` & `assemblyline-4.4.1.dev9.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.173734 assemblyline-4.4.1.dev85/
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (122)       47 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2394 2023-05-23 11:59:01.173734 assemblyline-4.4.1.dev85/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1558 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.125734 assemblyline-4.4.1.dev85/assemblyline/
--rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-23 11:58:58.000000 assemblyline-4.4.1.dev85/assemblyline/VERSION
--rw-r--r--   0 vsts      (1001) docker     (122)      277 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.125734 assemblyline-4.4.1.dev85/assemblyline/cachestore/
--rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/cachestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.141734 assemblyline-4.4.1.dev85/assemblyline/common/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4138 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/archiving.py
--rw-r--r--   0 vsts      (1001) docker     (122)  2243670 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/attack_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13368 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/backupmanager.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/banner.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15856 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/bundling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5646 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/caching.py
--rw-r--r--   0 vsts      (1001) docker     (122)      903 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/chunk.py
--rw-r--r--   0 vsts      (1001) docker     (122)    39563 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4950 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/classification.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     5811 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/cleanup_filestore.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1789 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/codec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5031 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/comms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2512 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5564 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/custom.magic
--rw-r--r--   0 vsts      (1001) docker     (122)    24725 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/custom.yara
--rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/dict_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2318 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/digests.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2041 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/entropy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1903 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8326 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/forge.py
--rw-r--r--   0 vsts      (1001) docker     (122)   168072 2023-05-23 11:59:00.000000 assemblyline-4.4.1.dev85/assemblyline/common/frequency.c
--rw-r--r--   0 vsts      (1001) docker     (122)      709 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/frequency.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     6402 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/heuristics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1398 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/hexdump.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20632 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/identify.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17758 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/identify_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/importing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4229 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/iprange.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3610 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/isotime.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4310 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/log.py
--rw-r--r--   0 vsts      (1001) docker     (122)      909 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/logformat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1564 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/lucene.lark
--rw-r--r--   0 vsts      (1001) docker     (122)     1105 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/memory_zip.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4815 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/net.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21606 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/net_static.py
--rw-r--r--   0 vsts      (1001) docker     (122)      231 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/null.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1515 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/path.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28163 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4971 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/random_user.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3148 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/security.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1437 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/signaturing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7002 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/str_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7665 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/common/tag_safelist.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     3715 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      640 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/uid.py
--rw-r--r--   0 vsts      (1001) docker     (122)       57 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/common/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.141734 assemblyline-4.4.1.dev85/assemblyline/datasource/
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/datasource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2183 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/datasource/al.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1462 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/datasource/alert.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/datasource/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.145734 assemblyline-4.4.1.dev85/assemblyline/datastore/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2950 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/bulk.py
--rw-r--r--   0 vsts      (1001) docker     (122)    86864 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/collection.py
--rw-r--r--   0 vsts      (1001) docker     (122)      572 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    52403 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11825 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/store.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.145734 assemblyline-4.4.1.dev85/assemblyline/datastore/support/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/support/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9259 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/support/build.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4531 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/datastore/support/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.145734 assemblyline-4.4.1.dev85/assemblyline/filestore/
--rw-r--r--   0 vsts      (1001) docker     (122)    10145 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.145734 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7663 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/azure.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2720 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9405 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/http.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5427 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/local.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6631 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/s3.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/filestore/transport/sftp.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.149734 assemblyline-4.4.1.dev85/assemblyline/odm/
--rw-r--r--   0 vsts      (1001) docker     (122)     1637 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48181 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)      323 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.153734 assemblyline-4.4.1.dev85/assemblyline/odm/messages/
--rw-r--r--   0 vsts      (1001) docker     (122)       75 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      596 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/alert.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/alerter_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1532 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/archive_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)      940 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/changes.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/dispatcher_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/dispatching.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1546 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/expiry_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3372 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/ingest_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)      848 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/scaler_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/scaler_status_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1787 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/service_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/service_timing_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2190 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/submission.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/task.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1116 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/messages/vacuum_heartbeat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.161734 assemblyline-4.4.1.dev85/assemblyline/odm/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/actions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6894 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/alert.py
--rw-r--r--   0 vsts      (1001) docker     (122)      281 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/cached_file.py
--rw-r--r--   0 vsts      (1001) docker     (122)    57459 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)      322 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/emptyresult.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2072 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/error.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2910 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/file.py
--rw-r--r--   0 vsts      (1001) docker     (122)      683 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/filescore.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1331 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/heuristic.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.161734 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.161734 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/filetypes/
--rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/filetypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24751 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/filetypes/pe.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5726 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/ontology.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.165734 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/
--rw-r--r--   0 vsts      (1001) docker     (122)      445 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/antivirus.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9903 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/malware_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3842 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/network.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/process.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2507 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/sandbox.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2886 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/signature.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3231 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8025 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/result.py
--rw-r--r--   0 vsts      (1001) docker     (122)      947 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/retrohunt.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3000 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10153 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/service.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/service_delta.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/signature.py
--rw-r--r--   0 vsts      (1001) docker     (122)      695 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/statistics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8661 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/submission.py
--rw-r--r--   0 vsts      (1001) docker     (122)      843 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/submission_summary.py
--rw-r--r--   0 vsts      (1001) docker     (122)      638 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/submission_tree.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35720 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9881 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/user.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1255 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/user_favorites.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2317 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1639 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/models/workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.169734 assemblyline-4.4.1.dev85/assemblyline/odm/random_data/
--rw-r--r--   0 vsts      (1001) docker     (122)    15995 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/random_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/random_data/create_test_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25241 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/random_data/sample_rules.yar
--rw-r--r--   0 vsts      (1001) docker     (122)     9244 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/odm/random_data/sample_suricata.rules
--rw-r--r--   0 vsts      (1001) docker     (122)    14680 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/odm/randomizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.169734 assemblyline-4.4.1.dev85/assemblyline/remote/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/remote/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.169734 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/
--rw-r--r--   0 vsts      (1001) docker     (122)     3448 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1984 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/counters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4112 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/events.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7000 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/exporting_counter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6018 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/hash.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1442 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/lock.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.173734 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1793 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/comms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/multi.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/named.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7394 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/priority.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2902 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/set.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1926 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/user_quota_tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.173734 assemblyline-4.4.1.dev85/assemblyline/run/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/run/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    53134 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/assemblyline/run/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/run/pubsub_reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3760 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/run/suricata_importer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4791 2023-05-23 11:58:41.000000 assemblyline-4.4.1.dev85/assemblyline/run/yara_importer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 11:59:01.125734 assemblyline-4.4.1.dev85/assemblyline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2394 2023-05-23 11:59:01.000000 assemblyline-4.4.1.dev85/assemblyline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     6041 2023-05-23 11:59:01.000000 assemblyline-4.4.1.dev85/assemblyline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 11:59:01.000000 assemblyline-4.4.1.dev85/assemblyline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      507 2023-05-23 11:59:01.000000 assemblyline-4.4.1.dev85/assemblyline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-05-23 11:59:01.000000 assemblyline-4.4.1.dev85/assemblyline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-05-23 11:59:01.173734 assemblyline-4.4.1.dev85/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     3678 2023-05-23 11:58:42.000000 assemblyline-4.4.1.dev85/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       47 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2393 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1558 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.138347 assemblyline-4.4.1.dev9/assemblyline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-03-24 16:14:10.000000 assemblyline-4.4.1.dev9/assemblyline/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (122)      277 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.142347 assemblyline-4.4.1.dev9/assemblyline/cachestore/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/cachestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.150347 assemblyline-4.4.1.dev9/assemblyline/common/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4138 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/archiving.py
+-rw-r--r--   0 vsts      (1001) docker     (122)  2243670 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/attack_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13368 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/backupmanager.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/banner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15837 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/bundling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5646 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/caching.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      903 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/chunk.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    38686 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4532 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/classification.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     5811 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/cleanup_filestore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1789 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5031 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2512 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5147 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/custom.magic
+-rw-r--r--   0 vsts      (1001) docker     (122)    23191 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/custom.yara
+-rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/dict_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2091 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/digests.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2041 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/entropy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1903 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8326 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/forge.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   168009 2023-03-24 16:14:11.000000 assemblyline-4.4.1.dev9/assemblyline/common/frequency.c
+-rw-r--r--   0 vsts      (1001) docker     (122)      709 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/frequency.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     6402 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/heuristics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1398 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/hexdump.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19731 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17758 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/identify_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/importing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4229 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/iprange.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3610 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/isotime.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4310 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/log.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      909 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/logformat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1564 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/lucene.lark
+-rw-r--r--   0 vsts      (1001) docker     (122)     1105 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/memory_zip.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4815 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/net.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21606 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/net_static.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      231 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/null.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1269 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/path.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28059 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4971 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/random_user.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3148 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/security.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1437 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/signaturing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7002 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/str_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7665 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/tag_safelist.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3715 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      640 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       57 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.150347 assemblyline-4.4.1.dev9/assemblyline/datasource/
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2183 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/al.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1462 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/datastore/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2950 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/bulk.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    86851 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      622 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    52444 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10135 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/store.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/datastore/support/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/support/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9259 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/support/build.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4531 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/support/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/filestore/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10145 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7663 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/azure.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2720 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9405 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/http.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5353 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/local.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6956 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/s3.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/sftp.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/odm/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1637 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48035 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      323 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.158347 assemblyline-4.4.1.dev9/assemblyline/odm/messages/
+-rw-r--r--   0 vsts      (1001) docker     (122)       75 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      596 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/alerter_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1532 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/archive_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      940 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/changes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatcher_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatching.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1546 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/expiry_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3372 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/ingest_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      848 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_status_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1787 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_timing_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2190 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/task.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1116 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/vacuum_heartbeat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6894 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      281 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/cached_file.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    55609 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      322 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/emptyresult.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2072 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/error.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2007 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/file.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      683 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/filescore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1331 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/heuristic.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/
+-rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24751 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5726 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/ontology.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/
+-rw-r--r--   0 vsts      (1001) docker     (122)      445 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/antivirus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9834 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/malware_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3842 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/network.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/process.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2507 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/sandbox.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2886 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3231 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/result.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      884 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/retrohunt.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3000 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10153 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/service.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/service_delta.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      695 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/statistics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8663 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      843 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_summary.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      638 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_tree.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35620 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9742 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/user.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1255 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/user_favorites.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2317 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1639 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15957 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/create_test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25241 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_rules.yar
+-rw-r--r--   0 vsts      (1001) docker     (122)     9244 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_suricata.rules
+-rw-r--r--   0 vsts      (1001) docker     (122)    14680 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/randomizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/remote/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3448 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1984 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/counters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/events.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7000 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/exporting_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6018 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/hash.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1442 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/lock.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1793 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/named.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7394 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/priority.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2902 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/set.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1926 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/user_quota_tracker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/run/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    53134 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/run/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/pubsub_reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3760 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/suricata_importer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4791 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/yara_importer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.138347 assemblyline-4.4.1.dev9/assemblyline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2393 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     6041 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      506 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     3681 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/setup.py
```

### Comparing `assemblyline-4.4.1.dev85/LICENCE.md` & `assemblyline-4.4.1.dev9/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/PKG-INFO` & `assemblyline-4.4.1.dev9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.4.1.dev85
+Version: 4.4.1.dev9
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-4.4.1.dev85/README.md` & `assemblyline-4.4.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/cachestore/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/cachestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/archiving.py` & `assemblyline-4.4.1.dev9/assemblyline/common/archiving.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/attack_map.py` & `assemblyline-4.4.1.dev9/assemblyline/common/attack_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/backupmanager.py` & `assemblyline-4.4.1.dev9/assemblyline/common/backupmanager.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/banner.py` & `assemblyline-4.4.1.dev9/assemblyline/common/banner.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/bundling.py` & `assemblyline-4.4.1.dev9/assemblyline/common/bundling.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             sha256s.append(key)
 
     return list(set(sha256s))
 
 
 # noinspection PyBroadException
 def create_bundle(sid, working_dir=WORK_DIR, use_alert=False):
-    with forge.get_datastore(archive_access=True) as datastore:
+    with forge.get_datastore() as datastore:
         temp_bundle_file = f"bundle_{get_random_id()}"
         current_working_dir = os.path.join(working_dir, temp_bundle_file)
         target_file = os.path.join(working_dir, f"{temp_bundle_file}.cart")
         tgz_file = os.path.join(working_dir, f"{temp_bundle_file}.tgz")
         try:
             if use_alert:
                 alert = datastore.alert.get(sid, as_obj=False)
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/caching.py` & `assemblyline-4.4.1.dev9/assemblyline/common/caching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/chunk.py` & `assemblyline-4.4.1.dev9/assemblyline/common/chunk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/classification.py` & `assemblyline-4.4.1.dev9/assemblyline/common/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,14 @@
         self.description = {}
         self.invalid_mode = False
         self._classification_cache = set()
         self._classification_cache_short = set()
 
         self.enforce = False
         self.dynamic_groups = False
-        # dynamic group type is one of: email | group | all
-        # defaults to email for original behavior
-        self.dynamic_groups_type = "email"
 
         # Add Invalid classification
         self.levels_map["INV"] = self.INVALID_LVL
         self.levels_map[str(self.INVALID_LVL)] = "INV"
         self.levels_map_stl["INV"] = self.INVALID_CLASSIFICATION
         self.levels_map_lts[self.INVALID_CLASSIFICATION] = "INV"
 
@@ -73,20 +70,14 @@
         self.levels_map[str(self.NULL_LVL)] = self.NULL_CLASSIFICATION
         self.levels_map_stl[self.NULL_CLASSIFICATION] = self.NULL_CLASSIFICATION
         self.levels_map_lts[self.NULL_CLASSIFICATION] = self.NULL_CLASSIFICATION
 
         try:
             self.enforce = classification_definition['enforce']
             self.dynamic_groups = classification_definition['dynamic_groups']
-            self.dynamic_groups_type = classification_definition['dynamic_groups_type']
-
-            if self.dynamic_groups_type not in ['email', 'group', 'all']:
-                raise InvalidDefinition(f"Invalid dynamic group type \"{self.dynamic_groups_type}\". "
-                                        "Valid types are: email | group | all")
-
             if self.enforce:
                 self._classification_cache = self.list_all_classification_combinations()
                 self._classification_cache_short = self.list_all_classification_combinations(long_format=False)
 
             for x in classification_definition['levels']:
                 short_name = x['short_name'].upper()
                 name = x['name'].upper()
@@ -255,16 +246,15 @@
                 for a in self.access_req_aliases[p]:
                     return_set.add(a)
 
         if long_format:
             return sorted([self.access_req_map_stl[r] for r in return_set])
         return sorted(list(return_set))
 
-    def _get_c12n_groups(self, c12n: str, long_format: bool = True,
-                         get_dynamic_groups: bool = True) -> Tuple[List, List]:
+    def _get_c12n_groups(self, c12n: str, long_format: bool = True) -> Tuple[List, List]:
         # Parse classifications in uppercase mode only
         c12n = c12n.upper()
 
         g1_set = set()
         g2_set = set()
         others = set()
 
@@ -291,15 +281,15 @@
                 g2_set.add(g)
             elif g in self.subgroups_aliases:
                 for a in self.subgroups_aliases[g]:
                     g2_set.add(a)
             else:
                 others.add(g)
 
-        if self.dynamic_groups and get_dynamic_groups:
+        if self.dynamic_groups:
             for o in others:
                 if o not in self.access_req_map_lts \
                         and o not in self.access_req_map_stl \
                         and o not in self.access_req_aliases \
                         and o not in self.levels_map \
                         and o not in self.levels_map_lts \
                         and o not in self.levels_aliases:
@@ -408,19 +398,19 @@
                 out += "/"
             else:
                 out += "//"
             out += "/".join(sorted(subgroups))
 
         return out
 
-    def _get_classification_parts(self, c12n: str, long_format: bool = True, get_dynamic_groups: bool = True) \
+    def _get_classification_parts(self, c12n: str, long_format: bool = True) \
             -> Tuple[Union[Union[int, str], Any], List, List, List]:
         lvl_idx = self._get_c12n_level_index(c12n)
         req = self._get_c12n_required(c12n, long_format=long_format)
-        groups, subgroups = self._get_c12n_groups(c12n, long_format=long_format, get_dynamic_groups=get_dynamic_groups)
+        groups, subgroups = self._get_c12n_groups(c12n, long_format=long_format)
 
         return lvl_idx, req, groups, subgroups
 
     @staticmethod
     def _max_groups(groups_1: List, groups_2: List) -> List:
         if len(groups_1) > 0 and len(groups_2) > 0:
             groups = set(groups_1) & set(groups_2)
@@ -857,16 +847,15 @@
 
         return self._get_normalized_classification_text(min(lvl_idx_1, lvl_idx_2),
                                                         req,
                                                         groups,
                                                         subgroups,
                                                         long_format=long_format)
 
-    def normalize_classification(self, c12n: str, long_format: bool = True, skip_auto_select: bool = False,
-                                 get_dynamic_groups: bool = True) -> str:
+    def normalize_classification(self, c12n: str, long_format: bool = True, skip_auto_select: bool = False) -> str:
         """
         Normalize a given classification by applying the rules defined in the classification definition.
         This function will remove any invalid parts and add missing parts to the classification.
         It will also ensure that the display of the classification is always done the same way
 
         Args:
             c12n: Classification to normalize
@@ -876,21 +865,20 @@
         Returns:
             A normalized version of the original classification
         """
         if not self.enforce or self.invalid_mode:
             return self.UNRESTRICTED
 
         # Has the classification has already been normalized before?
-        if long_format and c12n in self._classification_cache and get_dynamic_groups:
+        if long_format and c12n in self._classification_cache:
             return c12n
-        if not long_format and c12n in self._classification_cache_short and get_dynamic_groups:
+        if not long_format and c12n in self._classification_cache_short:
             return c12n
 
-        lvl_idx, req, groups, subgroups = self._get_classification_parts(c12n, long_format=long_format,
-                                                                         get_dynamic_groups=get_dynamic_groups)
+        lvl_idx, req, groups, subgroups = self._get_classification_parts(c12n, long_format=long_format)
         new_c12n = self._get_normalized_classification_text(lvl_idx, req, groups, subgroups,
                                                             long_format=long_format,
                                                             skip_auto_select=skip_auto_select)
         if long_format:
             self._classification_cache.add(new_c12n)
         else:
             self._classification_cache_short.add(new_c12n)
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/classification.yml` & `assemblyline-4.4.1.dev9/assemblyline/common/classification.yml`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,16 @@
 #  it showcases all the different features of the classification engine
 #  while providing a useful configuration
 
 # Turn on/off classification enforcement. When this flag is off, this
 #  completely disables the classification engine, any documents added while
 #  the classification engine is off gets the default unrestricted value
 enforce: false
-
-# Turn on/off dynamic group creation. This feature allow you to dynamically create classification groups based on
-#  features from the user.
 dynamic_groups: false
 
-# Set the type of dynamic groups to be used
-#  email: groups will be based of the user's email domain
-#  group: groups will be created out the the user's group values
-#  all: groups will be created out of both the email domain and the group values
-dynamic_groups_type: email
-
 # List of Classification level:
 #   Graded list were a smaller number is less restricted then an higher number.
 levels:
   # List of alternate names for the current marking
   - aliases:
       - UNRESTRICTED
       - UNCLASSIFIED
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/cleanup_filestore.py` & `assemblyline-4.4.1.dev9/assemblyline/common/cleanup_filestore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/codec.py` & `assemblyline-4.4.1.dev9/assemblyline/common/codec.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/comms.py` & `assemblyline-4.4.1.dev9/assemblyline/common/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/constants.py` & `assemblyline-4.4.1.dev9/assemblyline/common/constants.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/custom.magic` & `assemblyline-4.4.1.dev9/assemblyline/common/custom.magic`

 * *Files 6% similar despite different names*

```diff
@@ -114,31 +114,23 @@
 >>&0 search/300 ------MultipartBoundary-- custom: document/email
 # Quarantine Files
 0	string	AhnLab\040Inc.\0402006	custom: quarantine/ahnlab
 0	string	\055chest\055\040		custom: quarantine/avast
 0	string	AntiVir\040\Qua			custom: quarantine/avira
 0	beshort	0x0BAD					custom: quarantine/windowsdefender
 0	belong	0xDBE8C501				custom: quarantine/windowsdefender
-# Sysmon Files
-0		string
->0		search/0x70		\<Event\ xmlns=
->>&0	string			"http://schemas.microsoft.com/win/2004/08/events/event">	custom: metadata/sysmon/xml
->>&0	string			'http://schemas.microsoft.com/win/2004/08/events/event'>	custom: metadata/sysmon/xml
 # Memory Dump Files
 10   string _BIOPSY:                custom: metadata/memorydump
 # Windows URL Shortcut Files
 0 string [InternetShortcut] custom: shortcut/web
 # NSIS Installer
 4  string  \xef\xbe\xad\xdeNullsoftInst custom: archive/nsis
-# Assemblyline batch file, declared in Python code in identify.py
+# Assemblyline batch file
 0 string REM\ Batch\ extracted\ by\ Assemblyline\n custom: code/batch
-# Assemblyline powershell file, declared in Python code in identify.py
+# Assemblyline powershell file
 0 string \#\!\/usr\/bin\/env\ pwsh\n custom: code/ps1
 # xxencoded and uuencoded files
 0 string XXEncode\ \ 0\.0\ \(PowerArchiver\ 2009:\ www\.powerarchiver\.com\) custom: archive/xxe
 0 string UUEncode\ \ 0\.0\ \(PowerArchiver\ 2009:\ www\.powerarchiver\.com\) custom: archive/uue
 0 string begin
 >&0 search/50 \nh custom: archive/xxe
 >&0 search/50 \nM custom: archive/uue
-# Android OAT
-0 string \x7fELF
->0x1000 string oat custom: executable/android/oat
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/custom.yara` & `assemblyline-4.4.1.dev9/assemblyline/common/custom.yara`

 * *Files 2% similar despite different names*

```diff
@@ -22,48 +22,28 @@
         $strong_js7  = /submitForm\(['"]/
         $strong_js8  = /(document|window)(\[['"a-zA-Z]|\.)\w+/
         $strong_js9  = /setTimeout\(/
         $strong_js10 = /(^|;|\s)(var|let|const)[ \t]+\w+[ \t]*=[ \t]*/
         // If this is exactly in the sample, will trigger a second time because of strong_js10
         $strong_js11 = /(^|\n)window.location.href[ \t]*=/
 
-        // Used in a lot of malware samples to fail silently
-        $strong_js12 = /catch\s+\(\w*\)\s+\{.*\}/
-
-        // Firefox browser specific method
-        $strong_js13 = /user_pref\("[\w.]+",\s*[\w"']+\)/
-
         $weak_js2 = /String(\[['"]|\.)(fromCharCode|raw)(['"]\])?\(/
         $weak_js3 = /Math\.(round|pow|sin|cos)\(/
         $weak_js4 = /(isNaN|isFinite|parseInt|parseFloat|toLowerCase|toUpperCase)\(/
         $weak_js5 = /([^\w]|^)this\.[\w]+/
-        $weak_js6 = /([^\w]|^)[\w]+\.length/
 
     condition:
         // Note that application/javascript is obsolete
         not $not_html
-        and (
-                (
-                    (
-                        mime startswith "text" or mime == "application/javascript"
-                    )
-                    and (
-                        2 of ($strong_js*)
-                        or (
-                            1 of ($strong_js*)
-                            and 2 of ($weak_js*)
-                        )
-                        or (#strong_js1) > 5
-                    )
-                )
-                or (
-                    mime == "application/octet-stream"
-                    and 4 of ($strong_js*)
-                )
-            )
+        and (((mime startswith "text" or mime == "application/javascript")
+            and (2 of ($strong_js*)
+                or (1 of ($strong_js*)
+                    and 2 of ($weak_js*))))
+            or (mime == "application/octet-stream"
+            and 4 of ($strong_js*)))
 }
 
 /*
 code/jscript
 */
 
 rule code_jscript {
@@ -366,19 +346,19 @@
 text/json
 */
 
 rule text_json {
 
     meta:
         type = "text/json"
-        score = 2
+        score = 1
 
     strings:
         $start = "{"
-        $invalid_keys1 = /^\s*\w+:[\s]*[\{\["\d]/
+        $invalid_keys1 = /\w+:[\s]*[\{\["\d]/
         $valid_keys1 = /"\w+":[\s]*[\{\["\d]/
         $end = "}"
 
     condition:
         $start at 0
         and 0 of ($invalid_keys*)
         and $valid_keys1
@@ -441,39 +421,21 @@
 rule code_jsp {
 
     meta:
         type = "code/jsp"
         score = 3
 
     strings:
-        $xml_begin = "<jsp:"
-        $xml_end = "</jsp:"
-        $non_xml_begin = "<%"
-        $non_xml_end = "%>"
-        $java1 = "FileOutputStream"
-        $java2 = "System.getProperty"
-        $java3 = "public void"
-        $java4 = "public Class"
-        $java5 = "ClassLoad"
-        $java6 = "java.util.*"
-        $jsp1 = "<%@ page"
-        $jsp2 = "<%@ include"
-        $jsp3 = "<%@ taglib"
+        $ = /(^|\n)<%@page[ \t]+import=['"][\w\.]+['"][ \t]*%>/
+        $ = /(^|\n)<%![^%]*%>/
+        $ = /<%=\w+%>/
 
     condition:
         mime startswith "text"
-        and (
-            all of ($xml*)
-            or 2 of ($jsp*)
-            or (
-                #non_xml_begin >= 2
-                and #non_xml_end >= 2
-                and (#java1 + #java2 + #java3 + #java4 + #java5 + #java6) >= 2
-            )
-        )
+        and 2 of them
 }
 
 /*
 code/ps1
 */
 
 rule code_ps1 {
@@ -496,26 +458,18 @@
         $strong_pwsh11 = /\[Microsoft\.VisualBasic\.(Interaction|CallType)\]/i ascii wide
         $strong_pwsh12 = /[ \t;\n]foreach[ \t]*\([ \t]*\$\w+[ \t]+in[ \t]+[^)]+\)[ \t;\n]*{/i ascii wide
         $strong_pwsh13 = /\bfunction[ \t]+\w+[ \t]*\([^)]*\)[ \t\n]*{/i ascii wide
         $strong_pwsh14 = /\[char\][ \t]*(\d\d|0x[0-9a-f]{1,2})/i ascii wide
         $weak_pwsh1 = /\$\w+[ \t]*=[ \t]*[^;\n|]+[;\n|]/ ascii wide
 
     condition:
-        (
-            mime startswith "text"
-            and
-                (
-                    2 of ($strong_pwsh*)
-                    or
-                    3 of them
-                )
-        ) or (
-            mime == "application/octet-stream"
-            and 3 of ($strong_pwsh*)
-        )
+        (mime startswith "text"
+        and 2 of them) or
+            (mime == "application/octet-stream"
+            and 3 of ($strong_pwsh*))
 }
 
 rule code_ps1_in_ps1 {
 
     meta:
         type = "code/ps1"
         score = -1
@@ -619,24 +573,22 @@
 
 rule code_python {
 
     meta:
         type = "code/python"
 
     strings:
-        $strong_py1 = /(^|\n)[ \t]*if[ \t]+__name__[ \t]*==[ \t]*['"]__main__['"][ \t]*:/
-        $strong_py2 = /(^|\n)[ \t]*from[ \t]+[\w.]+[ \t]+import[ \t]+[\w.*]+([ \t]+as \w+)?/
-        $strong_py3 = /(^|\n)[ \t]*def[ \t]*\w+[ \t]*\([^)]*\)[ \t]*:/
-        $strong_py4 = /(try:|except:|else:)/
-        // High confidence one-liner used to execute base64 blobs
-        $strong_py5 = /exec\(__import__\(['"]base64['"]\)\.b64decode\(__import__\(['"]codecs['"]\)\.getencoder\(/
+        $ = /(^|\n)[ \t]*if[ \t]+__name__[ \t]*==[ \t]*['"]__main__['"][ \t]*:/
+        $ = /(^|\n)[ \t]*from[ \t]+[\w.]+[ \t]+import[ \t]+[\w.*]+([ \t]+as \w+)?/
+        $ = /(^|\n)[ \t]*def[ \t]*\w+[ \t]*\([^)]*\)[ \t]*:/
+        $ = /(try:|except:|else:)/
 
     condition:
         mime startswith "text"
-        and (2 of ($strong_py*) or $strong_py5)
+        and 2 of them
 }
 
 /*
 code/java
 */
 
 rule code_java {
@@ -709,28 +661,31 @@
 
     condition:
         mime startswith "text"
         and for all of ($css) : ( # > 2 )
 }
 
 /*
-code/ducky
+metadata/sysmon/evtx
 */
 
-rule code_ducky {
+rule metadata_sysmon_evtx {
+
     meta:
-        type = "code/ducky"
+        type = "metadata/sysmon/evtx"
+        score = 1
 
     strings:
-        $commands = /(^|\n)(REM|REM_BLOCK|END_REM|STRING|END_STRING|STRINGLN|END_STRINGLN|DELAY|ENTER|GUI)/
+        $ = /<Events[^>]*>/
+        $ = /<Event[^s][^>]*(\/)?>/
+        $ = /<\/Event(s)?>/
 
     condition:
         mime startswith "text"
-        and #commands >= 10
-
+        and all of them
 }
 
 /*
 code/batch
 */
 
 // rule code_batch {
@@ -771,17 +726,16 @@
         $obf2 = /\%([^:\n\r\%]+(\%\%)?)+\%/
         $power1 = /(^|\n|@|&)\^?p(\^|%.+%)?o(\^|%.+%)?w(\^|%.+%)?e(\^|%.+%)?r(\^|%.+%)?s(\^|%.+%)?h(\^|%.+%)?e(\^|%.+%)?l(\^|%.+%)?l(\^|%.+%)?(\.(\^|%.+%)?e(\^|%.+%)?x(\^|%.+%)?e(\^|%.+%)?)?.+(-c|-command)(\^|%.+%)?[ \t]/i
         // powershell does not need to be followed with -c or -command for it to be considered batch
         $power2 = /(^|\n|@|&|\b)\^?p(\^|%.+%)?o(\^|%.+%)?w(\^|%.+%)?e(\^|%.+%)?r(\^|%.+%)?s(\^|%.+%)?h(\^|%.+%)?e(\^|%.+%)?l(\^|%.+%)?l(\^|%.+%)?(\.(\^|%.+%)?e(\^|%.+%)?x(\^|%.+%)?e(\^|%.+%)?)?.+(-c|-command)?(\^|%.+%)?[ \t]/i
         $cmd1 = /(^|\n|@|&)(echo|netsh|goto|pkgmgr|del|netstat|timeout|taskkill|vssadmin|tasklist|schtasks)[ \t][\/]?\w+/i
         $cmd2 = /(^|\n|@|&)net[ \t]+(share|stop|start|accounts|computer|config|continue|file|group|localgroup|pause|session|statistics|time|use|user|view)/i
         $cmd3 = /(^|\n|@|&)reg[ \t]+(delete|query|add|copy|save|load|unload|restore|compare|export|import|flags)[ \t]+/i
-        $cmd4 = /(^|\n|@|&|^\s)start[ \t]+(\/(min|b|wait|belownormal|abovenormal|realtime|high|normal|low|shared|seperate|max|i)[ \t]+|"\w*"[ \t]+)+["']?([A-Z]:)?([\\|\/]?[\w.]+)+['"]?/i
+        $cmd4 = /(^|\n|@|&)start[ \t]+(\/(min|b|wait|belownormal|abovenormal|realtime|high|normal|low|shared|seperate|max|i)[ \t]+|"\w*"[ \t]+)+["']?([A-Z]:)?([\\|\/]?[\w.]+)+['"]?/i
         $cmd5 = /(^|\n)exit\s*$/i
-        $cmd6 = /(^|\n|@|&)%comspec%/i
         $rem = /(^|\n|@|&)\^?r\^?e\^?m\^?[ \t]\w+/i
         $set = /(^|\n|@|&)\^?s\^?e\^?t\^?[ \t]\^?\w+\^?=\^?\w+/i
         $bom = {FF FE}
         $exp = /setlocal[ \t](enableDelayedExpansion|disableDelayedExpansion)/i
 
     condition:
         (mime startswith "text" or $bom at 0)
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/dict_utils.py` & `assemblyline-4.4.1.dev9/assemblyline/common/dict_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/digests.py` & `assemblyline-4.4.1.dev9/assemblyline/common/digests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import hashlib
-import tlsh
 from typing import Dict
 
 from assemblyline.common import entropy
 
 DEFAULT_BLOCKSIZE = 65536
 
 
@@ -19,15 +18,14 @@
             pass
 
     result = {}
 
     md5 = hashlib.md5()
     sha1 = hashlib.sha1()
     sha256 = hashlib.sha256()
-    th = tlsh.Tlsh()
     size = 0
 
     with open(path, 'rb') as f:
         data = f.read(blocksize)
         length = len(data)
 
         if not size:
@@ -35,36 +33,28 @@
 
         while length > 0:
             if bc is not None:
                 bc.update(data, length)
             md5.update(data)
             sha1.update(data)
             sha256.update(data)
-            th.update(data)
             size += length
 
             data = f.read(blocksize)
             length = len(data)
 
     if bc is not None:
         result['entropy'] = bc.entropy()
     else:
         result['entropy'] = 0
     result['md5'] = md5.hexdigest()
     result['sha1'] = sha1.hexdigest()
     result['sha256'] = sha256.hexdigest()
     result['size'] = size
 
-    # Try to finalise the TLSH Hash and add it to the results
-    try:
-        th.final()
-        result['tlsh'] = th.hexdigest()
-    except Exception:
-        pass
-
     return result
 
 
 def get_md5_for_file(path: str, blocksize: int = DEFAULT_BLOCKSIZE) -> str:
     md5 = hashlib.md5()
     with open(path, 'rb') as f:
         data = f.read(blocksize)
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/entropy.py` & `assemblyline-4.4.1.dev9/assemblyline/common/entropy.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/exceptions.py` & `assemblyline-4.4.1.dev9/assemblyline/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/forge.py` & `assemblyline-4.4.1.dev9/assemblyline/common/forge.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/frequency.c` & `assemblyline-4.4.1.dev9/assemblyline/common/frequency.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "assemblyline.common.frequency",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_33"
+#define CYTHON_HEX_VERSION 0x001D21F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -212,15 +212,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
+    #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -251,15 +251,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
+    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/frequency.pyx` & `assemblyline-4.4.1.dev9/assemblyline/common/frequency.pyx`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/heuristics.py` & `assemblyline-4.4.1.dev9/assemblyline/common/heuristics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/hexdump.py` & `assemblyline-4.4.1.dev9/assemblyline/common/hexdump.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/identify.py` & `assemblyline-4.4.1.dev9/assemblyline/common/identify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 import logging
+import magic
+import msoffcrypto
 import re
+import ssdeep
 import struct
 import subprocess
 import sys
 import threading
 import uuid
+import yaml
+import yara
 import zipfile
+
 from binascii import hexlify
-from typing import Dict, Optional, Tuple, Union
+from cart import get_metadata_only
+from typing import Tuple, Union, Dict
 
-import magic
-import msoffcrypto
-import ssdeep
-import yaml
-import yara
 from assemblyline.common.digests import get_digests_for_file
-from assemblyline.common.forge import get_cachestore, get_config, get_constants, get_datastore
-from assemblyline.common.identify_defaults import OLE_CLSID_GUIDs
-from assemblyline.common.identify_defaults import magic_patterns as default_magic_patterns
-from assemblyline.common.identify_defaults import trusted_mimes as default_trusted_mimes
+from assemblyline.common.forge import get_constants, get_cachestore, get_config, get_datastore
+from assemblyline.common.identify_defaults import OLE_CLSID_GUIDs, magic_patterns as default_magic_patterns, \
+    trusted_mimes as default_trusted_mimes
 from assemblyline.common.str_utils import dotdump, safe_str
 from assemblyline.filestore import FileStoreException
 from assemblyline.remote.datatypes.events import EventWatcher
-from cart import get_metadata_only
 
 constants = get_constants()
 
 
-# These headers are found in the custom.magic file to assist with identification, and are imported by services
-# that can create files with a high-confidence type
-CUSTOM_PS1_ID = b"#!/usr/bin/env pwsh\n"
-CUSTOM_BATCH_ID = b"REM Batch extracted by Assemblyline\n"
-
-
 class Identify():
-    def __init__(self, use_cache: bool = True, config=None, datastore=None, log=None) -> None:
+    def __init__(self, use_cache=True, config=None, datastore=None, log=None) -> None:
         self.log = log or logging.getLogger('assemblyline.identify')
         self.config = None
         self.datastore = None
         self.use_cache = use_cache
         self.custom = re.compile(r"^custom: ", re.IGNORECASE)
         self.lock = threading.Lock()
         self.yara_default_externals = {'mime': '', 'magic': '', 'type': ''}
@@ -59,33 +53,27 @@
         if self.use_cache:
             self.reload_map = {
                 'magic': self._load_magic_file,
                 'mimes': self._load_trusted_mimes,
                 'patterns': self._load_magic_patterns,
                 'yara': self._load_yara_file
             }
-            self.reload_watcher: Optional[EventWatcher[str]] = EventWatcher()
+            self.reload_watcher = EventWatcher()
             self.reload_watcher.register('system.identify', self._handle_reload_event)
             self.reload_watcher.start()
         else:
             self.reload_watcher = None
             self.reload_map = {}
 
-    def _handle_reload_event(self, data: Optional[str]):
-        if data is None:
-            # handle disconnect event, we may be out of sync
-            for reload_func in self.reload_map.values():
-                reload_func()
+    def _handle_reload_event(self, data):
+        func = self.reload_map.get(data, None)
+        if func:
+            func()
         else:
-            # update information
-            func = self.reload_map.get(data, None)
-            if func is not None:
-                func()
-            else:
-                self.log.error(f"Invalid system.identify message received: {data}")
+            self.log.error(f"Invalid system.identify message received: {data}")
 
     def _load_magic_patterns(self):
         self.magic_patterns = default_magic_patterns
 
         if self.use_cache:
             self.log.info("Checking for custom magic patterns...")
             with get_cachestore('system', config=self.config, datastore=self.datastore) as cache:
@@ -231,17 +219,15 @@
                     break
 
             # First lets try to find any custom types
             for label in labels:
                 label = dotdump(label)
 
                 if self.custom.match(label):
-                    # Some things, like executable have additional data appended to their identification, like
-                    # ", dynamically linked, stripped" that we do not want to use as part of the type.
-                    data["type"] = label.split("custom: ")[1].split(",", 1)[0].strip()
+                    data["type"] = label.split("custom: ")[1].strip()
                     break
 
             # Second priority is mime times marked as trusted
             if data["type"] == "unknown":
                 with self.lock:
                     trusted_mimes = self.trusted_mimes
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/identify_defaults.py` & `assemblyline-4.4.1.dev9/assemblyline/common/identify_defaults.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/iprange.py` & `assemblyline-4.4.1.dev9/assemblyline/common/iprange.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/isotime.py` & `assemblyline-4.4.1.dev9/assemblyline/common/isotime.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/log.py` & `assemblyline-4.4.1.dev9/assemblyline/common/log.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/logformat.py` & `assemblyline-4.4.1.dev9/assemblyline/common/logformat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/lucene.lark` & `assemblyline-4.4.1.dev9/assemblyline/common/lucene.lark`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/memory_zip.py` & `assemblyline-4.4.1.dev9/assemblyline/common/memory_zip.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/metrics.py` & `assemblyline-4.4.1.dev9/assemblyline/common/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/net.py` & `assemblyline-4.4.1.dev9/assemblyline/common/net.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/net_static.py` & `assemblyline-4.4.1.dev9/assemblyline/common/net_static.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/path.py` & `assemblyline-4.4.1.dev9/assemblyline/common/path.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 import os
-import string
 import sys
 from typing import Optional
 
 
 def modulepath(modulename: str) -> str:
     m = sys.modules[modulename]
     f = getattr(m, '__file__', None)
@@ -14,19 +13,14 @@
 
 
 def splitpath(path: str, sep: Optional[str] = None) -> list:
     """ Split the path into a list of items """
     return list(filter(len, path.split(sep or os.path.sep)))
 
 
-def strip_path_inclusion(path: str, base: str) -> str:
-    path = path.replace("\\", os.path.sep).replace("/", os.path.sep)
-    return path if os.path.abspath(os.path.join(base, path)).startswith(base) else os.path.basename(path)
-
-
 ASCII_NUMBERS = list(range(48, 58))
 ASCII_UPPER_CASE_LETTERS = list(range(65, 91))
 ASCII_LOWER_CASE_LETTERS = list(range(97, 123))
 ASCII_OTHER = [45, 46, 92]  # "-", ".", and "\"
 
 # Create a set that contains all of the valid characters that
 # are allowed to appear in a Unified Naming Convention (UNC) path.
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/postprocess.py` & `assemblyline-4.4.1.dev9/assemblyline/common/postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,49 +637,49 @@
         self.reload_watcher.stop()
         while self.loop.is_running():
             if len(asyncio.all_tasks(self.loop)) == 0:
                 break
             time.sleep(0.1)
         self.loop.call_soon_threadsafe(self.loop.stop)
 
-    def _load_actions(self, _path: Optional[str] = None):
+    def _load_actions(self, _path=''):
         # Load the action data
         with CacheStore('system', config=self.config, datastore=self.datastore) as cache:
             objects = DEFAULT_POSTPROCESS_ACTIONS
             data = cache.get('postprocess_actions')
             if data:
                 try:
-                    raw: dict[str, Any] = yaml.safe_load(data)
+                    raw = yaml.safe_load(data)
                     objects = {
                         key: PostprocessAction(data)
                         for key, data in raw.items()
                     }
                 except Exception:
                     logger.exception("Couldn't load stored actions")
 
         # Check which ones can be active
-        ready_objects: dict[str, tuple[SubmissionFilter, PostprocessAction]] = {}
-        for key, action in objects.items():
-            if not action.enabled:
+        ready_objects = {}
+        for key, data in objects.items():
+            if not data.enabled:
                 continue
 
             try:
-                fltr = SubmissionFilter(action.filter)
+                fltr = SubmissionFilter(data.filter)
             except Exception:
                 logger.exception("Failed to load submission filter")
                 continue
 
-            if self.running_cache_tasks and action.run_on_cache:
+            if self.running_cache_tasks and data.run_on_cache:
                 if not fltr.cache_safe:
                     logger.error("Tried to apply non-cache-safe filter to cached submissions.")
                     continue
-                ready_objects[key] = fltr, action
+                ready_objects[key] = fltr, data
 
-            if not self.running_cache_tasks and action.run_on_completed:
-                ready_objects[key] = fltr, action
+            if not self.running_cache_tasks and data.run_on_completed:
+                ready_objects[key] = fltr, data
 
         # Swap in the new actions
         self.actions = ready_objects
 
     def process_submission(self, submission: Submission, tags: list[dict[str, Any]]) -> bool:
         return self.process(submission=submission, tags=tags, score=submission.max_score)
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/random_user.py` & `assemblyline-4.4.1.dev9/assemblyline/common/random_user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/security.py` & `assemblyline-4.4.1.dev9/assemblyline/common/security.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/signaturing.py` & `assemblyline-4.4.1.dev9/assemblyline/common/signaturing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/str_utils.py` & `assemblyline-4.4.1.dev9/assemblyline/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/tag_safelist.yml` & `assemblyline-4.4.1.dev9/assemblyline/common/tag_safelist.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/tagging.py` & `assemblyline-4.4.1.dev9/assemblyline/common/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/common/uid.py` & `assemblyline-4.4.1.dev9/assemblyline/common/uid.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datasource/al.py` & `assemblyline-4.4.1.dev9/assemblyline/datasource/al.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datasource/alert.py` & `assemblyline-4.4.1.dev9/assemblyline/datasource/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datasource/common.py` & `assemblyline-4.4.1.dev9/assemblyline/datasource/common.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/bulk.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/bulk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/collection.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 import elasticsearch
 import elasticsearch.helpers
 
 from assemblyline import odm
 from assemblyline.common.dict_utils import recursive_update
 from assemblyline.datastore.bulk import ElasticBulkPlan
-from assemblyline.datastore.exceptions import (DataStoreException, MultiKeyError, SearchException, ArchiveDisabled)
+from assemblyline.datastore.exceptions import (DataStoreException, MultiKeyError, SearchException,
+                                               SearchRetryException, ArchiveDisabled)
 from assemblyline.datastore.support.build import back_mapping, build_mapping
 from assemblyline.datastore.support.schemas import (default_dynamic_strings, default_dynamic_templates,
                                                     default_index, default_mapping)
 from assemblyline.odm.base import BANNED_FIELDS, Keyword, Integer, List, Mapping, Model, ClassificationObject, _Field
 
 
 if typing.TYPE_CHECKING:
@@ -208,63 +209,60 @@
 
         self.stored_fields = {}
         if model_class:
             for name, field in model_class.flat_fields().items():
                 if field.store:
                     self.stored_fields[name] = field
 
-    def is_archive_index(self, index):
-        return self.archive_name and index.startswith(self.archive_name)
-
     def get_index_list(self, index_type):
         # Default value
         if index_type is None:
             # If has an archive: hot + archive
-            if self.archive_name and self.datastore.archive_access:
-                return [self.name, self.archive_name]
+            if self.index_archive_name and self.datastore.archive_access:
+                return [self.index_name, self.index_archive_name]
             # Otherwise just hot
-            return [self.name]
+            return [self.index_name]
 
         # If specified index is HOT
         elif index_type == Index.HOT:
-            return [self.name]
+            return [self.index_name]
 
         # If only archive asked
         elif index_type == Index.ARCHIVE:
             # Crash if index has no archive
-            if not self.archive_name:
+            if not self.index_archive_name:
                 raise ArchiveDisabled(f"Index {self.name.upper()} does not have an archive")
 
             # Crash if no archive access
             if not self.datastore.archive_access:
                 raise ArchiveDisabled(
                     "Trying to get access to the archive on a datastore where archive_access is disabled")
 
             # Return only archive index
-            return [self.archive_name]
+            return [self.index_archive_name]
         else:
             # Crash if no archive access
             if not self.datastore.archive_access:
                 raise ArchiveDisabled(
                     "Trying to get access to the archive on a datastore where archive_access is disabled")
 
             # Return HOT if asked for both but only has HOT
-            if not self.archive_name:
-                return [self.name]
+            if not self.index_archive_name:
+                return [self.index_name]
 
             # Otherwise return hot and archive indices
-            return [self.name, self.archive_name]
+            return [self.index_name, self.index_archive_name]
 
     def get_joined_index(self, index_type):
         return ",".join(self.get_index_list(index_type))
 
     def scan_with_search_after(self, query, sort=None, source=None, index=None, keep_alive=KEEP_ALIVE, size=1000,
                                timeout=None):
         if index is None:
-            index = self.name
+            index = self.index_name
         if not sort:
             sort = []
 
         # Generate the point in time
         pit = {'id': self.with_retries(self.datastore.client.open_point_in_time,
                                        index=index, keep_alive=keep_alive)['id'],
                'keep_alive': keep_alive}
@@ -362,20 +360,14 @@
             except elasticsearch.exceptions.TransportError as e:
                 err_code, _, _ = e.args
                 if err_code == 408 or err_code == '408':
                     log.warning(f"Waiting for index {index} to get to status {min_status}...")
                     pass
                 else:
                     raise
-            except elasticsearch.ApiError as err:
-                if err.meta.status == 408:
-                    log.warning(f"Waiting for index {index} to get to status {min_status}...")
-                    pass
-                else:
-                    raise
 
     def _safe_index_copy(self, copy_function, src, target, settings=None, min_status='yellow'):
         ret = copy_function(index=src, target=target, settings=settings, timeout='60s')
         if not ret['acknowledged']:
             raise DataStoreException(f"Failed to create index {target} from {src}.")
 
         self._wait_for_status(target, min_status=min_status)
@@ -465,15 +457,15 @@
         """
         Copy/Move a single document into the archive and return the document that was archived.
 
         :param key: ID of the document to copy or move to the archive
         :param allow_missing: If True, does not crash if the document you are trying to archive is missing
         :param delete_after: Delete the document from hot storage after archive
         """
-        if not self.archive_name:
+        if not self.index_archive_name:
             raise ArchiveDisabled("This datastore object does not have archive access.")
 
         # Check if already in archive
         if not self.exists(key, index_type=Index.ARCHIVE):
             # Get the document from hot index
             doc = self.get_if_exists(key, index_type=Index.HOT)
             if doc:
@@ -496,31 +488,31 @@
     def archive_by_query(self, query, max_docs=None, sort=None, delete_after=False):
         """
         This function should archive to document that are matching to query to an time splitted index
 
         :param query: query to run to archive documents
         :return: Number of archived documents
         """
-        if not self.archive_name:
+        if not self.index_archive_name:
             raise ArchiveDisabled("This datastore object does not have archive access.")
 
         source = {
-            "index": self.name,
+            "index": self.index_name,
             "query": {
                 "bool": {
                     "must": {
                         "query_string": {
                             "query": query
                         }
                     }
                 }
             }
         }
         dest = {
-            "index": self.archive_name
+            "index": self.index_archive_name
         }
         if max_docs:
             source['size'] = max_docs
 
         if sort:
             source['sort'] = parse_sort(sort)
 
@@ -577,15 +569,15 @@
         specified in self.datastore.hosts.
 
         :param index_type: Type of indices to target
         :return: Should return True of the fix was successful on all hosts
         """
         results = []
         for index in self.get_index_list(index_type):
-            replicas = self._get_index_settings(archive=self.is_archive_index(index))['index']['number_of_replicas']
+            replicas = self._get_index_settings(archive=index == self.index_archive_name)['index']['number_of_replicas']
             settings = {"number_of_replicas": replicas}
             results.append(self.with_retries(
                 self.datastore.client.indices.put_settings, index=index, settings=settings)['acknowledged'])
         return all(results)
 
     def fix_shards(self, logger=None, index_type=None):
         """
@@ -594,18 +586,18 @@
 
         :param index_type: Type of indices to target
         :return: Should return True of the fix was successful on all hosts
         """
         if logger is None:
             logger = log
 
-        for name in self.get_index_list(index_type):
-            index = f"{name}_hot"
+        for index in self.get_index_list(index_type):
             logger.info(f'Processing index: {index.upper()}')
-            settings = self._get_index_settings(archive=self.is_archive_index(name))
+            name = index.replace("_hot", "")
+            settings = self._get_index_settings(archive=index == self.index_archive_name)
             index_copy_settings = {"index.number_of_replicas": 0}
             clone_finish_settings = None
             clone_setup_settings = None
             method = None
             target_node = ""
             temp_name = f'{name}__fix_shards'
 
@@ -647,15 +639,15 @@
             if method:
                 # Before we do anything, we should make sure the source index is in a good state
                 logger.info(f"Waiting for {name.upper()} status to be GREEN.")
                 self._wait_for_status(name, min_status='green')
 
                 # Block all indexes to be written to
                 logger.info("Set a datastore wide write block on Elastic.")
-                self.with_retries(self.datastore.client.indices.put_settings, index=name, settings=write_block_settings)
+                self.with_retries(self.datastore.client.indices.put_settings, settings=write_block_settings)
 
                 # Clone it onto a temporary index
                 if not self.with_retries(self.datastore.client.indices.exists, index=temp_name):
                     # if there are specific settings to be applied to the index, apply them
                     if clone_setup_settings:
                         logger.info(f"Rellocating index to node {target_node.upper()}.")
                         self.with_retries(self.datastore.client.indices.put_settings,
@@ -697,79 +689,90 @@
                             f"and delete {temp_name.upper()}.")
                 actions = [{"add":  {"index": index, "alias": name}}, {
                     "remove_index": {"index": temp_name}}]
                 self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
 
             # Restore writes
             logger.info("Restore datastore wide write operation on Elastic.")
-            self.with_retries(self.datastore.client.indices.put_settings, index=name, settings=write_unblock_settings)
+            self.with_retries(self.datastore.client.indices.put_settings, settings=write_unblock_settings)
 
             # Restore normal routing and replicas
             logger.info(f"Restore original routing table for {name.upper()}.")
             self.with_retries(self.datastore.client.indices.put_settings, index=name,
                               settings=clone_finish_settings)
 
     def reindex(self, index_type=None):
         """
-        This function triggers a reindex of the current index, this should almost never be used because:
-            1. There is no crash recovery
-            2. Even if the system is still accessible during that time the data is partially accessible
+        This function should be overloaded to perform a reindex of all the data of the different hosts
+        specified in self.datastore.hosts.
 
         :param index_type: Type of indices to target
         :return: Should return True of the commit was successful on all hosts
         """
-        for name in self.get_index_list(index_type):
-            index = f"{name}_hot"
-            archive = self.is_archive_index(index)
+        for index in self.get_index_list(index_type):
+            archive = index == self.index_archive_name
             new_name = f'{index}__reindex'
             if self.with_retries(self.datastore.client.indices.exists, index=index) and \
                     not self.with_retries(self.datastore.client.indices.exists, index=new_name):
 
+                # Get information about the index to reindex
+                index_data = self.with_retries(self.datastore.client.indices.get, index=index)[index]
+
                 # Create reindex target
                 self.with_retries(self.datastore.client.indices.create, index=new_name,
                                   mappings=self._get_index_mappings(),
                                   settings=self._get_index_settings(archive=archive))
 
-                # Swap indices
-                actions = [{"add": {"index": new_name, "alias": name}},
-                           {"remove": {"index": index, "alias": name}}, ]
-                self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
+                # For all aliases related to the index, add a new alias to the reindex index
+                for alias, alias_data in index_data['aliases'].items():
+                    # Make the reindex index the new write index if the original index was
+                    if alias_data.get('is_write_index', True):
+                        actions = [
+                            {"add": {"index": new_name, "alias": alias, "is_write_index": True}},
+                            {"add": {"index": index, "alias": alias, "is_write_index": False}}, ]
+                    else:
+                        actions = [
+                            {"add": {"index": new_name, "alias": alias}}]
+                    self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
 
                 # Reindex data into target
                 r_task = self.with_retries(self.datastore.client.reindex, source={"index": index},
                                            dest={"index": new_name}, wait_for_completion=False)
                 self._get_task_results(r_task)
 
                 # Commit reindexed data
                 self.with_retries(self.datastore.client.indices.refresh, index=new_name)
                 self.with_retries(self.datastore.client.indices.clear_cache, index=new_name)
 
                 # Delete old index
                 self.with_retries(self.datastore.client.indices.delete, index=index)
 
                 # Block write to the index
-                self.with_retries(self.datastore.client.indices.put_settings, index=name, settings=write_block_settings)
+                self.with_retries(self.datastore.client.indices.put_settings, settings=write_block_settings)
 
                 # Rename reindexed index
                 try:
                     self._safe_index_copy(self.datastore.client.indices.clone, new_name, index,
                                           settings=self._get_index_settings(archive=archive))
 
                     # Restore original aliases for the index
-                    actions = [{"add": {"index": index, "alias": name}},
-                               {"remove": {"index": new_name, "alias": name}}, ]
-                    self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
+                    for alias, alias_data in index_data['aliases'].items():
+                        # Make the reindex index the new write index if the original index was
+                        if alias_data.get('is_write_index', True):
+                            actions = [
+                                {"add": {"index": index, "alias": alias, "is_write_index": True}},
+                                {"remove_index": {"index": new_name}}]
+                            self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
 
                     # Delete the reindex target if it still exists
                     if self.with_retries(self.datastore.client.indices.exists, index=new_name):
                         self.with_retries(self.datastore.client.indices.delete, index=new_name)
                 finally:
                     # Unblock write to the index
-                    self.with_retries(self.datastore.client.indices.put_settings,
-                                      index=name, settings=write_unblock_settings)
+                    self.with_retries(self.datastore.client.indices.put_settings, settings=write_unblock_settings)
 
         return True
 
     def multiexists(self, key_list, index_type=None):
         """
         With a list of keys, check if all those keys exists in the specified indices
 
@@ -833,16 +836,16 @@
                 if 'found' in row and not row['found']:
                     continue
 
                 try:
                     key_list.remove(row['_id'])
 
                     # If this index has an archive, check is the document was found in it.
-                    if self.archive_name:
-                        row['_source']['from_archive'] = self.is_archive_index(index)
+                    if self.index_archive_name:
+                        row['_source']['from_archive'] = index == self.index_archive_name
 
                     add_to_output(row['_source'], row['_id'])
                 except ValueError:
                     log.error(f'MGet returned multiple documents for id: {row["_id"]}')
 
         if key_list and error_on_missing:
             raise MultiKeyError(key_list, out)
@@ -902,16 +905,16 @@
         done = False
         while not done:
             for index in index_list:
                 try:
                     doc = self.with_retries(self.datastore.client.get, index=index, id=key)
 
                     # If this index has an archive, check is the document was found in it.
-                    if self.archive_name:
-                        doc['_source']['from_archive'] = self.is_archive_index(index)
+                    if self.index_archive_name:
+                        doc['_source']['from_archive'] = index == self.index_archive_name
 
                     if version:
                         return self._normalize_output(doc['_source']), f"{doc['_seq_no']}---{doc['_primary_term']}"
                     return self._normalize_output(doc['_source'])
                 except elasticsearch.exceptions.NotFoundError:
                     pass
 
@@ -1181,37 +1184,25 @@
 
                 if prev_key:
                     field = fields[prev_key].child_type
                 else:
                     field = fields[doc_key]
 
                 if op in [self.UPDATE_APPEND, self.UPDATE_APPEND_IF_MISSING, self.UPDATE_REMOVE]:
-                    if not field.multivalued:
-                        raise DataStoreException(f"Invalid operation for field {doc_key}: {op}")
-
                     try:
                         value = field.check(value)
                     except (ValueError, TypeError, AttributeError):
                         raise DataStoreException(f"Invalid value for field {doc_key}: {value}")
 
-                elif op in [self.UPDATE_DEC, self.UPDATE_INC]:
+                elif op in [self.UPDATE_SET, self.UPDATE_DEC, self.UPDATE_INC]:
                     try:
                         value = field.check(value)
                     except (ValueError, TypeError):
                         raise DataStoreException(f"Invalid value for field {doc_key}: {value}")
 
-                elif op in self.UPDATE_SET:
-                    try:
-                        if field.multivalued and isinstance(value, list):
-                            value = [field.check(v) for v in value]
-                        else:
-                            value = field.check(value)
-                    except (ValueError, TypeError):
-                        raise DataStoreException(f"Invalid value for field {doc_key}: {value}")
-
                 if isinstance(value, Model):
                     value = value.as_primitives()
                 elif isinstance(value, datetime):
                     value = value.isoformat()
                 elif isinstance(value, ClassificationObject):
                     value = str(value)
 
@@ -1301,16 +1292,16 @@
         extra_fields = result.get('fields', {})
         source_data = result.pop('_source', None)
         for f in BANNED_FIELDS:
             source_data.pop(f, None)
         item_id = result['_id']
 
         # If this index has an archive, check is the document was found in it.
-        if self.archive_name:
-            source_data['from_archive'] = self.is_archive_index(result['_index'])
+        if self.index_archive_name:
+            source_data['from_archive'] = result['_index'] == self.index_archive_name
 
         if self.model_class:
             if not fields:
                 fields = list(self.stored_fields.keys())
                 fields.append('id')
             elif isinstance(fields, str):
                 fields = fields.split(',')
@@ -1506,14 +1497,17 @@
             else:
                 # Run the query
                 result = self.with_retries(self.datastore.client.search, index=index,
                                            track_total_hits=track_total_hits, **query_body)
 
             return result
 
+        except (elasticsearch.ConnectionError, elasticsearch.ConnectionTimeout) as error:
+            raise SearchRetryException("collection: %s, query: %s, error: %s" % (self.name, query_body, str(error)))
+
         except (elasticsearch.TransportError, elasticsearch.RequestError) as e:
             try:
                 err_msg = e.info['error']['root_cause'][0]['reason']
             except (ValueError, KeyError, IndexError):
                 err_msg = str(e)
             raise SearchException(err_msg)
 
@@ -1760,16 +1754,15 @@
             ('query', query),
             ('histogram_active', True),
             ('histogram_field', field),
             ('histogram_type', "date_histogram" if isinstance(gap, str) else 'histogram'),
             ('histogram_gap', gap.strip('+').strip('-') if isinstance(gap, str) else gap),
             ('histogram_mincount', mincount),
             ('histogram_start', start),
-            ('histogram_end', end),
-            ('df', self.DEFAULT_SEARCH_FIELD)
+            ('histogram_end', end)
         ]
 
         if access_control:
             filters.append(access_control)
 
         if filters:
             args.append(('filters', filters))
@@ -1788,16 +1781,15 @@
             filters = [filters]
 
         args = [
             ('query', query),
             ('facet_active', True),
             ('facet_fields', [field]),
             ('facet_mincount', mincount),
-            ('rows', 0),
-            ('df', self.DEFAULT_SEARCH_FIELD)
+            ('rows', 0)
         ]
 
         if access_control:
             filters.append(access_control)
 
         if filters:
             args.append(('filters', filters))
@@ -1817,16 +1809,15 @@
         elif isinstance(filters, str):
             filters = [filters]
 
         args = [
             ('query', query),
             ('stats_active', True),
             ('stats_fields', [field]),
-            ('rows', 0),
-            ('df', self.DEFAULT_SEARCH_FIELD)
+            ('rows', 0)
         ]
 
         if access_control:
             filters.append(access_control)
 
         if filters:
             args.append(('filters', filters))
@@ -1858,16 +1849,15 @@
             ('query', query),
             ('group_active', True),
             ('group_field', group_field),
             ('group_limit', limit),
             ('group_sort', group_sort),
             ('start', offset),
             ('rows', rows),
-            ('sort', sort),
-            ('df', self.DEFAULT_SEARCH_FIELD)
+            ('sort', sort)
         ]
 
         filters.append("%s:*" % group_field)
 
         if fl:
             field_list = fl.split(',')
             args.append(('field_list', field_list))
@@ -1917,16 +1907,16 @@
                 elif 'type' in value:
                     out[name] = value
                 else:
                     raise ValueError("Unknown field data " + str(props))
             return out
 
         data = self.with_retries(self.datastore.client.indices.get, index=self.name)
-        idx_name = list(data.keys())[0]
-        properties = flatten_fields(data[idx_name]['mappings'].get('properties', {}))
+        index_name = list(data.keys())[0]
+        properties = flatten_fields(data[index_name]['mappings'].get('properties', {}))
 
         if self.model_class:
             model_fields = self.model_class.flat_fields()
         else:
             model_fields = {}
 
         collection_data = {}
@@ -2023,45 +2013,43 @@
     def _ensure_collection(self):
         """
         This function should test if the collection that you are trying to access does indeed exist
         and should create it if it does not.
 
         :return:
         """
-        for alias in self.get_index_list(None):
-            index = f"{alias}_hot"
+        for index in self.get_index_list(None):
+            alias = index.replace("_hot", "")
             # Create HOT index
             if not self.with_retries(self.datastore.client.indices.exists, index=alias):
                 log.debug(f"Index {alias.upper()} does not exists. Creating it now...")
                 try:
                     self.with_retries(self.datastore.client.indices.create, index=index,
                                       mappings=self._get_index_mappings(),
-                                      settings=self._get_index_settings(archive=self.is_archive_index(index)))
+                                      settings=self._get_index_settings(archive=index == self.index_archive_name))
                 except elasticsearch.exceptions.RequestError as e:
                     if "resource_already_exists_exception" not in str(e):
                         raise
                     log.warning(f"Tried to create an index template that already exists: {alias.upper()}")
 
                 self.with_retries(self.datastore.client.indices.put_alias, index=index, name=alias)
             elif not self.with_retries(self.datastore.client.indices.exists, index=index) and \
                     not self.with_retries(self.datastore.client.indices.exists_alias, name=alias):
                 # Turn on write block
-                self.with_retries(self.datastore.client.indices.put_settings,
-                                  index=alias, settings=write_block_settings)
+                self.with_retries(self.datastore.client.indices.put_settings, settings=write_block_settings)
 
                 # Create a copy on the result index
                 self._safe_index_copy(self.datastore.client.indices.clone, alias, index)
 
                 # Make the hot index the new clone
                 actions = [{"add":  {"index": index, "alias": alias}}, {
                     "remove_index": {"index": alias}}]
                 self.with_retries(self.datastore.client.indices.update_aliases, actions=actions)
 
-                self.with_retries(self.datastore.client.indices.put_settings,
-                                  index=alias, settings=write_unblock_settings)
+                self.with_retries(self.datastore.client.indices.put_settings, settings=write_unblock_settings)
 
         self._check_fields()
 
     def _add_fields(self, missing_fields: Dict):
         no_fix = []
         properties = {}
         for name, field in missing_fields.items():
@@ -2094,15 +2082,15 @@
         This function should completely delete the collection
 
         NEVER USE THIS!
 
         :return:
         """
 
-        for name in self.get_index_list(index_type):
-            index = f"{name}_hot"
+        for index in self.get_index_list(index_type):
+            name = index.replace("_hot", "")
             log.debug("Wipe operation started for collection: %s" % name.upper())
             if self.with_retries(self.datastore.client.indices.exists, index=index):
                 self.with_retries(self.datastore.client.indices.delete, index=index)
 
         if recreate:
             self._ensure_collection()
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/exceptions.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import Iterable
 
 
+class SearchRetryException(Exception):
+    pass
+
+
 class DataStoreException(Exception):
     pass
 
 
 class SearchException(Exception):
     pass
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/helper.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,19 +791,24 @@
 
         for key, item in items.items():
             sorted_sections = sorted(item.get('result', {}).get('sections', []),
                                      key=lambda i: i['heuristic']['score'] if i['heuristic'] is not None else 0,
                                      reverse=True)
             for section in sorted_sections:
                 file_classification = files.get(key[:64], {}).get('classification', section['classification'])
-                combined_classification = cl_engine.max_classification(file_classification, section['classification'])
-                if user_classification and not cl_engine.is_accessible(user_classification, combined_classification):
-                    out["filtered"] = True
-                    continue
-                out["classification"] = cl_engine.max_classification(out["classification"], combined_classification)
+                if user_classification:
+                    if not cl_engine.is_accessible(user_classification, section['classification']):
+                        out["filtered"] = True
+                        continue
+                    if not cl_engine.is_accessible(user_classification, file_classification):
+                        out["filtered"] = True
+                        continue
+
+                out["classification"] = cl_engine.max_classification(out["classification"], section['classification'])
+                out["classification"] = cl_engine.max_classification(out["classification"], file_classification)
 
                 h_type = "info"
 
                 if section.get('heuristic', False):
                     heur_id = section['heuristic']['heur_id']
                     heur_name = section['heuristic']['name']
 
@@ -870,16 +875,15 @@
                             if cache_key not in done_map['tags']:
                                 out['tags'].append({
                                     'type': tag_type,
                                     'h_type': h_type,
                                     'short_type': tag_type.rsplit(".", 1)[-1],
                                     'value': tag,
                                     'key': key,
-                                    'safelisted': False,
-                                    'classification': combined_classification,
+                                    'safelisted': False
                                 })
                                 done_map['tags'].add(cache_key)
 
                 # Get safelisted tag data
                 for tag_type, tags in section.get('safelisted_tags', {}).items():
                     if tags is not None:
                         for tag in tags:
@@ -888,16 +892,15 @@
                             if cache_key not in done_map['tags']:
                                 out['tags'].append({
                                     'type': tag_type,
                                     'h_type': h_type,
                                     'short_type': tag_type.rsplit(".", 1)[-1],
                                     'value': tag,
                                     'key': key,
-                                    'safelisted': True,
-                                    'classification': combined_classification,
+                                    'safelisted': True
                                 })
                                 done_map['tags'].add(cache_key)
 
             for htype in out['heuristics']:
                 for heur in out['heuristics'][htype]:
                     cache_key = f"{heur_id}_{key}"
                     heur['signatures'].extend(signatures.get(cache_key, []))
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/store.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/store.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from urllib.parse import urlparse
 
 import elasticsearch
 import elasticsearch.helpers
 
 from assemblyline.common import forge
 from assemblyline.datastore.collection import ESCollection
-from assemblyline.datastore.exceptions import (DataStoreException, UnsupportedElasticVersion, VersionConflictException)
+from assemblyline.datastore.exceptions import (DataStoreException, UnsupportedElasticVersion,
+                                               SearchRetryException, VersionConflictException)
 
 from packaging import version
 
 TRANSPORT_TIMEOUT = int(environ.get('AL_DATASTORE_TRANSPORT_TIMEOUT', '90'))
 DATASTORE_ROOT_CA_PATH = environ.get('DATASTORE_ROOT_CA_PATH', '/etc/assemblyline/ssl/al_root-ca.crt')
 log = logging.getLogger('assemblyline.datastore')
 
@@ -231,27 +232,14 @@
                     ret_val['updated'] += updated
 
                 if deleted:
                     ret_val['deleted'] += deleted
 
                 return ret_val
 
-            except elasticsearch.NotFoundError as error:
-                index_name = kwargs.get('index', '').upper()
-                err_message = str(error)
-
-                # Validate exception type
-                if not index_name or "No search context found" not in err_message:
-                    raise
-
-                log.warning(f"Index {index_name} was removed while a query was running, retrying...")
-                time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
-                self.connection_reset()
-                retries += 1
-
             except elasticsearch.exceptions.ConflictError as ce:
                 if raise_conflicts:
                     # De-sync potential treads trying to write to the index
                     time.sleep(random() * 0.1)
                     raise VersionConflictException(str(ce))
                 updated += ce.info.get('updated', 0)
                 deleted += ce.info.get('deleted', 0)
@@ -260,79 +248,45 @@
                 self.connection_reset()
                 retries += 1
 
             except elasticsearch.exceptions.ConnectionTimeout:
                 log.warning(f"Elasticsearch connection timeout, server(s): "
                             f"{' | '.join(self.get_hosts(safe=True))}"
                             f", retrying {func.__name__}...")
-
                 time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
                 self.connection_reset()
                 retries += 1
 
-            except (elasticsearch.exceptions.ConnectionError,
+            except (SearchRetryException,
+                    elasticsearch.exceptions.ConnectionError,
                     elasticsearch.exceptions.AuthenticationException) as e:
-                log.warning(f"No connection to Elasticsearch server(s): "
-                            f"{' | '.join(self.get_hosts(safe=True))}"
-                            f", because [{e}] retrying {func.__name__}...")
+                if not isinstance(e, SearchRetryException):
+                    log.warning(f"No connection to Elasticsearch server(s): "
+                                f"{' | '.join(self.get_hosts(safe=True))}"
+                                f", because [{e}] retrying {func.__name__}...")
 
                 time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
                 self.connection_reset()
                 retries += 1
 
-            # Legacy retries, only for elastic 7.x client...
             except elasticsearch.exceptions.TransportError as e:
                 err_code, _, _ = e.args
-                err_code = int(err_code)
-                index_name = kwargs.get('index', '').upper()
-
-                # Validate exception type
-                if not index_name or err_code not in [503, 429, 403]:
-                    raise
-
-                # Display proper error message
-                if err_code == 503:
-                    log.warning(f"Looks like index {index_name} is not ready yet, retrying...")
-                elif err_code == 429:
+                if err_code == 503 or err_code == '503':
+                    log.warning(f"Looks like index {self.name} is not ready yet, retrying...")
+                    time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
+                    self.connection_reset()
+                    retries += 1
+                elif err_code == 429 or err_code == '429':
                     log.warning("Elasticsearch is too busy to perform the requested "
-                                f"task on index {index_name}, retrying...")
-                elif err_code == 403:
+                                f"task on index {self.name}, retrying...")
+                    time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
+                    self.connection_reset()
+                    retries += 1
+                elif err_code == 403 or err_code == '403':
                     log.warning("Elasticsearch cluster is preventing writing operations "
-                                f"on index {index_name}, retrying...")
-
-                # Loop and retry
-                time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
-                self.connection_reset()
-                retries += 1
+                                f"on index {self.name}, retrying...")
+                    time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
+                    self.connection_reset()
+                    retries += 1
 
-            # Elastic client 8.x retries
-            except elasticsearch.AuthorizationException:
-                index_name = kwargs.get('index', '').upper()
-                if not index_name:
+                else:
                     raise
-
-                log.warning("Elasticsearch cluster is preventing writing operations "
-                            f"on index {index_name}, retrying...")
-
-                time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
-                self.connection_reset()
-                retries += 1
-
-            except elasticsearch.ApiError as err:
-                index_name = kwargs.get('index', '').upper()
-                err_code = err.meta.status
-
-                # Validate exception type
-                if not index_name or err_code not in [503, 429, 403]:
-                    raise
-
-                # Display proper error message
-                if err_code == 503:
-                    log.warning(f"Looks like index {index_name} is not ready yet, retrying...")
-                elif err_code == 429:
-                    log.warning("Elasticsearch is too busy to perform the requested "
-                                f"task on index {index_name}, retrying...")
-
-                # Loop and retry
-                time.sleep(min(retries, self.MAX_RETRY_BACKOFF))
-                self.connection_reset()
-                retries += 1
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/support/build.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/support/build.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/datastore/support/schemas.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/support/schemas.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/azure.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/azure.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/base.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/ftp.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/ftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/http.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/http.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/local.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import shutil
 import re
 from typing import AnyStr, Iterable, Optional
 
 from assemblyline.common.exceptions import ChainAll
-from assemblyline.common.path import strip_path_inclusion
 from assemblyline.common.uid import get_random_id
 from assemblyline.filestore.transport.base import Transport, TransportException, normalize_srl_path
 
 NORMALIZED = re.compile('[a-z0-9]/[a-z0-9]/[a-z0-9]/[a-z0-9]/[a-z0-9]{64}')
 
 
 @ChainAll(TransportException)
@@ -164,8 +163,8 @@
 ###############################
 
 
 def _join(base, path):
     path = path.replace("\\", "/").replace("//", "/")
     if base is None:
         return path
-    return os.path.join(base, strip_path_inclusion(path, base)).replace("\\", "/")
+    return os.path.join(base, path.lstrip("/")).replace("\\", "/")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/s3.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,23 +52,30 @@
         else:
             self.port = port
 
         self.scheme = {True: "https", False: "http"}[self.use_ssl]
 
         self.endpoint_url = "{scheme}://{host}:{port}".format(scheme=self.scheme, host=self.host, port=self.port)
 
+        config = None
+        host_root_ca = os.environ.get(f'{host.upper()}_ROOT_CA_PATH', '/etc/assemblyline/ssl/al_root-ca.crt')
+        if self.use_ssl and os.path.exists(host_root_ca):
+            # Verify against the Root CA associated to the filestore host
+            verify = host_root_ca
+
         session = boto3.session.Session()
         self.client = session.client(
             "s3",
             aws_access_key_id=accesskey,
             aws_secret_access_key=secretkey,
             endpoint_url=self.endpoint_url,
             region_name=aws_region,
             use_ssl=self.use_ssl,
             verify=verify,
+            config=config
         )
 
         bucket_exist = False
         try:
             self.with_retries(self.client.head_bucket, Bucket=self.bucket)
             bucket_exist = True
         except TransportException as e:
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/filestore/transport/sftp.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/sftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/base.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,27 @@
     r"::(?:ffff(?::0{1,4}){0,1}:){0,1}(?:(?:25[0-5]|(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(?:25[0-5]|" \
     r"(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])|(?:[0-9a-fA-F]{1,4}:){1,4}:(?:(?:25[0-5]|" \
     r"(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(?:25[0-5]|(?:2[0-4]|1{0,1}[0-9]){0,1}[0-9]))"
 IP_REGEX = f"(?:{IPV4_REGEX}|{IPV6_REGEX})"
 IP_ONLY_REGEX = f"^{IP_REGEX}$"
 IPV4_ONLY_REGEX = f"^{IPV4_REGEX}$"
 IPV6_ONLY_REGEX = f"^{IPV6_REGEX}$"
-PORT_REGEX = r"(0|[1-9][0-9]{0,3}|[1-5][0-9]{4}|6[0-4][0-9]{3}|65[0-4][0-9]{2}|655[0-2][0-9]|6553[0-5])"
 PRIVATE_IP = r"(?:(?:127|10)(?:\.(?:[2](?:[0-5][0-5]|[01234][6-9])|[1][0-9][0-9]|[1-9][0-9]|[0-9])){3})|" \
              r"(?:172\.(?:1[6-9]|2[0-9]|3[0-1])(?:\.(?:2[0-4][0-9]|25[0-5]|[1][0-9][0-9]|[1-9][0-9]|[0-9])){2}|" \
              r"(?:192\.168(?:\.(?:25[0-5]|2[0-4][0-9]|1[0-9][0-9]|[1-9][0-9]|[0-9])){2}))"
 PHONE_REGEX = r"^(\+?\d{1,2})?[ .-]?(\(\d{3}\)|\d{3})[ .-](\d{3})[ .-](\d{4})$"
 SSDEEP_REGEX = r"^[0-9]{1,18}:[a-zA-Z0-9/+]{0,64}:[a-zA-Z0-9/+]{0,64}$"
 MD5_REGEX = r"^[a-f0-9]{32}$"
 SHA1_REGEX = r"^[a-f0-9]{40}$"
 SHA256_REGEX = r"^[a-f0-9]{64}$"
 MAC_REGEX = r"^(?:(?:[0-9a-f]{2}-){5}[0-9a-f]{2}|(?:[0-9a-f]{2}:){5}[0-9a-f]{2})$"
 URI_PATH = r"(?:[/?#]\S*)"
 FULL_URI = f"^((?:(?:[A-Za-z0-9+-.]{{1,}}:)?//)(?:\\S+(?::\\S*)?@)?({IP_REGEX}|{DOMAIN_REGEX})(?::\\d{{1,5}})?)" \
            f"{URI_PATH}?$"
 UNC_PATH_REGEX = r"^(?:\\\\(?:[a-zA-Z0-9-_\s]{1,15}){1}(?:\.[a-zA-Z0-9-_\s]{1,64}){0,3}){1}" \
-                 f"(?:@{PORT_REGEX})?" \
                  r'(?:\\[^\\\/\:\*\?\\"\<\>\|\r\n]{1,64}){1,}\\{0,}$'
 PLATFORM_REGEX = r"^(Windows|Linux|MacOS|Android|iOS)$"
 PROCESSOR_REGEX = r"^x(64|86)$"
 
 logger = logging.getLogger('assemblyline.odm')
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/alert.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/alerter_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/alerter_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/archive_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/archive_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/changes.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/changes.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/dispatcher_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatcher_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/dispatching.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/expiry_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/expiry_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/ingest_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/ingest_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/metrics.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/scaler_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/scaler_status_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_status_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/service_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/service_timing_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_timing_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/submission.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/task.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/task.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/messages/vacuum_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/vacuum_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/actions.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/actions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/alert.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/config.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List
 
 from assemblyline import odm
 from assemblyline.odm.models.service import EnvironmentVariable
 from assemblyline.odm.models.service_delta import DockerConfigDelta
 
 
-AUTO_PROPERTY_TYPE = ['access', 'classification', 'type', 'role', 'remove_role', 'group']
+AUTO_PROPERTY_TYPE = ['access', 'classification', 'type', 'role', 'remove_role']
 
 
 @odm.model(index=False, store=False, description="Password Requirement")
 class PasswordRequirement(odm.Model):
     lower: bool = odm.Boolean(description="Password must contain lowercase letters")
     number: bool = odm.Boolean(description="Password must contain numbers")
     special: bool = odm.Boolean(description="Password must contain special characters")
@@ -605,15 +605,15 @@
                                       description="Configurations to be used with container registries")
 
 
 DEFAULT_UPDATER = {
     'job_dockerconfig': {
         'cpu_cores': 1,
         'ram_mb': 1024,
-        'ram_mb_min': 256,
+        'ram_mb_min': 128,
     },
     'registry_configs': [{
         'name': 'registry.hub.docker.com',
         'proxies': {}
     }]
 }
 
@@ -698,39 +698,26 @@
 
 DEFAULT_ARCHIVE = {
     "enabled": False,
     "indices": ['file', 'submission', 'result'],
 }
 
 
-@odm.model(index=False, store=False, description="Datastore Retrohunt feature configuration")
-class Retrohunt(odm.Model):
-    enabled = odm.Boolean(description="Are we enabling Retrohunt features?")
-
-
-DEFAULT_RETROHUNT = {
-    "enabled": False
-}
-
-
 @odm.model(index=False, store=False, description="Datastore Configuration")
 class Datastore(odm.Model):
     hosts: List[str] = odm.List(odm.Keyword(), description="List of hosts used for the datastore")
     archive = odm.Compound(Archive, default=DEFAULT_ARCHIVE, description="Datastore Archive feature configuration")
-    retrohunt = odm.Compound(Retrohunt, default=DEFAULT_RETROHUNT,
-                             description="Datastore Retrohunt feature configuration")
     cache_dtl = odm.Integer(
         default=5, description="Default cache lenght for computed indices (submission_tree, submission_summary...")
     type = odm.Enum({"elasticsearch"}, description="Type of application used for the datastore")
 
 
 DEFAULT_DATASTORE = {
     "hosts": ["http://elastic:devpass@localhost:9200"],
     "archive": DEFAULT_ARCHIVE,
-    "retrohunt": DEFAULT_RETROHUNT,
     "cache_dtl": 5,
     "type": "elasticsearch",
 }
 
 
 @odm.model(index=False, store=False, description="Datasource Configuration")
 class Datasource(odm.Model):
@@ -962,43 +949,14 @@
         'url',
         'web_url'
     ]
 
 }
 
 
-@odm.model(index=False, store=False, description="Connection details for external systems/data sources.")
-class ExternalSource(odm.Model):
-    name: str = odm.Keyword(description="Name of the source.")
-    classification = odm.Optional(
-        odm.ClassificationString(
-            description="Minimum classification applied to information from the source"
-                        " and required to know the existance of the source."))
-    max_classification = odm.Optional(
-        odm.ClassificationString(description="Maximum classification of data that may be handled by the source"))
-    url: str = odm.Keyword(description="URL of the upstream source's lookup service.")
-
-
-EXAMPLE_EXTERNAL_SOURCE_VT = {
-    # This is an example on how this would work with VirusTotal
-    "name": "VirusTotal",
-    "url": "vt-lookup.namespace.svc.cluster.local",
-    "classification": "TLP:CLEAR",
-    "max_classification": "TLP:CLEAR",
-}
-
-EXAMPLE_EXTERNAL_SOURCE_MB = {
-    # This is an example on how this would work with Malware Bazaar
-    "name": "Malware Bazaar",
-    "url": "mb-lookup.namespace.scv.cluster.local",
-    "classification": "TLP:CLEAR",
-    "max_classification": "TLP:CLEAR",
-}
-
-
 @odm.model(index=False, store=False, description="UI Configuration")
 class UI(odm.Model):
     alerting_meta: AlertingMeta = odm.Compound(AlertingMeta, default=DEFAULT_ALERTING_META,
                                                description="Alerting metadata fields")
     allow_malicious_hinting: bool = odm.Boolean(
         description="Allow user to tell in advance the system that a file is malicious?")
     allow_raw_downloads: bool = odm.Boolean(description="Allow user to download raw files?")
@@ -1012,17 +970,14 @@
         values=["info", "warning", "success", "error"],
         description="Banner message level")
     debug: bool = odm.Boolean(description="Enable debugging?")
     discover_url: str = odm.Optional(odm.Keyword(), description="Discover URL")
     download_encoding = odm.Enum(values=["raw", "cart"], description="Which encoding will be used for downloads?")
     email: str = odm.Optional(odm.Email(), description="Assemblyline admins email address")
     enforce_quota: bool = odm.Boolean(description="Enforce the user's quotas?")
-    external_sources: List[ExternalSource] = odm.List(
-        odm.Compound(ExternalSource),
-        default=[], description="List of external sources to query")
     fqdn: str = odm.Text(description="Fully qualified domain name to use for the 2-factor authentication validation")
     ingest_max_priority: int = odm.Integer(description="Maximum priority for ingest API")
     read_only: bool = odm.Boolean(description="Turn on read only mode in the UI")
     read_only_offset: str = odm.Keyword(
         default="", description="Offset of the read only mode for all paging and searches")
     rss_feeds: List[str] = odm.List(odm.Keyword(), default=[], description="List of RSS feeds to display on the UI")
     services_feed: str = odm.Keyword(description="Feed of all the services available on AL")
@@ -1056,15 +1011,14 @@
     "banner": None,
     "banner_level": 'info',
     "debug": False,
     "discover_url": None,
     "download_encoding": "cart",
     "email": None,
     "enforce_quota": True,
-    "external_sources": [],
     "fqdn": "localhost",
     "ingest_max_priority": 250,
     "read_only": False,
     "read_only_offset": "",
     "rss_feeds": [
         "https://alpytest.blob.core.windows.net/pytest/stable.json",
         "https://alpytest.blob.core.windows.net/pytest/services.json"
@@ -1073,16 +1027,15 @@
     "secret_key": "This is the default flask secret key... you should change this!",
     "session_duration": 3600,
     "statistics": DEFAULT_STATISTICS,
     "tos": None,
     "tos_lockout": False,
     "tos_lockout_notify": None,
     "url_submission_headers": {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko)"
-                      " Chrome/110.0.0.0 Safari/537.36"
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
     },
     "url_submission_proxies": {},
     "validate_session_ip": True,
     "validate_session_useragent": True,
 }
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/error.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/error.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/file.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,45 +4,27 @@
 @odm.model(index=True, store=True, description="File Seen Model")
 class Seen(odm.Model):
     count = odm.Integer(default=1, description="How many times have we seen this file?")
     first = odm.Date(default="NOW", description="First seen timestamp")
     last = odm.Date(default="NOW", description="Last seen timestamp")
 
 
-@odm.model(index=True, store=True, description="Label Categories Model")
-class LabelCategories(odm.Model):
-    info = odm.List(
-        odm.Keyword(),
-        description="List of extra informational labels about the file", default=[])
-    technique = odm.List(
-        odm.Keyword(),
-        description="List of labels related to the technique used by the file and the signatures that hits on it.",
-        default=[])
-    attribution = odm.List(
-        odm.Keyword(),
-        description="List of labels related to attribution of this file (implant name, actor, campain...)",
-        default=[])
-
-
 @odm.model(index=True, store=True, description="Model of File")
 class File(odm.Model):
     archive_ts = odm.Optional(odm.Date(store=False, description="Archiving timestamp (Deprecated)"))
     ascii = odm.Keyword(index=False, store=False,
                         description="Dotted ASCII representation of the first 64 bytes of the file")
     classification = odm.Classification(description="Classification of the file")
     entropy = odm.Float(description="Entropy of the file")
     expiry_ts = odm.Optional(odm.Date(store=False), description="Expiry timestamp")
     is_section_image = odm.Boolean(default=False, description="Is this an image from an Image Result Section?")
     hex = odm.Keyword(index=False, store=False, description="Hex dump of the first 64 bytes of the file")
-    labels = odm.List(odm.Keyword(copyto="__text__"), description="List of labels of the file", default=[])
-    label_categories = odm.Compound(LabelCategories, default={}, description="Categories of label")
     md5 = odm.MD5(copyto="__text__", description="MD5 of the file")
     magic = odm.Keyword(store=False, description="Output from libmagic related to the file")
     mime = odm.Optional(odm.Keyword(store=False), description="MIME type of the file as identified by libmagic")
     seen = odm.Compound(Seen, default={}, description="Details about when the file was seen")
     sha1 = odm.SHA1(copyto="__text__", description="SHA1 hash of the file")
     sha256 = odm.SHA256(copyto="__text__", description="SHA256 hash of the file")
     size = odm.Integer(description="Size of the file in bytes")
     ssdeep = odm.SSDeepHash(store=False, description="SSDEEP hash of the file")
     type = odm.Keyword(copyto="__text__", description="Type of file as identified by Assemblyline")
-    tlsh = odm.Optional(odm.Keyword(copyto="__text__", description="TLSH hash of the file"))
     from_archive = odm.Boolean(index=False, default=False, description="Was loaded from the archive")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/filescore.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/filescore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/heuristic.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/filetypes/pe.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/pe.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/ontology.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from assemblyline import odm
 from assemblyline.common import forge
 from assemblyline.odm.models.tagging import Tagging
 from assemblyline.odm.models.ontology.results import Antivirus, Process, Sandbox, NetworkConnection, Signature, MalwareConfig
 from assemblyline.odm.models.ontology.filetypes import PE
 
 Classification = forge.get_classification()
-ODM_VERSION = "1.4"
+ODM_VERSION = "1.3"
 
 
 @odm.model(description="File Characteristics")
 class File(odm.Model):
     # Common information
     md5 = odm.MD5(description="MD5 of file")
     sha1 = odm.SHA1(description="SHA1 of file")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/antivirus.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/antivirus.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/malware_config.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/malware_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,14 @@
     value = odm.Optional(odm.Text(), description="Registry")
     usage = odm.Optional(
         odm.Enum(values=['persistence', 'store_data', 'store_payload', 'read', 'other']),
         description="Use of registry key")
 
 
 class MalwareConfig(odm.Model):
-    config_extractor = odm.Keyword(description="Name of extractor")
-
     family = odm.List(odm.Text(), description="What family is this associated to?")
     version = odm.Optional(odm.Text(), description="Version of the malware")
     category = odm.Optional(odm.List(odm.Enum(values=CATEGORIES)), description="Category of malware")
 
     attack = odm.Optional(odm.List(odm.Enum(values=list(attack_map.keys()))), description="ATT&CK ID associated")
     capability_enabled = odm.Optional(odm.List(odm.Text()), description="Enabled Capabilities")
     capability_disabled = odm.Optional(odm.List(odm.Text()), description="Disabled Capabilities")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/network.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/network.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/process.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/process.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/sandbox.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/sandbox.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/ontology/results/signature.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/replay.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/result.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
 @odm.model(index=True, store=False, description="Result Section")
 class Section(odm.Model):
     auto_collapse = odm.Boolean(default=False, description="Should the section be collapsed when displayed?")
     body = odm.Optional(odm.Text(copyto="__text__"), description="Text body of the result section")
     classification = odm.Classification(description="Classification of the section")
     body_format = odm.Enum(values=BODY_FORMAT, index=False, description="Type of body in this section")
-    body_config = odm.Optional(odm.Mapping(odm.Any(), index=False, description="Configurations for the body of this section"))
     depth = odm.Integer(index=False, description="Depth of the section")
     heuristic = odm.Optional(odm.Compound(Heuristic), description="Heuristic used to score result section")
     tags = odm.Compound(Tagging, default={}, description="List of tags associated to this section")
     safelisted_tags = odm.FlattenedListObject(store=False, default={}, description="List of safelisted tags")
     title_text = odm.Text(copyto="__text__", description="Title of the section")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/retrohunt.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/retrohunt.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,12 +13,11 @@
 
     # Search data
     yara_signature = odm.keyword(copyto="__text__")
     raw_query = odm.keyword()
     code = odm.keyword()
 
     # Completion data
-    finished = odm.boolean(default=False)
-    truncated = odm.boolean(default=False)
-    hits = odm.sequence(odm.keyword(store=False), store=False)
-    total_hits = odm.optional(odm.integer())
-    errors = odm.sequence(odm.keyword())
+    # finished = odm.boolean(default=False)
+    # truncated = odm.boolean(default=False)
+    # hits = odm.sequence(odm.keyword())
+    # error = odm.sequence(odm.keyword())
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/safelist.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/service.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                                                description="The username to use when pulling the image")
     registry_password: Opt[str] = odm.Optional(odm.Keyword(default=""),
                                                description="The password or token to use when pulling the image")
     registry_type: str = odm.Enum(values=["docker", "harbor"], default='docker',
                                   description="The type of container registry")
     ports: list[str] = odm.List(odm.Keyword(), default=[], description="What ports of container to expose?")
     ram_mb: int = odm.Integer(default=512, description="Container RAM limit")
-    ram_mb_min: int = odm.Integer(default=256, description="Container RAM request")
+    ram_mb_min: int = odm.Integer(default=128, description="Container RAM request")
     service_account = odm.optional(odm.keyword(description="Service account to use for pods in kubernetes"))
 
 
 @ odm.model(index=False, store=False, description="Container's Persistent Volume Configuration")
 class PersistentVolume(odm.Model):
     mount_path = odm.Keyword(description="Path into the container to mount volume")
     capacity = odm.Keyword(description="The amount of storage allocated for volume")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/service_delta.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/service_delta.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/signature.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/statistics.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/statistics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/submission.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/submission.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 @odm.model(index=True, store=False, description="Submission Parameters")
 class SubmissionParams(odm.Model):
     classification = odm.Classification(default=Classification.UNRESTRICTED,
                                         description="Original classification of the submission")
     deep_scan = odm.Boolean(default=False, description="Should a deep scan be performed?")
     description = odm.Text(store=True, copyto="__text__", description="Description of the submission")
     generate_alert = odm.Boolean(default=False, description="Should this submission generate an alert?")
-    groups = odm.List(odm.Keyword(), default=[], description="List of groups related to this scan")
+    groups = odm.List(odm.Keyword(), default=["USERS"], description="List of groups related to this scan")
     ignore_cache = odm.Boolean(default=False, description="Ignore the cached service results?")
     ignore_dynamic_recursion_prevention = odm.Boolean(
         default=False, description="Should we ignore dynamic recursion prevention?")
     ignore_filtering = odm.Boolean(default=False, description="Should we ignore filtering services?")
     ignore_size = odm.Boolean(default=False, description="Ignore the file size limits?")
     never_drop = odm.Boolean(default=False, description="Exempt from being dropped by ingester?")
     malicious = odm.Boolean(default=False, description="Is the file submitted already known to be malicious?")
@@ -130,15 +130,15 @@
     expiry_ts = odm.Optional(odm.Date(store=False), description="Expiry timestamp")
     file_count = odm.Integer(description="Total number of files in the submission")
     files: list[File] = odm.List(odm.Compound(File), description="List of files that were originally submitted")
     max_score = odm.Integer(description="Maximum score of all the files in the scan")
     metadata = odm.FlattenedObject(store=False, description="Metadata associated to the submission")
     params: SubmissionParams = odm.Compound(SubmissionParams, description="Submission parameter details")
     results: list[str] = odm.List(odm.Keyword(), store=False, description="List of result keys")
-    sid: str = odm.UUID(copyto="__text__", description="Submission ID")
+    sid = odm.UUID(copyto="__text__", description="Submission ID")
     state = odm.Enum(values=SUBMISSION_STATES, description="Status of the submission")
     to_be_deleted = odm.Boolean(
         default=False, description="This document is going to be deleted as soon as it finishes")
     times = odm.Compound(Times, default={}, description="Submission-specific times")
     verdict = odm.Compound(Verdict, default={}, description="Malicious verdict details")
     from_archive = odm.Boolean(index=False, default=False, description="Was loaded from the archive")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/submission_summary.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_summary.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/submission_tree.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_tree.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/tagging.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/tagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,14 @@
         ancestry = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="File Genealogy")
         behavior = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="File Behaviour")
         compiler = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="Compiler of File")
         config = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="File Configuration")
         date = odm.Optional(odm.Compound(FileDate), description="File's Date Information")
         elf = odm.Optional(odm.Compound(FileELF), description="ELF File Properties")
         lib = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="File Libraries")
-        lsh = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="File LSH hashes")
         name = odm.Optional(odm.Compound(FileName), description="File Name")
         path = odm.Optional(odm.List(odm.Keyword(copyto="__text__")), description="File Path")
         rule = odm.Optional(odm.Mapping(odm.List(odm.Keyword(copyto="__text__"))), description="Rule/Signature File")
         string = odm.Optional(odm.Compound(FileStrings), description="File Strings Properties")
         apk = odm.Optional(odm.Compound(FileAPK), description="APK File Properties")
         jar = odm.Optional(odm.Compound(FileJAR), description="JAR File Properties")
         img = odm.Optional(odm.Compound(FileIMG), description="Image File Properties")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/user.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     ("archive_view", 23),
     ("archive_manage", 24),
     ("archive_trigger", 25),
     ("archive_download", 26),
     ("self_manage", 27),
     ("retrohunt_view", 28),
     ("retrohunt_run", 29),
-    ("external_query", 30),
 ])
 
 
 SCOPES = {"r", "w", "rw", "c"}
 USER_TYPES = [
     TYPES.admin,               # Perform administartive task and has access to all roles
     TYPES.user,                # Normal user of the system
@@ -65,15 +64,14 @@
     ROLES.alert_view,          # View alerts in the system
     ROLES.archive_trigger,     # Send Submission, files and results to the archive
     ROLES.archive_view,        # View archived data in the system
     ROLES.archive_manage,      # Modify attributes of archived Submissions/Files/Results
     ROLES.archive_download,    # Download file from the archive
     ROLES.apikey_access,       # Allow access via API keys
     ROLES.bundle_download,     # Create bundle of a submission
-    ROLES.external_query,      # Allow federated searches against external systems
     ROLES.file_detail,         # View files in the file viewer
     ROLES.file_download,       # Download files from the system
     ROLES.heuristic_view,      # View heuristics of the system
     ROLES.obo_access,          # Allow access via On Behalf Off tokens
     ROLES.replay_trigger,      # Allow submission to be replayed on another server
     ROLES.safelist_view,       # View safelist items
     ROLES.safelist_manage,     # Manage (add/delete) safelist items,
@@ -134,15 +132,14 @@
 
 ACL_MAP = {
     "R": [
         ROLES.alert_view,
         ROLES.archive_view,
         ROLES.archive_download,
         ROLES.bundle_download,
-        ROLES.external_query,
         ROLES.file_detail,
         ROLES.file_download,
         ROLES.heuristic_view,
         ROLES.safelist_view,
         ROLES.signature_download,
         ROLES.signature_view,
         ROLES.submission_view,
@@ -232,15 +229,15 @@
     can_impersonate = odm.Boolean(default=False, index=False, store=False,
                                   description="Allowed to query on behalf of others?")
     classification = odm.Classification(is_user_classification=True, copyto="__text__",
                                         default=Classification.UNRESTRICTED,
                                         description="Maximum classification for the user")
     dn = odm.Optional(odm.Keyword(store=False, copyto="__text__"), description="User's LDAP DN")
     email = odm.Optional(odm.Email(copyto="__text__"), description="User's email address")
-    groups = odm.List(odm.UpperKeyword(), copyto="__text__", default=[],
+    groups = odm.List(odm.Keyword(), copyto="__text__", default=["USERS"],
                       description="List of groups the user submits to")
     is_active = odm.Boolean(default=True, description="Is the user active?")
     name = odm.Keyword(copyto="__text__", description="Full name of the user")
     otp_sk = odm.Optional(
         odm.Keyword(index=False, store=False),
         description="Secret key to generate one time passwords")
     password = odm.Keyword(index=False, store=False, description="BCrypt hash of the user's password")
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/user_favorites.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/user_favorites.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/user_settings.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/models/workflow.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/random_data/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,17 +339,14 @@
     for f in s.files:
         f.sha256 = first_level_files[fid]
         fid += 1
 
     s.params.psid = None
     s.state = 'completed'
 
-    if log:
-        log.info(f'{s}')
-
     ds.submission.save(s.sid, s)
 
     ds.emptyresult.commit()
     ds.error.commit()
     ds.file.commit()
     ds.result.commit()
     ds.submission.commit()
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/random_data/create_test_data.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/create_test_data.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/random_data/sample_rules.yar` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_rules.yar`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/random_data/sample_suricata.rules` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_suricata.rules`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/odm/randomizer.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/randomizer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/counters.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/counters.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/exporting_counter.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/exporting_counter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/hash.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/hash.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/lock.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/lock.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/comms.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/multi.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/multi.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/named.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/named.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/queues/priority.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/priority.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/set.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/set.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/remote/datatypes/user_quota_tracker.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/user_quota_tracker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/run/cli.py` & `assemblyline-4.4.1.dev9/assemblyline/run/cli.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/run/pubsub_reader.py` & `assemblyline-4.4.1.dev9/assemblyline/run/pubsub_reader.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/run/suricata_importer.py` & `assemblyline-4.4.1.dev9/assemblyline/run/suricata_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline/run/yara_importer.py` & `assemblyline-4.4.1.dev9/assemblyline/run/yara_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/assemblyline.egg-info/PKG-INFO` & `assemblyline-4.4.1.dev9/assemblyline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.4.1.dev85
+Version: 4.4.1.dev9
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-4.4.1.dev85/assemblyline.egg-info/SOURCES.txt` & `assemblyline-4.4.1.dev9/assemblyline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev85/setup.py` & `assemblyline-4.4.1.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,20 +87,20 @@
         'kubernetes>18',
         'notifications-python-client',
         # Blacklist a bad release of the azure library until a release newer than that comes out
         'azure-storage-blob!=12.4.0',
         'azure-identity',
         'msoffcrypto-tool',
         'chardet',
-        'yara-python',
-        'python-tlsh'
+        'yara-python'
     ],
     extras_require={
         'test': [
             'pytest',
+            'pytest-cov',
             'retrying',
             'pytest-mock',
             'pyftpdlib',
             'pyopenssl',
         ]
     },
     package_data={
```

