# Comparing `tmp/cloud-audit-tool-0.0.2.tar.gz` & `tmp/cloud-audit-tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-audit-tool-0.0.2.tar", last modified: Tue May 23 10:35:35 2023, max compression
+gzip compressed data, was "cloud-audit-tool-0.0.3.tar", last modified: Tue May 23 17:03:55 2023, max compression
```

## Comparing `cloud-audit-tool-0.0.2.tar` & `cloud-audit-tool-0.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.717979 cloud-audit-tool-0.0.2/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2318 2023-05-23 10:35:35.718099 cloud-audit-tool-0.0.2/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 10:35:35.718436 cloud-audit-tool-0.0.2/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1162 2023-05-23 10:33:25.000000 cloud-audit-tool-0.0.2/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.703644 cloud-audit-tool-0.0.2/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.703922 cloud-audit-tool-0.0.2/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.704688 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.705631 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.706520 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1707 2023-05-23 10:32:49.000000 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     8531 2023-05-23 10:32:49.000000 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.707342 cloud-audit-tool-0.0.2/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.708129 cloud-audit-tool-0.0.2/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.708836 cloud-audit-tool-0.0.2/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.709515 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.710252 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.711009 cloud-audit-tool-0.0.2/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.711681 cloud-audit-tool-0.0.2/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13466 2023-05-23 10:32:49.000000 cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.712342 cloud-audit-tool-0.0.2/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.713108 cloud-audit-tool-0.0.2/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.713897 cloud-audit-tool-0.0.2/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.714509 cloud-audit-tool-0.0.2/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.715608 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2318 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2386 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.715799 cloud-audit-tool-0.0.2/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.716076 cloud-audit-tool-0.0.2/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.716465 cloud-audit-tool-0.0.2/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.717553 cloud-audit-tool-0.0.2/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 09:38:47.000000 cloud-audit-tool-0.0.2/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.153937 cloud-audit-tool-0.0.3/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2253 2023-05-23 17:03:55.154036 cloud-audit-tool-0.0.3/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 17:03:55.154333 cloud-audit-tool-0.0.3/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1161 2023-05-23 17:02:26.000000 cloud-audit-tool-0.0.3/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.139855 cloud-audit-tool-0.0.3/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.140312 cloud-audit-tool-0.0.3/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.140962 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.141849 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.142813 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.143711 cloud-audit-tool-0.0.3/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.144469 cloud-audit-tool-0.0.3/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.145151 cloud-audit-tool-0.0.3/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.145895 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.146567 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.147236 cloud-audit-tool-0.0.3/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.147958 cloud-audit-tool-0.0.3/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.148616 cloud-audit-tool-0.0.3/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.149311 cloud-audit-tool-0.0.3/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.149996 cloud-audit-tool-0.0.3/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.150815 cloud-audit-tool-0.0.3/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.151865 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2253 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2386 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.152039 cloud-audit-tool-0.0.3/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.152282 cloud-audit-tool-0.0.3/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.152750 cloud-audit-tool-0.0.3/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.153687 cloud-audit-tool-0.0.3/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/main.py
```

### Comparing `cloud-audit-tool-0.0.2/PKG-INFO` & `cloud-audit-tool-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud-audit-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com , bhanuja497@gmail.com
+Maintainer-email: vishalrv1904@gmail.com, bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
 
@@ -16,35 +16,35 @@
 various AWS services security requirements and the best practices. Generates report to validate the security requirements and security best practices.
 
 
 # **Cloud Audit tool setup** #
 
 **The project basically uses boto client to connect to the aws services.**
 
