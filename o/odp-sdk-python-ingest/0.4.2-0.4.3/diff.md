# Comparing `tmp/odp_sdk_python_ingest-0.4.2.tar.gz` & `tmp/odp_sdk_python_ingest-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_sdk_python_ingest-0.4.2.tar", max compression
+gzip compressed data, was "odp_sdk_python_ingest-0.4.3.tar", max compression
```

## Comparing `odp_sdk_python_ingest-0.4.2.tar` & `odp_sdk_python_ingest-0.4.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0      842 2023-05-16 09:19:34.819400 odp_sdk_python_ingest-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/cdf/__init__.py
--rw-r--r--   0        0        0     3258 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/cdf/cdf_token_handler.py
--rw-r--r--   0        0        0     1764 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/cdf/federated_cognite_client.py
--rw-r--r--   0        0        0      163 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/odp/__init__.py
--rw-r--r--   0        0        0     3064 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/odp/interactive_login_token_handler.py
--rw-r--r--   0        0        0     1813 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/odp/ropc_token_handler.py
--rw-r--r--   0        0        0     1358 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/odp/token_handler.py
--rw-r--r--   0        0        0       49 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/prefect/__init__.py
--rw-r--r--   0        0        0     3877 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/auth/prefect/prefect_b2c_client.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/__init__.py
--rw-r--r--   0        0        0     2374 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/aad_client_credentials.py
--rw-r--r--   0        0        0     6042 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/azure_storage.py
--rw-r--r--   0        0        0     2879 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/cdf_storage.py
--rw-r--r--   0        0        0      579 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/db_engine.py
--rw-r--r--   0        0        0      354 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/odcat.py
--rw-r--r--   0        0        0     2378 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/blocks/postgres.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/__init__.py
--rw-r--r--   0        0        0      479 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/__main__.py
--rw-r--r--   0        0        0      435 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/authenticate.py
--rw-r--r--   0        0        0     2610 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/block.py
--rw-r--r--   0        0        0     5041 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/context.py
--rw-r--r--   0        0        0     7296 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/deploy.py
--rw-r--r--   0        0        0     2741 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/parameters.py
--rw-r--r--   0        0        0       43 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/params/__init__.py
--rw-r--r--   0        0        0      515 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/params/type_param_type.py
--rw-r--r--   0        0        0     3421 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/run.py
--rw-r--r--   0        0        0     1019 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/cli/schema.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/config/__init__.py
--rw-r--r--   0        0        0      708 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/config/cdf_config.py
--rw-r--r--   0        0        0      816 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/config/dask_config.py
--rw-r--r--   0        0        0      125 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/__init__.py
--rw-r--r--   0        0        0      216 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/abstract_deployment_block.py
--rw-r--r--   0        0        0       40 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/block/__init__.py
--rw-r--r--   0        0        0      501 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/block/generic_block.py
--rw-r--r--   0        0        0     1591 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/deployment_block_factory.py
--rw-r--r--   0        0        0      190 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/__init__.py
--rw-r--r--   0        0        0      481 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/abstract_runtime.py
--rw-r--r--   0        0        0     3463 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/kubernetes.py
--rw-r--r--   0        0        0     4567 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/kubernetes_dask.py
--rw-r--r--   0        0        0     1718 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
--rw-r--r--   0        0        0       88 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/schedule/__init__.py
--rw-r--r--   0        0        0      417 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/schedule/abstract_schedule.py
--rw-r--r--   0        0        0      471 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/schedule/cron_schedule.py
--rw-r--r--   0        0        0     1030 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/schedule/interval_schedule.py
--rw-r--r--   0        0        0       73 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/storage/__init__.py
--rw-r--r--   0        0        0      938 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/storage/abstract_storage.py
--rw-r--r--   0        0        0    10906 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/storage/docker.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/deploy/storage/prefect_healthcheck.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/__init__.py
--rw-r--r--   0        0        0     4679 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/stateful_value_impl.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/__init__.py
--rw-r--r--   0        0        0     1060 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/watermark_file_store.py
--rw-r--r--   0        0        0      639 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/watermark_inmemory_store.py
--rw-r--r--   0        0        0      728 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/watermark_redis_store.py
--rw-r--r--   0        0        0     5488 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/secrets.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/state_handlers/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/state_handlers/metrics_pusher.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/tasks/cdf/__init__.py
--rw-r--r--   0        0        0     3217 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/tasks/cdf/cdf_credentials.py
--rw-r--r--   0        0        0     1438 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/tasks/concurrency_limit.py
--rw-r--r--   0        0        0      705 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/tasks/measured_task.py
--rw-r--r--   0        0        0     1580 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/compute/tasks/tasks.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/metrics/__init__.py
--rw-r--r--   0        0        0     4749 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/metrics/abstract_metrics.py
--rw-r--r--   0        0        0     2192 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/metrics/metric_client.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.823400 odp_sdk_python_ingest-0.4.2/odp/metrics/mock/__init__.py
--rw-r--r--   0        0        0     2523 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/metrics/mock/metric_client.py
--rw-r--r--   0        0        0     3293 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/metrics/mock/metrics.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/metrics/prometheus/__init__.py
--rw-r--r--   0        0        0     2628 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/metrics/prometheus/metric_client.py
--rw-r--r--   0        0        0     3721 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/metrics/prometheus/metrics.py
--rw-r--r--   0        0        0        0 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/types/__init__.py
--rw-r--r--   0        0        0      361 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/types/file_info.py
--rw-r--r--   0        0        0      248 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/__init__.py
--rw-r--r--   0        0        0     2887 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/args.py
--rw-r--r--   0        0        0     1128 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/deploy_helpers.py
--rw-r--r--   0        0        0     4913 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/import_helpers.py
--rw-r--r--   0        0        0      607 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/naming.py
--rw-r--r--   0        0        0     5715 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/retry.py
--rw-r--r--   0        0        0      317 2023-05-16 09:19:34.827400 odp_sdk_python_ingest-0.4.2/odp/utils/timers.py
--rw-r--r--   0        0        0     1945 2023-05-16 09:21:04.000230 odp_sdk_python_ingest-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/cdf/__init__.py
+-rw-r--r--   0        0        0     3258 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/cdf/cdf_token_handler.py
+-rw-r--r--   0        0        0     1764 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/cdf/federated_cognite_client.py
+-rw-r--r--   0        0        0      163 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/odp/__init__.py
+-rw-r--r--   0        0        0     3064 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/odp/interactive_login_token_handler.py
+-rw-r--r--   0        0        0     1813 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/odp/ropc_token_handler.py
+-rw-r--r--   0        0        0     1358 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/odp/token_handler.py
+-rw-r--r--   0        0        0       49 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/prefect/__init__.py
+-rw-r--r--   0        0        0     3877 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/auth/prefect/prefect_b2c_client.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/__init__.py
+-rw-r--r--   0        0        0     2374 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/aad_client_credentials.py
+-rw-r--r--   0        0        0     6042 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/azure_storage.py
+-rw-r--r--   0        0        0     2879 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/cdf_storage.py
+-rw-r--r--   0        0        0      579 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/db_engine.py
+-rw-r--r--   0        0        0      354 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/odcat.py
+-rw-r--r--   0        0        0     2378 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/blocks/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/__main__.py
+-rw-r--r--   0        0        0      435 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/authenticate.py
+-rw-r--r--   0        0        0     2610 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/block.py
+-rw-r--r--   0        0        0     5041 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/context.py
+-rw-r--r--   0        0        0     7296 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/deploy.py
+-rw-r--r--   0        0        0     2741 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/parameters.py
+-rw-r--r--   0        0        0       43 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/params/__init__.py
+-rw-r--r--   0        0        0      515 2023-05-23 11:46:18.355424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/params/type_param_type.py
+-rw-r--r--   0        0        0     3421 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/run.py
+-rw-r--r--   0        0        0     1019 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/cli/schema.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/config/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/config/cdf_config.py
+-rw-r--r--   0        0        0      816 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/config/dask_config.py
+-rw-r--r--   0        0        0      125 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/abstract_deployment_block.py
+-rw-r--r--   0        0        0       40 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/block/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/block/generic_block.py
+-rw-r--r--   0        0        0     1591 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/deployment_block_factory.py
+-rw-r--r--   0        0        0      190 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/abstract_runtime.py
+-rw-r--r--   0        0        0     3463 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/kubernetes.py
+-rw-r--r--   0        0        0     4567 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/kubernetes_dask.py
+-rw-r--r--   0        0        0     1718 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/kubernetes_tiered_resource.py
+-rw-r--r--   0        0        0       88 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/schedule/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/schedule/abstract_schedule.py
+-rw-r--r--   0        0        0      471 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/schedule/cron_schedule.py
+-rw-r--r--   0        0        0     1030 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/schedule/interval_schedule.py
+-rw-r--r--   0        0        0       73 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/storage/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/storage/abstract_storage.py
+-rw-r--r--   0        0        0    10906 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/storage/docker.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/deploy/storage/prefect_healthcheck.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/__init__.py
+-rw-r--r--   0        0        0     4679 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/stateful_value_impl.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/__init__.py
+-rw-r--r--   0        0        0     1060 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/watermark_file_store.py
+-rw-r--r--   0        0        0      639 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/watermark_inmemory_store.py
+-rw-r--r--   0        0        0      728 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/watermark_redis_store.py
+-rw-r--r--   0        0        0     5488 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/secrets.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/state_handlers/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/state_handlers/metrics_pusher.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/tasks/cdf/__init__.py
+-rw-r--r--   0        0        0     3217 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/tasks/cdf/cdf_credentials.py
+-rw-r--r--   0        0        0     1438 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/tasks/concurrency_limit.py
+-rw-r--r--   0        0        0      705 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/tasks/measured_task.py
+-rw-r--r--   0        0        0     1580 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/compute/tasks/tasks.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/__init__.py
+-rw-r--r--   0        0        0     4758 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/abstract_metrics.py
+-rw-r--r--   0        0        0     2302 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/metric_client.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/mock/__init__.py
+-rw-r--r--   0        0        0     2523 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/mock/metric_client.py
+-rw-r--r--   0        0        0     3271 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/mock/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/prometheus/__init__.py
+-rw-r--r--   0        0        0     2612 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/prometheus/metric_client.py
+-rw-r--r--   0        0        0     3686 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/metrics/prometheus/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/types/__init__.py
+-rw-r--r--   0        0        0      361 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/types/file_info.py
+-rw-r--r--   0        0        0      248 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/__init__.py
+-rw-r--r--   0        0        0     2887 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/args.py
+-rw-r--r--   0        0        0     1128 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/deploy_helpers.py
+-rw-r--r--   0        0        0     4913 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/import_helpers.py
+-rw-r--r--   0        0        0      607 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/naming.py
+-rw-r--r--   0        0        0     5715 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/retry.py
+-rw-r--r--   0        0        0      317 2023-05-23 11:46:18.359424 odp_sdk_python_ingest-0.4.3/odp/utils/timers.py
+-rw-r--r--   0        0        0     1945 2023-05-23 11:47:26.116534 odp_sdk_python_ingest-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 odp_sdk_python_ingest-0.4.3/PKG-INFO
```

### Comparing `odp_sdk_python_ingest-0.4.2/README.md` & `odp_sdk_python_ingest-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/auth/cdf/cdf_token_handler.py` & `odp_sdk_python_ingest-0.4.3/odp/auth/cdf/cdf_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/auth/cdf/federated_cognite_client.py` & `odp_sdk_python_ingest-0.4.3/odp/auth/cdf/federated_cognite_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/auth/odp/interactive_login_token_handler.py` & `odp_sdk_python_ingest-0.4.3/odp/auth/odp/interactive_login_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/auth/odp/ropc_token_handler.py` & `odp_sdk_python_ingest-0.4.3/odp/auth/odp/ropc_token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/auth/odp/token_handler.py` & `odp_sdk_python_ingest-0.4.3/odp/auth/odp/token_handler.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/auth/prefect/prefect_b2c_client.py` & `odp_sdk_python_ingest-0.4.3/odp/auth/prefect/prefect_b2c_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/blocks/aad_client_credentials.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/blocks/aad_client_credentials.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/blocks/azure_storage.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/blocks/azure_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/blocks/cdf_storage.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/blocks/cdf_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/blocks/db_engine.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/blocks/db_engine.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/blocks/postgres.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/blocks/postgres.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/block.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/block.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/context.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/context.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/deploy.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/parameters.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/parameters.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/params/type_param_type.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/params/type_param_type.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/run.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/run.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/cli/schema.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/cli/schema.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/config/cdf_config.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/config/cdf_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/config/dask_config.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/config/dask_config.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/deployment_block_factory.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/deployment_block_factory.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/kubernetes.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/kubernetes.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/kubernetes_dask.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/kubernetes_dask.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/runtime/kubernetes_tiered_resource.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/runtime/kubernetes_tiered_resource.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/schedule/interval_schedule.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/schedule/interval_schedule.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/storage/abstract_storage.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/deploy/storage/docker.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/deploy/storage/docker.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/stateful_value_impl.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/stateful_value_impl.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/watermark_file_store.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/watermark_file_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/watermark_inmemory_store.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/watermark_inmemory_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/flow_state/store/watermark_redis_store.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/flow_state/store/watermark_redis_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/secrets.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/secrets.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/state_handlers/metrics_pusher.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/state_handlers/metrics_pusher.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/tasks/cdf/cdf_credentials.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/tasks/cdf/cdf_credentials.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/tasks/concurrency_limit.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/tasks/concurrency_limit.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/tasks/measured_task.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/tasks/measured_task.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/compute/tasks/tasks.py` & `odp_sdk_python_ingest-0.4.3/odp/compute/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/metrics/abstract_metrics.py` & `odp_sdk_python_ingest-0.4.3/odp/metrics/abstract_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     A counter is a cumulative metric that represents a single numerical value that only ever goes up. A counter is
     typically used to count requests served, tasks completed, errors occurred, etc. Counters should not be used to
     expose current counts of items whose number can also go down, e.g. the number of currently running coroutines.
     """
 
     @abstractmethod
-    def inc(self, value: float = 1, labels: Dict[str, str] = {}):
+    def inc(self, value: float = 1, labels: Dict[str, str] = None):
         """Increment the counter by the given value.
 
         Args:
             value: Value to increment the counter by.
             labels: dict with label name as key, label value as value
         """
 
@@ -99,24 +99,23 @@
     """Base class for all gauges.
 
     A gauge is a metric that represents a single numerical value that can arbitrarily go up and down. Gauges are
     typically used to represent current counts of items, e.g. the number of currently running coroutines.
     """
 
     @abstractmethod
-    def set(self, value: float, labels: Dict[str, str] = {}):
+    def set(self, value: float, labels: Dict[str, str] = None):
         ...
 
     @abstractmethod
-    def inc(self, value: float = 1, labels: Dict[str, str] = {}):
+    def inc(self, value: float = 1, labels: Dict[str, str] = None):
         ...
 
-    @abstractmethod
-    def dec(self, value: float = 1, labels: Dict[str, str] = {}):
-        self.inc(-value)
+    def dec(self, value: float = 1, labels: Dict[str, str] = None):
+        self.inc(value=-value, labels=labels)
 
 
 class HistogramABC(MetricABC):
     """Base class for all histograms.
 
     A histogram is a metric that represents the distribution of a set of values over time. Histograms are typically
     used to track request latencies, response sizes, etc.
