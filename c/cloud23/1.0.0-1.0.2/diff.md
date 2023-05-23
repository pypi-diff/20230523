# Comparing `tmp/cloud23-1.0.0.tar.gz` & `tmp/cloud23-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud23-1.0.0.tar", last modified: Tue May 23 17:38:10 2023, max compression
+gzip compressed data, was "cloud23-1.0.2.tar", last modified: Tue May 23 17:39:31 2023, max compression
```

## Comparing `cloud23-1.0.0.tar` & `cloud23-1.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.727881 cloud23-1.0.0/
--rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud23-1.0.0/MANIFEST.in
--rw-r--r--   0 ab         (501) staff       (20)     2243 2023-05-23 17:38:10.727981 cloud23-1.0.0/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 17:38:10.728331 cloud23-1.0.0/setup.cfg
--rw-r--r--   0 ab         (501) staff       (20)     1176 2023-05-23 17:38:03.000000 cloud23-1.0.0/setup.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.714575 cloud23-1.0.0/src/
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.714853 cloud23-1.0.0/src/aws_services/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.715480 cloud23-1.0.0/src/aws_services/api_gateway/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/api_gateway/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/api_gateway/api_gateway_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/api_gateway/api_gateway_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.716396 cloud23-1.0.0/src/aws_services/dat_lambda/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/dat_lambda/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/dat_lambda/lambda_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/dat_lambda/lambda_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.717256 cloud23-1.0.0/src/aws_services/dynamodb/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/dynamodb/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/dynamodb/dynamodb_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/dynamodb/dynamodb_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.718144 cloud23-1.0.0/src/aws_services/emr/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/emr/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/emr/emr_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/emr/emr_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.718890 cloud23-1.0.0/src/aws_services/fargate/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/fargate/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/fargate/fargate_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/fargate/fargate_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.719550 cloud23-1.0.0/src/aws_services/glue/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/glue/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/glue/glue_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/glue/glue_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.720162 cloud23-1.0.0/src/aws_services/kinesis_firehose/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/kinesis_firehose/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/kinesis_firehose/firehose_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.720794 cloud23-1.0.0/src/aws_services/kinesis_stream/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/kinesis_stream/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/kinesis_stream/kinesis_stream_constants.py
--rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/kinesis_stream/kinesis_stream_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.721431 cloud23-1.0.0/src/aws_services/rds/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/rds/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/rds/rds_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/rds/rds_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.722039 cloud23-1.0.0/src/aws_services/redshift/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/redshift/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/redshift/redshift_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/redshift/redshift_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.722660 cloud23-1.0.0/src/aws_services/s3/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/s3/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/s3/s3_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/s3/s3_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.723225 cloud23-1.0.0/src/aws_services/ses/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/ses/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/ses/ses_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/ses/ses_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.723856 cloud23-1.0.0/src/aws_services/sns/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/sns/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/sns/sns_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/sns/sns_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.724582 cloud23-1.0.0/src/aws_services/sqs/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/sqs/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/aws_services/sqs/sqs_constants.py
--rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/aws_services/sqs/sqs_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.725669 cloud23-1.0.0/src/cloud23.egg-info/
--rw-r--r--   0 ab         (501) staff       (20)     2243 2023-05-23 17:38:10.000000 cloud23-1.0.0/src/cloud23.egg-info/PKG-INFO
--rw-r--r--   0 ab         (501) staff       (20)     2332 2023-05-23 17:38:10.000000 cloud23-1.0.0/src/cloud23.egg-info/SOURCES.txt
--rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 17:38:10.000000 cloud23-1.0.0/src/cloud23.egg-info/dependency_links.txt
--rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 17:38:10.000000 cloud23-1.0.0/src/cloud23.egg-info/entry_points.txt
--rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 17:38:10.000000 cloud23-1.0.0/src/cloud23.egg-info/requires.txt
--rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 17:38:10.000000 cloud23-1.0.0/src/cloud23.egg-info/top_level.txt
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.725836 cloud23-1.0.0/src/common/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/__init__.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.726081 cloud23-1.0.0/src/common/constants/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/constants/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/constants/application_constants.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.726851 cloud23-1.0.0/src/common/service/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/service/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/service/dat_service.py
-drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:38:10.727665 cloud23-1.0.0/src/common/utils/
--rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/utils/__init__.py
--rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/utils/helper.py
--rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud23-1.0.0/src/common/utils/initialize_logger.py
--rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/common/utils/instance_initializer.py
--rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud23-1.0.0/src/main.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.727329 cloud23-1.0.2/
+-rw-r--r--   0 ab         (501) staff       (20)       17 2023-05-23 16:51:20.000000 cloud23-1.0.2/MANIFEST.in
+-rw-r--r--   0 ab         (501) staff       (20)     2244 2023-05-23 17:39:31.727445 cloud23-1.0.2/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)      176 2023-05-23 17:39:31.727796 cloud23-1.0.2/setup.cfg
+-rw-r--r--   0 ab         (501) staff       (20)     1177 2023-05-23 17:39:29.000000 cloud23-1.0.2/setup.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.713348 cloud23-1.0.2/src/
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.713722 cloud23-1.0.2/src/aws_services/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.714619 cloud23-1.0.2/src/aws_services/api_gateway/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/api_gateway/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1267 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/api_gateway/api_gateway_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     7883 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/api_gateway/api_gateway_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.715475 cloud23-1.0.2/src/aws_services/dat_lambda/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/dat_lambda/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      574 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/dat_lambda/lambda_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     3854 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/dat_lambda/lambda_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.716504 cloud23-1.0.2/src/aws_services/dynamodb/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/dynamodb/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1311 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/dynamodb/dynamodb_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     6770 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/dynamodb/dynamodb_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.717255 cloud23-1.0.2/src/aws_services/emr/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/emr/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1537 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/emr/emr_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10580 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/emr/emr_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.717958 cloud23-1.0.2/src/aws_services/fargate/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/fargate/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1459 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/fargate/fargate_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10989 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/fargate/fargate_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.718702 cloud23-1.0.2/src/aws_services/glue/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/glue/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2141 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/glue/glue_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    15754 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/glue/glue_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.719313 cloud23-1.0.2/src/aws_services/kinesis_firehose/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/kinesis_firehose/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)      964 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/kinesis_firehose/firehose_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5882 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/kinesis_firehose/kinesis_firehose_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.720001 cloud23-1.0.2/src/aws_services/kinesis_stream/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/kinesis_stream/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1085 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/kinesis_stream/kinesis_stream_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)     5542 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/kinesis_stream/kinesis_stream_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.720669 cloud23-1.0.2/src/aws_services/rds/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/rds/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2663 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/rds/rds_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13762 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/rds/rds_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.721340 cloud23-1.0.2/src/aws_services/redshift/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/redshift/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2922 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/redshift/redshift_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    13529 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/redshift/redshift_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.722210 cloud23-1.0.2/src/aws_services/s3/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/s3/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2146 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/s3/s3_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11711 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/s3/s3_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.722953 cloud23-1.0.2/src/aws_services/ses/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/ses/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1808 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/ses/ses_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10018 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/ses/ses_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.723680 cloud23-1.0.2/src/aws_services/sns/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/sns/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     1907 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/sns/sns_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    11294 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/sns/sns_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.724281 cloud23-1.0.2/src/aws_services/sqs/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/sqs/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2360 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/aws_services/sqs/sqs_constants.py
+-rw-r--r--   0 ab         (501) staff       (20)    10990 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/aws_services/sqs/sqs_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.725470 cloud23-1.0.2/src/cloud23.egg-info/
+-rw-r--r--   0 ab         (501) staff       (20)     2244 2023-05-23 17:39:31.000000 cloud23-1.0.2/src/cloud23.egg-info/PKG-INFO
+-rw-r--r--   0 ab         (501) staff       (20)     2332 2023-05-23 17:39:31.000000 cloud23-1.0.2/src/cloud23.egg-info/SOURCES.txt
+-rw-r--r--   0 ab         (501) staff       (20)        1 2023-05-23 17:39:31.000000 cloud23-1.0.2/src/cloud23.egg-info/dependency_links.txt
+-rw-r--r--   0 ab         (501) staff       (20)       74 2023-05-23 17:39:31.000000 cloud23-1.0.2/src/cloud23.egg-info/entry_points.txt
+-rw-r--r--   0 ab         (501) staff       (20)      114 2023-05-23 17:39:31.000000 cloud23-1.0.2/src/cloud23.egg-info/requires.txt
+-rw-r--r--   0 ab         (501) staff       (20)       25 2023-05-23 17:39:31.000000 cloud23-1.0.2/src/cloud23.egg-info/top_level.txt
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.725629 cloud23-1.0.2/src/common/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/__init__.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.725865 cloud23-1.0.2/src/common/constants/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/constants/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     2428 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/constants/application_constants.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.726280 cloud23-1.0.2/src/common/service/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/service/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)     6395 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/service/dat_service.py
+drwxr-xr-x   0 ab         (501) staff       (20)        0 2023-05-23 17:39:31.727090 cloud23-1.0.2/src/common/utils/
+-rw-r--r--   0 ab         (501) staff       (20)        0 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/utils/__init__.py
+-rw-r--r--   0 ab         (501) staff       (20)    10345 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/utils/helper.py
+-rw-r--r--   0 ab         (501) staff       (20)      188 2023-05-11 06:33:05.000000 cloud23-1.0.2/src/common/utils/initialize_logger.py
+-rw-r--r--   0 ab         (501) staff       (20)     1624 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/common/utils/instance_initializer.py
+-rw-r--r--   0 ab         (501) staff       (20)     3206 2023-05-23 16:51:20.000000 cloud23-1.0.2/src/main.py
```

### Comparing `cloud23-1.0.0/PKG-INFO` & `cloud23-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud23
-Version: 1.0.0
+Version: 1.0.2
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com,bhanuja497@gmail.com
+Maintainer-email: vishalrv1904@gmail.com ,bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud23-1.0.0/setup.py` & `cloud23-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import os
 
 with open("README_PIP.md", "r") as fh:
     long_description = fh.read()
 with open("requirements.txt","r") as req:
     required_packages = req.read().splitlines()
 
