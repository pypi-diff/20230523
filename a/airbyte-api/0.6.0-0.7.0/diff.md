# Comparing `tmp/airbyte-api-0.6.0.tar.gz` & `tmp/airbyte-api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-api-0.6.0.tar", last modified: Tue May 16 00:26:00 2023, max compression
+gzip compressed data, was "airbyte-api-0.7.0.tar", last modified: Tue May 16 18:12:31 2023, max compression
```

## Comparing `airbyte-api-0.6.0.tar` & `airbyte-api-0.7.0.tar`

### file list

```diff
@@ -1,311 +1,319 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.817398 airbyte-api-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-16 00:26:00.817398 airbyte-api-0.6.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7474 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:26:00.817398 airbyte-api-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.765398 airbyte-api-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.765398 airbyte-api-0.6.0/src/airbyte/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5298 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5369 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/destinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5410 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.765398 airbyte-api-0.6.0/src/airbyte/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.769398 airbyte-api-0.6.0/src/airbyte/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/canceljob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/createconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/createdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/createjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/createsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/createworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/deleteconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/deletedestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/deletesource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/getconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/getdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/getjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/getsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/getstreamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/getworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/initiateoauth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/listconnections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/listdestinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1601 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/listjobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/listsources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/operations/listworkspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.817398 airbyte-api-0.6.0/src/airbyte/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    49472 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectioncreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectionschedulecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectionscheduleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectionstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9258 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_aws_datalake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12146 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10897 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_cassandra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6136 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_convex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_databend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8016 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_databricks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2752 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_elasticsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3749 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_firestore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21027 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2044 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_keen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_kinesis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6284 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_meilisearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9179 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8107 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6051 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6750 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11112 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_pubsub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5795 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_pulsar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_rabbitmq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8012 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_redis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13955 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_rockset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18868 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8927 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_s3_glue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_scylla.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_sftp_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16047 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destination_typesense.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destinationcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destinationresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/destinationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/geographyenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/initiateoauthrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/jobcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/jobresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/jobsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/jobstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/jobtypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/scheduletypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_airtable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7489 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_alloydb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4938 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_amazon_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5139 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_amazon_seller_partner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3915 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_amplitude.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1295 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_apify_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_asana.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_auth0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_aws_cloudtrail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3043 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_azure_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1621 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_bamboo_hr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_bigcommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2739 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_bing_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_braintree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_braze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_chargebee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_chartmogul.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5703 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2895 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_clickup_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_close_com.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_coda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_coin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_coinmarketcap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_configcat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_confluence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_datascope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1163 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_delighted.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_dixa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_dockerhub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_dremio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4278 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_e2e_test_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_emailoctopus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_exchange_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17556 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_facebook_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_facebook_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_faker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_fauna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10260 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_file_secure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2006 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_freshcaller.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_freshdesk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_freshsales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_getlago.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_github.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4124 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_gitlab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_glassfrog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_gnews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5187 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_analytics_data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4945 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_analytics_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_directory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_search_console.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_webfonts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_greenhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_gridly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_harvest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_hubplanner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_hubspot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_insightly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_instagram.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_instatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_intercom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_ip2whois.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_iterable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_jira.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_k6_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_klarna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_klaviyo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_kustomer_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_launchdarkly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_lemlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_linkedin_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_linkedin_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_linnworks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_lokalise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mailchimp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mailgun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mailjet_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_marketo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_metabase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_microsoft_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6224 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mixpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_monday.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4394 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12174 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_my_hours.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12789 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_netsuite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3005 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_notion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_nytimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_omnisend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2679 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_onesignal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_openweather.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_orb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_orbit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_outreach.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_paypal_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_paystack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pendo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_persistiq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pexels_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3220 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pinterest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pipedrive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pocket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pokeapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2961 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_polygon_stock_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7508 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_posthog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_postmarkapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_prestashop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_public_apis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_punk_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_pypi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_qualaroo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3521 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_quickbooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_railz.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_recharge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_recreation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_recruitee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_recurly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_retently.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_rki_covid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_rss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13786 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_salesforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3502 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_salesforce_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_salesloft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sap_fieldglass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_secoda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sendgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sendinblue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_senseforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sentry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sftp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3453 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sftp_bulk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3197 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_shopify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1127 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_shortio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_slack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_smaily.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      772 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_smartengage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4159 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_smartsheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_snapchat_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4381 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2194 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_sonar_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_spacex_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_square.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_strava.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_stripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_survey_sparrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3720 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_surveymonkey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_tempo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_the_guardian_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_tiktok_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_todoist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_trello.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_trustpilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_tvmaze_schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_twilio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_twilio_taskrouter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2168 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_twitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_typeform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_us_census.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_vantage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_webflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_whisky_hunter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_woocommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_xero.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_xkcd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_yandex_metrica.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_younium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_youtube_analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_chat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3128 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_sunshine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_support.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_talk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1879 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zenloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3086 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zoho_crm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zoom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/source_zuora.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/sourcecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/sourceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/sourcesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/streamconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/streamconfigurations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/streamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/workspacecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1262 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/workspaceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/models/shared/workspacesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6864 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/sources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.817398 airbyte-api-0.6.0/src/airbyte/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6126 2023-05-16 00:25:45.000000 airbyte-api-0.6.0/src/airbyte/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:26:00.817398 airbyte-api-0.6.0/src/airbyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-16 00:26:00.000000 airbyte-api-0.6.0/src/airbyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-05-16 00:26:00.000000 airbyte-api-0.6.0/src/airbyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:26:00.000000 airbyte-api-0.6.0/src/airbyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 00:26:00.000000 airbyte-api-0.6.0/src/airbyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 00:26:00.000000 airbyte-api-0.6.0/src/airbyte_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.891106 airbyte-api-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-16 18:12:31.887106 airbyte-api-0.7.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7724 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:12:31.891106 airbyte-api-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.835107 airbyte-api-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.839107 airbyte-api-0.7.0/src/airbyte/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5298 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5369 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/destinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5410 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.839107 airbyte-api-0.7.0/src/airbyte/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.843107 airbyte-api-0.7.0/src/airbyte/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/canceljob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/createconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/createdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/createjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/createsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/createworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/deleteconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/deletedestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/deletesource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/deleteworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/getconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/getdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/getjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/getsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/getstreamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/getworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/initiateoauth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/listconnections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/listdestinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1601 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/listjobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/listsources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/listworkspaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/operations/updateworkspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.887106 airbyte-api-0.7.0/src/airbyte/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49754 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/actortypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectioncreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3197 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectionschedulecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectionscheduleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectionstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9258 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_aws_datalake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12641 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11392 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_cassandra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6136 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_convex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_cumulio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_databend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8016 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_databricks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2752 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_elasticsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3749 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_firestore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21027 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2044 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_keen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_kinesis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6284 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_meilisearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9179 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8107 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6051 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6750 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11112 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_pubsub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5795 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_pulsar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_rabbitmq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8012 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_redis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13955 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_rockset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18868 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8927 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_s3_glue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_scylla.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_sftp_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14064 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destination_typesense.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destinationcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destinationresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/destinationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/geographyenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/initiateoauthrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/jobcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/jobresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/jobsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/jobstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/jobtypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/namespacedefinitionenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      361 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/nonbreakingschemaupdatesbehaviorenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/scheduletypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1457 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_aircall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_airtable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7489 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_alloydb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4938 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_amazon_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5139 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_amazon_seller_partner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3915 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_amplitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1295 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_apify_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_asana.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_auth0.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_aws_cloudtrail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3043 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_azure_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1621 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_bamboo_hr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_bigcommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3210 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_bing_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_braintree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_braze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_chargebee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_chartmogul.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5703 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2895 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_clickup_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_close_com.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_coda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_coin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_coinmarketcap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_configcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_confluence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_datascope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1163 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_delighted.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_dixa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_dockerhub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_dremio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4278 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_e2e_test_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_emailoctopus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_exchange_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17683 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_facebook_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_facebook_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_faker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_fauna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10260 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_file_secure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2006 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_freshcaller.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_freshdesk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_freshsales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_getlago.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_github.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4124 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_gitlab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_glassfrog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_gnews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5437 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_analytics_data_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4945 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_analytics_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_directory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_search_console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_webfonts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_greenhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_gridly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_harvest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_hubplanner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_hubspot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_insightly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_instagram.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_instatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_intercom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_ip2whois.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_iterable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_jira.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_k6_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_klarna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_klaviyo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_kustomer_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_launchdarkly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_lemlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_linkedin_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_linkedin_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_linnworks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_lokalise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mailchimp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mailgun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mailjet_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_marketo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_metabase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_microsoft_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6224 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mixpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_monday.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4394 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12174 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_my_hours.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12789 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_netsuite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3005 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_notion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_nytimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_omnisend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2679 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_onesignal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_openweather.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_orb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_orbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_outreach.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2189 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_paypal_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_paystack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pendo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_persistiq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pexels_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3219 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pinterest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pipedrive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pocket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pokeapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2961 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_polygon_stock_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7508 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_posthog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_postmarkapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_prestashop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_public_apis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_punk_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_pypi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_qualaroo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3521 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_quickbooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_railz.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_recharge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_recreation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_recruitee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_recurly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_retently.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_rki_covid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_rss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13786 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_salesforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3502 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_salesforce_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_salesloft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sap_fieldglass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_secoda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sendgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sendinblue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_senseforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sentry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sftp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sftp_bulk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3373 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_shopify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1127 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_shortio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_slack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_smaily.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      772 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_smartengage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4159 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_smartsheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_snapchat_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4381 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2194 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_sonar_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_spacex_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3492 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_square.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_strava.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_stripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_survey_sparrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3720 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_surveymonkey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_tempo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_the_guardian_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_tiktok_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_todoist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_trello.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_trustpilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_tvmaze_schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_twilio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_twilio_taskrouter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2168 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_twitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_typeform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_us_census.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_vantage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_webflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_whisky_hunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_woocommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_xero.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_xkcd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_yandex_metrica.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_younium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_youtube_analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_chat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3128 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_sunshine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_talk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1879 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zenloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3086 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zoho_crm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zoom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3317 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/source_zuora.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/sourcecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/sourceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      935 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/sourcesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/streamconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/streamconfigurations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/streamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/workspacecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1112 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/workspaceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/workspacesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/models/shared/workspaceupdaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6864 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/sources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.887106 airbyte-api-0.7.0/src/airbyte/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8407 2023-05-16 18:12:13.000000 airbyte-api-0.7.0/src/airbyte/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:31.887106 airbyte-api-0.7.0/src/airbyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-16 18:12:31.000000 airbyte-api-0.7.0/src/airbyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-05-16 18:12:31.000000 airbyte-api-0.7.0/src/airbyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:12:31.000000 airbyte-api-0.7.0/src/airbyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 18:12:31.000000 airbyte-api-0.7.0/src/airbyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 18:12:31.000000 airbyte-api-0.7.0/src/airbyte_api.egg-info/top_level.txt
```

### Comparing `airbyte-api-0.6.0/LICENSE.md` & `airbyte-api-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/PKG-INFO` & `airbyte-api-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Airbyte
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -107,22 +107,23 @@
                 sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
         ],
     ),
     data_residency=shared.GeographyEnumEnum.EU,
     destination_id='c816742c-b739-4205-9293-96fea7596eb1',
     name='Lela Orn',
-    namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+    namespace_definition=shared.NamespaceDefinitionEnumEnum.SOURCE,
     namespace_format='${SOURCE_NAMESPACE}',
-    prefix='dolorem',
+    non_breaking_schema_updates_behavior=shared.NonBreakingSchemaUpdatesBehaviorEnumEnum.IGNORE,
+    prefix='corporis',
     schedule=shared.ConnectionScheduleCreate(
-        cron_expression='corporis',
-        schedule_type=shared.ScheduleTypeEnumEnum.MANUAL,
+        cron_expression='explicabo',
+        schedule_type=shared.ScheduleTypeEnumEnum.CRON,
     ),