```

### Comparing `odp_sdk_python_ingest-0.4.2/odp/metrics/metric_client.py` & `odp_sdk_python_ingest-0.4.3/odp/metrics/metric_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from abc import ABC, abstractmethod
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from odp.metrics.abstract_metrics import CounterABC, GaugeABC, HistogramABC
 from odp.utils.import_helpers import import_object
 
 
 class MetricClient(ABC):
     """Base class for metric clients"""
@@ -18,19 +18,23 @@
         namespace: str = "",
         subsystem: str = "",
         unit: str = "",
     ) -> CounterABC:
         """Base method to create a counter from the metric client"""
 
     @abstractmethod
-    def create_gauge(self, name: str, documentation: str, labels: Optional[List] = None) -> GaugeABC:
+    def create_gauge(
+        self, name: str, documentation: str, labels: Optional[Dict[str, Union[str, int, float]]] = None
+    ) -> GaugeABC:
         """Base method to create a gauge from the metric client"""
 
     @abstractmethod
-    def create_histogram(self, name: str, description: str, labels: Optional[List] = None) -> HistogramABC:
+    def create_histogram(
+        self, name: str, description: str, labels: Optional[Dict[str, Union[str, int, float]]] = None
+    ) -> HistogramABC:
         """Base method to create a gauge from the metric client"""
 
     @abstractmethod
     def push_metrics(self):
         """Base method to push metrics"""
 
 