-1. Update the session credentials in the terminal or give the session credentials through the arguments of the command line by specifying --access-key, --secret-key and --session-token.
-
-2. You can specify the region name, config file path, report file path and tags through --region, --config-path, --report-path arguments respectively while running the program.
-
-3. If no region is specified us-east-1 is taken as default region, Similarly if no config file path and report path is given current working directory path is taken as default and the audit checks are performed for the services accordingly.
-
-4. To check tags, we can pass as argument --tags while running the tool and we can also update the config.json file by mentioning the tags in the account tags provided. Moreover the tags passed as the argument through the command line takes the first priority.
-
-5. Tags that are passed through the argument in command line should be separated using commas (,)
+1. Update the session credentials in the terminal or give them through the arguments in the command line by specifying --access-key, --secret-key, and --session-token.
+ 
+2. While running the program, You can specify the region name, config file path, report file path, and tags through --region, --config-path, -report-path arguments.
+ 
+3. If no region is specified us-east-1 is taken as the default region, Similarly if no config file path and report path are given, the current working directory's path is taken as the default path and the audit checks are performed for the default values.
+ 
+4. Tags are checked by passing as an argument --tags or updating account tags in the config.json file. Moreover, the tags passed through the argument in the command line take priority.
+ 
+5. The format of the tags that are passed through the argument in the command line should be separated using commas (,).
 
 
 # **Cloud Audit Tool Execution** #
 
 Command to Run the audit tool in the command line after installing the package.
 ```
 cloud-audit-tool
 ```
 
 Arguments that can be passed
 ```
-cloud-audit-tool --region {region_name} --config-path {config-path} --report-path {report-path} --access-key {access-key} --secret-key {secret-key} --session-token {session-token} --tags {tag1,tag2,..}
+cloud-audit-tool --region {region-name} --config-path {config-path} --report-path {report-path} --access-key {access-key} --secret-key {secret-key} --session-token {session-token} --tags {tag1,tag2,..}
 ```
 
 # **Final Report** #
 
 The overall report is provided as a HTML document in the path specified in the report-path argument. If no path is specified report is generated in the current working directory.