-    source_id='c5955907-aff1-4a3a-afa9-467739251aa5',
+    source_id='5955907a-ff1a-43a2-ba94-67739251aa52',
 )
 
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
@@ -165,16 +166,18 @@
 
 * [get_stream_properties](docs/streams/README.md#get_stream_properties) - Get stream properties
 
 ### [workspaces](docs/workspaces/README.md)
 
 * [create_or_update_workspace_o_auth_credentials](docs/workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create OAuth override credentials for a workspace and source type.
 * [create_workspace](docs/workspaces/README.md#create_workspace) - Create a workspace
+* [delete_workspace](docs/workspaces/README.md#delete_workspace) - Delete a Workspace
 * [get_workspace](docs/workspaces/README.md#get_workspace) - Get Workspace details
 * [list_workspaces](docs/workspaces/README.md#list_workspaces) - List workspaces
+* [update_workspace](docs/workspaces/README.md#update_workspace) - Update a workspace
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airbyte-api Version: 0.6.0 Summary: Python Client
+Metadata-Version: 2.1 Name: airbyte-api Version: 0.7.0 Summary: Python Client
 SDK for Airbyte API Home-page: UNKNOWN Author: Airbyte License: UNKNOWN
 Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE.md
  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
                           4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
@@ -32,53 +32,56 @@
 Bernier MD', primary_key=[ [ 'repellendus', 'sapiente', ], ],
 sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY, ),
 shared.StreamConfiguration( cursor_field=[ 'at', ], name='Emilio Krajcik',
 primary_key=[ [ 'porro', 'dolorum', 'dicta', ], [ 'officia', 'occaecati',
 'fugit', ], ], sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
 ), ], ), data_residency=shared.GeographyEnumEnum.EU, destination_id='c816742c-
 b739-4205-9293-96fea7596eb1', name='Lela Orn',
-namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
-namespace_format='${SOURCE_NAMESPACE}', prefix='dolorem',
-schedule=shared.ConnectionScheduleCreate( cron_expression='corporis',
-schedule_type=shared.ScheduleTypeEnumEnum.MANUAL, ), source_id='c5955907-aff1-
-4a3a-afa9-467739251aa5', ) res = s.connections.create_connection(req) if
-res.connection_response is not None: # handle response ```   ## Available
-Resources and Operations ### [connections](docs/connections/README.md) *
-[create_connection](docs/connections/README.md#create_connection) - Create a
-connection * [delete_connection](docs/connections/README.md#delete_connection)
-- Delete a Connection * [get_connection](docs/connections/
-README.md#get_connection) - Get Connection details * [list_connections](docs/
-connections/README.md#list_connections) - List connections ### [destinations]
-(docs/destinations/README.md) * [create_destination](docs/destinations/
-README.md#create_destination) - Create a destination * [delete_destination]
-(docs/destinations/README.md#delete_destination) - Delete a Destination *
-[get_destination](docs/destinations/README.md#get_destination) - Get
-Destination details * [list_destinations](docs/destinations/
-README.md#list_destinations) - List destinations ### [jobs](docs/jobs/
-README.md) * [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running
-Job * [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset
-job of a connection * [get_job](docs/jobs/README.md#get_job) - Get Job status
-and details * [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync
-type ### [sources](docs/sources/README.md) * [create_source](docs/sources/
-README.md#create_source) - Create a source * [delete_source](docs/sources/
-README.md#delete_source) - Delete a Source * [get_source](docs/sources/
-README.md#get_source) - Get Source details * [initiate_o_auth](docs/sources/
-README.md#initiate_o_auth) - Initiate OAuth for a source * [list_sources](docs/
-sources/README.md#list_sources) - List sources ### [streams](docs/streams/
-README.md) * [get_stream_properties](docs/streams/
+namespace_definition=shared.NamespaceDefinitionEnumEnum.SOURCE,
+namespace_format='${SOURCE_NAMESPACE}',
+non_breaking_schema_updates_behavior=shared.NonBreakingSchemaUpdatesBehaviorEnumEnum.IGNORE,
+prefix='corporis', schedule=shared.ConnectionScheduleCreate
+( cron_expression='explicabo', schedule_type=shared.ScheduleTypeEnumEnum.CRON,
+), source_id='5955907a-ff1a-43a2-ba94-67739251aa52', ) res =
+s.connections.create_connection(req) if res.connection_response is not None: #
+handle response ```   ## Available Resources and Operations ### [connections]
+(docs/connections/README.md) * [create_connection](docs/connections/
+README.md#create_connection) - Create a connection * [delete_connection](docs/
+connections/README.md#delete_connection) - Delete a Connection *
+[get_connection](docs/connections/README.md#get_connection) - Get Connection
+details * [list_connections](docs/connections/README.md#list_connections) -
+List connections ### [destinations](docs/destinations/README.md) *
+[create_destination](docs/destinations/README.md#create_destination) - Create a
+destination * [delete_destination](docs/destinations/
+README.md#delete_destination) - Delete a Destination * [get_destination](docs/
+destinations/README.md#get_destination) - Get Destination details *
+[list_destinations](docs/destinations/README.md#list_destinations) - List
+destinations ### [jobs](docs/jobs/README.md) * [cancel_job](docs/jobs/
+README.md#cancel_job) - Cancel a running Job * [create_job](docs/jobs/
+README.md#create_job) - Trigger a sync or reset job of a connection * [get_job]
+(docs/jobs/README.md#get_job) - Get Job status and details * [list_jobs](docs/
+jobs/README.md#list_jobs) - List Jobs by sync type ### [sources](docs/sources/
+README.md) * [create_source](docs/sources/README.md#create_source) - Create a
+source * [delete_source](docs/sources/README.md#delete_source) - Delete a
+Source * [get_source](docs/sources/README.md#get_source) - Get Source details *
+[initiate_o_auth](docs/sources/README.md#initiate_o_auth) - Initiate OAuth for
+a source * [list_sources](docs/sources/README.md#list_sources) - List sources
+### [streams](docs/streams/README.md) * [get_stream_properties](docs/streams/
 README.md#get_stream_properties) - Get stream properties ### [workspaces](docs/
 workspaces/README.md) * [create_or_update_workspace_o_auth_credentials](docs/
 workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create
 OAuth override credentials for a workspace and source type. *
 [create_workspace](docs/workspaces/README.md#create_workspace) - Create a
-workspace * [get_workspace](docs/workspaces/README.md#get_workspace) - Get
-Workspace details * [list_workspaces](docs/workspaces/
-README.md#list_workspaces) - List workspaces  ### Maturity This SDK is in beta,
-and there may be breaking changes between versions without a major version
-update. Therefore, we recommend pinning usage to a specific package version.
-This way, you can install the same version each time without breaking changes
-unless you are intentionally looking for the latest version. ### Contributions
-While we value open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release ! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+workspace * [delete_workspace](docs/workspaces/README.md#delete_workspace) -
+Delete a Workspace * [get_workspace](docs/workspaces/README.md#get_workspace) -
+Get Workspace details * [list_workspaces](docs/workspaces/
+README.md#list_workspaces) - List workspaces * [update_workspace](docs/
+workspaces/README.md#update_workspace) - Update a workspace  ### Maturity This
+SDK is in beta, and there may be breaking changes between versions without a
+major version update. Therefore, we recommend pinning usage to a specific
+package version. This way, you can install the same version each time without
+breaking changes unless you are intentionally looking for the latest version.
+### Contributions While we value open-source contributions to this SDK, this
+library is generated programmatically. Feel free to open a PR or a Github issue
+as a proof of concept and we'll do our best to include it in a future release !
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
+speakeasy/client-sdks)
```

### Comparing `airbyte-api-0.6.0/README.md` & `airbyte-api-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -95,22 +95,23 @@
                 sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
         ],
     ),
     data_residency=shared.GeographyEnumEnum.EU,
     destination_id='c816742c-b739-4205-9293-96fea7596eb1',
     name='Lela Orn',
-    namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+    namespace_definition=shared.NamespaceDefinitionEnumEnum.SOURCE,
     namespace_format='${SOURCE_NAMESPACE}',
-    prefix='dolorem',
+    non_breaking_schema_updates_behavior=shared.NonBreakingSchemaUpdatesBehaviorEnumEnum.IGNORE,
+    prefix='corporis',
     schedule=shared.ConnectionScheduleCreate(
-        cron_expression='corporis',
-        schedule_type=shared.ScheduleTypeEnumEnum.MANUAL,
+        cron_expression='explicabo',
+        schedule_type=shared.ScheduleTypeEnumEnum.CRON,
     ),
-    source_id='c5955907-aff1-4a3a-afa9-467739251aa5',
+    source_id='5955907a-ff1a-43a2-ba94-67739251aa52',
 )
 
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
@@ -153,16 +154,18 @@
 
 * [get_stream_properties](docs/streams/README.md#get_stream_properties) - Get stream properties
 
 ### [workspaces](docs/workspaces/README.md)
 
 * [create_or_update_workspace_o_auth_credentials](docs/workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create OAuth override credentials for a workspace and source type.
 * [create_workspace](docs/workspaces/README.md#create_workspace) - Create a workspace
+* [delete_workspace](docs/workspaces/README.md#delete_workspace) - Delete a Workspace
 * [get_workspace](docs/workspaces/README.md#get_workspace) - Get Workspace details
 * [list_workspaces](docs/workspaces/README.md#list_workspaces) - List workspaces
+* [update_workspace](docs/workspaces/README.md#update_workspace) - Update a workspace
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
```

#### html2text {}

```diff
@@ -28,53 +28,56 @@
 Bernier MD', primary_key=[ [ 'repellendus', 'sapiente', ], ],
 sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY, ),
 shared.StreamConfiguration( cursor_field=[ 'at', ], name='Emilio Krajcik',
 primary_key=[ [ 'porro', 'dolorum', 'dicta', ], [ 'officia', 'occaecati',
 'fugit', ], ], sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
 ), ], ), data_residency=shared.GeographyEnumEnum.EU, destination_id='c816742c-
 b739-4205-9293-96fea7596eb1', name='Lela Orn',
-namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
-namespace_format='${SOURCE_NAMESPACE}', prefix='dolorem',
-schedule=shared.ConnectionScheduleCreate( cron_expression='corporis',
-schedule_type=shared.ScheduleTypeEnumEnum.MANUAL, ), source_id='c5955907-aff1-
-4a3a-afa9-467739251aa5', ) res = s.connections.create_connection(req) if
-res.connection_response is not None: # handle response ```   ## Available
-Resources and Operations ### [connections](docs/connections/README.md) *
-[create_connection](docs/connections/README.md#create_connection) - Create a
-connection * [delete_connection](docs/connections/README.md#delete_connection)
-- Delete a Connection * [get_connection](docs/connections/
-README.md#get_connection) - Get Connection details * [list_connections](docs/
-connections/README.md#list_connections) - List connections ### [destinations]
-(docs/destinations/README.md) * [create_destination](docs/destinations/
-README.md#create_destination) - Create a destination * [delete_destination]
-(docs/destinations/README.md#delete_destination) - Delete a Destination *
-[get_destination](docs/destinations/README.md#get_destination) - Get
-Destination details * [list_destinations](docs/destinations/
-README.md#list_destinations) - List destinations ### [jobs](docs/jobs/
-README.md) * [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running
-Job * [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset
-job of a connection * [get_job](docs/jobs/README.md#get_job) - Get Job status
-and details * [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync
-type ### [sources](docs/sources/README.md) * [create_source](docs/sources/
-README.md#create_source) - Create a source * [delete_source](docs/sources/
-README.md#delete_source) - Delete a Source * [get_source](docs/sources/
-README.md#get_source) - Get Source details * [initiate_o_auth](docs/sources/
-README.md#initiate_o_auth) - Initiate OAuth for a source * [list_sources](docs/
-sources/README.md#list_sources) - List sources ### [streams](docs/streams/
-README.md) * [get_stream_properties](docs/streams/
+namespace_definition=shared.NamespaceDefinitionEnumEnum.SOURCE,
+namespace_format='${SOURCE_NAMESPACE}',
+non_breaking_schema_updates_behavior=shared.NonBreakingSchemaUpdatesBehaviorEnumEnum.IGNORE,
+prefix='corporis', schedule=shared.ConnectionScheduleCreate
+( cron_expression='explicabo', schedule_type=shared.ScheduleTypeEnumEnum.CRON,
+), source_id='5955907a-ff1a-43a2-ba94-67739251aa52', ) res =
+s.connections.create_connection(req) if res.connection_response is not None: #
+handle response ```   ## Available Resources and Operations ### [connections]
+(docs/connections/README.md) * [create_connection](docs/connections/
+README.md#create_connection) - Create a connection * [delete_connection](docs/
+connections/README.md#delete_connection) - Delete a Connection *
+[get_connection](docs/connections/README.md#get_connection) - Get Connection
+details * [list_connections](docs/connections/README.md#list_connections) -
+List connections ### [destinations](docs/destinations/README.md) *
+[create_destination](docs/destinations/README.md#create_destination) - Create a
+destination * [delete_destination](docs/destinations/
+README.md#delete_destination) - Delete a Destination * [get_destination](docs/
+destinations/README.md#get_destination) - Get Destination details *
+[list_destinations](docs/destinations/README.md#list_destinations) - List
+destinations ### [jobs](docs/jobs/README.md) * [cancel_job](docs/jobs/
+README.md#cancel_job) - Cancel a running Job * [create_job](docs/jobs/
+README.md#create_job) - Trigger a sync or reset job of a connection * [get_job]
+(docs/jobs/README.md#get_job) - Get Job status and details * [list_jobs](docs/
+jobs/README.md#list_jobs) - List Jobs by sync type ### [sources](docs/sources/
+README.md) * [create_source](docs/sources/README.md#create_source) - Create a
+source * [delete_source](docs/sources/README.md#delete_source) - Delete a
+Source * [get_source](docs/sources/README.md#get_source) - Get Source details *
+[initiate_o_auth](docs/sources/README.md#initiate_o_auth) - Initiate OAuth for
+a source * [list_sources](docs/sources/README.md#list_sources) - List sources
+### [streams](docs/streams/README.md) * [get_stream_properties](docs/streams/
 README.md#get_stream_properties) - Get stream properties ### [workspaces](docs/
 workspaces/README.md) * [create_or_update_workspace_o_auth_credentials](docs/
 workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create
 OAuth override credentials for a workspace and source type. *
 [create_workspace](docs/workspaces/README.md#create_workspace) - Create a
-workspace * [get_workspace](docs/workspaces/README.md#get_workspace) - Get
-Workspace details * [list_workspaces](docs/workspaces/
-README.md#list_workspaces) - List workspaces  ### Maturity This SDK is in beta,
-and there may be breaking changes between versions without a major version
-update. Therefore, we recommend pinning usage to a specific package version.
-This way, you can install the same version each time without breaking changes
-unless you are intentionally looking for the latest version. ### Contributions
-While we value open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release ! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+workspace * [delete_workspace](docs/workspaces/README.md#delete_workspace) -
+Delete a Workspace * [get_workspace](docs/workspaces/README.md#get_workspace) -
+Get Workspace details * [list_workspaces](docs/workspaces/
+README.md#list_workspaces) - List workspaces * [update_workspace](docs/
+workspaces/README.md#update_workspace) - Update a workspace  ### Maturity This
+SDK is in beta, and there may be breaking changes between versions without a
+major version update. Therefore, we recommend pinning usage to a specific
+package version. This way, you can install the same version each time without
+breaking changes unless you are intentionally looking for the latest version.
+### Contributions While we value open-source contributions to this SDK, this
+library is generated programmatically. Feel free to open a PR or a Github issue
+as a proof of concept and we'll do our best to include it in a future release !
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
+speakeasy/client-sdks)
```

### Comparing `airbyte-api-0.6.0/setup.py` & `airbyte-api-0.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="airbyte-api",
-    version="0.6.0",
+    version="0.7.0",
     author="Airbyte",
     description="Python Client SDK for Airbyte API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `airbyte-api-0.6.0/src/airbyte/connections.py` & `airbyte-api-0.7.0/src/airbyte/connections.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/destinations.py` & `airbyte-api-0.7.0/src/airbyte/destinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/jobs.py` & `airbyte-api-0.7.0/src/airbyte/jobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/__init__.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from .createjob import *
 from .createorupdateworkspaceoauthcredentials import *
 from .createsource import *
 from .createworkspace import *
 from .deleteconnection import *
 from .deletedestination import *
 from .deletesource import *
+from .deleteworkspace import *
 from .getconnection import *
 from .getdestination import *
 from .getjob import *
 from .getsource import *
 from .getstreamproperties import *
 from .getworkspace import *
 from .initiateoauth import *
 from .listconnections import *
 from .listdestinations import *
 from .listjobs import *
 from .listsources import *
 from .listworkspaces import *
+from .updateworkspace import *
 
-__all__ = ["CancelJobRequest","CancelJobResponse","CreateConnectionResponse","CreateDestinationResponse","CreateJobResponse","CreateOrUpdateWorkspaceOAuthCredentialsRequest","CreateOrUpdateWorkspaceOAuthCredentialsResponse","CreateSourceResponse","CreateWorkspaceResponse","DeleteConnectionRequest","DeleteConnectionResponse","DeleteDestinationRequest","DeleteDestinationResponse","DeleteSourceRequest","DeleteSourceResponse","GetConnectionRequest","GetConnectionResponse","GetDestinationRequest","GetDestinationResponse","GetJobRequest","GetJobResponse","GetSourceRequest","GetSourceResponse","GetStreamPropertiesRequest","GetStreamPropertiesResponse","GetWorkspaceRequest","GetWorkspaceResponse","InitiateOAuthResponse","ListConnectionsRequest","ListConnectionsResponse","ListDestinationsRequest","ListDestinationsResponse","ListJobsRequest","ListJobsResponse","ListSourcesRequest","ListSourcesResponse","ListWorkspacesRequest","ListWorkspacesResponse"]
+__all__ = ["CancelJobRequest","CancelJobResponse","CreateConnectionResponse","CreateDestinationResponse","CreateJobResponse","CreateOrUpdateWorkspaceOAuthCredentialsRequest","CreateOrUpdateWorkspaceOAuthCredentialsResponse","CreateSourceResponse","CreateWorkspaceResponse","DeleteConnectionRequest","DeleteConnectionResponse","DeleteDestinationRequest","DeleteDestinationResponse","DeleteSourceRequest","DeleteSourceResponse","DeleteWorkspaceRequest","DeleteWorkspaceResponse","GetConnectionRequest","GetConnectionResponse","GetDestinationRequest","GetDestinationResponse","GetJobRequest","GetJobResponse","GetSourceRequest","GetSourceResponse","GetStreamPropertiesRequest","GetStreamPropertiesResponse","GetWorkspaceRequest","GetWorkspaceResponse","InitiateOAuthResponse","ListConnectionsRequest","ListConnectionsResponse","ListDestinationsRequest","ListDestinationsResponse","ListJobsRequest","ListJobsResponse","ListSourcesRequest","ListSourcesResponse","ListWorkspacesRequest","ListWorkspacesResponse","UpdateWorkspaceRequest","UpdateWorkspaceResponse"]
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/canceljob.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/canceljob.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/createconnection.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/createconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/createdestination.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/createdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/createjob.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/createjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/createsource.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/createsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/createworkspace.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/deleteconnection.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/deleteconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/deletedestination.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/deletedestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/deletesource.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/deletesource.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/getconnection.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/getconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/getdestination.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/getdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/getjob.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/getjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/getsource.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/getsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/getstreamproperties.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/getstreamproperties.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 @dataclasses.dataclass
 class GetStreamPropertiesRequest:
     
     destination_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'destinationId', 'style': 'form', 'explode': True }})
     r"""ID of the destination"""
     source_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'sourceId', 'style': 'form', 'explode': True }})
     r"""ID of the source"""
+    ignore_cache: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ignoreCache', 'style': 'form', 'explode': True }})
+    r"""If true pull the latest schema from the source, else pull from cache (default false)"""
     
 
 @dataclasses.dataclass
 class GetStreamPropertiesResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/getworkspace.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/listconnections.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/listconnections.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/listdestinations.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/listdestinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/listjobs.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/listjobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/listsources.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/listsources.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/operations/listworkspaces.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/listworkspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/__init__.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
+from .actortypeenum_enum import *
 from .connectioncreaterequest import *
 from .connectionresponse import *
 from .connectionschedulecreate import *
 from .connectionscheduleresponse import *
 from .connectionsresponse import *
 from .connectionstatusenum_enum import *
 from .connectionsyncmodeenum_enum import *
@@ -11,14 +12,15 @@
 from .destination_aws_datalake import *
 from .destination_azure_blob_storage import *
 from .destination_bigquery import *
 from .destination_bigquery_denormalized import *
 from .destination_cassandra import *
 from .destination_clickhouse import *
 from .destination_convex import *
+from .destination_cumulio import *
 from .destination_databend import *
 from .destination_databricks import *
 from .destination_dynamodb import *
 from .destination_elasticsearch import *
 from .destination_firebolt import *
 from .destination_firestore import *
 from .destination_gcs import *
@@ -50,17 +52,20 @@
 from .geographyenum_enum import *
 from .initiateoauthrequest import *
 from .jobcreaterequest import *
 from .jobresponse import *
 from .jobsresponse import *
 from .jobstatusenum_enum import *
 from .jobtypeenum_enum import *
+from .namespacedefinitionenum_enum import *
+from .nonbreakingschemaupdatesbehaviorenum_enum import *
 from .scheduletypeenum_enum import *
 from .scheduletypewithbasicenum_enum import *
 from .security import *
+from .source_aircall import *
 from .source_airtable import *
 from .source_alloydb import *
 from .source_amazon_ads import *
 from .source_amazon_seller_partner import *
 from .source_amazon_sqs import *
 from .source_amplitude import *
 from .source_apify_dataset import *
@@ -253,9 +258,10 @@
 from .streamconfiguration import *
 from .streamconfigurations import *
 from .streamproperties import *
 from .workspacecreaterequest import *
 from .workspaceoauthcredentialsrequest import *
 from .workspaceresponse import *
 from .workspacesresponse import *
+from .workspaceupdaterequest import *
 
-__all__ = ["ConnectionCreateRequest","ConnectionCreateRequestNamespaceDefinitionEnum","ConnectionResponse","ConnectionScheduleCreate","ConnectionScheduleResponse","ConnectionStatusEnumEnum","ConnectionSyncModeEnumEnum","ConnectionsResponse","DestinationAmazonSqs","DestinationAmazonSqsAWSRegionEnum","DestinationAmazonSqsAmazonSqsEnum","DestinationAwsDatalake","DestinationAwsDatalakeAwsDatalakeEnum","DestinationAwsDatalakeChooseHowToPartitionDataEnum","DestinationAwsDatalakeCredentialsIAMRole","DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum","DestinationAwsDatalakeCredentialsIAMUser","DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum","DestinationAwsDatalakeFormatParquetColumnarStorage","DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum","DestinationAwsDatalakeS3BucketRegionEnum","DestinationAzureBlobStorage","DestinationAzureBlobStorageAzureBlobStorageEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValues","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationBigquery","DestinationBigqueryBigqueryEnum","DestinationBigqueryDatasetLocationEnum","DestinationBigqueryDenormalized","DestinationBigqueryDenormalizedBigqueryDenormalizedEnum","DestinationBigqueryDenormalizedDatasetLocationEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStaging","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum","DestinationBigqueryDenormalizedLoadingMethodStandardInserts","DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryLoadingMethodGCSStaging","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryLoadingMethodGCSStagingMethodEnum","DestinationBigqueryLoadingMethodStandardInserts","DestinationBigqueryLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryTransformationQueryRunTypeEnum","DestinationCassandra","DestinationCassandraCassandraEnum","DestinationClickhouse","DestinationClickhouseClickhouseEnum","DestinationClickhouseTunnelMethodNoTunnel","DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum","DestinationClickhouseTunnelMethodPasswordAuthentication","DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationClickhouseTunnelMethodSSHKeyAuthentication","DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationConvex","DestinationConvexConvexEnum","DestinationCreateRequest","DestinationDatabend","DestinationDatabendDatabendEnum","DestinationDatabricks","DestinationDatabricksDataSourceAmazonS3","DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum","DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum","DestinationDatabricksDataSourceAzureBlobStorage","DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum","DestinationDatabricksDataSourceRecommendedManagedTables","DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum","DestinationDatabricksDatabricksEnum","DestinationDynamodb","DestinationDynamodbDynamoDBRegionEnum","DestinationDynamodbDynamodbEnum","DestinationElasticsearch","DestinationElasticsearchAuthenticationMethodAPIKeySecret","DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum","DestinationElasticsearchAuthenticationMethodUsernamePassword","DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum","DestinationElasticsearchElasticsearchEnum","DestinationFirebolt","DestinationFireboltFireboltEnum","DestinationFireboltLoadingMethodExternalTableViaS3","DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum","DestinationFireboltLoadingMethodSQLInserts","DestinationFireboltLoadingMethodSQLInsertsMethodEnum","DestinationFirestore","DestinationFirestoreFirestoreEnum","DestinationGCSGCSBucketRegionEnum","DestinationGcs","DestinationGcsCredentialHMACKey","DestinationGcsCredentialHMACKeyCredentialTypeEnum","DestinationGcsFormatAvroApacheAvro","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecXz","DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationGcsFormatAvroApacheAvroFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValues","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSON","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationGcsFormatParquetColumnarStorage","DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum","DestinationGcsFormatParquetColumnarStorageFormatTypeEnum","DestinationGcsGcsEnum","DestinationGoogleSheets","DestinationGoogleSheetsAuthenticationViaGoogleOAuth","DestinationGoogleSheetsGoogleSheetsEnum","DestinationKeen","DestinationKeenKeenEnum","DestinationKinesis","DestinationKinesisKinesisEnum","DestinationMariadbColumnstore","DestinationMariadbColumnstoreMariadbColumnstoreEnum","DestinationMariadbColumnstoreTunnelMethodNoTunnel","DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication","DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMeilisearch","DestinationMeilisearchMeilisearchEnum","DestinationMongodb","DestinationMongodbAuthTypeLoginPassword","DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum","DestinationMongodbAuthTypeNone","DestinationMongodbAuthTypeNoneAuthorizationEnum","DestinationMongodbInstanceTypeMongoDBAtlas","DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum","DestinationMongodbInstanceTypeReplicaSet","DestinationMongodbInstanceTypeReplicaSetInstanceEnum","DestinationMongodbInstanceTypeStandaloneMongoDbInstance","DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","DestinationMongodbMongodbEnum","DestinationMongodbTunnelMethodNoTunnel","DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum","DestinationMongodbTunnelMethodPasswordAuthentication","DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMongodbTunnelMethodSSHKeyAuthentication","DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMssql","DestinationMssqlMssqlEnum","DestinationMssqlSslMethodEncryptedTrustServerCertificate","DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","DestinationMssqlSslMethodEncryptedVerifyCertificate","DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","DestinationMssqlTunnelMethodNoTunnel","DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMssqlTunnelMethodPasswordAuthentication","DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMssqlTunnelMethodSSHKeyAuthentication","DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMysql","DestinationMysqlMysqlEnum","DestinationMysqlTunnelMethodNoTunnel","DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMysqlTunnelMethodPasswordAuthentication","DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMysqlTunnelMethodSSHKeyAuthentication","DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationOracle","DestinationOracleOracleEnum","DestinationOracleTunnelMethodNoTunnel","DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum","DestinationOracleTunnelMethodPasswordAuthentication","DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationOracleTunnelMethodSSHKeyAuthentication","DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPostgres","DestinationPostgresPostgresEnum","DestinationPostgresSslModeAllow","DestinationPostgresSslModeAllowModeEnum","DestinationPostgresSslModeDisable","DestinationPostgresSslModeDisableModeEnum","DestinationPostgresSslModePrefer","DestinationPostgresSslModePreferModeEnum","DestinationPostgresSslModeRequire","DestinationPostgresSslModeRequireModeEnum","DestinationPostgresSslModeVerifyCa","DestinationPostgresSslModeVerifyCaModeEnum","DestinationPostgresSslModeVerifyFull","DestinationPostgresSslModeVerifyFullModeEnum","DestinationPostgresTunnelMethodNoTunnel","DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum","DestinationPostgresTunnelMethodPasswordAuthentication","DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationPostgresTunnelMethodSSHKeyAuthentication","DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPubsub","DestinationPubsubPubsubEnum","DestinationPulsar","DestinationPulsarCompressionTypeEnum","DestinationPulsarPulsarEnum","DestinationPulsarTopicTypeEnum","DestinationRabbitmq","DestinationRabbitmqRabbitmqEnum","DestinationRedis","DestinationRedisCacheTypeEnum","DestinationRedisRedisEnum","DestinationRedisSslModeDisable","DestinationRedisSslModeDisableModeEnum","DestinationRedisSslModeVerifyFull","DestinationRedisSslModeVerifyFullModeEnum","DestinationRedisTunnelMethodNoTunnel","DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedisTunnelMethodPasswordAuthentication","DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedisTunnelMethodSSHKeyAuthentication","DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshift","DestinationRedshiftRedshiftEnum","DestinationRedshiftTunnelMethodNoTunnel","DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedshiftTunnelMethodPasswordAuthentication","DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedshiftTunnelMethodSSHKeyAuthentication","DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshiftUploadingMethodS3Staging","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingMethodEnum","DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum","DestinationRedshiftUploadingMethodStandard","DestinationRedshiftUploadingMethodStandardMethodEnum","DestinationResponse","DestinationRockset","DestinationRocksetRocksetEnum","DestinationS3","DestinationS3FormatAvroApacheAvro","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecDeflate","DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecSnappy","DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecXz","DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecZstandard","DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationS3FormatAvroApacheAvroFormatTypeEnum","DestinationS3FormatCSVCommaSeparatedValues","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum","DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSON","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3FormatParquetColumnarStorage","DestinationS3FormatParquetColumnarStorageCompressionCodecEnum","DestinationS3FormatParquetColumnarStorageFormatTypeEnum","DestinationS3Glue","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3GlueS3BucketRegionEnum","DestinationS3GlueS3GlueEnum","DestinationS3GlueSerializationLibraryEnum","DestinationS3S3BucketRegionEnum","DestinationS3S3Enum","DestinationScylla","DestinationScyllaScyllaEnum","DestinationSftpJSON","DestinationSftpJSONSftpJSONEnum","DestinationSnowflake","DestinationSnowflakeCredentialsKeyPairAuthentication","DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum","DestinationSnowflakeCredentialsOAuth20","DestinationSnowflakeCredentialsOAuth20AuthTypeEnum","DestinationSnowflakeCredentialsUsernameAndPassword","DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","DestinationSnowflakeLoadingMethodAWSS3Staging","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum","DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum","DestinationSnowflakeLoadingMethodAzureBlobStorageStaging","DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging","DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodRecommendedInternalStaging","DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum","DestinationSnowflakeLoadingMethodSelectAnotherOption","DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum","DestinationSnowflakeSnowflakeEnum","DestinationTypesense","DestinationTypesenseTypesenseEnum","DestinationsResponse","GeographyEnumEnum","InitiateOauthRequest","JobCreateRequest","JobResponse","JobStatusEnumEnum","JobTypeEnumEnum","JobsResponse","ScheduleTypeEnumEnum","ScheduleTypeWithBasicEnumEnum","Security","SourceAirtable","SourceAirtableAirtableEnum","SourceAirtableCredentialsOAuth20","SourceAirtableCredentialsOAuth20AuthMethodEnum","SourceAirtableCredentialsPersonalAccessToken","SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum","SourceAlloydb","SourceAlloydbAlloydbEnum","SourceAlloydbReplicationMethodStandard","SourceAlloydbReplicationMethodStandardMethodEnum","SourceAlloydbTunnelMethodNoTunnel","SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum","SourceAlloydbTunnelMethodPasswordAuthentication","SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceAlloydbTunnelMethodSSHKeyAuthentication","SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceAmazonAds","SourceAmazonAdsAmazonAdsEnum","SourceAmazonAdsAuthTypeEnum","SourceAmazonAdsRegionEnum","SourceAmazonAdsReportRecordTypesEnum","SourceAmazonAdsStateFilterEnum","SourceAmazonSellerPartner","SourceAmazonSellerPartnerAWSEnvironmentEnum","SourceAmazonSellerPartnerAWSRegionEnum","SourceAmazonSellerPartnerAmazonSellerPartnerEnum","SourceAmazonSellerPartnerAuthTypeEnum","SourceAmazonSqs","SourceAmazonSqsAWSRegionEnum","SourceAmazonSqsAmazonSqsEnum","SourceAmplitude","SourceAmplitudeAmplitudeEnum","SourceAmplitudeDataRegionEnum","SourceApifyDataset","SourceApifyDatasetApifyDatasetEnum","SourceAsana","SourceAsanaAsanaEnum","SourceAsanaCredentialsAuthenticateViaAsanaOauth","SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum","SourceAsanaCredentialsAuthenticateWithPersonalAccessToken","SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum","SourceAuth0","SourceAuth0Auth0Enum","SourceAuth0CredentialsOAuth2AccessToken","SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum","SourceAuth0CredentialsOAuth2ConfidentialApplication","SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum","SourceAwsCloudtrail","SourceAwsCloudtrailAwsCloudtrailEnum","SourceAzureBlobStorage","SourceAzureBlobStorageAzureBlobStorageEnum","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","SourceAzureTable","SourceAzureTableAzureTableEnum","SourceBambooHr","SourceBambooHrBambooHrEnum","SourceBigcommerce","SourceBigcommerceBigcommerceEnum","SourceBigquery","SourceBigqueryBigqueryEnum","SourceBingAds","SourceBingAdsAuthMethodEnum","SourceBingAdsBingAdsEnum","SourceBraintree","SourceBraintreeBraintreeEnum","SourceBraintreeEnvironmentEnum","SourceBraze","SourceBrazeBrazeEnum","SourceChargebee","SourceChargebeeChargebeeEnum","SourceChargebeeProductCatalogEnum","SourceChartmogul","SourceChartmogulChartmogulEnum","SourceChartmogulIntervalEnum","SourceClickhouse","SourceClickhouseClickhouseEnum","SourceClickhouseTunnelMethodNoTunnel","SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum","SourceClickhouseTunnelMethodPasswordAuthentication","SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceClickhouseTunnelMethodSSHKeyAuthentication","SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceClickupAPI","SourceClickupAPIClickupAPIEnum","SourceCloseCom","SourceCloseComCloseComEnum","SourceCoda","SourceCodaCodaEnum","SourceCoinAPI","SourceCoinAPICoinAPIEnum","SourceCoinAPIEnvironmentEnum","SourceCoinmarketcap","SourceCoinmarketcapCoinmarketcapEnum","SourceCoinmarketcapDataTypeEnum","SourceConfigcat","SourceConfigcatConfigcatEnum","SourceConfluence","SourceConfluenceConfluenceEnum","SourceCreateRequest","SourceDatascope","SourceDatascopeDatascopeEnum","SourceDelighted","SourceDelightedDelightedEnum","SourceDixa","SourceDixaDixaEnum","SourceDockerhub","SourceDockerhubDockerhubEnum","SourceDremio","SourceDremioDremioEnum","SourceDynamodb","SourceDynamodbDynamodbEnum","SourceDynamodbDynamodbRegionEnum","SourceE2eTestCloud","SourceE2eTestCloudE2eTestCloudEnum","SourceE2eTestCloudMockCatalogMultiSchema","SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum","SourceE2eTestCloudMockCatalogSingleSchema","SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum","SourceE2eTestCloudTypeEnum","SourceEmailoctopus","SourceEmailoctopusEmailoctopusEnum","SourceExchangeRates","SourceExchangeRatesExchangeRatesEnum","SourceFacebookMarketing","SourceFacebookMarketingFacebookMarketingEnum","SourceFacebookMarketingInsightConfig","SourceFacebookMarketingInsightConfigLevelEnum","SourceFacebookMarketingInsightConfigValidActionBreakdownsEnum","SourceFacebookMarketingInsightConfigValidBreakdownsEnum","SourceFacebookMarketingInsightConfigValidEnumsEnum","SourceFacebookPages","SourceFacebookPagesFacebookPagesEnum","SourceFaker","SourceFakerFakerEnum","SourceFauna","SourceFaunaCollection","SourceFaunaCollectionDeletionsDisabled","SourceFaunaCollectionDeletionsDisabledDeletionModeEnum","SourceFaunaCollectionDeletionsEnabled","SourceFaunaCollectionDeletionsEnabledDeletionModeEnum","SourceFaunaFaunaEnum","SourceFileSecure","SourceFileSecureFileFormatEnum","SourceFileSecureFileSecureEnum","SourceFileSecureProviderAzBlobAzureBlobStorage","SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum","SourceFileSecureProviderGCSGoogleCloudStorage","SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum","SourceFileSecureProviderHTTPSPublicWeb","SourceFileSecureProviderHTTPSPublicWebStorageEnum","SourceFileSecureProviderS3AmazonWebServices","SourceFileSecureProviderS3AmazonWebServicesStorageEnum","SourceFileSecureProviderSCPSecureCopyProtocol","SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum","SourceFileSecureProviderSFTPSecureFileTransferProtocol","SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum","SourceFileSecureProviderSSHSecureShell","SourceFileSecureProviderSSHSecureShellStorageEnum","SourceFirebolt","SourceFireboltFireboltEnum","SourceFreshcaller","SourceFreshcallerFreshcallerEnum","SourceFreshdesk","SourceFreshdeskFreshdeskEnum","SourceFreshsales","SourceFreshsalesFreshsalesEnum","SourceGcs","SourceGcsGcsEnum","SourceGetlago","SourceGetlagoGetlagoEnum","SourceGithub","SourceGithubCredentialsOAuth","SourceGithubCredentialsOAuthOptionTitleEnum","SourceGithubCredentialsPersonalAccessToken","SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum","SourceGithubGithubEnum","SourceGitlab","SourceGitlabCredentialsOAuth20","SourceGitlabCredentialsOAuth20AuthTypeEnum","SourceGitlabCredentialsPrivateToken","SourceGitlabCredentialsPrivateTokenAuthTypeEnum","SourceGitlabGitlabEnum","SourceGlassfrog","SourceGlassfrogGlassfrogEnum","SourceGnews","SourceGnewsCountryEnum","SourceGnewsGnewsEnum","SourceGnewsInEnum","SourceGnewsLanguageEnum","SourceGnewsNullableEnum","SourceGnewsSortByEnum","SourceGnewsTopHeadlinesTopicEnum","SourceGoogleAds","SourceGoogleAdsCustomQueries","SourceGoogleAdsGoogleAdsEnum","SourceGoogleAdsGoogleCredentials","SourceGoogleAnalyticsDataAPI","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum","SourceGoogleAnalyticsV4","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum","SourceGoogleDirectory","SourceGoogleDirectoryGoogleDirectoryEnum","SourceGoogleSearchConsole","SourceGoogleSearchConsoleAuthorizationOAuth","SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSearchConsoleGoogleSearchConsoleEnum","SourceGoogleSheets","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum","SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication","SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSheetsGoogleSheetsEnum","SourceGoogleWebfonts","SourceGoogleWebfontsGoogleWebfontsEnum","SourceGoogleWorkspaceAdminReports","SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum","SourceGreenhouse","SourceGreenhouseGreenhouseEnum","SourceGridly","SourceGridlyGridlyEnum","SourceHarvest","SourceHarvestHarvestEnum","SourceHubplanner","SourceHubplannerHubplannerEnum","SourceHubspot","SourceHubspotCredentialsOAuth","SourceHubspotCredentialsOAuthCredentialsEnum","SourceHubspotCredentialsPrivateApp","SourceHubspotCredentialsPrivateAppCredentialsEnum","SourceHubspotHubspotEnum","SourceInsightly","SourceInsightlyInsightlyEnum","SourceInstagram","SourceInstagramInstagramEnum","SourceInstatus","SourceInstatusInstatusEnum","SourceIntercom","SourceIntercomIntercomEnum","SourceIp2whois","SourceIp2whoisIp2whoisEnum","SourceIterable","SourceIterableIterableEnum","SourceJira","SourceJiraJiraEnum","SourceK6Cloud","SourceK6CloudK6CloudEnum","SourceKlarna","SourceKlarnaKlarnaEnum","SourceKlarnaRegionEnum","SourceKlaviyo","SourceKlaviyoKlaviyoEnum","SourceKustomerSinger","SourceKustomerSingerKustomerSingerEnum","SourceLaunchdarkly","SourceLaunchdarklyLaunchdarklyEnum","SourceLemlist","SourceLemlistLemlistEnum","SourceLinkedinAds","SourceLinkedinAdsCredentialsAccessToken","SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum","SourceLinkedinAdsCredentialsOAuth20","SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum","SourceLinkedinAdsLinkedinAdsEnum","SourceLinkedinPages","SourceLinkedinPagesCredentialsAccessToken","SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum","SourceLinkedinPagesCredentialsOAuth20","SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum","SourceLinkedinPagesLinkedinPagesEnum","SourceLinnworks","SourceLinnworksLinnworksEnum","SourceLokalise","SourceLokaliseLokaliseEnum","SourceMailchimp","SourceMailchimpCredentialsAPIKey","SourceMailchimpCredentialsAPIKeyAuthTypeEnum","SourceMailchimpCredentialsOAuth20","SourceMailchimpCredentialsOAuth20AuthTypeEnum","SourceMailchimpMailchimpEnum","SourceMailgun","SourceMailgunMailgunEnum","SourceMailjetSms","SourceMailjetSmsMailjetSmsEnum","SourceMarketo","SourceMarketoMarketoEnum","SourceMetabase","SourceMetabaseMetabaseEnum","SourceMicrosoftTeams","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum","SourceMicrosoftTeamsMicrosoftTeamsEnum","SourceMixpanel","SourceMixpanelCredentialsProjectSecret","SourceMixpanelCredentialsProjectSecretOptionTitleEnum","SourceMixpanelCredentialsServiceAccount","SourceMixpanelCredentialsServiceAccountOptionTitleEnum","SourceMixpanelMixpanelEnum","SourceMixpanelRegionEnum","SourceMonday","SourceMondayCredentialsAPIToken","SourceMondayCredentialsAPITokenAuthTypeEnum","SourceMondayCredentialsOAuth20","SourceMondayCredentialsOAuth20AuthTypeEnum","SourceMondayMondayEnum","SourceMongodb","SourceMongodbInstanceTypeMongoDBAtlas","SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum","SourceMongodbInstanceTypeReplicaSet","SourceMongodbInstanceTypeReplicaSetInstanceEnum","SourceMongodbInstanceTypeStandaloneMongoDbInstance","SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","SourceMongodbMongodbEnum","SourceMssql","SourceMssqlMssqlEnum","SourceMssqlReplicationMethodLogicalReplicationCDC","SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum","SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum","SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMssqlReplicationMethodStandard","SourceMssqlReplicationMethodStandardMethodEnum","SourceMssqlSslMethodEncryptedTrustServerCertificate","SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","SourceMssqlSslMethodEncryptedVerifyCertificate","SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","SourceMssqlTunnelMethodNoTunnel","SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMssqlTunnelMethodPasswordAuthentication","SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMssqlTunnelMethodSSHKeyAuthentication","SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceMyHours","SourceMyHoursMyHoursEnum","SourceMysql","SourceMysqlMysqlEnum","SourceMysqlReplicationMethodLogicalReplicationCDC","SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMysqlReplicationMethodStandard","SourceMysqlReplicationMethodStandardMethodEnum","SourceMysqlSslModePreferred","SourceMysqlSslModePreferredModeEnum","SourceMysqlSslModeRequired","SourceMysqlSslModeRequiredModeEnum","SourceMysqlSslModeVerifyCA","SourceMysqlSslModeVerifyCAModeEnum","SourceMysqlSslModeVerifyIdentity","SourceMysqlSslModeVerifyIdentityModeEnum","SourceMysqlTunnelMethodNoTunnel","SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMysqlTunnelMethodPasswordAuthentication","SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMysqlTunnelMethodSSHKeyAuthentication","SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceNetsuite","SourceNetsuiteNetsuiteEnum","SourceNotion","SourceNotionCredentialsAccessToken","SourceNotionCredentialsAccessTokenAuthTypeEnum","SourceNotionCredentialsOAuth20","SourceNotionCredentialsOAuth20AuthTypeEnum","SourceNotionNotionEnum","SourceNytimes","SourceNytimesNytimesEnum","SourceNytimesPeriodUsedForMostPopularStreamsEnum","SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum","SourceOkta","SourceOktaCredentialsAPIToken","SourceOktaCredentialsAPITokenAuthTypeEnum","SourceOktaCredentialsOAuth20","SourceOktaCredentialsOAuth20AuthTypeEnum","SourceOktaOktaEnum","SourceOmnisend","SourceOmnisendOmnisendEnum","SourceOnesignal","SourceOnesignalApplications","SourceOnesignalOnesignalEnum","SourceOpenweather","SourceOpenweatherLanguageEnum","SourceOpenweatherOpenweatherEnum","SourceOpenweatherUnitsEnum","SourceOracle","SourceOracleConnectionDataServiceName","SourceOracleConnectionDataServiceNameConnectionTypeEnum","SourceOracleConnectionDataSystemIDSID","SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum","SourceOracleEncryptionNativeNetworkEncryptionNNE","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum","SourceOracleEncryptionTLSEncryptedVerifyCertificate","SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum","SourceOracleOracleEnum","SourceOracleTunnelMethodNoTunnel","SourceOracleTunnelMethodNoTunnelTunnelMethodEnum","SourceOracleTunnelMethodPasswordAuthentication","SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceOracleTunnelMethodSSHKeyAuthentication","SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceOrb","SourceOrbOrbEnum","SourceOrbit","SourceOrbitOrbitEnum","SourceOutreach","SourceOutreachOutreachEnum","SourcePaypalTransaction","SourcePaypalTransactionPaypalTransactionEnum","SourcePaystack","SourcePaystackPaystackEnum","SourcePendo","SourcePendoPendoEnum","SourcePersistiq","SourcePersistiqPersistiqEnum","SourcePexelsAPI","SourcePexelsAPIPexelsAPIEnum","SourcePinterest","SourcePinterestCredentialsAccessToken","SourcePinterestCredentialsAccessTokenAuthMethodEnum","SourcePinterestCredentialsOAuth20","SourcePinterestCredentialsOAuth20AuthMethodEnum","SourcePinterestPinterestEnum","SourcePinterestStatusEnum","SourcePipedrive","SourcePipedriveAPIKeyAuthentication","SourcePipedriveAPIKeyAuthenticationAuthTypeEnum","SourcePipedrivePipedriveEnum","SourcePocket","SourcePocketContentTypeEnum","SourcePocketDetailTypeEnum","SourcePocketPocketEnum","SourcePocketSortByEnum","SourcePocketStateEnum","SourcePokeapi","SourcePokeapiPokeapiEnum","SourcePolygonStockAPI","SourcePolygonStockAPIPolygonStockAPIEnum","SourcePostgres","SourcePostgresPostgresEnum","SourcePostgresReplicationMethodStandard","SourcePostgresReplicationMethodStandardMethodEnum","SourcePostgresTunnelMethodNoTunnel","SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum","SourcePostgresTunnelMethodPasswordAuthentication","SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourcePostgresTunnelMethodSSHKeyAuthentication","SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourcePosthog","SourcePosthogPosthogEnum","SourcePostmarkapp","SourcePostmarkappPostmarkappEnum","SourcePrestashop","SourcePrestashopPrestashopEnum","SourcePublicApis","SourcePublicApisPublicApisEnum","SourcePunkAPI","SourcePunkAPIPunkAPIEnum","SourcePypi","SourcePypiPypiEnum","SourceQualaroo","SourceQualarooQualarooEnum","SourceQuickbooks","SourceQuickbooksCredentialsOAuth20","SourceQuickbooksCredentialsOAuth20AuthTypeEnum","SourceQuickbooksQuickbooksEnum","SourceRailz","SourceRailzRailzEnum","SourceRecharge","SourceRechargeRechargeEnum","SourceRecreation","SourceRecreationRecreationEnum","SourceRecruitee","SourceRecruiteeRecruiteeEnum","SourceRecurly","SourceRecurlyRecurlyEnum","SourceRedshift","SourceRedshiftRedshiftEnum","SourceResponse","SourceRetently","SourceRetentlyRetentlyEnum","SourceRkiCovid","SourceRkiCovidRkiCovidEnum","SourceRss","SourceRssRssEnum","SourceS3","SourceS3FormatAvro","SourceS3FormatAvroFiletypeEnum","SourceS3FormatCSV","SourceS3FormatCSVFiletypeEnum","SourceS3FormatJsonl","SourceS3FormatJsonlFiletypeEnum","SourceS3FormatJsonlUnexpectedFieldBehaviorEnum","SourceS3FormatParquet","SourceS3FormatParquetFiletypeEnum","SourceS3S3AmazonWebServices","SourceS3S3Enum","SourceSalesforce","SourceSalesforceAuthTypeEnum","SourceSalesforceSalesforceEnum","SourceSalesforceSinger","SourceSalesforceSingerAPITypeEnum","SourceSalesforceSingerSalesforceSingerEnum","SourceSalesforceStreamsCriteria","SourceSalesforceStreamsCriteriaSearchCriteriaEnum","SourceSalesloft","SourceSalesloftCredentialsAuthenticateViaAPIKey","SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum","SourceSalesloftCredentialsAuthenticateViaOAuth","SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum","SourceSalesloftSalesloftEnum","SourceSapFieldglass","SourceSapFieldglassSapFieldglassEnum","SourceSecoda","SourceSecodaSecodaEnum","SourceSendgrid","SourceSendgridSendgridEnum","SourceSendinblue","SourceSendinblueSendinblueEnum","SourceSenseforce","SourceSenseforceSenseforceEnum","SourceSentry","SourceSentrySentryEnum","SourceSftp","SourceSftpBulk","SourceSftpBulkFileTypeEnum","SourceSftpBulkSftpBulkEnum","SourceSftpCredentialsPasswordAuthentication","SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum","SourceSftpCredentialsSSHKeyAuthentication","SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum","SourceSftpSftpEnum","SourceShopify","SourceShopifyCredentialsAPIPassword","SourceShopifyCredentialsAPIPasswordAuthMethodEnum","SourceShopifyCredentialsOAuth20","SourceShopifyCredentialsOAuth20AuthMethodEnum","SourceShopifyShopifyEnum","SourceShortio","SourceShortioShortioEnum","SourceSlack","SourceSlackCredentialsAPIToken","SourceSlackCredentialsAPITokenOptionTitleEnum","SourceSlackCredentialsSignInViaSlackOAuth","SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum","SourceSlackSlackEnum","SourceSmaily","SourceSmailySmailyEnum","SourceSmartengage","SourceSmartengageSmartengageEnum","SourceSmartsheets","SourceSmartsheetsCredentialsAPIAccessToken","SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum","SourceSmartsheetsCredentialsOAuth20","SourceSmartsheetsCredentialsOAuth20AuthTypeEnum","SourceSmartsheetsSmartsheetsEnum","SourceSnapchatMarketing","SourceSnapchatMarketingSnapchatMarketingEnum","SourceSnowflake","SourceSnowflakeCredentialsOAuth20","SourceSnowflakeCredentialsOAuth20AuthTypeEnum","SourceSnowflakeCredentialsUsernameAndPassword","SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","SourceSnowflakeSnowflakeEnum","SourceSonarCloud","SourceSonarCloudSonarCloudEnum","SourceSpacexAPI","SourceSpacexAPISpacexAPIEnum","SourceSquare","SourceSquareCredentialsAPIKey","SourceSquareCredentialsAPIKeyCredentialsTitleEnum","SourceSquareCredentialsOauthAuthentication","SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum","SourceSquareSquareEnum","SourceStrava","SourceStravaAuthTypeEnum","SourceStravaStravaEnum","SourceStripe","SourceStripeStripeEnum","SourceSurveySparrow","SourceSurveySparrowRegionEUBasedAccount","SourceSurveySparrowRegionEUBasedAccountURLBaseEnum","SourceSurveySparrowRegionGlobalAccount","SourceSurveySparrowRegionGlobalAccountURLBaseEnum","SourceSurveySparrowSurveySparrowEnum","SourceSurveymonkey","SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum","SourceSurveymonkeySurveyMonkeyAuthorizationMethod","SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum","SourceSurveymonkeySurveymonkeyEnum","SourceTempo","SourceTempoTempoEnum","SourceTheGuardianAPI","SourceTheGuardianAPITheGuardianAPIEnum","SourceTiktokMarketing","SourceTiktokMarketingCredentialsOAuth20","SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum","SourceTiktokMarketingCredentialsSandboxAccessToken","SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum","SourceTiktokMarketingTiktokMarketingEnum","SourceTodoist","SourceTodoistTodoistEnum","SourceTrello","SourceTrelloTrelloEnum","SourceTrustpilot","SourceTrustpilotCredentialsAPIKey","SourceTrustpilotCredentialsAPIKeyAuthTypeEnum","SourceTrustpilotCredentialsOAuth20","SourceTrustpilotCredentialsOAuth20AuthTypeEnum","SourceTrustpilotTrustpilotEnum","SourceTvmazeSchedule","SourceTvmazeScheduleTvmazeScheduleEnum","SourceTwilio","SourceTwilioTaskrouter","SourceTwilioTaskrouterTwilioTaskrouterEnum","SourceTwilioTwilioEnum","SourceTwitter","SourceTwitterTwitterEnum","SourceTypeform","SourceTypeformTypeformEnum","SourceUsCensus","SourceUsCensusUsCensusEnum","SourceVantage","SourceVantageVantageEnum","SourceWebflow","SourceWebflowWebflowEnum","SourceWhiskyHunter","SourceWhiskyHunterWhiskyHunterEnum","SourceWikipediaPageviews","SourceWikipediaPageviewsWikipediaPageviewsEnum","SourceWoocommerce","SourceWoocommerceWoocommerceEnum","SourceXero","SourceXeroAuthenticateViaXeroOAuth","SourceXeroXeroEnum","SourceXkcd","SourceXkcdXkcdEnum","SourceYandexMetrica","SourceYandexMetricaYandexMetricaEnum","SourceYounium","SourceYouniumYouniumEnum","SourceYoutubeAnalytics","SourceYoutubeAnalyticsYoutubeAnalyticsEnum","SourceZendeskChat","SourceZendeskChatCredentialsAccessToken","SourceZendeskChatCredentialsAccessTokenCredentialsEnum","SourceZendeskChatCredentialsOAuth20","SourceZendeskChatCredentialsOAuth20CredentialsEnum","SourceZendeskChatZendeskChatEnum","SourceZendeskSunshine","SourceZendeskSunshineCredentialsAPIToken","SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum","SourceZendeskSunshineCredentialsOAuth20","SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum","SourceZendeskSunshineZendeskSunshineEnum","SourceZendeskSupport","SourceZendeskSupportZendeskSupportEnum","SourceZendeskTalk","SourceZendeskTalkZendeskTalkEnum","SourceZenloop","SourceZenloopZenloopEnum","SourceZohoCRMZohoCRMEditionEnum","SourceZohoCrm","SourceZohoCrmDataCenterLocationEnum","SourceZohoCrmEnvironmentEnum","SourceZohoCrmZohoCrmEnum","SourceZoom","SourceZoomZoomEnum","SourceZuora","SourceZuoraZuoraEnum","SourcesResponse","StreamConfiguration","StreamConfigurations","StreamProperties","WorkspaceCreateRequest","WorkspaceOAuthCredentialsRequest","WorkspaceOAuthCredentialsRequestActorTypeEnum","WorkspaceResponse","WorkspacesResponse"]
+__all__ = ["ActorTypeEnumEnum","ConnectionCreateRequest","ConnectionResponse","ConnectionScheduleCreate","ConnectionScheduleResponse","ConnectionStatusEnumEnum","ConnectionSyncModeEnumEnum","ConnectionsResponse","DestinationAmazonSqs","DestinationAmazonSqsAWSRegionEnum","DestinationAmazonSqsAmazonSqsEnum","DestinationAwsDatalake","DestinationAwsDatalakeAwsDatalakeEnum","DestinationAwsDatalakeChooseHowToPartitionDataEnum","DestinationAwsDatalakeCredentialsIAMRole","DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum","DestinationAwsDatalakeCredentialsIAMUser","DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum","DestinationAwsDatalakeFormatParquetColumnarStorage","DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum","DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum","DestinationAwsDatalakeS3BucketRegionEnum","DestinationAzureBlobStorage","DestinationAzureBlobStorageAzureBlobStorageEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValues","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationBigquery","DestinationBigqueryBigqueryEnum","DestinationBigqueryDatasetLocationEnum","DestinationBigqueryDenormalized","DestinationBigqueryDenormalizedBigqueryDenormalizedEnum","DestinationBigqueryDenormalizedDatasetLocationEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStaging","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum","DestinationBigqueryDenormalizedLoadingMethodStandardInserts","DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryLoadingMethodGCSStaging","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey","DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum","DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum","DestinationBigqueryLoadingMethodGCSStagingMethodEnum","DestinationBigqueryLoadingMethodStandardInserts","DestinationBigqueryLoadingMethodStandardInsertsMethodEnum","DestinationBigqueryTransformationQueryRunTypeEnum","DestinationCassandra","DestinationCassandraCassandraEnum","DestinationClickhouse","DestinationClickhouseClickhouseEnum","DestinationClickhouseTunnelMethodNoTunnel","DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum","DestinationClickhouseTunnelMethodPasswordAuthentication","DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationClickhouseTunnelMethodSSHKeyAuthentication","DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationConvex","DestinationConvexConvexEnum","DestinationCreateRequest","DestinationCumulio","DestinationCumulioCumulioEnum","DestinationDatabend","DestinationDatabendDatabendEnum","DestinationDatabricks","DestinationDatabricksDataSourceAmazonS3","DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum","DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum","DestinationDatabricksDataSourceAzureBlobStorage","DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum","DestinationDatabricksDataSourceRecommendedManagedTables","DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum","DestinationDatabricksDatabricksEnum","DestinationDynamodb","DestinationDynamodbDynamoDBRegionEnum","DestinationDynamodbDynamodbEnum","DestinationElasticsearch","DestinationElasticsearchAuthenticationMethodAPIKeySecret","DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum","DestinationElasticsearchAuthenticationMethodUsernamePassword","DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum","DestinationElasticsearchElasticsearchEnum","DestinationFirebolt","DestinationFireboltFireboltEnum","DestinationFireboltLoadingMethodExternalTableViaS3","DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum","DestinationFireboltLoadingMethodSQLInserts","DestinationFireboltLoadingMethodSQLInsertsMethodEnum","DestinationFirestore","DestinationFirestoreFirestoreEnum","DestinationGCSGCSBucketRegionEnum","DestinationGcs","DestinationGcsCredentialHMACKey","DestinationGcsCredentialHMACKeyCredentialTypeEnum","DestinationGcsFormatAvroApacheAvro","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2","DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate","DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression","DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy","DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecXz","DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard","DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationGcsFormatAvroApacheAvroFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValues","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP","DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSON","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationGcsFormatParquetColumnarStorage","DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum","DestinationGcsFormatParquetColumnarStorageFormatTypeEnum","DestinationGcsGcsEnum","DestinationGoogleSheets","DestinationGoogleSheetsAuthenticationViaGoogleOAuth","DestinationGoogleSheetsGoogleSheetsEnum","DestinationKeen","DestinationKeenKeenEnum","DestinationKinesis","DestinationKinesisKinesisEnum","DestinationMariadbColumnstore","DestinationMariadbColumnstoreMariadbColumnstoreEnum","DestinationMariadbColumnstoreTunnelMethodNoTunnel","DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication","DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication","DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMeilisearch","DestinationMeilisearchMeilisearchEnum","DestinationMongodb","DestinationMongodbAuthTypeLoginPassword","DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum","DestinationMongodbAuthTypeNone","DestinationMongodbAuthTypeNoneAuthorizationEnum","DestinationMongodbInstanceTypeMongoDBAtlas","DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum","DestinationMongodbInstanceTypeReplicaSet","DestinationMongodbInstanceTypeReplicaSetInstanceEnum","DestinationMongodbInstanceTypeStandaloneMongoDbInstance","DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","DestinationMongodbMongodbEnum","DestinationMongodbTunnelMethodNoTunnel","DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum","DestinationMongodbTunnelMethodPasswordAuthentication","DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMongodbTunnelMethodSSHKeyAuthentication","DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMssql","DestinationMssqlMssqlEnum","DestinationMssqlSslMethodEncryptedTrustServerCertificate","DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","DestinationMssqlSslMethodEncryptedVerifyCertificate","DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","DestinationMssqlTunnelMethodNoTunnel","DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMssqlTunnelMethodPasswordAuthentication","DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMssqlTunnelMethodSSHKeyAuthentication","DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationMysql","DestinationMysqlMysqlEnum","DestinationMysqlTunnelMethodNoTunnel","DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum","DestinationMysqlTunnelMethodPasswordAuthentication","DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationMysqlTunnelMethodSSHKeyAuthentication","DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationOracle","DestinationOracleOracleEnum","DestinationOracleTunnelMethodNoTunnel","DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum","DestinationOracleTunnelMethodPasswordAuthentication","DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationOracleTunnelMethodSSHKeyAuthentication","DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPostgres","DestinationPostgresPostgresEnum","DestinationPostgresSslModeAllow","DestinationPostgresSslModeAllowModeEnum","DestinationPostgresSslModeDisable","DestinationPostgresSslModeDisableModeEnum","DestinationPostgresSslModePrefer","DestinationPostgresSslModePreferModeEnum","DestinationPostgresSslModeRequire","DestinationPostgresSslModeRequireModeEnum","DestinationPostgresSslModeVerifyCa","DestinationPostgresSslModeVerifyCaModeEnum","DestinationPostgresSslModeVerifyFull","DestinationPostgresSslModeVerifyFullModeEnum","DestinationPostgresTunnelMethodNoTunnel","DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum","DestinationPostgresTunnelMethodPasswordAuthentication","DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationPostgresTunnelMethodSSHKeyAuthentication","DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationPubsub","DestinationPubsubPubsubEnum","DestinationPulsar","DestinationPulsarCompressionTypeEnum","DestinationPulsarPulsarEnum","DestinationPulsarTopicTypeEnum","DestinationRabbitmq","DestinationRabbitmqRabbitmqEnum","DestinationRedis","DestinationRedisCacheTypeEnum","DestinationRedisRedisEnum","DestinationRedisSslModeDisable","DestinationRedisSslModeDisableModeEnum","DestinationRedisSslModeVerifyFull","DestinationRedisSslModeVerifyFullModeEnum","DestinationRedisTunnelMethodNoTunnel","DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedisTunnelMethodPasswordAuthentication","DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedisTunnelMethodSSHKeyAuthentication","DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshift","DestinationRedshiftRedshiftEnum","DestinationRedshiftTunnelMethodNoTunnel","DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum","DestinationRedshiftTunnelMethodPasswordAuthentication","DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum","DestinationRedshiftTunnelMethodSSHKeyAuthentication","DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","DestinationRedshiftUploadingMethodS3Staging","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption","DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationRedshiftUploadingMethodS3StagingMethodEnum","DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum","DestinationRedshiftUploadingMethodStandard","DestinationRedshiftUploadingMethodStandardMethodEnum","DestinationResponse","DestinationRockset","DestinationRocksetRocksetEnum","DestinationS3","DestinationS3FormatAvroApacheAvro","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2","DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecDeflate","DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression","DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecSnappy","DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecXz","DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum","DestinationS3FormatAvroApacheAvroCompressionCodecZstandard","DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum","DestinationS3FormatAvroApacheAvroFormatTypeEnum","DestinationS3FormatCSVCommaSeparatedValues","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP","DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression","DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum","DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSON","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3FormatParquetColumnarStorage","DestinationS3FormatParquetColumnarStorageCompressionCodecEnum","DestinationS3FormatParquetColumnarStorageFormatTypeEnum","DestinationS3Glue","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum","DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","DestinationS3GlueS3BucketRegionEnum","DestinationS3GlueS3GlueEnum","DestinationS3GlueSerializationLibraryEnum","DestinationS3S3BucketRegionEnum","DestinationS3S3Enum","DestinationScylla","DestinationScyllaScyllaEnum","DestinationSftpJSON","DestinationSftpJSONSftpJSONEnum","DestinationSnowflake","DestinationSnowflakeCredentialsKeyPairAuthentication","DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum","DestinationSnowflakeCredentialsOAuth20","DestinationSnowflakeCredentialsOAuth20AuthTypeEnum","DestinationSnowflakeCredentialsUsernameAndPassword","DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","DestinationSnowflakeLoadingMethodAWSS3Staging","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption","DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum","DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum","DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum","DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging","DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum","DestinationSnowflakeLoadingMethodRecommendedInternalStaging","DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum","DestinationSnowflakeLoadingMethodSelectAnotherOption","DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum","DestinationSnowflakeSnowflakeEnum","DestinationTypesense","DestinationTypesenseTypesenseEnum","DestinationsResponse","GeographyEnumEnum","InitiateOauthRequest","JobCreateRequest","JobResponse","JobStatusEnumEnum","JobTypeEnumEnum","JobsResponse","NamespaceDefinitionEnumEnum","NonBreakingSchemaUpdatesBehaviorEnumEnum","ScheduleTypeEnumEnum","ScheduleTypeWithBasicEnumEnum","Security","SourceAircall","SourceAircallAircallEnum","SourceAirtable","SourceAirtableAirtableEnum","SourceAirtableCredentialsOAuth20","SourceAirtableCredentialsOAuth20AuthMethodEnum","SourceAirtableCredentialsPersonalAccessToken","SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum","SourceAlloydb","SourceAlloydbAlloydbEnum","SourceAlloydbReplicationMethodStandard","SourceAlloydbReplicationMethodStandardMethodEnum","SourceAlloydbTunnelMethodNoTunnel","SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum","SourceAlloydbTunnelMethodPasswordAuthentication","SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceAlloydbTunnelMethodSSHKeyAuthentication","SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceAmazonAds","SourceAmazonAdsAmazonAdsEnum","SourceAmazonAdsAuthTypeEnum","SourceAmazonAdsRegionEnum","SourceAmazonAdsReportRecordTypesEnum","SourceAmazonAdsStateFilterEnum","SourceAmazonSellerPartner","SourceAmazonSellerPartnerAWSEnvironmentEnum","SourceAmazonSellerPartnerAWSRegionEnum","SourceAmazonSellerPartnerAmazonSellerPartnerEnum","SourceAmazonSellerPartnerAuthTypeEnum","SourceAmazonSqs","SourceAmazonSqsAWSRegionEnum","SourceAmazonSqsAmazonSqsEnum","SourceAmplitude","SourceAmplitudeAmplitudeEnum","SourceAmplitudeDataRegionEnum","SourceApifyDataset","SourceApifyDatasetApifyDatasetEnum","SourceAsana","SourceAsanaAsanaEnum","SourceAsanaCredentialsAuthenticateViaAsanaOauth","SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum","SourceAsanaCredentialsAuthenticateWithPersonalAccessToken","SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum","SourceAuth0","SourceAuth0Auth0Enum","SourceAuth0CredentialsOAuth2AccessToken","SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum","SourceAuth0CredentialsOAuth2ConfidentialApplication","SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum","SourceAwsCloudtrail","SourceAwsCloudtrailAwsCloudtrailEnum","SourceAzureBlobStorage","SourceAzureBlobStorageAzureBlobStorageEnum","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON","SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum","SourceAzureTable","SourceAzureTableAzureTableEnum","SourceBambooHr","SourceBambooHrBambooHrEnum","SourceBigcommerce","SourceBigcommerceBigcommerceEnum","SourceBigquery","SourceBigqueryBigqueryEnum","SourceBingAds","SourceBingAdsAuthMethodEnum","SourceBingAdsBingAdsEnum","SourceBraintree","SourceBraintreeBraintreeEnum","SourceBraintreeEnvironmentEnum","SourceBraze","SourceBrazeBrazeEnum","SourceChargebee","SourceChargebeeChargebeeEnum","SourceChargebeeProductCatalogEnum","SourceChartmogul","SourceChartmogulChartmogulEnum","SourceChartmogulIntervalEnum","SourceClickhouse","SourceClickhouseClickhouseEnum","SourceClickhouseTunnelMethodNoTunnel","SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum","SourceClickhouseTunnelMethodPasswordAuthentication","SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceClickhouseTunnelMethodSSHKeyAuthentication","SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceClickupAPI","SourceClickupAPIClickupAPIEnum","SourceCloseCom","SourceCloseComCloseComEnum","SourceCoda","SourceCodaCodaEnum","SourceCoinAPI","SourceCoinAPICoinAPIEnum","SourceCoinAPIEnvironmentEnum","SourceCoinmarketcap","SourceCoinmarketcapCoinmarketcapEnum","SourceCoinmarketcapDataTypeEnum","SourceConfigcat","SourceConfigcatConfigcatEnum","SourceConfluence","SourceConfluenceConfluenceEnum","SourceCreateRequest","SourceDatascope","SourceDatascopeDatascopeEnum","SourceDelighted","SourceDelightedDelightedEnum","SourceDixa","SourceDixaDixaEnum","SourceDockerhub","SourceDockerhubDockerhubEnum","SourceDremio","SourceDremioDremioEnum","SourceDynamodb","SourceDynamodbDynamodbEnum","SourceDynamodbDynamodbRegionEnum","SourceE2eTestCloud","SourceE2eTestCloudE2eTestCloudEnum","SourceE2eTestCloudMockCatalogMultiSchema","SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum","SourceE2eTestCloudMockCatalogSingleSchema","SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum","SourceE2eTestCloudTypeEnum","SourceEmailoctopus","SourceEmailoctopusEmailoctopusEnum","SourceExchangeRates","SourceExchangeRatesExchangeRatesEnum","SourceFacebookMarketing","SourceFacebookMarketingFacebookMarketingEnum","SourceFacebookMarketingInsightConfig","SourceFacebookMarketingInsightConfigLevelEnum","SourceFacebookMarketingInsightConfigValidActionBreakdownsEnum","SourceFacebookMarketingInsightConfigValidBreakdownsEnum","SourceFacebookMarketingInsightConfigValidEnumsEnum","SourceFacebookPages","SourceFacebookPagesFacebookPagesEnum","SourceFaker","SourceFakerFakerEnum","SourceFauna","SourceFaunaCollection","SourceFaunaCollectionDeletionsDisabled","SourceFaunaCollectionDeletionsDisabledDeletionModeEnum","SourceFaunaCollectionDeletionsEnabled","SourceFaunaCollectionDeletionsEnabledDeletionModeEnum","SourceFaunaFaunaEnum","SourceFileSecure","SourceFileSecureFileFormatEnum","SourceFileSecureFileSecureEnum","SourceFileSecureProviderAzBlobAzureBlobStorage","SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum","SourceFileSecureProviderGCSGoogleCloudStorage","SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum","SourceFileSecureProviderHTTPSPublicWeb","SourceFileSecureProviderHTTPSPublicWebStorageEnum","SourceFileSecureProviderS3AmazonWebServices","SourceFileSecureProviderS3AmazonWebServicesStorageEnum","SourceFileSecureProviderSCPSecureCopyProtocol","SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum","SourceFileSecureProviderSFTPSecureFileTransferProtocol","SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum","SourceFileSecureProviderSSHSecureShell","SourceFileSecureProviderSSHSecureShellStorageEnum","SourceFirebolt","SourceFireboltFireboltEnum","SourceFreshcaller","SourceFreshcallerFreshcallerEnum","SourceFreshdesk","SourceFreshdeskFreshdeskEnum","SourceFreshsales","SourceFreshsalesFreshsalesEnum","SourceGcs","SourceGcsGcsEnum","SourceGetlago","SourceGetlagoGetlagoEnum","SourceGithub","SourceGithubCredentialsOAuth","SourceGithubCredentialsOAuthOptionTitleEnum","SourceGithubCredentialsPersonalAccessToken","SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum","SourceGithubGithubEnum","SourceGitlab","SourceGitlabCredentialsOAuth20","SourceGitlabCredentialsOAuth20AuthTypeEnum","SourceGitlabCredentialsPrivateToken","SourceGitlabCredentialsPrivateTokenAuthTypeEnum","SourceGitlabGitlabEnum","SourceGlassfrog","SourceGlassfrogGlassfrogEnum","SourceGnews","SourceGnewsCountryEnum","SourceGnewsGnewsEnum","SourceGnewsInEnum","SourceGnewsLanguageEnum","SourceGnewsNullableEnum","SourceGnewsSortByEnum","SourceGnewsTopHeadlinesTopicEnum","SourceGoogleAds","SourceGoogleAdsCustomQueries","SourceGoogleAdsGoogleAdsEnum","SourceGoogleAdsGoogleCredentials","SourceGoogleAnalyticsDataAPI","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum","SourceGoogleAnalyticsV4","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth","SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication","SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum","SourceGoogleDirectory","SourceGoogleDirectoryGoogleDirectoryEnum","SourceGoogleSearchConsole","SourceGoogleSearchConsoleAuthorizationOAuth","SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication","SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSearchConsoleGoogleSearchConsoleEnum","SourceGoogleSheets","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth","SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum","SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication","SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum","SourceGoogleSheetsGoogleSheetsEnum","SourceGoogleWebfonts","SourceGoogleWebfontsGoogleWebfontsEnum","SourceGoogleWorkspaceAdminReports","SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum","SourceGreenhouse","SourceGreenhouseGreenhouseEnum","SourceGridly","SourceGridlyGridlyEnum","SourceHarvest","SourceHarvestHarvestEnum","SourceHubplanner","SourceHubplannerHubplannerEnum","SourceHubspot","SourceHubspotCredentialsOAuth","SourceHubspotCredentialsOAuthCredentialsEnum","SourceHubspotCredentialsPrivateApp","SourceHubspotCredentialsPrivateAppCredentialsEnum","SourceHubspotHubspotEnum","SourceInsightly","SourceInsightlyInsightlyEnum","SourceInstagram","SourceInstagramInstagramEnum","SourceInstatus","SourceInstatusInstatusEnum","SourceIntercom","SourceIntercomIntercomEnum","SourceIp2whois","SourceIp2whoisIp2whoisEnum","SourceIterable","SourceIterableIterableEnum","SourceJira","SourceJiraJiraEnum","SourceK6Cloud","SourceK6CloudK6CloudEnum","SourceKlarna","SourceKlarnaKlarnaEnum","SourceKlarnaRegionEnum","SourceKlaviyo","SourceKlaviyoKlaviyoEnum","SourceKustomerSinger","SourceKustomerSingerKustomerSingerEnum","SourceLaunchdarkly","SourceLaunchdarklyLaunchdarklyEnum","SourceLemlist","SourceLemlistLemlistEnum","SourceLinkedinAds","SourceLinkedinAdsCredentialsAccessToken","SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum","SourceLinkedinAdsCredentialsOAuth20","SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum","SourceLinkedinAdsLinkedinAdsEnum","SourceLinkedinPages","SourceLinkedinPagesCredentialsAccessToken","SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum","SourceLinkedinPagesCredentialsOAuth20","SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum","SourceLinkedinPagesLinkedinPagesEnum","SourceLinnworks","SourceLinnworksLinnworksEnum","SourceLokalise","SourceLokaliseLokaliseEnum","SourceMailchimp","SourceMailchimpCredentialsAPIKey","SourceMailchimpCredentialsAPIKeyAuthTypeEnum","SourceMailchimpCredentialsOAuth20","SourceMailchimpCredentialsOAuth20AuthTypeEnum","SourceMailchimpMailchimpEnum","SourceMailgun","SourceMailgunMailgunEnum","SourceMailjetSms","SourceMailjetSmsMailjetSmsEnum","SourceMarketo","SourceMarketoMarketoEnum","SourceMetabase","SourceMetabaseMetabaseEnum","SourceMicrosoftTeams","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20","SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum","SourceMicrosoftTeamsMicrosoftTeamsEnum","SourceMixpanel","SourceMixpanelCredentialsProjectSecret","SourceMixpanelCredentialsProjectSecretOptionTitleEnum","SourceMixpanelCredentialsServiceAccount","SourceMixpanelCredentialsServiceAccountOptionTitleEnum","SourceMixpanelMixpanelEnum","SourceMixpanelRegionEnum","SourceMonday","SourceMondayCredentialsAPIToken","SourceMondayCredentialsAPITokenAuthTypeEnum","SourceMondayCredentialsOAuth20","SourceMondayCredentialsOAuth20AuthTypeEnum","SourceMondayMondayEnum","SourceMongodb","SourceMongodbInstanceTypeMongoDBAtlas","SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum","SourceMongodbInstanceTypeReplicaSet","SourceMongodbInstanceTypeReplicaSetInstanceEnum","SourceMongodbInstanceTypeStandaloneMongoDbInstance","SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum","SourceMongodbMongodbEnum","SourceMssql","SourceMssqlMssqlEnum","SourceMssqlReplicationMethodLogicalReplicationCDC","SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum","SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum","SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMssqlReplicationMethodStandard","SourceMssqlReplicationMethodStandardMethodEnum","SourceMssqlSslMethodEncryptedTrustServerCertificate","SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum","SourceMssqlSslMethodEncryptedVerifyCertificate","SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum","SourceMssqlTunnelMethodNoTunnel","SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMssqlTunnelMethodPasswordAuthentication","SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMssqlTunnelMethodSSHKeyAuthentication","SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceMyHours","SourceMyHoursMyHoursEnum","SourceMysql","SourceMysqlMysqlEnum","SourceMysqlReplicationMethodLogicalReplicationCDC","SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum","SourceMysqlReplicationMethodStandard","SourceMysqlReplicationMethodStandardMethodEnum","SourceMysqlSslModePreferred","SourceMysqlSslModePreferredModeEnum","SourceMysqlSslModeRequired","SourceMysqlSslModeRequiredModeEnum","SourceMysqlSslModeVerifyCA","SourceMysqlSslModeVerifyCAModeEnum","SourceMysqlSslModeVerifyIdentity","SourceMysqlSslModeVerifyIdentityModeEnum","SourceMysqlTunnelMethodNoTunnel","SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum","SourceMysqlTunnelMethodPasswordAuthentication","SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceMysqlTunnelMethodSSHKeyAuthentication","SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceNetsuite","SourceNetsuiteNetsuiteEnum","SourceNotion","SourceNotionCredentialsAccessToken","SourceNotionCredentialsAccessTokenAuthTypeEnum","SourceNotionCredentialsOAuth20","SourceNotionCredentialsOAuth20AuthTypeEnum","SourceNotionNotionEnum","SourceNytimes","SourceNytimesNytimesEnum","SourceNytimesPeriodUsedForMostPopularStreamsEnum","SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum","SourceOkta","SourceOktaCredentialsAPIToken","SourceOktaCredentialsAPITokenAuthTypeEnum","SourceOktaCredentialsOAuth20","SourceOktaCredentialsOAuth20AuthTypeEnum","SourceOktaOktaEnum","SourceOmnisend","SourceOmnisendOmnisendEnum","SourceOnesignal","SourceOnesignalApplications","SourceOnesignalOnesignalEnum","SourceOpenweather","SourceOpenweatherLanguageEnum","SourceOpenweatherOpenweatherEnum","SourceOpenweatherUnitsEnum","SourceOracle","SourceOracleConnectionDataServiceName","SourceOracleConnectionDataServiceNameConnectionTypeEnum","SourceOracleConnectionDataSystemIDSID","SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum","SourceOracleEncryptionNativeNetworkEncryptionNNE","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum","SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum","SourceOracleEncryptionTLSEncryptedVerifyCertificate","SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum","SourceOracleOracleEnum","SourceOracleTunnelMethodNoTunnel","SourceOracleTunnelMethodNoTunnelTunnelMethodEnum","SourceOracleTunnelMethodPasswordAuthentication","SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourceOracleTunnelMethodSSHKeyAuthentication","SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourceOrb","SourceOrbOrbEnum","SourceOrbit","SourceOrbitOrbitEnum","SourceOutreach","SourceOutreachOutreachEnum","SourcePaypalTransaction","SourcePaypalTransactionPaypalTransactionEnum","SourcePaystack","SourcePaystackPaystackEnum","SourcePendo","SourcePendoPendoEnum","SourcePersistiq","SourcePersistiqPersistiqEnum","SourcePexelsAPI","SourcePexelsAPIPexelsAPIEnum","SourcePinterest","SourcePinterestCredentialsAccessToken","SourcePinterestCredentialsAccessTokenAuthMethodEnum","SourcePinterestCredentialsOAuth20","SourcePinterestCredentialsOAuth20AuthMethodEnum","SourcePinterestPinterestEnum","SourcePinterestStatusEnum","SourcePipedrive","SourcePipedriveAPIKeyAuthentication","SourcePipedriveAPIKeyAuthenticationAuthTypeEnum","SourcePipedrivePipedriveEnum","SourcePocket","SourcePocketContentTypeEnum","SourcePocketDetailTypeEnum","SourcePocketPocketEnum","SourcePocketSortByEnum","SourcePocketStateEnum","SourcePokeapi","SourcePokeapiPokeapiEnum","SourcePolygonStockAPI","SourcePolygonStockAPIPolygonStockAPIEnum","SourcePostgres","SourcePostgresPostgresEnum","SourcePostgresReplicationMethodStandard","SourcePostgresReplicationMethodStandardMethodEnum","SourcePostgresTunnelMethodNoTunnel","SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum","SourcePostgresTunnelMethodPasswordAuthentication","SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum","SourcePostgresTunnelMethodSSHKeyAuthentication","SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum","SourcePosthog","SourcePosthogPosthogEnum","SourcePostmarkapp","SourcePostmarkappPostmarkappEnum","SourcePrestashop","SourcePrestashopPrestashopEnum","SourcePublicApis","SourcePublicApisPublicApisEnum","SourcePunkAPI","SourcePunkAPIPunkAPIEnum","SourcePypi","SourcePypiPypiEnum","SourceQualaroo","SourceQualarooQualarooEnum","SourceQuickbooks","SourceQuickbooksCredentialsOAuth20","SourceQuickbooksCredentialsOAuth20AuthTypeEnum","SourceQuickbooksQuickbooksEnum","SourceRailz","SourceRailzRailzEnum","SourceRecharge","SourceRechargeRechargeEnum","SourceRecreation","SourceRecreationRecreationEnum","SourceRecruitee","SourceRecruiteeRecruiteeEnum","SourceRecurly","SourceRecurlyRecurlyEnum","SourceRedshift","SourceRedshiftRedshiftEnum","SourceResponse","SourceRetently","SourceRetentlyRetentlyEnum","SourceRkiCovid","SourceRkiCovidRkiCovidEnum","SourceRss","SourceRssRssEnum","SourceS3","SourceS3FormatAvro","SourceS3FormatAvroFiletypeEnum","SourceS3FormatCSV","SourceS3FormatCSVFiletypeEnum","SourceS3FormatJsonl","SourceS3FormatJsonlFiletypeEnum","SourceS3FormatJsonlUnexpectedFieldBehaviorEnum","SourceS3FormatParquet","SourceS3FormatParquetFiletypeEnum","SourceS3S3AmazonWebServices","SourceS3S3Enum","SourceSalesforce","SourceSalesforceAuthTypeEnum","SourceSalesforceSalesforceEnum","SourceSalesforceSinger","SourceSalesforceSingerAPITypeEnum","SourceSalesforceSingerSalesforceSingerEnum","SourceSalesforceStreamsCriteria","SourceSalesforceStreamsCriteriaSearchCriteriaEnum","SourceSalesloft","SourceSalesloftCredentialsAuthenticateViaAPIKey","SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum","SourceSalesloftCredentialsAuthenticateViaOAuth","SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum","SourceSalesloftSalesloftEnum","SourceSapFieldglass","SourceSapFieldglassSapFieldglassEnum","SourceSecoda","SourceSecodaSecodaEnum","SourceSendgrid","SourceSendgridSendgridEnum","SourceSendinblue","SourceSendinblueSendinblueEnum","SourceSenseforce","SourceSenseforceSenseforceEnum","SourceSentry","SourceSentrySentryEnum","SourceSftp","SourceSftpBulk","SourceSftpBulkFileTypeEnum","SourceSftpBulkSftpBulkEnum","SourceSftpCredentialsPasswordAuthentication","SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum","SourceSftpCredentialsSSHKeyAuthentication","SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum","SourceSftpSftpEnum","SourceShopify","SourceShopifyCredentialsAPIPassword","SourceShopifyCredentialsAPIPasswordAuthMethodEnum","SourceShopifyCredentialsOAuth20","SourceShopifyCredentialsOAuth20AuthMethodEnum","SourceShopifyShopifyEnum","SourceShortio","SourceShortioShortioEnum","SourceSlack","SourceSlackCredentialsAPIToken","SourceSlackCredentialsAPITokenOptionTitleEnum","SourceSlackCredentialsSignInViaSlackOAuth","SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum","SourceSlackSlackEnum","SourceSmaily","SourceSmailySmailyEnum","SourceSmartengage","SourceSmartengageSmartengageEnum","SourceSmartsheets","SourceSmartsheetsCredentialsAPIAccessToken","SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum","SourceSmartsheetsCredentialsOAuth20","SourceSmartsheetsCredentialsOAuth20AuthTypeEnum","SourceSmartsheetsSmartsheetsEnum","SourceSnapchatMarketing","SourceSnapchatMarketingSnapchatMarketingEnum","SourceSnowflake","SourceSnowflakeCredentialsOAuth20","SourceSnowflakeCredentialsOAuth20AuthTypeEnum","SourceSnowflakeCredentialsUsernameAndPassword","SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum","SourceSnowflakeSnowflakeEnum","SourceSonarCloud","SourceSonarCloudSonarCloudEnum","SourceSpacexAPI","SourceSpacexAPISpacexAPIEnum","SourceSquare","SourceSquareCredentialsAPIKey","SourceSquareCredentialsAPIKeyAuthTypeEnum","SourceSquareCredentialsOauthAuthentication","SourceSquareCredentialsOauthAuthenticationAuthTypeEnum","SourceSquareSquareEnum","SourceStrava","SourceStravaAuthTypeEnum","SourceStravaStravaEnum","SourceStripe","SourceStripeStripeEnum","SourceSurveySparrow","SourceSurveySparrowRegionEUBasedAccount","SourceSurveySparrowRegionEUBasedAccountURLBaseEnum","SourceSurveySparrowRegionGlobalAccount","SourceSurveySparrowRegionGlobalAccountURLBaseEnum","SourceSurveySparrowSurveySparrowEnum","SourceSurveymonkey","SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum","SourceSurveymonkeySurveyMonkeyAuthorizationMethod","SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum","SourceSurveymonkeySurveymonkeyEnum","SourceTempo","SourceTempoTempoEnum","SourceTheGuardianAPI","SourceTheGuardianAPITheGuardianAPIEnum","SourceTiktokMarketing","SourceTiktokMarketingCredentialsOAuth20","SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum","SourceTiktokMarketingCredentialsSandboxAccessToken","SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum","SourceTiktokMarketingTiktokMarketingEnum","SourceTodoist","SourceTodoistTodoistEnum","SourceTrello","SourceTrelloTrelloEnum","SourceTrustpilot","SourceTrustpilotCredentialsAPIKey","SourceTrustpilotCredentialsAPIKeyAuthTypeEnum","SourceTrustpilotCredentialsOAuth20","SourceTrustpilotCredentialsOAuth20AuthTypeEnum","SourceTrustpilotTrustpilotEnum","SourceTvmazeSchedule","SourceTvmazeScheduleTvmazeScheduleEnum","SourceTwilio","SourceTwilioTaskrouter","SourceTwilioTaskrouterTwilioTaskrouterEnum","SourceTwilioTwilioEnum","SourceTwitter","SourceTwitterTwitterEnum","SourceTypeform","SourceTypeformTypeformEnum","SourceUsCensus","SourceUsCensusUsCensusEnum","SourceVantage","SourceVantageVantageEnum","SourceWebflow","SourceWebflowWebflowEnum","SourceWhiskyHunter","SourceWhiskyHunterWhiskyHunterEnum","SourceWikipediaPageviews","SourceWikipediaPageviewsWikipediaPageviewsEnum","SourceWoocommerce","SourceWoocommerceWoocommerceEnum","SourceXero","SourceXeroAuthenticateViaXeroOAuth","SourceXeroXeroEnum","SourceXkcd","SourceXkcdXkcdEnum","SourceYandexMetrica","SourceYandexMetricaYandexMetricaEnum","SourceYounium","SourceYouniumYouniumEnum","SourceYoutubeAnalytics","SourceYoutubeAnalyticsYoutubeAnalyticsEnum","SourceZendeskChat","SourceZendeskChatCredentialsAccessToken","SourceZendeskChatCredentialsAccessTokenCredentialsEnum","SourceZendeskChatCredentialsOAuth20","SourceZendeskChatCredentialsOAuth20CredentialsEnum","SourceZendeskChatZendeskChatEnum","SourceZendeskSunshine","SourceZendeskSunshineCredentialsAPIToken","SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum","SourceZendeskSunshineCredentialsOAuth20","SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum","SourceZendeskSunshineZendeskSunshineEnum","SourceZendeskSupport","SourceZendeskSupportZendeskSupportEnum","SourceZendeskTalk","SourceZendeskTalkZendeskTalkEnum","SourceZenloop","SourceZenloopZenloopEnum","SourceZohoCRMZohoCRMEditionEnum","SourceZohoCrm","SourceZohoCrmDataCenterLocationEnum","SourceZohoCrmEnvironmentEnum","SourceZohoCrmZohoCrmEnum","SourceZoom","SourceZoomZoomEnum","SourceZuora","SourceZuoraDataQueryTypeEnum","SourceZuoraTenantEndpointLocationEnum","SourceZuoraZuoraEnum","SourcesResponse","StreamConfiguration","StreamConfigurations","StreamProperties","WorkspaceCreateRequest","WorkspaceOAuthCredentialsRequest","WorkspaceResponse","WorkspaceUpdateRequest","WorkspacesResponse"]
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/connectioncreaterequest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/connectioncreaterequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import connectionschedulecreate as shared_connectionschedulecreate
 from ..shared import geographyenum_enum as shared_geographyenum_enum
+from ..shared import namespacedefinitionenum_enum as shared_namespacedefinitionenum_enum
+from ..shared import nonbreakingschemaupdatesbehaviorenum_enum as shared_nonbreakingschemaupdatesbehaviorenum_enum
 from ..shared import streamconfigurations as shared_streamconfigurations
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 
-class ConnectionCreateRequestNamespaceDefinitionEnum(str, Enum):
-    r"""Define the location where the data will be stored in the destination"""
-    SOURCE = 'source'
-    DESTINATION = 'destination'
-    CUSTOM_FORMAT = 'custom_format'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionCreateRequest:
     
     destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
     configurations: Optional[shared_streamconfigurations.StreamConfigurations] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configurations'), 'exclude': lambda f: f is None }})
     r"""A list of configured stream options for a connection."""
     data_residency: Optional[shared_geographyenum_enum.GeographyEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Optional name of the connection"""
-    namespace_definition: Optional[ConnectionCreateRequestNamespaceDefinitionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceDefinition'), 'exclude': lambda f: f is None }})
+    namespace_definition: Optional[shared_namespacedefinitionenum_enum.NamespaceDefinitionEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceDefinition'), 'exclude': lambda f: f is None }})
     r"""Define the location where the data will be stored in the destination"""
     namespace_format: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceFormat'), 'exclude': lambda f: f is None }})
     r"""Used when namespaceDefinition is 'custom_format'. If blank then behaves like namespaceDefinition = 'destination'. If \\"${SOURCE_NAMESPACE}\\" then behaves like namespaceDefinition = 'source'."""
+    non_breaking_schema_updates_behavior: Optional[shared_nonbreakingschemaupdatesbehaviorenum_enum.NonBreakingSchemaUpdatesBehaviorEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nonBreakingSchemaUpdatesBehavior'), 'exclude': lambda f: f is None }})
+    r"""Set how Airbyte handles syncs when it detects a non-breaking schema change in the source"""
     prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
     r"""Prefix that will be prepended to the name of each stream when it is written to the destination (ex. “airbyte_” causes “projects” => “airbyte_projects”)."""
     schedule: Optional[shared_connectionschedulecreate.ConnectionScheduleCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule'), 'exclude': lambda f: f is None }})
     r"""schedule for when the the connection should run, per the schedule type"""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/connectionresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_scylla.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import connectionscheduleresponse as shared_connectionscheduleresponse
-from ..shared import connectionstatusenum_enum as shared_connectionstatusenum_enum
-from ..shared import geographyenum_enum as shared_geographyenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
+from typing import Optional
+
+class DestinationScyllaScyllaEnum(str, Enum):
+    SCYLLA = 'scylla'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ConnectionResponse:
-    r"""Provides details of a single connection."""
+class DestinationScylla:
+    r"""The values required to configure the destination."""
     
-    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
-    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})
-    destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    schedule: shared_connectionscheduleresponse.ConnectionScheduleResponse = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule') }})
-    r"""schedule for when the the connection should run, per the schedule type"""
-    source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-    status: shared_connectionstatusenum_enum.ConnectionStatusEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
+    address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
+    r"""Address to connect to."""
+    destination_type: DestinationScyllaScyllaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
+    keyspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keyspace') }})
+    r"""Default Scylla keyspace to create data in."""
+    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
+    r"""Password associated with Scylla."""
+    port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
+    r"""Port of Scylla."""
+    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+    r"""Username to use to access Scylla."""
+    replication: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication'), 'exclude': lambda f: f is None }})
+    r"""Indicates to how many nodes the data should be replicated to."""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/connectionschedulecreate.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/connectionschedulecreate.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/connectionscheduleresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/connectionscheduleresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/connectionsresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/connectionsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_amazon_sqs.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_aws_datalake.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_aws_datalake.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_azure_blob_storage.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_bigquery.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     credential: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential') }})
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     gcs_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_name') }})
     r"""The name of the GCS bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/naming-buckets\\">here</a>."""
     gcs_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_path') }})
     r"""Directory under the GCS bucket where data will be written."""
     method: DestinationBigqueryLoadingMethodGCSStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
+    file_buffer_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_buffer_count'), 'exclude': lambda f: f is None }})
+    r"""Number of file buffers allocated for writing data. Increasing this number is beneficial for connections using Change Data Capture (CDC) and up to the number of streams within a connection. Increasing the number of file buffers past the maximum number of streams has deteriorating effects"""
     keep_files_in_gcs_bucket: Optional[DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keep_files_in_gcs-bucket'), 'exclude': lambda f: f is None }})
     r"""This upload method is supposed to temporary store records in GCS bucket. By this select you can chose if these records should be removed from GCS when migration has finished. The default \\"Delete all tmp files from GCS\\" value is used if not set explicitly."""
     
 class DestinationBigqueryLoadingMethodStandardInsertsMethodEnum(str, Enum):
     STANDARD = 'Standard'
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_bigquery_denormalized.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_bigquery_denormalized.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     credential: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential') }})
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     gcs_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_name') }})
     r"""The name of the GCS bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/naming-buckets\\">here</a>."""
     gcs_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_path') }})
     r"""Directory under the GCS bucket where data will be written. Read more <a href=\\"https://cloud.google.com/storage/docs/locations\\">here</a>."""
     method: DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
+    file_buffer_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_buffer_count'), 'exclude': lambda f: f is None }})
+    r"""Number of file buffers allocated for writing data. Increasing this number is beneficial for connections using Change Data Capture (CDC) and up to the number of streams within a connection. Increasing the number of file buffers past the maximum number of streams has deteriorating effects"""
     keep_files_in_gcs_bucket: Optional[DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keep_files_in_gcs-bucket'), 'exclude': lambda f: f is None }})
     r"""This upload method is supposed to temporary store records in GCS bucket. By this select you can chose if these records should be removed from GCS when migration has finished. The default \\"Delete all tmp files from GCS\\" value is used if not set explicitly."""
     
 class DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum(str, Enum):
     STANDARD = 'Standard'
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_cassandra.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_cassandra.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_clickhouse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_convex.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_convex.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_databend.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_databend.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_databricks.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_databricks.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_dynamodb.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_elasticsearch.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_firebolt.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_firestore.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_firestore.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_gcs.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_google_sheets.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_keen.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_keen.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_kinesis.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_kinesis.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_mariadb_columnstore.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_mariadb_columnstore.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_meilisearch.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_meilisearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_mongodb.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_mssql.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_mysql.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_oracle.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_postgres.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_pubsub.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_pubsub.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_pulsar.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_pulsar.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_rabbitmq.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_redis.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_redis.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_redshift.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_rockset.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_rockset.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_s3.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_s3_glue.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_s3_glue.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_scylla.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_my_hours.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class DestinationScyllaScyllaEnum(str, Enum):
-    SCYLLA = 'scylla'
+class SourceMyHoursMyHoursEnum(str, Enum):
+    MY_HOURS = 'my-hours'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DestinationScylla:
-    r"""The values required to configure the destination."""
+class SourceMyHours:
+    r"""The values required to configure the source."""
     
-    address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
-    r"""Address to connect to."""
-    destination_type: DestinationScyllaScyllaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-    keyspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keyspace') }})
-    r"""Default Scylla keyspace to create data in."""
+    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
+    r"""Your My Hours username"""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-    r"""Password associated with Scylla."""
-    port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-    r"""Port of Scylla."""
-    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-    r"""Username to use to access Scylla."""
-    replication: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication'), 'exclude': lambda f: f is None }})
-    r"""Indicates to how many nodes the data should be replicated to."""
+    r"""The password associated to the username"""
+    source_type: SourceMyHoursMyHoursEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""Start date for collecting time logs"""
+    logs_batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logs_batch_size'), 'exclude': lambda f: f is None }})
+    r"""Pagination size used for retrieving logs in days"""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_sftp_json.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_sftp_json.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_snowflake.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_snowflake.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,33 +50,14 @@
     r"""Enter your application's Client ID"""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
     r"""Enter your application's Client secret"""
     
 class DestinationSnowflakeSnowflakeEnum(str, Enum):
     SNOWFLAKE = 'snowflake'
 
-class DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum(str, Enum):
-    AZURE_BLOB_STAGING = 'Azure Blob Staging'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class DestinationSnowflakeLoadingMethodAzureBlobStorageStaging:
-    r"""Recommended for large production workloads for better speed and scalability."""
-    
-    azure_blob_storage_account_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_name') }})
-    r"""Enter your Azure Blob Storage account name"""
-    azure_blob_storage_container_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_container_name') }})
-    r"""Enter your Azure Blob Storage <a href=\\"https://docs.microsoft.com/en-us/rest/api/storageservices/naming-and-referencing-containers--blobs--and-metadata#container-names\\">container name</a>"""
-    azure_blob_storage_sas_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_sas_token') }})
-    r"""Enter the <a href=\\"https://docs.snowflake.com/en/user-guide/data-load-azure-config.html#option-2-generating-a-sas-token\\">Shared access signature</a> (SAS) token to grant Snowflake limited access to objects in your Azure Blob Storage account"""
-    method: DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-    azure_blob_storage_endpoint_domain_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_endpoint_domain_name'), 'exclude': lambda f: f is None }})
-    r"""Enter the Azure Blob Storage <a href=\\"https://docs.microsoft.com/en-us/azure/storage/common/storage-account-overview#storage-account-endpoints\\">endpoint domain name</a>"""
-    
 class DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum(str, Enum):
     GCS_STAGING = 'GCS Staging'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging:
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destination_typesense.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destination_typesense.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destinationcreaterequest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destinationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destinationresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destinationresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/destinationsresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pendo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import destinationresponse as shared_destinationresponse
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
+
+class SourcePendoPendoEnum(str, Enum):
+    PENDO = 'pendo'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DestinationsResponse:
-    r"""Successful operation"""
+class SourcePendo:
+    r"""The values required to configure the source."""
     
-    data: list[shared_destinationresponse.DestinationResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    next: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next') }})
-    previous: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous') }})
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    source_type: SourcePendoPendoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/initiateoauthrequest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/initiateoauthrequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/jobcreaterequest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/jobcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/jobresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/jobresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/jobsresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/workspaceresponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import jobresponse as shared_jobresponse
+from ..shared import geographyenum_enum as shared_geographyenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class JobsResponse:
-    r"""List all the Jobs by connectionId."""
+class WorkspaceResponse:
+    r"""Provides details of a single workspace."""
     
-    data: list[shared_jobresponse.JobResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    next: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next') }})
-    previous: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous') }})
+    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_airtable.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_airtable.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_alloydb.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_alloydb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_amazon_ads.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_amazon_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_amazon_seller_partner.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_amazon_seller_partner.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_amazon_sqs.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_amplitude.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_amplitude.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_apify_dataset.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_apify_dataset.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_asana.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_asana.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_auth0.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_auth0.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_aws_cloudtrail.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_aws_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_azure_blob_storage.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_azure_table.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_azure_table.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_bamboo_hr.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_bamboo_hr.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_bigcommerce.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_bigcommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_bigquery.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_bing_ads.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_shopify.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,56 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
-from typing import Optional
+from typing import Any, Optional
 
-class SourceBingAdsAuthMethodEnum(str, Enum):
+class SourceShopifyCredentialsOAuth20AuthMethodEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
-class SourceBingAdsBingAdsEnum(str, Enum):
-    BING_ADS = 'bing-ads'
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SourceShopifyCredentialsOAuth20:
+    r"""OAuth2.0"""
+    
+    auth_method: SourceShopifyCredentialsOAuth20AuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
+    r"""The Access Token for making authenticated requests."""
+    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
+    r"""The Client ID of the Shopify developer application."""
+    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
+    r"""The Client Secret of the Shopify developer application."""
+    
+class SourceShopifyCredentialsAPIPasswordAuthMethodEnum(str, Enum):
+    API_PASSWORD = 'api_password'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceBingAds:
+class SourceShopifyCredentialsAPIPassword:
+    r"""API Password Auth"""
+    
+    api_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_password') }})
+    r"""The API Password for your private application in the `Shopify` store."""
+    auth_method: SourceShopifyCredentialsAPIPasswordAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
+    
+class SourceShopifyShopifyEnum(str, Enum):
+    SHOPIFY = 'shopify'
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SourceShopify:
     r"""The values required to configure the source."""
     
-    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-    r"""The Client ID of your Microsoft Advertising developer application."""
-    developer_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('developer_token') }})
-    r"""Developer token associated with user. See more info <a href=\\"https://docs.microsoft.com/en-us/advertising/guides/get-started?view=bingads-13#get-developer-token\\"> in the docs</a>."""
-    refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-    r"""Refresh Token to renew the expired Access Token."""
-    reports_start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reports_start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-    r"""The start date from which to begin replicating report data. Any data generated before this date will not be replicated in reports. This is a UTC date in YYYY-MM-DD format."""
-    source_type: SourceBingAdsBingAdsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    auth_method: Optional[SourceBingAdsAuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-    r"""The Client Secret of your Microsoft Advertising developer application."""
-    tenant_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tenant_id'), 'exclude': lambda f: f is None }})
-    r"""The Tenant ID of your Microsoft Advertising developer application. Set this to \\"common\\" unless you know you need a different value."""
+    shop: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shop') }})
+    r"""The name of your Shopify store found in the URL. For example, if your URL was https://NAME.myshopify.com, then the name would be 'NAME'."""
+    source_type: SourceShopifyShopifyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
+    r"""The date you would like to replicate data from. Format: YYYY-MM-DD. Any data before this date will not be replicated."""
+    credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
+    r"""The authorization method to use to retrieve data from Shopify"""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_braintree.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_braintree.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_braze.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_braze.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_chargebee.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_chargebee.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_chartmogul.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_chartmogul.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_clickhouse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_clickup_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_clickup_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_close_com.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_close_com.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_coda.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_coda.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_coin_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_coin_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_coinmarketcap.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_configcat.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_configcat.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_confluence.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_confluence.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_datascope.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_datascope.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_delighted.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_delighted.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_dixa.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_dixa.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_dockerhub.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_dockerhub.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_dremio.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_dremio.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_dynamodb.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_e2e_test_cloud.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_e2e_test_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_emailoctopus.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_emailoctopus.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_exchange_rates.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_exchange_rates.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_facebook_marketing.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_facebook_marketing.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     source_type: SourceFacebookMarketingFacebookMarketingEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     r"""The date from which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
     action_breakdowns_allow_empty: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action_breakdowns_allow_empty'), 'exclude': lambda f: f is None }})
     r"""Allows action_breakdowns to be an empty list"""
     custom_insights: Optional[list[SourceFacebookMarketingInsightConfig]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_insights'), 'exclude': lambda f: f is None }})
     r"""A list which contains ad statistics entries, each entry must have a name and can contains fields, breakdowns or action_breakdowns. Click on \\"add\\" to fill this field."""
-    end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
+    end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     r"""The date until which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DDT00:00:00Z. All data generated between the start date and this end date will be replicated. Not setting this option will result in always syncing the latest data."""
     fetch_thumbnail_images: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fetch_thumbnail_images'), 'exclude': lambda f: f is None }})
     r"""Set to active if you want to fetch the thumbnail_url and store the result in thumbnail_data_url for each Ad Creative."""
     include_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_deleted'), 'exclude': lambda f: f is None }})
     r"""Set to active if you want to include data from deleted Campaigns, Ads, and AdSets."""
     insights_lookback_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('insights_lookback_window'), 'exclude': lambda f: f is None }})
     r"""The attribution window. Facebook freezes insight data 28 days after it was generated, which means that all data from the past 28 days may have changed since we last emitted it, so you can retrieve refreshed insights from the past by setting this parameter. If you set a custom lookback window value in Facebook account, please provide the same value here."""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_facebook_pages.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_facebook_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_faker.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_faker.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_fauna.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_fauna.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_file_secure.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_file_secure.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_firebolt.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_freshcaller.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_freshcaller.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_freshdesk.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_freshdesk.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_freshsales.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_freshsales.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_gcs.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_getlago.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_getlago.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_github.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_github.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_gitlab.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_gitlab.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_glassfrog.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_glassfrog.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_gnews.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_gnews.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_ads.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_analytics_data_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_analytics_data_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsDataAPI:
     r"""The values required to configure the source."""
     
     date_ranges_start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date_ranges_start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-    r"""The start date from which to replicate report data in the format YYYY-MM-DD. Data generated before this date will not be included in the report."""
+    r"""The start date from which to replicate report data in the format YYYY-MM-DD. Data generated before this date will not be included in the report. Not applied to custom Cohort reports."""
     property_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('property_id') }})
-    r"""A Google Analytics GA4 property identifier whose events are tracked. Specified in the URL path and not the body"""
+    r"""A Google Analytics GA4 property identifier whose events are tracked. Specified in the URL path and not the body such as \\"123...\\". See <a href=\\"https://developers.google.com/analytics/devguides/reporting/data/v1/property-id#what_is_my_property_id\\">the docs</a> for more details."""
     source_type: SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
     r"""Credentials for the service"""
     custom_reports: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_reports'), 'exclude': lambda f: f is None }})
     r"""A JSON array describing the custom reports you want to sync from Google Analytics. See <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4/#custom-reports\\">the docs</a> for more information about the exact format you can use to fill out this field."""
     window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-    r"""The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4/#sampling-in-reports\\">the docs</a>. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364."""
+    r"""The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4/#sampling-in-reports\\">the docs</a>. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364. Not applied to custom Cohort reports."""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_analytics_v4.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_analytics_v4.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_directory.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_directory.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_search_console.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_search_console.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_sheets.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_webfonts.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_webfonts.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_greenhouse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_greenhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_gridly.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_gridly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_harvest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_harvest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_hubplanner.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_hubplanner.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_hubspot.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_hubspot.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_insightly.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_insightly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_instagram.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_instagram.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_instatus.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_instatus.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_intercom.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_intercom.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_ip2whois.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_ip2whois.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_iterable.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_iterable.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_jira.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_jira.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_k6_cloud.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_k6_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_klarna.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_klarna.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_klaviyo.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_klaviyo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_kustomer_singer.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_kustomer_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_launchdarkly.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_launchdarkly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_lemlist.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_lemlist.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_linkedin_ads.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_linkedin_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_linkedin_pages.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_linkedin_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_linnworks.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_linnworks.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_lokalise.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_lokalise.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mailchimp.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mailchimp.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mailgun.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mailgun.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mailjet_sms.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mailjet_sms.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_marketo.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_marketo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_metabase.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_metabase.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_microsoft_teams.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mixpanel.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mixpanel.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_monday.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_monday.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mongodb.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mssql.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_my_hours.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_recreation.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,21 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class SourceMyHoursMyHoursEnum(str, Enum):
-    MY_HOURS = 'my-hours'
+class SourceRecreationRecreationEnum(str, Enum):
+    RECREATION = 'recreation'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceMyHours:
+class SourceRecreation:
     r"""The values required to configure the source."""
     
-    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-    r"""Your My Hours username"""
-    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-    r"""The password associated to the username"""
-    source_type: SourceMyHoursMyHoursEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""Start date for collecting time logs"""
-    logs_batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logs_batch_size'), 'exclude': lambda f: f is None }})
-    r"""Pagination size used for retrieving logs in days"""
+    apikey: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apikey') }})
+    r"""API Key"""
+    source_type: SourceRecreationRecreationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    query_campsites: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query_campsites'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_mysql.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_netsuite.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_netsuite.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_notion.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_notion.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_nytimes.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_nytimes.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_okta.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_okta.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_omnisend.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_omnisend.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_onesignal.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_onesignal.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_openweather.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_openweather.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_oracle.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_orb.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_orb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_orbit.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_orbit.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_outreach.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_outreach.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_paypal_transaction.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_paypal_transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Optional
 
 class SourcePaypalTransactionPaypalTransactionEnum(str, Enum):
     PAYPAL_TRANSACTION = 'paypal-transaction'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePaypalTransaction:
     r"""The values required to configure the source."""
     
     is_sandbox: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox') }})
     r"""Determines whether to use the sandbox or production environment."""
     source_type: SourcePaypalTransactionPaypalTransactionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     r"""Start Date for data extraction in <a href=\\"https://datatracker.ietf.org/doc/html/rfc3339#section-5.6\\">ISO format</a>. Date must be in range from 3 years till 12 hrs before present time."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
     r"""The Client ID of your Paypal developer application."""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
     r"""The Client Secret of your Paypal developer application."""
     refresh_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token'), 'exclude': lambda f: f is None }})
     r"""The key to refresh the expired access token."""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_paystack.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_paystack.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pendo.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zoom.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourcePendoPendoEnum(str, Enum):
-    PENDO = 'pendo'
+class SourceZoomZoomEnum(str, Enum):
+    ZOOM = 'zoom'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePendo:
+class SourceZoom:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-    source_type: SourcePendoPendoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    jwt_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jwt_token') }})
+    r"""JWT Token"""
+    source_type: SourceZoomZoomEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_persistiq.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_persistiq.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pexels_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pexels_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pinterest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pinterest.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePinterest:
     r"""The values required to configure the source."""
     
     source_type: SourcePinterestPinterestEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""A date in the format YYYY-MM-DD. If you have not set a date, it would be defaulted to latest allowed date by api (914 days from today)."""
+    r"""A date in the format YYYY-MM-DD. If you have not set a date, it would be defaulted to latest allowed date by api (89 days from today)."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
     status: Optional[list[SourcePinterestStatusEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""Entity statuses based off of campaigns, ad_groups, and ads. If you do not have a status set, it will be ignored completely."""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pipedrive.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pipedrive.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pocket.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pocket.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pokeapi.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pokeapi.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_polygon_stock_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_polygon_stock_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_postgres.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_posthog.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_posthog.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_postmarkapp.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_postmarkapp.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_prestashop.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_prestashop.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_public_apis.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_public_apis.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_punk_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_punk_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_pypi.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_pypi.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_qualaroo.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_qualaroo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_quickbooks.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_quickbooks.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_railz.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_railz.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_recharge.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_recharge.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_recreation.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_secoda.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from typing import Optional
 
-class SourceRecreationRecreationEnum(str, Enum):
-    RECREATION = 'recreation'
+class SourceSecodaSecodaEnum(str, Enum):
+    SECODA = 'secoda'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceRecreation:
+class SourceSecoda:
     r"""The values required to configure the source."""
     
-    apikey: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apikey') }})
-    r"""API Key"""
-    source_type: SourceRecreationRecreationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    query_campsites: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query_campsites'), 'exclude': lambda f: f is None }})
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    r"""Your API Access Key. See <a href=\\"https://docs.secoda.co/secoda-api/authentication\\">here</a>. The key is case sensitive."""
+    source_type: SourceSecodaSecodaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_recruitee.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_recruitee.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_recurly.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_recurly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_redshift.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_retently.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_retently.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_rki_covid.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_rki_covid.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_rss.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_rss.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_s3.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_salesforce.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_salesforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_salesforce_singer.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_salesforce_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_salesloft.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_salesloft.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sap_fieldglass.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sap_fieldglass.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_secoda.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/destinationsresponse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import destinationresponse as shared_destinationresponse
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-
-class SourceSecodaSecodaEnum(str, Enum):
-    SECODA = 'secoda'
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSecoda:
-    r"""The values required to configure the source."""
+class DestinationsResponse:
+    r"""Successful operation"""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-    r"""Your API Access Key. See <a href=\\"https://docs.secoda.co/secoda-api/authentication\\">here</a>. The key is case sensitive."""
-    source_type: SourceSecodaSecodaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    data: list[shared_destinationresponse.DestinationResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sendgrid.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sendgrid.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sendinblue.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sendinblue.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_senseforce.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_senseforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sentry.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sentry.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sftp.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sftp.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sftp_bulk.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sftp_bulk.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,8 +43,10 @@
     r"""The regular expression to specify files for sync in a chosen Folder Path"""
     file_type: Optional[SourceSftpBulkFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_type'), 'exclude': lambda f: f is None }})
     r"""The file type you want to sync. Currently only 'csv' and 'json' files are supported."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
     r"""OS-level password for logging into the jump server host"""
     private_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('private_key'), 'exclude': lambda f: f is None }})
     r"""The private key"""
+    separator: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('separator'), 'exclude': lambda f: f is None }})
+    r"""The separator used in the CSV files. Define None if you want to use the Sniffer functionality"""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_shopify.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zoho_crm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
-from typing import Any, Optional
+from marshmallow import fields
+from typing import Optional
 
-class SourceShopifyCredentialsOAuth20AuthMethodEnum(str, Enum):
-    OAUTH2_0 = 'oauth2.0'
+class SourceZohoCrmDataCenterLocationEnum(str, Enum):
+    r"""Please choose the region of your Data Center location. More info by this <a href=\\"https://www.zoho.com/crm/developer/docs/api/v2/multi-dc.html\\">Link</a>"""
+    US = 'US'
+    AU = 'AU'
+    EU = 'EU'
+    IN = 'IN'
+    CN = 'CN'
+    JP = 'JP'
+
+class SourceZohoCRMZohoCRMEditionEnum(str, Enum):
+    r"""Choose your Edition of Zoho CRM to determine API Concurrency Limits"""
+    FREE = 'Free'
+    STANDARD = 'Standard'
+    PROFESSIONAL = 'Professional'
+    ENTERPRISE = 'Enterprise'
+    ULTIMATE = 'Ultimate'
+
+class SourceZohoCrmEnvironmentEnum(str, Enum):
+    r"""Please choose the environment"""
+    PRODUCTION = 'Production'
+    DEVELOPER = 'Developer'
+    SANDBOX = 'Sandbox'
 
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SourceShopifyCredentialsOAuth20:
-    r"""OAuth2.0"""
-    
-    auth_method: SourceShopifyCredentialsOAuth20AuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-    r"""The Access Token for making authenticated requests."""
-    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-    r"""The Client ID of the Shopify developer application."""
-    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-    r"""The Client Secret of the Shopify developer application."""
-    
-class SourceShopifyCredentialsAPIPasswordAuthMethodEnum(str, Enum):
-    API_PASSWORD = 'api_password'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SourceShopifyCredentialsAPIPassword:
-    r"""API Password Auth"""
-    
-    api_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_password') }})
-    r"""The API Password for your private application in the `Shopify` store."""
-    auth_method: SourceShopifyCredentialsAPIPasswordAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-    
-class SourceShopifyShopifyEnum(str, Enum):
-    SHOPIFY = 'shopify'
+class SourceZohoCrmZohoCrmEnum(str, Enum):
+    ZOHO_CRM = 'zoho-crm'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceShopify:
+class SourceZohoCrm:
     r"""The values required to configure the source."""
     
-    shop: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shop') }})
-    r"""The name of your Shopify store found in the URL. For example, if your URL was https://NAME.myshopify.com, then the name would be 'NAME'."""
-    source_type: SourceShopifyShopifyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""The date you would like to replicate data from. Format: YYYY-MM-DD. Any data before this date will not be replicated."""
-    credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-    r"""The authorization method to use to retrieve data from Shopify"""
+    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
+    r"""OAuth2.0 Client ID"""
+    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
+    r"""OAuth2.0 Client Secret"""
+    dc_region: SourceZohoCrmDataCenterLocationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dc_region') }})
+    r"""Please choose the region of your Data Center location. More info by this <a href=\\"https://www.zoho.com/crm/developer/docs/api/v2/multi-dc.html\\">Link</a>"""
+    edition: SourceZohoCRMZohoCRMEditionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('edition') }})
+    r"""Choose your Edition of Zoho CRM to determine API Concurrency Limits"""
+    environment: SourceZohoCrmEnvironmentEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('environment') }})
+    r"""Please choose the environment"""
+    refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
+    r"""OAuth2.0 Refresh Token"""
+    source_type: SourceZohoCrmZohoCrmEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_datetime: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_datetime'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""ISO 8601, for instance: `YYYY-MM-DD`, `YYYY-MM-DD HH:MM:SS+HH:MM`"""
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_shortio.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_shortio.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_slack.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_slack.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_smaily.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_smaily.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_smartengage.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_smartengage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_smartsheets.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_smartsheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_snapchat_marketing.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_snapchat_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_snowflake.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_sonar_cloud.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_spacex_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_spacex_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_square.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_square.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
 from typing import Any, Optional
 
-class SourceSquareCredentialsAPIKeyCredentialsTitleEnum(str, Enum):
+class SourceSquareCredentialsAPIKeyAuthTypeEnum(str, Enum):
     API_KEY = 'API Key'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSquareCredentialsAPIKey:
     r"""Choose how to authenticate to Square."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
     r"""The API key for a Square application"""
-    credentials_title: Optional[SourceSquareCredentialsAPIKeyCredentialsTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title'), 'exclude': lambda f: f is None }})
+    auth_type: SourceSquareCredentialsAPIKeyAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
     
-class SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum(str, Enum):
-    O_AUTH_CREDENTIALS = 'OAuth Credentials'
+class SourceSquareCredentialsOauthAuthenticationAuthTypeEnum(str, Enum):
+    O_AUTH = 'OAuth'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSquareCredentialsOauthAuthentication:
     r"""Choose how to authenticate to Square."""
     
+    auth_type: SourceSquareCredentialsOauthAuthenticationAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
     r"""The Square-issued ID of your application"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
     r"""The Square-issued application secret for your application"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
     r"""A refresh token generated using the above client ID and secret"""
-    credentials_title: Optional[SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title'), 'exclude': lambda f: f is None }})
     
 class SourceSquareSquareEnum(str, Enum):
     SQUARE = 'square'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_strava.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_strava.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_stripe.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_stripe.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_survey_sparrow.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_survey_sparrow.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_surveymonkey.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_surveymonkey.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_tempo.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_tempo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_the_guardian_api.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_the_guardian_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_tiktok_marketing.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_tiktok_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_todoist.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_todoist.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_trello.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_trello.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_trustpilot.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_trustpilot.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_tvmaze_schedule.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_tvmaze_schedule.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_twilio.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_twilio.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_twilio_taskrouter.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_twilio_taskrouter.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_twitter.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_twitter.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_typeform.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_typeform.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_us_census.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_us_census.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_vantage.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_vantage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_webflow.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_webflow.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_whisky_hunter.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_whisky_hunter.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_wikipedia_pageviews.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_wikipedia_pageviews.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_woocommerce.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_woocommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_xero.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_xero.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_xkcd.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_xkcd.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_yandex_metrica.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_yandex_metrica.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_younium.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_younium.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_youtube_analytics.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_youtube_analytics.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_chat.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_chat.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_sunshine.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_sunshine.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_support.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_support.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zendesk_talk.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zendesk_talk.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zenloop.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/source_zenloop.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zoom.py` & `airbyte-api-0.7.0/src/airbyte/models/operations/deleteworkspace.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from airbyte import utils
-from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
+import requests as requests_http
+from typing import Optional
 
-class SourceZoomZoomEnum(str, Enum):
-    ZOOM = 'zoom'
 
+@dataclasses.dataclass
+class DeleteWorkspaceRequest:
+    
+    workspace_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'workspaceId', 'style': 'simple', 'explode': False }})
+    
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZoom:
-    r"""The values required to configure the source."""
+class DeleteWorkspaceResponse:
     
-    jwt_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jwt_token') }})
-    r"""JWT Token"""
-    source_type: SourceZoomZoomEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/source_zuora.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/streamproperties.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import connectionsyncmodeenum_enum as shared_connectionsyncmodeenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 
-class SourceZuoraZuoraEnum(str, Enum):
-    ZUORA = 'zuora'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZuora:
-    r"""The values required to configure the source."""
+class StreamProperties:
+    r"""The stream properties associated with a connection."""
     
-    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-    r"""Client ID"""
-    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-    r"""Client Secret"""
-    source_type: SourceZuoraZuoraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-    r"""Start Date in format: YYYY-MM-DD"""
-    is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
-    r"""Defines whether use the SANDBOX or PRODUCTION environment."""
-    window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-    r"""The amount of days for each data-chunk begining from start_date. Bigger the value - faster the fetch. (Min=1, as for a Day; Max=364, as for a Year)."""
+    default_cursor_field: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultCursorField'), 'exclude': lambda f: f is None }})
+    property_fields: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('propertyFields'), 'exclude': lambda f: f is None }})
+    source_defined_cursor_field: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedCursorField'), 'exclude': lambda f: f is None }})
+    source_defined_primary_key: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedPrimaryKey'), 'exclude': lambda f: f is None }})
+    stream_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamName'), 'exclude': lambda f: f is None }})
+    sync_modes: Optional[list[shared_connectionsyncmodeenum_enum.ConnectionSyncModeEnumEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncModes'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/sourcecreaterequest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/sourcecreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/sourceresponse.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/sourceresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/streamconfiguration.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/streamconfiguration.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/streamconfigurations.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/streamconfigurations.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/streamproperties.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/connectionresponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import connectionsyncmodeenum_enum as shared_connectionsyncmodeenum_enum
+from ..shared import connectionscheduleresponse as shared_connectionscheduleresponse
+from ..shared import connectionstatusenum_enum as shared_connectionstatusenum_enum
+from ..shared import geographyenum_enum as shared_geographyenum_enum
+from ..shared import namespacedefinitionenum_enum as shared_namespacedefinitionenum_enum
+from ..shared import nonbreakingschemaupdatesbehaviorenum_enum as shared_nonbreakingschemaupdatesbehaviorenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class StreamProperties:
-    r"""The stream properties associated with a connection."""
+class ConnectionResponse:
+    r"""Provides details of a single connection."""
     
-    default_cursor_field: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultCursorField'), 'exclude': lambda f: f is None }})
-    property_fields: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('propertyFields'), 'exclude': lambda f: f is None }})
-    source_defined_cursor_field: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedCursorField'), 'exclude': lambda f: f is None }})
-    source_defined_primary_key: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedPrimaryKey'), 'exclude': lambda f: f is None }})
-    stream_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamName'), 'exclude': lambda f: f is None }})
-    sync_modes: Optional[list[shared_connectionsyncmodeenum_enum.ConnectionSyncModeEnumEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncModes'), 'exclude': lambda f: f is None }})
+    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
+    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})
+    destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    schedule: shared_connectionscheduleresponse.ConnectionScheduleResponse = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule') }})
+    r"""schedule for when the the connection should run, per the schedule type"""
+    source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
+    status: shared_connectionstatusenum_enum.ConnectionStatusEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
+    namespace_definition: Optional[shared_namespacedefinitionenum_enum.NamespaceDefinitionEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceDefinition'), 'exclude': lambda f: f is None }})
+    r"""Define the location where the data will be stored in the destination"""
+    namespace_format: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceFormat'), 'exclude': lambda f: f is None }})
+    non_breaking_schema_updates_behavior: Optional[shared_nonbreakingschemaupdatesbehaviorenum_enum.NonBreakingSchemaUpdatesBehaviorEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nonBreakingSchemaUpdatesBehavior'), 'exclude': lambda f: f is None }})
+    r"""Set how Airbyte handles syncs when it detects a non-breaking schema change in the source"""
+    prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py` & `airbyte-api-0.7.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import actortypeenum_enum as shared_actortypeenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Any
 
-class WorkspaceOAuthCredentialsRequestActorTypeEnum(str, Enum):
-    r"""Whether you're setting this override for a source or destination"""
-    SOURCE = 'source'
-    DESTINATION = 'destination'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WorkspaceOAuthCredentialsRequest:
     r"""POST body for creating/updating workspace level OAuth credentials"""
     
-    actor_type: WorkspaceOAuthCredentialsRequestActorTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('actorType') }})
+    actor_type: shared_actortypeenum_enum.ActorTypeEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('actorType') }})
     r"""Whether you're setting this override for a source or destination"""
     configuration: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configuration') }})
     r"""The configuration for this source/destination based on the OAuth section of the relevant specification."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
```

### Comparing `airbyte-api-0.6.0/src/airbyte/sdk.py` & `airbyte-api-0.7.0/src/airbyte/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     streams: Streams
     workspaces: Workspaces
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.6.0"
-    _gen_version: str = "2.28.0"
+    _sdk_version: str = "0.7.0"
+    _gen_version: str = "2.29.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `airbyte-api-0.6.0/src/airbyte/sources.py` & `airbyte-api-0.7.0/src/airbyte/sources.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/streams.py` & `airbyte-api-0.7.0/src/airbyte/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/utils/retries.py` & `airbyte-api-0.7.0/src/airbyte/utils/retries.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/utils/utils.py` & `airbyte-api-0.7.0/src/airbyte/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.6.0/src/airbyte/workspaces.py` & `airbyte-api-0.7.0/src/airbyte/workspaces.py`

 * *Files 19% similar despite different names*

```diff
@@ -77,14 +77,34 @@
                 res.workspace_response = out
         elif http_res.status_code in [400, 403]:
             pass
 
         return res
 
     
+    def delete_workspace(self, request: operations.DeleteWorkspaceRequest) -> operations.DeleteWorkspaceResponse:
+        r"""Delete a Workspace"""
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.DeleteWorkspaceRequest, base_url, '/workspaces/{workspaceId}', request)
+        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        client = self._security_client
+        
+        http_res = client.request('DELETE', url, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.DeleteWorkspaceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+
+        return res
+
+    
     def get_workspace(self, request: operations.GetWorkspaceRequest) -> operations.GetWorkspaceResponse:
         r"""Get Workspace details"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetWorkspaceRequest, base_url, '/workspaces/{workspaceId}', request)
         
         headers = {}
@@ -129,8 +149,39 @@
                 out = utils.unmarshal_json(http_res.text, Optional[shared.WorkspacesResponse])
                 res.workspaces_response = out
         elif http_res.status_code in [403, 404]:
             pass
 
         return res
 
+    
+    def update_workspace(self, request: operations.UpdateWorkspaceRequest) -> operations.UpdateWorkspaceResponse:
+        r"""Update a workspace"""
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.UpdateWorkspaceRequest, base_url, '/workspaces/{workspaceId}', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "workspace_update_request", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        client = self._security_client
+        
+        http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.UpdateWorkspaceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.WorkspaceResponse])
+                res.workspace_response = out
+        elif http_res.status_code in [400, 403]:
+            pass
+
+        return res
+
```

### Comparing `airbyte-api-0.6.0/src/airbyte_api.egg-info/PKG-INFO` & `airbyte-api-0.7.0/src/airbyte_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Airbyte
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -107,22 +107,23 @@
                 sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
             ),
         ],
     ),
     data_residency=shared.GeographyEnumEnum.EU,
     destination_id='c816742c-b739-4205-9293-96fea7596eb1',
     name='Lela Orn',
-    namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
+    namespace_definition=shared.NamespaceDefinitionEnumEnum.SOURCE,
     namespace_format='${SOURCE_NAMESPACE}',
-    prefix='dolorem',
+    non_breaking_schema_updates_behavior=shared.NonBreakingSchemaUpdatesBehaviorEnumEnum.IGNORE,
+    prefix='corporis',
     schedule=shared.ConnectionScheduleCreate(
-        cron_expression='corporis',
-        schedule_type=shared.ScheduleTypeEnumEnum.MANUAL,
+        cron_expression='explicabo',
+        schedule_type=shared.ScheduleTypeEnumEnum.CRON,
     ),
-    source_id='c5955907-aff1-4a3a-afa9-467739251aa5',
+    source_id='5955907a-ff1a-43a2-ba94-67739251aa52',
 )
 
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
@@ -165,16 +166,18 @@
 
 * [get_stream_properties](docs/streams/README.md#get_stream_properties) - Get stream properties
 
 ### [workspaces](docs/workspaces/README.md)
 
 * [create_or_update_workspace_o_auth_credentials](docs/workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create OAuth override credentials for a workspace and source type.
 * [create_workspace](docs/workspaces/README.md#create_workspace) - Create a workspace
+* [delete_workspace](docs/workspaces/README.md#delete_workspace) - Delete a Workspace
 * [get_workspace](docs/workspaces/README.md#get_workspace) - Get Workspace details
 * [list_workspaces](docs/workspaces/README.md#list_workspaces) - List workspaces
+* [update_workspace](docs/workspaces/README.md#update_workspace) - Update a workspace
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airbyte-api Version: 0.6.0 Summary: Python Client
+Metadata-Version: 2.1 Name: airbyte-api Version: 0.7.0 Summary: Python Client
 SDK for Airbyte API Home-page: UNKNOWN Author: Airbyte License: UNKNOWN
 Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE.md
  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
                           4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
@@ -32,53 +32,56 @@
 Bernier MD', primary_key=[ [ 'repellendus', 'sapiente', ], ],
 sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_DEDUPED_HISTORY, ),
 shared.StreamConfiguration( cursor_field=[ 'at', ], name='Emilio Krajcik',
 primary_key=[ [ 'porro', 'dolorum', 'dicta', ], [ 'officia', 'occaecati',
 'fugit', ], ], sync_mode=shared.ConnectionSyncModeEnumEnum.INCREMENTAL_APPEND,
 ), ], ), data_residency=shared.GeographyEnumEnum.EU, destination_id='c816742c-
 b739-4205-9293-96fea7596eb1', name='Lela Orn',
-namespace_definition=shared.ConnectionCreateRequestNamespaceDefinitionEnum.SOURCE,
-namespace_format='${SOURCE_NAMESPACE}', prefix='dolorem',
-schedule=shared.ConnectionScheduleCreate( cron_expression='corporis',
-schedule_type=shared.ScheduleTypeEnumEnum.MANUAL, ), source_id='c5955907-aff1-
-4a3a-afa9-467739251aa5', ) res = s.connections.create_connection(req) if
-res.connection_response is not None: # handle response ```   ## Available
-Resources and Operations ### [connections](docs/connections/README.md) *
-[create_connection](docs/connections/README.md#create_connection) - Create a
-connection * [delete_connection](docs/connections/README.md#delete_connection)
-- Delete a Connection * [get_connection](docs/connections/
-README.md#get_connection) - Get Connection details * [list_connections](docs/
-connections/README.md#list_connections) - List connections ### [destinations]
-(docs/destinations/README.md) * [create_destination](docs/destinations/
-README.md#create_destination) - Create a destination * [delete_destination]
-(docs/destinations/README.md#delete_destination) - Delete a Destination *
-[get_destination](docs/destinations/README.md#get_destination) - Get
-Destination details * [list_destinations](docs/destinations/
-README.md#list_destinations) - List destinations ### [jobs](docs/jobs/
-README.md) * [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running
-Job * [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset
-job of a connection * [get_job](docs/jobs/README.md#get_job) - Get Job status
-and details * [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync
-type ### [sources](docs/sources/README.md) * [create_source](docs/sources/
-README.md#create_source) - Create a source * [delete_source](docs/sources/
-README.md#delete_source) - Delete a Source * [get_source](docs/sources/
-README.md#get_source) - Get Source details * [initiate_o_auth](docs/sources/
-README.md#initiate_o_auth) - Initiate OAuth for a source * [list_sources](docs/
-sources/README.md#list_sources) - List sources ### [streams](docs/streams/
-README.md) * [get_stream_properties](docs/streams/
+namespace_definition=shared.NamespaceDefinitionEnumEnum.SOURCE,
+namespace_format='${SOURCE_NAMESPACE}',
+non_breaking_schema_updates_behavior=shared.NonBreakingSchemaUpdatesBehaviorEnumEnum.IGNORE,
+prefix='corporis', schedule=shared.ConnectionScheduleCreate
+( cron_expression='explicabo', schedule_type=shared.ScheduleTypeEnumEnum.CRON,
+), source_id='5955907a-ff1a-43a2-ba94-67739251aa52', ) res =
+s.connections.create_connection(req) if res.connection_response is not None: #
+handle response ```   ## Available Resources and Operations ### [connections]
+(docs/connections/README.md) * [create_connection](docs/connections/
+README.md#create_connection) - Create a connection * [delete_connection](docs/
+connections/README.md#delete_connection) - Delete a Connection *
+[get_connection](docs/connections/README.md#get_connection) - Get Connection
+details * [list_connections](docs/connections/README.md#list_connections) -
+List connections ### [destinations](docs/destinations/README.md) *
+[create_destination](docs/destinations/README.md#create_destination) - Create a
+destination * [delete_destination](docs/destinations/
+README.md#delete_destination) - Delete a Destination * [get_destination](docs/
+destinations/README.md#get_destination) - Get Destination details *
+[list_destinations](docs/destinations/README.md#list_destinations) - List
+destinations ### [jobs](docs/jobs/README.md) * [cancel_job](docs/jobs/
+README.md#cancel_job) - Cancel a running Job * [create_job](docs/jobs/
+README.md#create_job) - Trigger a sync or reset job of a connection * [get_job]
+(docs/jobs/README.md#get_job) - Get Job status and details * [list_jobs](docs/
+jobs/README.md#list_jobs) - List Jobs by sync type ### [sources](docs/sources/
+README.md) * [create_source](docs/sources/README.md#create_source) - Create a
+source * [delete_source](docs/sources/README.md#delete_source) - Delete a
+Source * [get_source](docs/sources/README.md#get_source) - Get Source details *
+[initiate_o_auth](docs/sources/README.md#initiate_o_auth) - Initiate OAuth for
+a source * [list_sources](docs/sources/README.md#list_sources) - List sources
+### [streams](docs/streams/README.md) * [get_stream_properties](docs/streams/
 README.md#get_stream_properties) - Get stream properties ### [workspaces](docs/
 workspaces/README.md) * [create_or_update_workspace_o_auth_credentials](docs/
 workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create
 OAuth override credentials for a workspace and source type. *
 [create_workspace](docs/workspaces/README.md#create_workspace) - Create a
-workspace * [get_workspace](docs/workspaces/README.md#get_workspace) - Get
-Workspace details * [list_workspaces](docs/workspaces/
-README.md#list_workspaces) - List workspaces  ### Maturity This SDK is in beta,
-and there may be breaking changes between versions without a major version
-update. Therefore, we recommend pinning usage to a specific package version.
-This way, you can install the same version each time without breaking changes
-unless you are intentionally looking for the latest version. ### Contributions
-While we value open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release ! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+workspace * [delete_workspace](docs/workspaces/README.md#delete_workspace) -
+Delete a Workspace * [get_workspace](docs/workspaces/README.md#get_workspace) -
+Get Workspace details * [list_workspaces](docs/workspaces/
+README.md#list_workspaces) - List workspaces * [update_workspace](docs/
+workspaces/README.md#update_workspace) - Update a workspace  ### Maturity This
+SDK is in beta, and there may be breaking changes between versions without a
+major version update. Therefore, we recommend pinning usage to a specific
+package version. This way, you can install the same version each time without
+breaking changes unless you are intentionally looking for the latest version.
+### Contributions While we value open-source contributions to this SDK, this
+library is generated programmatically. Feel free to open a PR or a Github issue
+as a proof of concept and we'll do our best to include it in a future release !
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
+speakeasy/client-sdks)
```

### Comparing `airbyte-api-0.6.0/src/airbyte_api.egg-info/SOURCES.txt` & `airbyte-api-0.7.0/src/airbyte_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 src/airbyte/models/operations/createjob.py
 src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py
 src/airbyte/models/operations/createsource.py
 src/airbyte/models/operations/createworkspace.py
 src/airbyte/models/operations/deleteconnection.py
 src/airbyte/models/operations/deletedestination.py
 src/airbyte/models/operations/deletesource.py
+src/airbyte/models/operations/deleteworkspace.py
 src/airbyte/models/operations/getconnection.py
 src/airbyte/models/operations/getdestination.py
 src/airbyte/models/operations/getjob.py
 src/airbyte/models/operations/getsource.py
 src/airbyte/models/operations/getstreamproperties.py
 src/airbyte/models/operations/getworkspace.py
 src/airbyte/models/operations/initiateoauth.py
 src/airbyte/models/operations/listconnections.py
 src/airbyte/models/operations/listdestinations.py
 src/airbyte/models/operations/listjobs.py
 src/airbyte/models/operations/listsources.py
 src/airbyte/models/operations/listworkspaces.py
+src/airbyte/models/operations/updateworkspace.py
 src/airbyte/models/shared/__init__.py
+src/airbyte/models/shared/actortypeenum_enum.py
 src/airbyte/models/shared/connectioncreaterequest.py
 src/airbyte/models/shared/connectionresponse.py
 src/airbyte/models/shared/connectionschedulecreate.py
 src/airbyte/models/shared/connectionscheduleresponse.py
 src/airbyte/models/shared/connectionsresponse.py
 src/airbyte/models/shared/connectionstatusenum_enum.py
 src/airbyte/models/shared/connectionsyncmodeenum_enum.py
@@ -45,14 +48,15 @@
 src/airbyte/models/shared/destination_aws_datalake.py
 src/airbyte/models/shared/destination_azure_blob_storage.py
 src/airbyte/models/shared/destination_bigquery.py
 src/airbyte/models/shared/destination_bigquery_denormalized.py
 src/airbyte/models/shared/destination_cassandra.py
 src/airbyte/models/shared/destination_clickhouse.py
 src/airbyte/models/shared/destination_convex.py
+src/airbyte/models/shared/destination_cumulio.py
 src/airbyte/models/shared/destination_databend.py
 src/airbyte/models/shared/destination_databricks.py
 src/airbyte/models/shared/destination_dynamodb.py
 src/airbyte/models/shared/destination_elasticsearch.py
 src/airbyte/models/shared/destination_firebolt.py
 src/airbyte/models/shared/destination_firestore.py
 src/airbyte/models/shared/destination_gcs.py
@@ -84,17 +88,20 @@
 src/airbyte/models/shared/geographyenum_enum.py
 src/airbyte/models/shared/initiateoauthrequest.py
 src/airbyte/models/shared/jobcreaterequest.py
 src/airbyte/models/shared/jobresponse.py
 src/airbyte/models/shared/jobsresponse.py
 src/airbyte/models/shared/jobstatusenum_enum.py
 src/airbyte/models/shared/jobtypeenum_enum.py
+src/airbyte/models/shared/namespacedefinitionenum_enum.py
+src/airbyte/models/shared/nonbreakingschemaupdatesbehaviorenum_enum.py
 src/airbyte/models/shared/scheduletypeenum_enum.py
 src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
 src/airbyte/models/shared/security.py
+src/airbyte/models/shared/source_aircall.py
 src/airbyte/models/shared/source_airtable.py
 src/airbyte/models/shared/source_alloydb.py
 src/airbyte/models/shared/source_amazon_ads.py
 src/airbyte/models/shared/source_amazon_seller_partner.py
 src/airbyte/models/shared/source_amazon_sqs.py
 src/airbyte/models/shared/source_amplitude.py
 src/airbyte/models/shared/source_apify_dataset.py
@@ -287,14 +294,15 @@
 src/airbyte/models/shared/streamconfiguration.py
 src/airbyte/models/shared/streamconfigurations.py
 src/airbyte/models/shared/streamproperties.py
 src/airbyte/models/shared/workspacecreaterequest.py
 src/airbyte/models/shared/workspaceoauthcredentialsrequest.py
 src/airbyte/models/shared/workspaceresponse.py
 src/airbyte/models/shared/workspacesresponse.py
+src/airbyte/models/shared/workspaceupdaterequest.py
 src/airbyte/utils/__init__.py
 src/airbyte/utils/retries.py
 src/airbyte/utils/utils.py
 src/airbyte_api.egg-info/PKG-INFO
 src/airbyte_api.egg-info/SOURCES.txt
 src/airbyte_api.egg-info/dependency_links.txt
 src/airbyte_api.egg-info/requires.txt
```