@@ -43,10 +47,12 @@
     If no keyword arguments are passed, the metrics object will be instantiated from environment variables.
     Args:
         client_cls: The class name of the metrics object to instantiate.
         **kwargs: Keyword arguments to pass to the metrics object constructor.
     Returns:
         A metrics object.
     """
-    client_cls_path = client_cls or os.getenv("ODP_METRICS_CLASS", "odp.metrics.mock.metric_client.MockMetricClient")
+    client_cls_path = client_cls or os.getenv(
+        "ODP_METRIC_CLIENT_CLS", "odp.metrics.mock.metric_client.MockMetricClient"
+    )
     cls: MetricClient = import_object(client_cls_path)
     return cls(**kwargs)
```

### Comparing `odp_sdk_python_ingest-0.4.2/odp/metrics/mock/metric_client.py` & `odp_sdk_python_ingest-0.4.3/odp/metrics/mock/metric_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/metrics/mock/metrics.py` & `odp_sdk_python_ingest-0.4.3/odp/metrics/mock/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         namespace: str = "",
         subsystem: str = "",
         unit: str = "",
         registry: Optional[CollectorRegistry] = REGISTRY,
         _labelvalues: Optional[Sequence[str]] = None,
     ):
         super().__init__(name, documentation, labelnames, namespace, subsystem, unit, registry, _labelvalues)
-        self.value = 0
+        self._value = 0
         self._created = time.time()
 
-    def inc(self, value: float = 1, labels: Dict = {}) -> None:
+    def inc(self, value: float = 1, labels: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if labels:
             self.labels(**labels).inc(value=value)
         else:
-            self.value += value
+            self._value += value
 
 
 class MockGauge(GaugeABC):
     def __init__(
         self,
         name: str,
         documentation: str,
@@ -40,33 +40,27 @@
         namespace: str = "",
         subsystem: str = "",
         unit: str = "",
         registry: Optional[CollectorRegistry] = REGISTRY,
         _labelvalues: Optional[Sequence[str]] = None,
     ):
         super().__init__(name, documentation, labelnames, namespace, subsystem, unit, registry, _labelvalues)
-        self.value = 0
+        self._value = 0
 
-    def set(self, value: float, labels: Dict = {}) -> None:
+    def set(self, value: float, labels: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if labels:
             self.labels(**labels).set(value=value)
         else:
-            self.value = value
+            self._value = value
 
-    def inc(self, value: float = 1, labels: Dict = {}) -> None:
+    def inc(self, value: float = 1, labels: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if labels:
             self.labels(**labels).inc(value=value)
         else:
-            self.value += value
-
-    def dec(self, value: float = 1, labels: Dict = {}) -> None:
-        if labels:
-            self.labels(**labels).dec(value=value)
-        else:
-            self.value -= value
+            self._value += value
 
 
 class MockHistogram(HistogramABC):
     def __init__(
         self,
         name: str,
         documentation: str,
@@ -90,15 +84,15 @@
         )
         self.upper_bounds = buckets
         self.buckets = []
         self.sum = 0
         for b in self.upper_bounds:
             self.buckets.append({"upper_bound": b, "value": 0})
 
-    def observe(self, value: float, labels: Dict[str, str] = {}) -> None:
+    def observe(self, value: float, labels: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if labels:
             self.labels(**labels).observe(value=value)
         else:
             self.sum += 1
             for i, bound in enumerate(self.upper_bounds):
                 if value <= bound:
                     self.buckets[i]["value"] += 1
```

### Comparing `odp_sdk_python_ingest-0.4.2/odp/metrics/prometheus/metric_client.py` & `odp_sdk_python_ingest-0.4.3/odp/metrics/prometheus/metric_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from odp.metrics.abstract_metrics import CounterABC, GaugeABC, HistogramABC
 from odp.metrics.metric_client import MetricClient
 from odp.metrics.prometheus.metrics import PrometheusCounter, PrometheusGauge, PrometheusHistogram
 
 
 class PrometheusMetricClient(MetricClient):
     def __init__(self, pushgateway_url: Optional[str] = None, job_name: Optional[str] = None):
-        self._pushgateway_url = pushgateway_url or getenv("ODP_METRICS_PROMETHEUS_PUSHGATEWAY_URL")
+        self._pushgateway_url = pushgateway_url or getenv("ODP_METRIC_CLIENT_ARGS")
         self._job_name = job_name
         self._registry = CollectorRegistry()
         self._run = getenv("PREFECT__CONTEXT__FLOW_RUN_ID", "UNKNOWN_RUN")
 
     def create_counter(
         self,
         name: str,
```

### Comparing `odp_sdk_python_ingest-0.4.2/odp/metrics/prometheus/metrics.py` & `odp_sdk_python_ingest-0.4.3/odp/metrics/prometheus/metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             labelnames=labelnames,
             namespace=namespace,
             subsystem=subsystem,
             unit=unit,
             registry=registry,
         )
 
-    def inc(self, value: float = 1, labels: Dict = {}):
+    def inc(self, value: float = 1, labels: Optional[Dict[str, Union[str, int, float]]] = None):
         if labels:
             self._counter.labels(**labels).inc(value)
         else:
             self._counter.inc(value)
 
 
 class PrometheusGauge(GaugeABC):
@@ -57,32 +57,26 @@
             labelnames=labelnames,
             namespace=namespace,
             subsystem=subsystem,
             unit=unit,
             registry=registry,
         )
 
-    def set(self, value: float, labels: Dict = {}) -> None:
+    def set(self, value: float, labels: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if labels:
             self._gauge.labels(**labels).set(value=value)
         else:
             self._gauge.set(value=value)
 
-    def inc(self, value: float = 1, labels: Dict = {}) -> None:
+    def inc(self, value: float = 1, labels: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if labels:
             self._gauge.labels(**labels).inc(amount=value)
         else:
             self._gauge.inc(amount=value)
 
-    def dec(self, value: float = 1, labels: Dict = {}) -> None:
-        if labels:
-            self._gauge.labels(**labels).dec(amount=value)
-        else:
-            self._gauge.dec(amount=value)
-
 
 class PrometheusHistogram(HistogramABC):
     def __init__(
         self,
         name: str,
         documentation: str,
         labelnames: Iterable[str] = (),
@@ -101,12 +95,12 @@
             namespace=namespace,
             subsystem=subsystem,
             unit=unit,
             registry=registry,
             buckets=buckets,
         )
 
-    def observe(self, value: float = 1, labels: Dict = {}):
+    def observe(self, value: float = 1, labels: Optional[Dict[str, Union[str, int, float]]] = None):
         if labels:
             self._histogram.labels(**labels).observe(amount=value)
         else:
             self._histogram.observe(amount=value)
```

### Comparing `odp_sdk_python_ingest-0.4.2/odp/utils/args.py` & `odp_sdk_python_ingest-0.4.3/odp/utils/args.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/utils/deploy_helpers.py` & `odp_sdk_python_ingest-0.4.3/odp/utils/deploy_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/utils/import_helpers.py` & `odp_sdk_python_ingest-0.4.3/odp/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/utils/naming.py` & `odp_sdk_python_ingest-0.4.3/odp/utils/naming.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/odp/utils/retry.py` & `odp_sdk_python_ingest-0.4.3/odp/utils/retry.py`

 * *Files identical despite different names*

### Comparing `odp_sdk_python_ingest-0.4.2/pyproject.toml` & `odp_sdk_python_ingest-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp-sdk-python-ingest"
-version = "0.4.2"
+version = "0.4.3"
 description = "ODP ingest SDK"
 authors = ["Thomas Li Fredriksen <thomas.fredriksen@oceandata.earth>"]
 readme = "README.md"
 packages = [
     {include="odp"}
 ]
```

### Comparing `odp_sdk_python_ingest-0.4.2/PKG-INFO` & `odp_sdk_python_ingest-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp-sdk-python-ingest
-Version: 0.4.2
+Version: 0.4.3
 Summary: ODP ingest SDK
 Author: Thomas Li Fredriksen
 Author-email: thomas.fredriksen@oceandata.earth
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.2 Summary: ODP
+Metadata-Version: 2.1 Name: odp-sdk-python-ingest Version: 0.4.3 Summary: ODP
 ingest SDK Author: Thomas Li Fredriksen Author-email:
 thomas.fredriksen@oceandata.earth Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 azure-common (>=1.1.28,<2.0.0) Requires-Dist: azure-identity (>=1.11.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0) Requires-Dist: azure-keyvault-
 secrets (>=4.6.0,<5.0.0) Requires-Dist: azure-storage-blob (>=12.13.1,<13.0.0)
```

