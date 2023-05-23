# Comparing `tmp/cloud-audit-tool-0.0.1.tar.gz` & `tmp/cloud-audit-tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-audit-tool-0.0.1.tar", last modified: Tue May 16 12:14:50 2023, max compression
+gzip compressed data, was "cloud-audit-tool-0.0.2.tar", last modified: Tue May 23 10:35:35 2023, max compression
```

## Comparing `cloud-audit-tool-0.0.1.tar` & `cloud-audit-tool-0.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.417556 cloud-audit-tool-0.0.1/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2318 2023-05-16 12:14:50.417641 cloud-audit-tool-0.0.1/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-16 12:14:50.417926 cloud-audit-tool-0.0.1/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1162 2023-05-16 05:33:07.000000 cloud-audit-tool-0.0.1/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.406017 cloud-audit-tool-0.0.1/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.406282 cloud-audit-tool-0.0.1/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.406861 cloud-audit-tool-0.0.1/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.407628 cloud-audit-tool-0.0.1/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.408439 cloud-audit-tool-0.0.1/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1707 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     8531 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.409123 cloud-audit-tool-0.0.1/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.409653 cloud-audit-tool-0.0.1/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.410193 cloud-audit-tool-0.0.1/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.410749 cloud-audit-tool-0.0.1/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.411327 cloud-audit-tool-0.0.1/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.411805 cloud-audit-tool-0.0.1/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.412387 cloud-audit-tool-0.0.1/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13466 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.412893 cloud-audit-tool-0.0.1/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.413392 cloud-audit-tool-0.0.1/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.413929 cloud-audit-tool-0.0.1/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-11 06:33:22.000000 cloud-audit-tool-0.0.1/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.414423 cloud-audit-tool-0.0.1/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-12 10:27:59.000000 cloud-audit-tool-0.0.1/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.415651 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2318 2023-05-16 12:14:50.000000 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2386 2023-05-16 12:14:50.000000 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-16 12:14:50.000000 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-16 12:14:50.000000 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-16 12:14:50.000000 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-16 12:14:50.000000 cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.415792 cloud-audit-tool-0.0.1/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.416070 cloud-audit-tool-0.0.1/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.416497 cloud-audit-tool-0.0.1/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-16 12:14:50.417276 cloud-audit-tool-0.0.1/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.1/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-11 07:07:52.000000 cloud-audit-tool-0.0.1/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-16 05:29:48.000000 cloud-audit-tool-0.0.1/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.717979 cloud-audit-tool-0.0.2/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2318 2023-05-23 10:35:35.718099 cloud-audit-tool-0.0.2/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 10:35:35.718436 cloud-audit-tool-0.0.2/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1162 2023-05-23 10:33:25.000000 cloud-audit-tool-0.0.2/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.703644 cloud-audit-tool-0.0.2/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.703922 cloud-audit-tool-0.0.2/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.704688 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.705631 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.706520 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1707 2023-05-23 10:32:49.000000 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     8531 2023-05-23 10:32:49.000000 cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.707342 cloud-audit-tool-0.0.2/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.708129 cloud-audit-tool-0.0.2/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.708836 cloud-audit-tool-0.0.2/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.709515 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.710252 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.711009 cloud-audit-tool-0.0.2/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.711681 cloud-audit-tool-0.0.2/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13466 2023-05-23 10:32:49.000000 cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.712342 cloud-audit-tool-0.0.2/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.713108 cloud-audit-tool-0.0.2/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.713897 cloud-audit-tool-0.0.2/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.714509 cloud-audit-tool-0.0.2/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.715608 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2318 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2386 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 10:35:35.000000 cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.715799 cloud-audit-tool-0.0.2/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.716076 cloud-audit-tool-0.0.2/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.716465 cloud-audit-tool-0.0.2/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 10:35:35.717553 cloud-audit-tool-0.0.2/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.2/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 09:38:47.000000 cloud-audit-tool-0.0.2/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 07:14:45.000000 cloud-audit-tool-0.0.2/src/main.py
```

### Comparing `cloud-audit-tool-0.0.1/PKG-INFO` & `cloud-audit-tool-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-audit-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
 Maintainer-email: vishalrv1904@gmail.com , bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cloud-audit-tool-0.0.1/setup.py` & `cloud-audit-tool-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 __author__='Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay'
 __maintainer_email__ = 'vishalrv1904@gmail.com , bhanuja497@gmail.com'
 
 setuptools.setup(
     name="cloud-audit-tool",                
     version=__version__,                        
     author=__author__,
```

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/api_gateway/api_gateway_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/dat_lambda/lambda_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/dat_lambda/lambda_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/dynamodb/dynamodb_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/emr/emr_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/emr/emr_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/fargate/fargate_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/fargate/fargate_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/glue/glue_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/glue/glue_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/rds/rds_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/rds/rds_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/redshift/redshift_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/redshift/redshift_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/s3/s3_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/s3/s3_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/ses/ses_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/ses/ses_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/sns/sns_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/sns/sns_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/sqs/sqs_constants.py` & `cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/aws_services/sqs/sqs_service.py` & `cloud-audit-tool-0.0.2/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/PKG-INFO` & `cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-audit-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
 Maintainer-email: vishalrv1904@gmail.com , bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cloud-audit-tool-0.0.1/src/cloud_audit_tool.egg-info/SOURCES.txt` & `cloud-audit-tool-0.0.2/src/cloud_audit_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/common/constants/application_constants.py` & `cloud-audit-tool-0.0.2/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/common/service/dat_service.py` & `cloud-audit-tool-0.0.2/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/common/utils/helper.py` & `cloud-audit-tool-0.0.2/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/common/utils/instance_initializer.py` & `cloud-audit-tool-0.0.2/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.1/src/main.py` & `cloud-audit-tool-0.0.2/src/main.py`

 * *Files identical despite different names*