```

### Comparing `cloud-audit-tool-0.0.2/setup.py` & `cloud-audit-tool-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 __author__='Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay'
-__maintainer_email__ = 'vishalrv1904@gmail.com , bhanuja497@gmail.com'
+__maintainer_email__ = 'vishalrv1904@gmail.com, bhanuja497@gmail.com'
 
 setuptools.setup(
     name="cloud-audit-tool",                
     version=__version__,                        
     author=__author__,  
     maintainer_email=__maintainer_email__,
     license= 'MIT',
```

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 class DynamoDbChecks:
-    DYNAMODB_CHECK_AT_REST_ENCRYPTION = "DynamoDB tables MUST be configured for at-rest encryption using a KMS Key"
     DYNAMODB_CHECK_AUTOMATIC_BACKUP = "DynamoDB tables MUST be configured for automatic backup"
     DYNAMODB_CHECK_DELETE_PROTECTION = "DynamoDB tables MUST be enabled for DeleteProtection"
     DYNAMODB_CHECK_TAGS = "MUST be tagged in accordance with tagging standards"
 
 
 class DynamoDbMethodAssociations:
-    DYNAMODB_CHECK_AT_REST_ENCRYPTION = "check_encryption_at_rest"
     DYNAMODB_CHECK_AUTOMATIC_BACKUP = "check_automatic_backups"
     DYNAMODB_CHECK_DELETE_PROTECTION = "check_delete_protection"
     DYNAMODB_CHECK_TAGS = "check_dynamodb_tags"
 
 
 security_checks = {
-    "DYNAMODB_CHECK_AT_REST_ENCRYPTION": {
-        "method_name": DynamoDbMethodAssociations.DYNAMODB_CHECK_AT_REST_ENCRYPTION,
-        "check_description": DynamoDbChecks.DYNAMODB_CHECK_AT_REST_ENCRYPTION
-    },
     "DYNAMODB_CHECK_AUTOMATIC_BACKUP": {
         "method_name": DynamoDbMethodAssociations.DYNAMODB_CHECK_AUTOMATIC_BACKUP,
         "check_description": DynamoDbChecks.DYNAMODB_CHECK_AUTOMATIC_BACKUP
     },
     "DYNAMODB_CHECK_DELETE_PROTECTION": {
         "method_name": DynamoDbMethodAssociations.DYNAMODB_CHECK_DELETE_PROTECTION,
         "check_description": DynamoDbChecks.DYNAMODB_CHECK_DELETE_PROTECTION
```

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,61 +43,24 @@
                 self.resource_list += page['TableNames']
             return self.resource_list
 
         except botocore.exceptions.ClientError as ex:
             logger.error("Error occurred when listing DynamoDB resources: %s", str(ex))
             raise
 
-    def check_encryption_at_rest(self, table_name):
-        """
-        Check if encryption at rest is enabled for a given dynamodb table .
-
-        Args:
-            table_name (str): Table name of the dynamodb table to check.
-
-        Returns:
-            Returns the Status of the Validation Check.
-
-        Raises:
-            ClientError: if there is an error communicating with AWS.
-            ResourceNotFoundException: if the requested table not found
-            InternalServerError : if the server responded with internal server error
-            Exception: If any error occurs during the check.
-
-        """
-        logger.info("gathering the encryption settings for %s", table_name)
-        try:
-            table = self.dynamodb_client.describe_table(TableName=table_name)['Table']
-            if 'SSEDescription' in table and 'Status' in table['SSEDescription'] and table['SSEDescription'][
-                'Status'] == 'ENABLED':
-                check_result = application_constants.ResultStatus.PASSED
-            else:
-                check_result = application_constants.ResultStatus.FAILED
-        except (
-                self.dynamodb_client.exceptions.ResourceNotFoundException,
-                self.dynamodb_client.exceptions.InternalServerError,
-                self.dynamodb_client.exceptions.ClientError) as ex:
-            logger.error("error while gathering the encryption settings for %s: %s", table_name, str(ex))
-            check_result = application_constants.ResultStatus.UNKNOWN
-        except Exception as ex:
-            logger.error("error while gathering the encryption settings for %s: %s", table_name, str(ex))
-            raise ex
-
-        logger.info("Completed fetching encryption settings for dynamodb table : %s", table_name)
-        return check_result
 
     def check_automatic_backups(self, table_name):
         """
         Check if automatic backup is enabled for a given dynamodb table .
 
         Args:
             table_name (str): Table name of the dynamodb table to check.
 
         Returns:
-            Returns the Status of the Validation Check.
+            check_result: Returns the status of the validation check.
 
         Raises:
             ClientError: if there is an error communicating with AWS.
             TableNotFoundException: if the requested table not found
             InternalServerError : if the server responded with internal server error
             Exception: If any error occurs during the check.
 
@@ -126,27 +89,27 @@
         """
         Check if delete protection is enabled for a given dynamodb table .
 
         Args:
             table_name (str): Table name of the dynamodb table to check.
 
         Returns:
-            Returns the Status of the Validation Check.
+            check_result: Returns the status of the validation check.
 
         Raises:
             ClientError: if there is an error communicating with AWS.
             ResourceNotFoundException: if the requested table not found
             InternalServerError : if the server responded with internal server error
             Exception: If any error occurs during the check.
 
         """
         logger.info("gathering the delete protection settings for %s", table_name)
         try:
             table = self.dynamodb_client.describe_table(TableName=table_name)['Table']
-            if 'DeletionProtectionEnabled' in table and table['DeletionProtectionEnabled'] == 'True':
+            if 'DeletionProtectionEnabled' in table and table['DeletionProtectionEnabled'] == True:
                 check_result = application_constants.ResultStatus.PASSED
             else:
                 check_result = application_constants.ResultStatus.FAILED
         except (
                 self.dynamodb_client.exceptions.ResourceNotFoundException,
                 self.dynamodb_client.exceptions.InternalServerError,
                 self.dynamodb_client.exceptions.ClientError) as ex:
@@ -163,15 +126,15 @@
         """
         Checks if the specified DynamoDB table has the required tags.
 
         Args:
              table_name (str): Table name of the DynamoDb Table to check.
 
         Returns:
-            Returns the Status of the Validation Check.
+            check_result: Returns the status of the validation check.
         """
 
         if required_tags is None:
             required_tags = application_constants.Generic.REQUIRED_TAGS
 
         if not required_tags:
             check_result = application_constants.ResultStatus.PASSED
```

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/emr/emr_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/emr/emr_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/glue/glue_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/glue/glue_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/rds/rds_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/rds/rds_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         """
         Check if encryption at rest is enabled for a given redshift .
 
         Args:
             cluster_identifier (str): Cluster Identifier of the Redshift Cluster to check.
 
         Returns:
-            None: This method updates the status of the check in the `self.service` dictionary.
+            check_result: Returns the status of the validation check.
 
         Raises:
             ClientError: if there is an error communicating with AWS.
             ClusterNotFoundFault: if the requested cluster not found
             Exception: If any error occurs during the check.
 
         """
@@ -88,15 +88,15 @@
         """
         Check if given redshift cluster allows anonymous access.
 
         Args:
             cluster_identifier (str): Cluster Identifier of the Redshift Cluster to check.
 
         Returns:
-            None: This method updates the status of the check in the `self.service` dictionary.
+            check_result: Returns the status of the validation check.
 
         Raises:
             ClientError: if there is an error communicating with AWS.
             ClusterNotFoundFault: if the requested cluster not found
             Exception: If any error occurs during the check.
 
         """
@@ -123,16 +123,15 @@
         """
        Check if given redshift cluster is only in a private subnet.
 
        Args:
            cluster_identifier (str): Cluster Identifier of the Redshift Cluster to check.
 
        Returns:
-           None: This method updates the status of the check in the `self.service` dictionary.
-
+           check_result: Returns the status of the validation check.
        Raises:
            ClientError: if there is an error communicating with AWS.
            ClusterNotFoundFault: if the requested cluster not found
            ClusterSubnetGroupNotFoundFault: if subnet group of the given cluster not found
            Exception: If any error occurs during the check.
 
        """
@@ -167,37 +166,40 @@
         """
         Check if given redshift cluster has a dedicated security group.
 
         Args:
             cluster_identifier (str): Cluster Identifier of the Redshift Cluster to check.
 
         Returns:
-            None: This method updates the status of the check in the `self.service` dictionary.
+            check_result: Returns the status of the validation check.
 
         Raises:
             ClientError: if there is an error communicating with AWS.
             ClusterNotFoundFault: if the requested cluster not found
             Exception: If any error occurs during the check.
 
         """
         logger.info("gathering the dedicated vpc security group settings for %s", cluster_identifier)
         try:
+            cluster_details=self.redshift_client.describe_clusters(ClusterIdentifier=cluster_identifier)['Clusters'][0]
             security_groups = \
-                self.redshift_client.describe_clusters(ClusterIdentifier=cluster_identifier)['Clusters'][0][
-                    'VpcSecurityGroups']
+                cluster_details['VpcSecurityGroups']
+            nodes_count=cluster_details['NumberOfNodes']
+            if(nodes_count>1):
+                nodes_count+=1  # In multi-node type clusters, extra one leader node gets created.
             if len(security_groups):
                 security_group_ids = [security_group['VpcSecurityGroupId'] for security_group in security_groups]
                 paginator = self.ec2_client.get_paginator('describe_network_interfaces')
                 pages = paginator.paginate(Filters=[{
                     'Name': 'group-id',
                     'Values': security_group_ids
                 }], PaginationConfig={'PageSize': 10})
                 network_interfaces = [page['NetworkInterfaces'] for page in pages]
                 network_interfaces = list(itertools.chain(*network_interfaces))
-                if len(network_interfaces) == 1:
+                if len(network_interfaces) == nodes_count:
                     check_result = application_constants.ResultStatus.PASSED
                 else:
                     check_result = application_constants.ResultStatus.FAILED
             else:
                 check_result = application_constants.ResultStatus.FAILED
 
         except (self.redshift_client.exceptions.ClientError, self.redshift_client.exceptions.ClusterNotFoundFault) as ex:
@@ -215,15 +217,15 @@
         """
          Check if given redshift cluster has security group only with least ingress and egress rules.
 
          Args:
              cluster_identifier (str): Cluster Identifier of the Redshift Cluster to check.
 
          Returns:
-             None: This method updates the status of the check in the `self.service` dictionary.
+             check_result: Returns the status of the validation check.
 
          Raises:
              ClientError: if there is an error communicating with AWS.
              ClusterNotFoundFault: if the requested cluster not found
              Exception: If any error occurs during the check.
 
          """
@@ -256,15 +258,15 @@
         """
         Checks if the specified Redshift cluster has the required tags.
 
         Args:
              cluster_identifier (str): Cluster Identifier of the Redshift Cluster to check.
 
         Returns:
-            None: This method updates the status of the check in the `self.service` dictionary.
+            check_result: Returns the status of the validation check.
         """
 
         if required_tags is None:
             required_tags = application_constants.Generic.REQUIRED_TAGS
 
         if not required_tags:
             check_result = application_constants.ResultStatus.PASSED
```

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/s3/s3_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/s3/s3_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/ses/ses_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/ses/ses_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/sns/sns_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/sns/sns_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_constants.py` & `cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_service.py` & `cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/PKG-INFO` & `cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud-audit-tool
-Version: 0.0.2
+Version: 0.0.3
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com , bhanuja497@gmail.com
+Maintainer-email: vishalrv1904@gmail.com, bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
 
@@ -16,35 +16,35 @@
 various AWS services security requirements and the best practices. Generates report to validate the security requirements and security best practices.
 
 
 # **Cloud Audit tool setup** #
 
 **The project basically uses boto client to connect to the aws services.**
 
-1. Update the session credentials in the terminal or give the session credentials through the arguments of the command line by specifying --access-key, --secret-key and --session-token.
-
-2. You can specify the region name, config file path, report file path and tags through --region, --config-path, --report-path arguments respectively while running the program.
-
-3. If no region is specified us-east-1 is taken as default region, Similarly if no config file path and report path is given current working directory path is taken as default and the audit checks are performed for the services accordingly.
-
-4. To check tags, we can pass as argument --tags while running the tool and we can also update the config.json file by mentioning the tags in the account tags provided. Moreover the tags passed as the argument through the command line takes the first priority.
-
-5. Tags that are passed through the argument in command line should be separated using commas (,)
+1. Update the session credentials in the terminal or give them through the arguments in the command line by specifying --access-key, --secret-key, and --session-token.
+ 
+2. While running the program, You can specify the region name, config file path, report file path, and tags through --region, --config-path, -report-path arguments.
+ 
+3. If no region is specified us-east-1 is taken as the default region, Similarly if no config file path and report path are given, the current working directory's path is taken as the default path and the audit checks are performed for the default values.
+ 
+4. Tags are checked by passing as an argument --tags or updating account tags in the config.json file. Moreover, the tags passed through the argument in the command line take priority.
+ 
+5. The format of the tags that are passed through the argument in the command line should be separated using commas (,).
 
 
 # **Cloud Audit Tool Execution** #
 
 Command to Run the audit tool in the command line after installing the package.
 ```
 cloud-audit-tool
 ```
 
 Arguments that can be passed
 ```
-cloud-audit-tool --region {region_name} --config-path {config-path} --report-path {report-path} --access-key {access-key} --secret-key {secret-key} --session-token {session-token} --tags {tag1,tag2,..}
+cloud-audit-tool --region {region-name} --config-path {config-path} --report-path {report-path} --access-key {access-key} --secret-key {secret-key} --session-token {session-token} --tags {tag1,tag2,..}
 ```
 
 # **Final Report** #
 
 The overall report is provided as a HTML document in the path specified in the report-path argument. If no path is specified report is generated in the current working directory.
```

### Comparing `cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/SOURCES.txt` & `cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/common/constants/application_constants.py` & `cloud-audit-tool-0.0.3/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/common/service/dat_service.py` & `cloud-audit-tool-0.0.3/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/common/utils/helper.py` & `cloud-audit-tool-0.0.3/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/common/utils/instance_initializer.py` & `cloud-audit-tool-0.0.3/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.2/src/main.py` & `cloud-audit-tool-0.0.3/src/main.py`

 * *Files identical despite different names*

