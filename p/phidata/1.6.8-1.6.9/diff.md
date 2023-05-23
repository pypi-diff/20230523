# Comparing `tmp/phidata-1.6.8.tar.gz` & `tmp/phidata-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.6.8.tar", last modified: Tue May 23 01:16:04 2023, max compression
+gzip compressed data, was "phidata-1.6.9.tar", last modified: Tue May 23 01:53:19 2023, max compression
```

## Comparing `phidata-1.6.8.tar` & `phidata-1.6.9.tar`

### file list

```diff
@@ -1,513 +1,513 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.111652 phidata-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-23 01:15:43.000000 phidata-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 01:16:04.111652 phidata-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 01:15:43.000000 phidata-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.051653 phidata-1.6.8/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.051653 phidata-1.6.8/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.051653 phidata-1.6.8/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.055652 phidata-1.6.8/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.055652 phidata-1.6.8/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.055652 phidata-1.6.8/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.059652 phidata-1.6.8/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.059652 phidata-1.6.8/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.059652 phidata-1.6.8/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.063653 phidata-1.6.8/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.063653 phidata-1.6.8/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.063653 phidata-1.6.8/phidata/app/django/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/django/django_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.063653 phidata-1.6.8/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.063653 phidata-1.6.8/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.063653 phidata-1.6.8/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.067653 phidata-1.6.8/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/redis/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.071653 phidata-1.6.8/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.075652 phidata-1.6.8/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.079653 phidata-1.6.8/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.083653 phidata-1.6.8/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.083653 phidata-1.6.8/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.083653 phidata-1.6.8/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.083653 phidata-1.6.8/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.083653 phidata-1.6.8/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.083653 phidata-1.6.8/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.087653 phidata-1.6.8/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.091652 phidata-1.6.8/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.091652 phidata-1.6.8/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.091652 phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.091652 phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.091652 phidata-1.6.8/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.095652 phidata-1.6.8/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.095652 phidata-1.6.8/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.095652 phidata-1.6.8/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.095652 phidata-1.6.8/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.099653 phidata-1.6.8/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.103653 phidata-1.6.8/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.107653 phidata-1.6.8/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.111652 phidata-1.6.8/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.111652 phidata-1.6.8/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.111652 phidata-1.6.8/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.111652 phidata-1.6.8/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-23 01:15:43.000000 phidata-1.6.8/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.051653 phidata-1.6.8/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 01:16:04.000000 phidata-1.6.8/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-23 01:16:04.000000 phidata-1.6.8/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:16:04.000000 phidata-1.6.8/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 01:16:04.000000 phidata-1.6.8/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:16:04.000000 phidata-1.6.8/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-23 01:15:43.000000 phidata-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:16:04.111652 phidata-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:15:43.000000 phidata-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:16:04.111652 phidata-1.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 01:15:43.000000 phidata-1.6.8/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-23 01:52:54.000000 phidata-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 01:53:19.962381 phidata-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 01:52:54.000000 phidata-1.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.870379 phidata-1.6.9/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.870379 phidata-1.6.9/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.874379 phidata-1.6.9/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/assistant/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/django/django_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.878379 phidata-1.6.9/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18443 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/k8s/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.882380 phidata-1.6.9/phidata/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37973 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.886380 phidata-1.6.9/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.890380 phidata-1.6.9/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.890380 phidata-1.6.9/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.890380 phidata-1.6.9/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.894380 phidata-1.6.9/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/create/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.898380 phidata-1.6.9/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.902380 phidata-1.6.9/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.902380 phidata-1.6.9/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.902380 phidata-1.6.9/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.906380 phidata-1.6.9/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.910380 phidata-1.6.9/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.914380 phidata-1.6.9/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.914380 phidata-1.6.9/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.918380 phidata-1.6.9/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.918380 phidata-1.6.9/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.918380 phidata-1.6.9/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.922380 phidata-1.6.9/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.926380 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.930380 phidata-1.6.9/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.934381 phidata-1.6.9/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.934381 phidata-1.6.9/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.938381 phidata-1.6.9/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.942381 phidata-1.6.9/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.946381 phidata-1.6.9/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.950381 phidata-1.6.9/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.954381 phidata-1.6.9/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.958381 phidata-1.6.9/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/utils/workspace_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.958381 phidata-1.6.9/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-23 01:52:54.000000 phidata-1.6.9/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.870379 phidata-1.6.9/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:53:19.000000 phidata-1.6.9/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-23 01:52:54.000000 phidata-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:53:19.962381 phidata-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:52:54.000000 phidata-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:53:19.962381 phidata-1.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 01:52:54.000000 phidata-1.6.9/tests/test_placeholder.py
```

### Comparing `phidata-1.6.8/LICENSE` & `phidata-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/PKG-INFO` & `phidata-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.6.8
+Version: 1.6.9
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.6.8 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.9 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.6.8/README.md` & `phidata-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/airflow/operators/empty.py` & `phidata-1.6.9/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/airflow/airflow_base.py` & `phidata-1.6.9/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/airflow/airflow_flower.py` & `phidata-1.6.9/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/airflow/airflow_manager.py` & `phidata-1.6.9/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.6.9/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/airflow/airflow_webserver.py` & `phidata-1.6.9/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/airflow/airflow_worker.py` & `phidata-1.6.9/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/alertmanager/alertmanager.py` & `phidata-1.6.9/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/amundsen/frontend.py` & `phidata-1.6.9/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/amundsen/metadata.py` & `phidata-1.6.9/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/amundsen/search.py` & `phidata-1.6.9/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/assistant/assistant.py` & `phidata-1.6.9/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/cadvisor/cadvisor.py` & `phidata-1.6.9/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/databox/databox.py` & `phidata-1.6.9/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/db/base_db.py` & `phidata-1.6.9/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/django/django_app.py` & `phidata-1.6.9/phidata/app/django/django_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/elastic/elastic_app.py` & `phidata-1.6.9/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.6.9/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/fastapi/fastapi.py` & `phidata-1.6.9/phidata/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/grafana/grafana.py` & `phidata-1.6.9/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/group.py` & `phidata-1.6.9/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.6.9/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.6.9/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/k8s/app.py` & `phidata-1.6.9/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/k8s/dir.py` & `phidata-1.6.9/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/k8s/url.py` & `phidata-1.6.9/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/mysql/mysql_db.py` & `phidata-1.6.9/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/neo4j/neo4j.py` & `phidata-1.6.9/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.6.9/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/phidata_app.py` & `phidata-1.6.9/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/postgres/postgres_db.py` & `phidata-1.6.9/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/prometheus/prometheus.py` & `phidata-1.6.9/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/redis/redis.py` & `phidata-1.6.9/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/redis/stack.py` & `phidata-1.6.9/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/server/api_server.py` & `phidata-1.6.9/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/server/server_base.py` & `phidata-1.6.9/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/spark/spark_base.py` & `phidata-1.6.9/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/spark/spark_driver.py` & `phidata-1.6.9/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/spark/spark_worker.py` & `phidata-1.6.9/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/streamlit/streamlit.py` & `phidata-1.6.9/phidata/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/superset/superset_base.py` & `phidata-1.6.9/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/superset/superset_init.py` & `phidata-1.6.9/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/superset/superset_webserver.py` & `phidata-1.6.9/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/superset/superset_worker.py` & `phidata-1.6.9/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/superset/superset_worker_beat.py` & `phidata-1.6.9/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/traefik/crds.py` & `phidata-1.6.9/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/traefik/ingress_route.py` & `phidata-1.6.9/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/app/traefik/router.py` & `phidata-1.6.9/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/asset/aws/aws_asset.py` & `phidata-1.6.9/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/asset/data_asset.py` & `phidata-1.6.9/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/asset/local/file.py` & `phidata-1.6.9/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/asset/local/local_asset.py` & `phidata-1.6.9/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/api_client.py` & `phidata-1.6.9/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/athena/query.py` & `phidata-1.6.9/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/config.py` & `phidata-1.6.9/phidata/aws/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,25 @@
         aws_region: Optional[str] = None,
         aws_profile: Optional[str] = None,
         aws_config_file: Optional[str] = None,
         aws_shared_credentials_file: Optional[str] = None,
     ):
         super().__init__()
         _resources: Optional[List[AwsResourceGroup]] = None
