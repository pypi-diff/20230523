# Comparing `tmp/pulumi_aiven-6.3.0a1684387394.tar.gz` & `tmp/pulumi_aiven-6.3.0a1684862833.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.3.0a1684387394.tar", last modified: Thu May 18 05:33:13 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.3.0a1684862833.tar", last modified: Tue May 23 17:31:28 2023, max compression
```

## Comparing `pulumi_aiven-6.3.0a1684387394.tar` & `pulumi_aiven-6.3.0a1684862833.tar`

### file list

```diff
@@ -1,141 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:33:13.102557 pulumi_aiven-6.3.0a1684387394/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-18 05:33:13.102557 pulumi_aiven-6.3.0a1684387394/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:33:13.102557 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   594789 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:33:13.102557 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22363 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21870 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22139 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21817 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)   890191 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:33:13.102557 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 05:33:13.106557 pulumi_aiven-6.3.0a1684387394/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-18 05:33:12.000000 pulumi_aiven-6.3.0a1684387394/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:28.790396 pulumi_aiven-6.3.0a1684862833/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-23 17:31:28.790396 pulumi_aiven-6.3.0a1684862833/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:28.786396 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   595384 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:28.790396 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22363 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21870 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22139 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21817 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   891068 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:31:28.790396 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:31:28.790396 pulumi_aiven-6.3.0a1684862833/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 17:31:28.000000 pulumi_aiven-6.3.0a1684862833/setup.py
```

### Comparing `pulumi_aiven-6.3.0a1684387394/PKG-INFO` & `pulumi_aiven-6.3.0a1684862833/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.3.0a1684387394
+Version: 6.3.0a1684862833
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.3.0a1684387394/README.md` & `pulumi_aiven-6.3.0a1684862833/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/__init__.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 from .get_my_sql import *
 from .get_mysql_database import *
 from .get_mysql_user import *
 from .get_open_search import *
 from .get_open_search_acl_config import *
 from .get_open_search_acl_rule import *
 from .get_opensearch_user import *
+from .get_organization import *
+from .get_organizational_unit import *
 from .get_pg import *
 from .get_pg_database import *
 from .get_pg_user import *
 from .get_project import *
 from .get_project_user import *
 from .get_project_vpc import *
 from .get_redis import *
@@ -107,14 +109,16 @@
 from .my_sql import *
 from .mysql_database import *
 from .mysql_user import *
 from .open_search import *
 from .open_search_acl_config import *
 from .open_search_acl_rule import *
 from .opensearch_user import *
+from .organization import *
+from .organizational_unit import *
 from .pg import *
 from .pg_database import *
 from .pg_user import *
 from .project import *
 from .project_user import *
 from .project_vpc import *
 from .provider import *
