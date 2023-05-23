# Comparing `tmp/cloud-audit-tool-0.0.3.tar.gz` & `tmp/cloud-audit-tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-audit-tool-0.0.3.tar", last modified: Tue May 23 17:03:55 2023, max compression
+gzip compressed data, was "cloud-audit-tool-0.0.4.tar", last modified: Tue May 23 17:06:12 2023, max compression
```

## Comparing `cloud-audit-tool-0.0.3.tar` & `cloud-audit-tool-0.0.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.153937 cloud-audit-tool-0.0.3/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2253 2023-05-23 17:03:55.154036 cloud-audit-tool-0.0.3/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 17:03:55.154333 cloud-audit-tool-0.0.3/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1161 2023-05-23 17:02:26.000000 cloud-audit-tool-0.0.3/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.139855 cloud-audit-tool-0.0.3/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.140312 cloud-audit-tool-0.0.3/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.140962 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.141849 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.142813 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.143711 cloud-audit-tool-0.0.3/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.144469 cloud-audit-tool-0.0.3/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.145151 cloud-audit-tool-0.0.3/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.145895 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.146567 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.147236 cloud-audit-tool-0.0.3/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.147958 cloud-audit-tool-0.0.3/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.148616 cloud-audit-tool-0.0.3/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.149311 cloud-audit-tool-0.0.3/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.149996 cloud-audit-tool-0.0.3/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.150815 cloud-audit-tool-0.0.3/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.151865 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2253 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2386 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 17:03:55.000000 cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.152039 cloud-audit-tool-0.0.3/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.152282 cloud-audit-tool-0.0.3/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.152750 cloud-audit-tool-0.0.3/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:03:55.153687 cloud-audit-tool-0.0.3/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.3/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.3/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.644799 cloud-audit-tool-0.0.4/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2253 2023-05-23 17:06:12.644912 cloud-audit-tool-0.0.4/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 17:06:12.645638 cloud-audit-tool-0.0.4/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1161 2023-05-23 17:06:04.000000 cloud-audit-tool-0.0.4/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.627031 cloud-audit-tool-0.0.4/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.627517 cloud-audit-tool-0.0.4/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.628295 cloud-audit-tool-0.0.4/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.629294 cloud-audit-tool-0.0.4/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.630152 cloud-audit-tool-0.0.4/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.630915 cloud-audit-tool-0.0.4/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.631479 cloud-audit-tool-0.0.4/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.632290 cloud-audit-tool-0.0.4/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.632878 cloud-audit-tool-0.0.4/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.633674 cloud-audit-tool-0.0.4/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.634382 cloud-audit-tool-0.0.4/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.635084 cloud-audit-tool-0.0.4/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.635682 cloud-audit-tool-0.0.4/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.638280 cloud-audit-tool-0.0.4/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.639361 cloud-audit-tool-0.0.4/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.641088 cloud-audit-tool-0.0.4/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.643132 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2253 2023-05-23 17:06:12.000000 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2386 2023-05-23 17:06:12.000000 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 17:06:12.000000 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 17:06:12.000000 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 17:06:12.000000 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 17:06:12.000000 cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.643297 cloud-audit-tool-0.0.4/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.643516 cloud-audit-tool-0.0.4/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.643823 cloud-audit-tool-0.0.4/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:06:12.644602 cloud-audit-tool-0.0.4/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud-audit-tool-0.0.4/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud-audit-tool-0.0.4/src/main.py
```

### Comparing `cloud-audit-tool-0.0.3/PKG-INFO` & `cloud-audit-tool-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud-audit-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com, bhanuja497@gmail.com
+Maintainer-email: vishalrv1904@gmail.com ,bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud-audit-tool-0.0.3/setup.py` & `cloud-audit-tool-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 __author__='Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay'
-__maintainer_email__ = 'vishalrv1904@gmail.com, bhanuja497@gmail.com'
+__maintainer_email__ = 'vishalrv1904@gmail.com ,bhanuja497@gmail.com'
 
 setuptools.setup(
     name="cloud-audit-tool",                
     version=__version__,                        
     author=__author__,  
     maintainer_email=__maintainer_email__,
     license= 'MIT',
```

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/api_gateway/api_gateway_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/dat_lambda/lambda_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/dynamodb/dynamodb_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/emr/emr_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/emr/emr_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/fargate/fargate_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/glue/glue_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/glue/glue_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/rds/rds_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/rds/rds_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/redshift/redshift_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/s3/s3_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/s3/s3_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/ses/ses_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/ses/ses_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/sns/sns_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/sns/sns_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_constants.py` & `cloud-audit-tool-0.0.4/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/aws_services/sqs/sqs_service.py` & `cloud-audit-tool-0.0.4/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/PKG-INFO` & `cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud-audit-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com, bhanuja497@gmail.com
+Maintainer-email: vishalrv1904@gmail.com ,bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud-audit-tool-0.0.3/src/cloud_audit_tool.egg-info/SOURCES.txt` & `cloud-audit-tool-0.0.4/src/cloud_audit_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/common/constants/application_constants.py` & `cloud-audit-tool-0.0.4/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/common/service/dat_service.py` & `cloud-audit-tool-0.0.4/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/common/utils/helper.py` & `cloud-audit-tool-0.0.4/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/common/utils/instance_initializer.py` & `cloud-audit-tool-0.0.4/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud-audit-tool-0.0.3/src/main.py` & `cloud-audit-tool-0.0.4/src/main.py`

 * *Files identical despite different names*