-        if isinstance(resources, AwsResourceGroup):
-            _resources = [resources]
-        elif isinstance(resources, list):
-            for _r in resources:
-                if isinstance(_r, AwsResourceGroup):
-                    if _resources is None:
-                        _resources = []
-                    _resources.append(_r)
-                else:
-                    logger.error(f"Invalid resource group: {_r}")
+        if resources is not None:
+            if isinstance(resources, list):
+                for _r in resources:
+                    if isinstance(_r, AwsResourceGroup):
+                        if _resources is None:
+                            _resources = []
+                        _resources.append(_r)
+                    else:
+                        logger.error(f"Invalid resource group: {_r}")
+            elif isinstance(resources, AwsResourceGroup):
+                _resources = [resources]
 
         _apps = apps if apps is not None else []
         if app_groups is not None:
             _apps.extend(get_apps_from_app_groups(app_groups))
 
         try:
             self.args: AwsArgs = AwsArgs(
```

### Comparing `phidata-1.6.8/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.6.9/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/create/iam/role.py` & `phidata-1.6.9/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/enums/manager_status.py` & `phidata-1.6.9/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/manager.py` & `phidata-1.6.9/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/acm/certificate.py` & `phidata-1.6.9/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/athena/query.py` & `phidata-1.6.9/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/base.py` & `phidata-1.6.9/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.6.9/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ec2/subnet.py` & `phidata-1.6.9/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ec2/volume.py` & `phidata-1.6.9/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ecs/cluster.py` & `phidata-1.6.9/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ecs/container.py` & `phidata-1.6.9/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ecs/service.py` & `phidata-1.6.9/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.6.9/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/ecs/volume.py` & `phidata-1.6.9/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/eks/addon.py` & `phidata-1.6.9/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/eks/cluster.py` & `phidata-1.6.9/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.6.9/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.6.9/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/eks/node_group.py` & `phidata-1.6.9/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.6.9/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.6.9/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/elb/listener.py` & `phidata-1.6.9/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.6.9/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/elb/target_group.py` & `phidata-1.6.9/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/emr/cluster.py` & `phidata-1.6.9/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/glue/crawler.py` & `phidata-1.6.9/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/group.py` & `phidata-1.6.9/phidata/aws/resource/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from phidata.aws.resource.elb.load_balancer import LoadBalancer
 from phidata.aws.resource.elb.target_group import TargetGroup
 from phidata.aws.resource.elb.listener import Listener
 from phidata.aws.resource.iam.role import IamRole
 from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.aws.resource.glue.crawler import GlueCrawler
 from phidata.aws.resource.s3.bucket import S3Bucket
-from phidata.aws.resource.secret.manager import SecretsManager
+# from phidata.aws.resource.secret.manager import SecretsManager
 from phidata.aws.resource.emr.cluster import EmrCluster
 from phidata.aws.resource.rds.db_cluster import DbCluster
 from phidata.aws.resource.rds.db_instance import DbInstance
 from phidata.aws.resource.rds.db_subnet_group import DbSubnetGroup
 from phidata.aws.resource.elasticache.cluster import CacheCluster
 from phidata.aws.resource.elasticache.subnet_group import CacheSubnetGroup
 
@@ -38,15 +38,15 @@
     enabled: bool = True
     weight: int = 100
 
     subnets: Optional[List[Subnet]] = None
     iam_roles: Optional[List[IamRole]] = None
     iam_policies: Optional[List[IamPolicy]] = None
     acm_certificates: Optional[List[AcmCertificate]] = None
-    secrets: Optional[List[SecretsManager]] = None
+    # secrets: Optional[List[SecretsManager]] = None
     s3_buckets: Optional[List[S3Bucket]] = None
     cache_clusters: Optional[List[CacheCluster]] = None
     cache_subnet_groups: Optional[List[CacheSubnetGroup]] = None
     db_clusters: Optional[List[DbCluster]] = None
     db_subnet_groups: Optional[List[DbSubnetGroup]] = None
     db_instances: Optional[List[DbInstance]] = None
     ecs_clusters: Optional[List[EcsCluster]] = None
```

### Comparing `phidata-1.6.8/phidata/aws/resource/iam/group.py` & `phidata-1.6.9/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/iam/policy.py` & `phidata-1.6.9/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/iam/role.py` & `phidata-1.6.9/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.6.9/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/rds/db_instance.py` & `phidata-1.6.9/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.6.9/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/s3/bucket.py` & `phidata-1.6.9/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/secret/manager.py` & `phidata-1.6.9/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/types.py` & `phidata-1.6.9/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/resource/utils.py` & `phidata-1.6.9/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/s3/csv_dataset.py` & `phidata-1.6.9/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/s3/dataset.py` & `phidata-1.6.9/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/s3/dataset_base.py` & `phidata-1.6.9/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/s3/object.py` & `phidata-1.6.9/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/aws/worker.py` & `phidata-1.6.9/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/base.py` & `phidata-1.6.9/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/checks/check.py` & `phidata-1.6.9/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/checks/not_empty.py` & `phidata-1.6.9/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/constants.py` & `phidata-1.6.9/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/decorators/timer.py` & `phidata-1.6.9/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/decorators/validate_env.py` & `phidata-1.6.9/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/api_client.py` & `phidata-1.6.9/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/args.py` & `phidata-1.6.9/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/config.py` & `phidata-1.6.9/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/enums.py` & `phidata-1.6.9/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/manager.py` & `phidata-1.6.9/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/base.py` & `phidata-1.6.9/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/container.py` & `phidata-1.6.9/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/group.py` & `phidata-1.6.9/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/image.py` & `phidata-1.6.9/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/network.py` & `phidata-1.6.9/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/types.py` & `phidata-1.6.9/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/utils.py` & `phidata-1.6.9/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/resource/volume.py` & `phidata-1.6.9/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/utils/container.py` & `phidata-1.6.9/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/docker/worker.py` & `phidata-1.6.9/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/infra/args.py` & `phidata-1.6.9/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/infra/config.py` & `phidata-1.6.9/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/infra/resource.py` & `phidata-1.6.9/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/api_client.py` & `phidata-1.6.9/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/args.py` & `phidata-1.6.9/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/config.py` & `phidata-1.6.9/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.9/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.6.9/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/common/port.py` & `phidata-1.6.9/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/container.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/secret.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/service.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/core/v1/volume.py` & `phidata-1.6.9/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.6.9/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/group.py` & `phidata-1.6.9/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/kubeconfig.py` & `phidata-1.6.9/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.6.9/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.9/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.9/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/enums/api_version.py` & `phidata-1.6.9/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/enums/kind.py` & `phidata-1.6.9/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/enums/manager_status.py` & `phidata-1.6.9/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/enums/pv.py` & `phidata-1.6.9/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/manager.py` & `phidata-1.6.9/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.9/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.6.9/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/base.py` & `phidata-1.6.9/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/container.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/service.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.6.9/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/group.py` & `phidata-1.6.9/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/kubeconfig.py` & `phidata-1.6.9/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.6.9/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.6.9/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.6.9/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.9/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.9/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/types.py` & `phidata-1.6.9/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/resource/utils.py` & `phidata-1.6.9/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/utils/pod.py` & `phidata-1.6.9/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/k8s/worker.py` & `phidata-1.6.9/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/llm/duckdb/agent.py` & `phidata-1.6.9/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/llm/duckdb/chain.py` & `phidata-1.6.9/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/llm/duckdb/connection.py` & `phidata-1.6.9/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/llm/duckdb/loader.py` & `phidata-1.6.9/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/llm/duckdb/query.py` & `phidata-1.6.9/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/llm/duckdb/tool.py` & `phidata-1.6.9/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/product/data_product.py` & `phidata-1.6.9/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/local/csv.py` & `phidata-1.6.9/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/local/local_table.py` & `phidata-1.6.9/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/local/parquet.py` & `phidata-1.6.9/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/s3/csv.py` & `phidata-1.6.9/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/s3/parquet.py` & `phidata-1.6.9/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/s3/s3_table.py` & `phidata-1.6.9/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/sql/postgres.py` & `phidata-1.6.9/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/table/sql/sql_table.py` & `phidata-1.6.9/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/aws/athena/run_query.py` & `phidata-1.6.9/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/aws/emr/create_cluster.py` & `phidata-1.6.9/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.6.9/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/aws/glue/start_crawler.py` & `phidata-1.6.9/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/decorator.py` & `phidata-1.6.9/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/download/s3/to_file.py` & `phidata-1.6.9/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/download/url/to_file.py` & `phidata-1.6.9/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/download/url/to_s3.py` & `phidata-1.6.9/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/download/url/to_sql.py` & `phidata-1.6.9/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/plot/sql/query.py` & `phidata-1.6.9/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/python_task.py` & `phidata-1.6.9/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/run/sql/query.py` & `phidata-1.6.9/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/task.py` & `phidata-1.6.9/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/task_relatives.py` & `phidata-1.6.9/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/upload/file/to_s3.py` & `phidata-1.6.9/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/task/upload/file/to_sql.py` & `phidata-1.6.9/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/types/airflow.py` & `phidata-1.6.9/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/types/context.py` & `phidata-1.6.9/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/types/phidata_runtime.py` & `phidata-1.6.9/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/cli_console.py` & `phidata-1.6.9/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/common.py` & `phidata-1.6.9/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/compare.py` & `phidata-1.6.9/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/context.py` & `phidata-1.6.9/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/dttm.py` & `phidata-1.6.9/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/enums.py` & `phidata-1.6.9/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/env_file.py` & `phidata-1.6.9/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/env_var.py` & `phidata-1.6.9/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/filesystem.py` & `phidata-1.6.9/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/log.py` & `phidata-1.6.9/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/prep_infra_config.py` & `phidata-1.6.9/phidata/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/print_table.py` & `phidata-1.6.9/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/utils/workspace_path.py` & `phidata-1.6.9/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/workflow/decorator.py` & `phidata-1.6.9/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/workflow/workflow.py` & `phidata-1.6.9/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/workflow/workflow_relatives.py` & `phidata-1.6.9/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/workspace/config.py` & `phidata-1.6.9/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata/workspace/settings.py` & `phidata-1.6.9/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/phidata.egg-info/PKG-INFO` & `phidata-1.6.9/phidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.6.8
+Version: 1.6.9
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.6.8 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.9 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.6.8/phidata.egg-info/SOURCES.txt` & `phidata-1.6.9/phidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phidata-1.6.8/pyproject.toml` & `phidata-1.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "phidata"
-version = "1.6.8"
+version = "1.6.9"
 description = "Building blocks for Data Engineering"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3",
-  "phiterm==1.6.8",
+  "phiterm==1.6.9",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
```