@@ -519,14 +523,30 @@
   "fqn": "pulumi_aiven",
   "classes": {
    "aiven:index/opensearchUser:OpensearchUser": "OpensearchUser"
   }
  },
  {
   "pkg": "aiven",
+  "mod": "index/organization",
+  "fqn": "pulumi_aiven",
+  "classes": {
+   "aiven:index/organization:Organization": "Organization"
+  }
+ },
+ {
+  "pkg": "aiven",
+  "mod": "index/organizationalUnit",
+  "fqn": "pulumi_aiven",
+  "classes": {
+   "aiven:index/organizationalUnit:OrganizationalUnit": "OrganizationalUnit"
+  }
+ },
+ {
+  "pkg": "aiven",
   "mod": "index/pg",
   "fqn": "pulumi_aiven",
   "classes": {
    "aiven:index/pg:Pg": "Pg"
   }
  },
  {
```

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9862,20 +9862,23 @@
 @pulumi.input_type
 class OpenSearchOpensearchUserConfigSamlArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool],
                  idp_entity_id: pulumi.Input[str],
                  idp_metadata_url: pulumi.Input[str],
                  sp_entity_id: pulumi.Input[str],
+                 idp_pemtrustedcas_content: Optional[pulumi.Input[str]] = None,
                  roles_key: Optional[pulumi.Input[str]] = None,
                  subject_key: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "idp_entity_id", idp_entity_id)
         pulumi.set(__self__, "idp_metadata_url", idp_metadata_url)
         pulumi.set(__self__, "sp_entity_id", sp_entity_id)
+        if idp_pemtrustedcas_content is not None:
+            pulumi.set(__self__, "idp_pemtrustedcas_content", idp_pemtrustedcas_content)
         if roles_key is not None:
             pulumi.set(__self__, "roles_key", roles_key)
         if subject_key is not None:
             pulumi.set(__self__, "subject_key", subject_key)
 
     @property
     @pulumi.getter
@@ -9910,14 +9913,23 @@
         return pulumi.get(self, "sp_entity_id")
 
     @sp_entity_id.setter
     def sp_entity_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "sp_entity_id", value)
 
     @property
+    @pulumi.getter(name="idpPemtrustedcasContent")
+    def idp_pemtrustedcas_content(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "idp_pemtrustedcas_content")
+
+    @idp_pemtrustedcas_content.setter
+    def idp_pemtrustedcas_content(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "idp_pemtrustedcas_content", value)
+
+    @property
     @pulumi.getter(name="rolesKey")
     def roles_key(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "roles_key")
 
     @roles_key.setter
     def roles_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "roles_key", value)
@@ -13321,15 +13333,15 @@
                  ssl_ca_cert: Optional[pulumi.Input[str]] = None,
                  ssl_client_cert: Optional[pulumi.Input[str]] = None,
                  ssl_client_key: Optional[pulumi.Input[str]] = None,
                  ssl_endpoint_identification_algorithm: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bootstrap_servers: Bootstrap servers.
         :param pulumi.Input[str] security_protocol: Security protocol.
-        :param pulumi.Input[str] sasl_mechanism: The list of SASL mechanisms enabled in the Kafka server.
+        :param pulumi.Input[str] sasl_mechanism: SASL mechanism used for connections to the Kafka server.
         :param pulumi.Input[str] sasl_plain_password: Password for SASL PLAIN mechanism in the Kafka server.
         :param pulumi.Input[str] sasl_plain_username: Username for SASL PLAIN mechanism in the Kafka server.
         :param pulumi.Input[str] ssl_ca_cert: PEM-encoded CA certificate.
         :param pulumi.Input[str] ssl_client_cert: PEM-encoded client certificate.
         :param pulumi.Input[str] ssl_client_key: PEM-encoded client key.
         :param pulumi.Input[str] ssl_endpoint_identification_algorithm: The endpoint identification algorithm to validate server hostname using server certificate.
         """
@@ -13374,15 +13386,15 @@
     def security_protocol(self, value: pulumi.Input[str]):
         pulumi.set(self, "security_protocol", value)
 
     @property
     @pulumi.getter(name="saslMechanism")
     def sasl_mechanism(self) -> Optional[pulumi.Input[str]]:
         """
-        The list of SASL mechanisms enabled in the Kafka server.
+        SASL mechanism used for connections to the Kafka server.
         """
         return pulumi.get(self, "sasl_mechanism")
 
     @sasl_mechanism.setter
     def sasl_mechanism(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sasl_mechanism", value)
```

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         The set of arguments for constructing a Account resource.
         :param pulumi.Input[str] name: Account name
         :param pulumi.Input[str] primary_billing_group_id: Billing group id
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if primary_billing_group_id is not None:
+            warnings.warn("""The new aiven_organization resource won't have it, and will not have a replacement.""", DeprecationWarning)
+            pulumi.log.warn("""primary_billing_group_id is deprecated: The new aiven_organization resource won't have it, and will not have a replacement.""")
+        if primary_billing_group_id is not None:
             pulumi.set(__self__, "primary_billing_group_id", primary_billing_group_id)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Account name
@@ -70,24 +73,36 @@
         :param pulumi.Input[str] name: Account name
         :param pulumi.Input[str] owner_team_id: Owner team id
         :param pulumi.Input[str] primary_billing_group_id: Billing group id
         :param pulumi.Input[str] tenant_id: Tenant id
         :param pulumi.Input[str] update_time: Time of last update
         """
         if account_id is not None:
+            warnings.warn("""The new aiven_organization resource won't have it, use the built-in ID field instead.""", DeprecationWarning)
+            pulumi.log.warn("""account_id is deprecated: The new aiven_organization resource won't have it, use the built-in ID field instead.""")
+        if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if create_time is not None:
             pulumi.set(__self__, "create_time", create_time)
         if is_account_owner is not None:
+            warnings.warn("""The new aiven_organization resource won't have it, and will not have a replacement.""", DeprecationWarning)
+            pulumi.log.warn("""is_account_owner is deprecated: The new aiven_organization resource won't have it, and will not have a replacement.""")
+        if is_account_owner is not None:
             pulumi.set(__self__, "is_account_owner", is_account_owner)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if owner_team_id is not None:
+            warnings.warn("""The new aiven_organization resource won't have it, and will not have a replacement.""", DeprecationWarning)
+            pulumi.log.warn("""owner_team_id is deprecated: The new aiven_organization resource won't have it, and will not have a replacement.""")
+        if owner_team_id is not None:
             pulumi.set(__self__, "owner_team_id", owner_team_id)
         if primary_billing_group_id is not None:
+            warnings.warn("""The new aiven_organization resource won't have it, and will not have a replacement.""", DeprecationWarning)
+            pulumi.log.warn("""primary_billing_group_id is deprecated: The new aiven_organization resource won't have it, and will not have a replacement.""")
+        if primary_billing_group_id is not None:
             pulumi.set(__self__, "primary_billing_group_id", primary_billing_group_id)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
         if update_time is not None:
             pulumi.set(__self__, "update_time", update_time)
 
     @property
@@ -265,14 +280,17 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AccountArgs.__new__(AccountArgs)
 
             __props__.__dict__["name"] = name
+            if primary_billing_group_id is not None and not opts.urn:
+                warnings.warn("""The new aiven_organization resource won't have it, and will not have a replacement.""", DeprecationWarning)
+                pulumi.log.warn("""primary_billing_group_id is deprecated: The new aiven_organization resource won't have it, and will not have a replacement.""")
             __props__.__dict__["primary_billing_group_id"] = primary_billing_group_id
             __props__.__dict__["account_id"] = None
             __props__.__dict__["create_time"] = None
             __props__.__dict__["is_account_owner"] = None
             __props__.__dict__["owner_team_id"] = None
             __props__.__dict__["tenant_id"] = None
             __props__.__dict__["update_time"] = None
```

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_team.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/flink.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_project.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/grafana.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/open_search.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/outputs.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9417,14 +9417,16 @@
         suggest = None
         if key == "idpEntityId":
             suggest = "idp_entity_id"
         elif key == "idpMetadataUrl":
             suggest = "idp_metadata_url"
         elif key == "spEntityId":
             suggest = "sp_entity_id"
+        elif key == "idpPemtrustedcasContent":
+            suggest = "idp_pemtrustedcas_content"
         elif key == "rolesKey":
             suggest = "roles_key"
         elif key == "subjectKey":
             suggest = "subject_key"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in OpenSearchOpensearchUserConfigSaml. Access the value via the '{suggest}' property getter instead.")
@@ -9438,20 +9440,23 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  enabled: bool,
                  idp_entity_id: str,
                  idp_metadata_url: str,
                  sp_entity_id: str,
+                 idp_pemtrustedcas_content: Optional[str] = None,
                  roles_key: Optional[str] = None,
                  subject_key: Optional[str] = None):
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "idp_entity_id", idp_entity_id)
         pulumi.set(__self__, "idp_metadata_url", idp_metadata_url)
         pulumi.set(__self__, "sp_entity_id", sp_entity_id)
+        if idp_pemtrustedcas_content is not None:
+            pulumi.set(__self__, "idp_pemtrustedcas_content", idp_pemtrustedcas_content)
         if roles_key is not None:
             pulumi.set(__self__, "roles_key", roles_key)
         if subject_key is not None:
             pulumi.set(__self__, "subject_key", subject_key)
 
     @property
     @pulumi.getter
@@ -9470,14 +9475,19 @@
 
     @property
     @pulumi.getter(name="spEntityId")
     def sp_entity_id(self) -> str:
         return pulumi.get(self, "sp_entity_id")
 
     @property
+    @pulumi.getter(name="idpPemtrustedcasContent")
+    def idp_pemtrustedcas_content(self) -> Optional[str]:
+        return pulumi.get(self, "idp_pemtrustedcas_content")
+
+    @property
     @pulumi.getter(name="rolesKey")
     def roles_key(self) -> Optional[str]:
         return pulumi.get(self, "roles_key")
 
     @property
     @pulumi.getter(name="subjectKey")
     def subject_key(self) -> Optional[str]:
@@ -12572,15 +12582,15 @@
                  ssl_ca_cert: Optional[str] = None,
                  ssl_client_cert: Optional[str] = None,
                  ssl_client_key: Optional[str] = None,
                  ssl_endpoint_identification_algorithm: Optional[str] = None):
         """
         :param str bootstrap_servers: Bootstrap servers.
         :param str security_protocol: Security protocol.
-        :param str sasl_mechanism: The list of SASL mechanisms enabled in the Kafka server.
+        :param str sasl_mechanism: SASL mechanism used for connections to the Kafka server.
         :param str sasl_plain_password: Password for SASL PLAIN mechanism in the Kafka server.
         :param str sasl_plain_username: Username for SASL PLAIN mechanism in the Kafka server.
         :param str ssl_ca_cert: PEM-encoded CA certificate.
         :param str ssl_client_cert: PEM-encoded client certificate.
         :param str ssl_client_key: PEM-encoded client key.
         :param str ssl_endpoint_identification_algorithm: The endpoint identification algorithm to validate server hostname using server certificate.
         """
@@ -12617,15 +12627,15 @@
         """
         return pulumi.get(self, "security_protocol")
 
     @property
     @pulumi.getter(name="saslMechanism")
     def sasl_mechanism(self) -> Optional[str]:
         """
-        The list of SASL mechanisms enabled in the Kafka server.
+        SASL mechanism used for connections to the Kafka server.
         """
         return pulumi.get(self, "sasl_mechanism")
 
     @property
     @pulumi.getter(name="saslPlainPassword")
     def sasl_plain_password(self) -> Optional[str]:
         """
@@ -20190,20 +20200,23 @@
 @pulumi.output_type
 class GetOpenSearchOpensearchUserConfigSamlResult(dict):
     def __init__(__self__, *,
                  enabled: bool,
                  idp_entity_id: str,
                  idp_metadata_url: str,
                  sp_entity_id: str,
+                 idp_pemtrustedcas_content: Optional[str] = None,
                  roles_key: Optional[str] = None,
                  subject_key: Optional[str] = None):
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "idp_entity_id", idp_entity_id)
         pulumi.set(__self__, "idp_metadata_url", idp_metadata_url)
         pulumi.set(__self__, "sp_entity_id", sp_entity_id)
+        if idp_pemtrustedcas_content is not None:
+            pulumi.set(__self__, "idp_pemtrustedcas_content", idp_pemtrustedcas_content)
         if roles_key is not None:
             pulumi.set(__self__, "roles_key", roles_key)
         if subject_key is not None:
             pulumi.set(__self__, "subject_key", subject_key)
 
     @property
     @pulumi.getter
@@ -20222,14 +20235,19 @@
 
     @property
     @pulumi.getter(name="spEntityId")
     def sp_entity_id(self) -> str:
         return pulumi.get(self, "sp_entity_id")
 
     @property
+    @pulumi.getter(name="idpPemtrustedcasContent")
+    def idp_pemtrustedcas_content(self) -> Optional[str]:
+        return pulumi.get(self, "idp_pemtrustedcas_content")
+
+    @property
     @pulumi.getter(name="rolesKey")
     def roles_key(self) -> Optional[str]:
         return pulumi.get(self, "roles_key")
 
     @property
     @pulumi.getter(name="subjectKey")
     def subject_key(self) -> Optional[str]:
```

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pg.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/project.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/project_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/provider.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/redis.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.3.0a1684387394
+Version: 6.3.0a1684862833
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.3.0a1684387394/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.3.0a1684862833/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,16 @@
 pulumi_aiven/get_my_sql.py
 pulumi_aiven/get_mysql_database.py
 pulumi_aiven/get_mysql_user.py
 pulumi_aiven/get_open_search.py
 pulumi_aiven/get_open_search_acl_config.py
 pulumi_aiven/get_open_search_acl_rule.py
 pulumi_aiven/get_opensearch_user.py
+pulumi_aiven/get_organization.py
+pulumi_aiven/get_organizational_unit.py
 pulumi_aiven/get_pg.py
 pulumi_aiven/get_pg_database.py
 pulumi_aiven/get_pg_user.py
 pulumi_aiven/get_project.py
 pulumi_aiven/get_project_user.py
 pulumi_aiven/get_project_vpc.py
 pulumi_aiven/get_redis.py
@@ -105,14 +107,16 @@
 pulumi_aiven/my_sql.py
 pulumi_aiven/mysql_database.py
 pulumi_aiven/mysql_user.py
 pulumi_aiven/open_search.py
 pulumi_aiven/open_search_acl_config.py
 pulumi_aiven/open_search_acl_rule.py
 pulumi_aiven/opensearch_user.py
+pulumi_aiven/organization.py
+pulumi_aiven/organizational_unit.py
 pulumi_aiven/outputs.py
 pulumi_aiven/pg.py
 pulumi_aiven/pg_database.py
 pulumi_aiven/pg_user.py
 pulumi_aiven/project.py
 pulumi_aiven/project_user.py
 pulumi_aiven/project_vpc.py
```

### Comparing `pulumi_aiven-6.3.0a1684387394/setup.py` & `pulumi_aiven-6.3.0a1684862833/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.3.0a1684387394"
-PLUGIN_VERSION = "6.3.0-alpha.1684387394+d85051a2"
+VERSION = "6.3.0a1684862833"
+PLUGIN_VERSION = "6.3.0-alpha.1684862833+3fd494b1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