-__version__ = '1.0.0'
+__version__ = '1.0.2'
 __author__='Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay'
 __maintainer_email__ = 'vishalrv1904@gmail.com,bhanuja497@gmail.com'
 
 setuptools.setup(
     name="cloud23",                
     version=__version__,                        
     author=__author__,  
-    maintainer_email='vishalrv1904@gmail.com,bhanuja497@gmail.com',
+    maintainer_email='vishalrv1904@gmail.com ,bhanuja497@gmail.com',
     license= 'MIT',              
     description="AWS Cloud Audit Tool",
     long_description=long_description,     
     long_description_content_type="text/markdown",
     packages=find_packages('src'),
     package_dir={'': 'src'},
     package_data={
```

### Comparing `cloud23-1.0.0/src/aws_services/api_gateway/api_gateway_constants.py` & `cloud23-1.0.2/src/aws_services/api_gateway/api_gateway_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/api_gateway/api_gateway_service.py` & `cloud23-1.0.2/src/aws_services/api_gateway/api_gateway_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/dat_lambda/lambda_constants.py` & `cloud23-1.0.2/src/aws_services/dat_lambda/lambda_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/dat_lambda/lambda_service.py` & `cloud23-1.0.2/src/aws_services/dat_lambda/lambda_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/dynamodb/dynamodb_constants.py` & `cloud23-1.0.2/src/aws_services/dynamodb/dynamodb_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/dynamodb/dynamodb_service.py` & `cloud23-1.0.2/src/aws_services/dynamodb/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/emr/emr_constants.py` & `cloud23-1.0.2/src/aws_services/emr/emr_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/emr/emr_service.py` & `cloud23-1.0.2/src/aws_services/emr/emr_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/fargate/fargate_constants.py` & `cloud23-1.0.2/src/aws_services/fargate/fargate_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/fargate/fargate_service.py` & `cloud23-1.0.2/src/aws_services/fargate/fargate_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/glue/glue_constants.py` & `cloud23-1.0.2/src/aws_services/glue/glue_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/glue/glue_service.py` & `cloud23-1.0.2/src/aws_services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/kinesis_firehose/firehose_constants.py` & `cloud23-1.0.2/src/aws_services/kinesis_firehose/firehose_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/kinesis_firehose/kinesis_firehose_service.py` & `cloud23-1.0.2/src/aws_services/kinesis_firehose/kinesis_firehose_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/kinesis_stream/kinesis_stream_constants.py` & `cloud23-1.0.2/src/aws_services/kinesis_stream/kinesis_stream_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/kinesis_stream/kinesis_stream_service.py` & `cloud23-1.0.2/src/aws_services/kinesis_stream/kinesis_stream_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/rds/rds_constants.py` & `cloud23-1.0.2/src/aws_services/rds/rds_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/rds/rds_service.py` & `cloud23-1.0.2/src/aws_services/rds/rds_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/redshift/redshift_constants.py` & `cloud23-1.0.2/src/aws_services/redshift/redshift_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/redshift/redshift_service.py` & `cloud23-1.0.2/src/aws_services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/s3/s3_constants.py` & `cloud23-1.0.2/src/aws_services/s3/s3_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/s3/s3_service.py` & `cloud23-1.0.2/src/aws_services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/ses/ses_constants.py` & `cloud23-1.0.2/src/aws_services/ses/ses_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/ses/ses_service.py` & `cloud23-1.0.2/src/aws_services/ses/ses_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/sns/sns_constants.py` & `cloud23-1.0.2/src/aws_services/sns/sns_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/sns/sns_service.py` & `cloud23-1.0.2/src/aws_services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/sqs/sqs_constants.py` & `cloud23-1.0.2/src/aws_services/sqs/sqs_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/aws_services/sqs/sqs_service.py` & `cloud23-1.0.2/src/aws_services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/cloud23.egg-info/PKG-INFO` & `cloud23-1.0.2/src/cloud23.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cloud23
-Version: 1.0.0
+Version: 1.0.2
 Summary: AWS Cloud Audit Tool
 Home-page: UNKNOWN
 Author: Vishal, Koushik, Sudharshan, Vikneshwar, Bhanuja, Ajay
-Maintainer-email: vishalrv1904@gmail.com,bhanuja497@gmail.com
+Maintainer-email: vishalrv1904@gmail.com ,bhanuja497@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # **CLOUD AUDIT TOOL** #
```

### Comparing `cloud23-1.0.0/src/cloud23.egg-info/SOURCES.txt` & `cloud23-1.0.2/src/cloud23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/common/constants/application_constants.py` & `cloud23-1.0.2/src/common/constants/application_constants.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/common/service/dat_service.py` & `cloud23-1.0.2/src/common/service/dat_service.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/common/utils/helper.py` & `cloud23-1.0.2/src/common/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/common/utils/instance_initializer.py` & `cloud23-1.0.2/src/common/utils/instance_initializer.py`

 * *Files identical despite different names*

### Comparing `cloud23-1.0.0/src/main.py` & `cloud23-1.0.2/src/main.py`

 * *Files identical despite different names*

