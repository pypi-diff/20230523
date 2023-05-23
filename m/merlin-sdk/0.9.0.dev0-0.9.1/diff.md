# Comparing `tmp/merlin-sdk-0.9.0.dev0.tar.gz` & `tmp/merlin-sdk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/merlin-sdk-0.9.0.dev0.tar", last modified: Wed Dec 16 03:15:18 2020, max compression
+gzip compressed data, was "dist/merlin-sdk-0.9.1.tar", last modified: Fri Jan  8 09:14:19 2021, max compression
```

## Comparing `merlin-sdk-0.9.0.dev0.tar` & `merlin-sdk-0.9.1.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (116)      801 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      546 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      248 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      269 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (116)     1639 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/client/
--rw-r--r--   0 runner    (1001) docker     (116)     2966 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/client/api/
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20720 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/alert_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    29865 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/endpoint_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     3958 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/environment_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     7074 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    25748 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/model_endpoints_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    32579 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/models_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    28640 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/prediction_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14728 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    16375 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/secret_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    12001 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api/version_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    24953 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     8085 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/client/models/
--rw-r--r--   0 runner    (1001) docker     (116)     2345 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2639 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/alert_condition_metric_type.py
--rw-r--r--   0 runner    (1001) docker     (116)     2559 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/alert_condition_severity.py
--rw-r--r--   0 runner    (1001) docker     (116)     6179 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     6486 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/container.py
--rw-r--r--   0 runner    (1001) docker     (116)     2601 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/endpoint_status.py
--rw-r--r--   0 runner    (1001) docker     (116)     3530 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/env_var.py
--rw-r--r--   0 runner    (1001) docker     (116)     8693 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (116)     2585 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/file_format.py
--rw-r--r--   0 runner    (1001) docker     (116)     3498 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/label.py
--rw-r--r--   0 runner    (1001) docker     (116)     8691 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     9077 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/model_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)     6467 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/model_endpoint_alert.py
--rw-r--r--   0 runner    (1001) docker     (116)     6885 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/model_endpoint_alert_condition.py
--rw-r--r--   0 runner    (1001) docker     (116)     3971 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/model_endpoint_rule.py
--rw-r--r--   0 runner    (1001) docker     (116)     5031 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/model_endpoint_rule_destination.py
--rw-r--r--   0 runner    (1001) docker     (116)    10467 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (116)     8357 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     6377 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_bigquery_sink.py
--rw-r--r--   0 runner    (1001) docker     (116)     4706 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_bigquery_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     6078 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_gcs_sink.py
--rw-r--r--   0 runner    (1001) docker     (116)     5288 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_gcs_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     5538 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     3940 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_model_result.py
--rw-r--r--   0 runner    (1001) docker     (116)     7257 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/prediction_job_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     8991 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/project.py
--rw-r--r--   0 runner    (1001) docker     (116)     5416 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/resource_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     2587 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/result_type.py
--rw-r--r--   0 runner    (1001) docker     (116)     2581 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/save_mode.py
--rw-r--r--   0 runner    (1001) docker     (116)     4023 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (116)     7804 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (116)     8474 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/version.py
--rw-r--r--   0 runner    (1001) docker     (116)    12460 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/models/version_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)    13183 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)      633 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      528 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     3230 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2747 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (116)      367 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      850 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (116)      452 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/docs/sample/
--rw-r--r--   0 runner    (1001) docker     (116)       94 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/batch_iris.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       93 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/batch_taxi.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       58 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/metrics.nblink
--rw-r--r--   0 runner    (1001) docker     (116)      382 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/pyfunc.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       58 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/pytorch.nblink
--rw-r--r--   0 runner    (1001) docker     (116)   160727 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/sample_metric.png
--rw-r--r--   0 runner    (1001) docker     (116)       58 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/sklearn.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       64 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/tensorflow.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       58 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sample/xgboost.nblink
--rw-r--r--   0 runner    (1001) docker     (116)       97 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/serve.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (116)      892 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/source/merlin.batch.rst
--rw-r--r--   0 runner    (1001) docker     (116)      301 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/source/merlin.docker.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/source/merlin.rst
--rw-r--r--   0 runner    (1001) docker     (116)       55 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/docs/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (116)      154 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sphinxcontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/docs/sphinxcontrib/confluencebuilder_nbsphinx/
--rw-r--r--   0 runner    (1001) docker     (116)     1036 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/docs/sphinxcontrib/confluencebuilder_nbsphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin/
--rw-r--r--   0 runner    (1001) docker     (116)     2959 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin/batch/
--rw-r--r--   0 runner    (1001) docker     (116)      584 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3689 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/batch/big_query_util.py
--rw-r--r--   0 runner    (1001) docker     (116)     4531 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/batch/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     2906 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/batch/job.py
--rw-r--r--   0 runner    (1001) docker     (116)     4136 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/batch/sink.py
--rw-r--r--   0 runner    (1001) docker     (116)     3089 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/batch/source.py
--rw-r--r--   0 runner    (1001) docker     (116)     8282 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin/docker/
--rw-r--r--   0 runner    (1001) docker     (116)      584 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/docker/docker.py
--rw-r--r--   0 runner    (1001) docker     (116)      889 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/docker/pyfunc.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)      665 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/docker/standard.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)     3057 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)     1568 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/environment.py
--rw-r--r--   0 runner    (1001) docker     (116)    13066 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/fluent.py
--rw-r--r--   0 runner    (1001) docker     (116)     5325 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/merlin.py
--rw-r--r--   0 runner    (1001) docker     (116)    54368 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     1916 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/resource_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1675 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/transformer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2797 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/util.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/validation.py
--rw-r--r--   0 runner    (1001) docker     (116)      607 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin/version.py
--rw-r--r--   0 runner    (1001) docker     (116)   484515 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/merlin_cli.gif
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      248 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4756 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       64 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      370 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1895 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      585 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/batch/
--rw-r--r--   0 runner    (1001) docker     (116)     8805 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/batch/big_query_util_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/batch/model/
--rw-r--r--   0 runner    (1001) docker     (116)      111 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/batch/model/env.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     5081 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/batch/sink_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     5647 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/batch/source_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     4329 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/batch_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     7021 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/cli_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    14499 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/client_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2580 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/docker/
--rw-r--r--   0 runner    (1001) docker     (116)     1028 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/docker/docker_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    16888 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/integration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/onnx-model-invalid/
--rw-r--r--   0 runner    (1001) docker     (116)     2246 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/onnx-model-invalid/invalid.onnx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/pyfunc-model-invalid/
--rw-r--r--   0 runner    (1001) docker     (116)      226 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/pyfunc-model-invalid/MLmodel
--rw-r--r--   0 runner    (1001) docker     (116)      108 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/pyfunc-model-invalid/conda.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    21513 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/pyfunc-model-invalid/invalid_model.pkl
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/pytorch-model-invalid/
--rw-r--r--   0 runner    (1001) docker     (116)    44673 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/pytorch-model-invalid/invalid.pt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/sklearn-model-invalid/
--rw-r--r--   0 runner    (1001) docker     (116)     5563 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/sklearn-model-invalid/invalid.joblib
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/
--rw-r--r--   0 runner    (1001) docker     (116)    63548 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/invalid_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/variables/
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/variables/variables.data-00000-of-00002
--rw-r--r--   0 runner    (1001) docker     (116)     1972 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/variables/variables.data-00001-of-00002
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/xgboost-model-invalid/
--rw-r--r--   0 runner    (1001) docker     (116)    25539 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/invalid-models/xgboost-model-invalid/invalid.bst
--rw-r--r--   0 runner    (1001) docker     (116)     6869 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/local_server_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    10659 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/merlin_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    26678 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/model_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1869 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/model_validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/onnx-model/
--rw-r--r--   0 runner    (1001) docker     (116)     2246 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/onnx-model/model.onnx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/pyfunc/
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/pyfunc/env.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    14756 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/pyfunc/model_1.bst
--rw-r--r--   0 runner    (1001) docker     (116)     5592 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/pyfunc/model_2.joblib
--rw-r--r--   0 runner    (1001) docker     (116)     6440 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/pyfunc_integration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/pytorch-model/
--rw-r--r--   0 runner    (1001) docker     (116)    44673 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/pytorch-model/model.pt
--rw-r--r--   0 runner    (1001) docker     (116)     1061 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/pytorch-model/model.py
--rw-r--r--   0 runner    (1001) docker     (116)      970 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/resource_request_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/sklearn-model/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/sklearn-model/.keep
--rw-r--r--   0 runner    (1001) docker     (116)     5538 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/sklearn-model/model.joblib
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/
--rw-r--r--   0 runner    (1001) docker     (116)    63548 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/variables/
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/variables/variables.data-00000-of-00002
--rw-r--r--   0 runner    (1001) docker     (116)     1972 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/variables/variables.data-00001-of-00002
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/transformer/
--rw-r--r--   0 runner    (1001) docker     (116)     4089 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/transformer/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (116)   249602 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/transformer/model.pt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/transformer/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      827 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1500 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/utils_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:18.000000 merlin-sdk-0.9.0.dev0/test/xgboost-model/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/xgboost-model/.keep
--rw-r--r--   0 runner    (1001) docker     (116)    25539 2020-12-16 03:15:07.000000 merlin-sdk-0.9.0.dev0/test/xgboost-model/model.bst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)      801 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      546 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      269 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (116)     1639 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/client/
+-rw-r--r--   0 runner    (1001) docker     (116)     2966 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/client/api/
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20720 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/alert_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29865 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/endpoint_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3958 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/environment_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7074 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25748 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/model_endpoints_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32579 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28640 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/prediction_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14728 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16375 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/secret_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16648 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api/version_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25083 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8097 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/client/models/
+-rw-r--r--   0 runner    (1001) docker     (116)     2345 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2639 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/alert_condition_metric_type.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2559 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/alert_condition_severity.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6179 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6486 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2601 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/endpoint_status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3530 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8693 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/environment.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2585 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3498 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8691 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9077 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/model_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6467 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/model_endpoint_alert.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6885 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/model_endpoint_alert_condition.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3971 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/model_endpoint_rule.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5031 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/model_endpoint_rule_destination.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10467 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8357 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6377 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config_bigquery_sink.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4706 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config_bigquery_source.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6078 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config_gcs_sink.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5288 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config_gcs_source.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5538 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3940 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_config_model_result.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7257 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/prediction_job_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8991 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5416 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2587 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2581 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/save_mode.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4023 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7804 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8474 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12460 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/models/version_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13183 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     1072 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (116)      633 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)      528 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)     3230 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2747 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      367 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      850 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      452 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/docs/sample/
+-rw-r--r--   0 runner    (1001) docker     (116)       94 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/batch_iris.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)       93 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/batch_taxi.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/metrics.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)      382 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       56 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/pyfunc.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/pytorch.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)   160727 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/sample_metric.png
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/sklearn.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/tensorflow.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sample/xgboost.nblink
+-rw-r--r--   0 runner    (1001) docker     (116)       97 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/serve.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (116)      892 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/source/merlin.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      301 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/source/merlin.docker.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1559 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/source/merlin.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/docs/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (116)      154 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sphinxcontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/docs/sphinxcontrib/confluencebuilder_nbsphinx/
+-rw-r--r--   0 runner    (1001) docker     (116)     1036 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/docs/sphinxcontrib/confluencebuilder_nbsphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/merlin/
+-rw-r--r--   0 runner    (1001) docker     (116)     2959 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/merlin/batch/
+-rw-r--r--   0 runner    (1001) docker     (116)      584 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3689 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/batch/big_query_util.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4531 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/batch/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2906 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/batch/job.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4136 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/batch/sink.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3089 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/batch/source.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8283 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/merlin/docker/
+-rw-r--r--   0 runner    (1001) docker     (116)      584 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1753 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (116)      889 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/docker/pyfunc.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (116)      665 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/docker/standard.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (116)     3057 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1568 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/environment.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13066 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5325 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/merlin.py
+-rw-r--r--   0 runner    (1001) docker     (116)    55641 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1916 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1675 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2797 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/util.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2174 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/validation.py
+-rw-r--r--   0 runner    (1001) docker     (116)      602 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)   484515 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/merlin_cli.gif
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2021-01-08 09:14:18.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4756 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-08 09:14:18.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2021-01-08 09:14:18.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      370 2021-01-08 09:14:18.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2021-01-08 09:14:18.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-08 09:14:18.000000 merlin-sdk-0.9.1/merlin_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1895 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (116)      585 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (116)     8805 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/batch/big_query_util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/batch/model/
+-rw-r--r--   0 runner    (1001) docker     (116)      111 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/batch/model/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     5081 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/batch/sink_unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5647 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/batch/source_unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4329 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/batch_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7021 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/cli_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14499 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2580 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/docker/
+-rw-r--r--   0 runner    (1001) docker     (116)     1028 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/docker/docker_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16888 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/integration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/onnx-model-invalid/
+-rw-r--r--   0 runner    (1001) docker     (116)     2246 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/onnx-model-invalid/invalid.onnx
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/pyfunc-model-invalid/
+-rw-r--r--   0 runner    (1001) docker     (116)      226 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/pyfunc-model-invalid/MLmodel
+-rw-r--r--   0 runner    (1001) docker     (116)      108 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/pyfunc-model-invalid/conda.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    21513 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/pyfunc-model-invalid/invalid_model.pkl
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/pytorch-model-invalid/
+-rw-r--r--   0 runner    (1001) docker     (116)    44673 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/pytorch-model-invalid/invalid.pt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/sklearn-model-invalid/
+-rw-r--r--   0 runner    (1001) docker     (116)     5563 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/sklearn-model-invalid/invalid.joblib
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/
+-rw-r--r--   0 runner    (1001) docker     (116)    63548 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/invalid_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/variables/
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/variables/variables.data-00000-of-00002
+-rw-r--r--   0 runner    (1001) docker     (116)     1972 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/variables/variables.data-00001-of-00002
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/invalid-models/xgboost-model-invalid/
+-rw-r--r--   0 runner    (1001) docker     (116)    25539 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/invalid-models/xgboost-model-invalid/invalid.bst
+-rw-r--r--   0 runner    (1001) docker     (116)     6869 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/local_server_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10659 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/merlin_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26837 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1869 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/model_validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/onnx-model/
+-rw-r--r--   0 runner    (1001) docker     (116)     2246 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/onnx-model/model.onnx
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/pyfunc/
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/pyfunc/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    14756 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/pyfunc/model_1.bst
+-rw-r--r--   0 runner    (1001) docker     (116)     5592 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/pyfunc/model_2.joblib
+-rw-r--r--   0 runner    (1001) docker     (116)     6440 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/pyfunc_integration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/pytorch-model/
+-rw-r--r--   0 runner    (1001) docker     (116)    44673 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/pytorch-model/model.pt
+-rw-r--r--   0 runner    (1001) docker     (116)     1061 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/pytorch-model/model.py
+-rw-r--r--   0 runner    (1001) docker     (116)      970 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/resource_request_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/sklearn-model/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/sklearn-model/.keep
+-rw-r--r--   0 runner    (1001) docker     (116)     5538 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/sklearn-model/model.joblib
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/tensorflow-model/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/tensorflow-model/1/
+-rw-r--r--   0 runner    (1001) docker     (116)    63548 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/tensorflow-model/1/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/tensorflow-model/1/variables/
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/tensorflow-model/1/variables/variables.data-00000-of-00002
+-rw-r--r--   0 runner    (1001) docker     (116)     1972 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/tensorflow-model/1/variables/variables.data-00001-of-00002
+-rw-r--r--   0 runner    (1001) docker     (116)      333 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/tensorflow-model/1/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/transformer/
+-rw-r--r--   0 runner    (1001) docker     (116)     4089 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/transformer/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3425 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (116)   249602 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/transformer/model.pt
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/transformer/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      827 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1500 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/utils_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:19.000000 merlin-sdk-0.9.1/test/xgboost-model/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/xgboost-model/.keep
+-rw-r--r--   0 runner    (1001) docker     (116)    25539 2021-01-08 09:14:07.000000 merlin-sdk-0.9.1/test/xgboost-model/model.bst
```

### Comparing `merlin-sdk-0.9.0.dev0/.gitignore` & `merlin-sdk-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/Makefile` & `merlin-sdk-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/README.md` & `merlin-sdk-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/__init__.py` & `merlin-sdk-0.9.1/client/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/__init__.py` & `merlin-sdk-0.9.1/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/alert_api.py` & `merlin-sdk-0.9.1/client/api/alert_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/endpoint_api.py` & `merlin-sdk-0.9.1/client/api/endpoint_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/environment_api.py` & `merlin-sdk-0.9.1/client/api/environment_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/log_api.py` & `merlin-sdk-0.9.1/client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/model_endpoints_api.py` & `merlin-sdk-0.9.1/client/api/model_endpoints_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/models_api.py` & `merlin-sdk-0.9.1/client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/prediction_jobs_api.py` & `merlin-sdk-0.9.1/client/api/prediction_jobs_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/project_api.py` & `merlin-sdk-0.9.1/client/api/project_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/secret_api.py` & `merlin-sdk-0.9.1/client/api/secret_api.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/api/version_api.py` & `merlin-sdk-0.9.1/client/api/version_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.models_model_id_versions_get(model_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int model_id: (required)
+        :param int limit:
+        :param str cursor:
+        :param str search:
         :return: list[Version]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.models_model_id_versions_get_with_http_info(model_id, **kwargs)  # noqa: E501
@@ -60,20 +63,23 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.models_model_id_versions_get_with_http_info(model_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int model_id: (required)
+        :param int limit:
+        :param str cursor:
+        :param str search:
         :return: list[Version]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['model_id']  # noqa: E501
+        all_params = ['model_id', 'limit', 'cursor', 'search']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -92,14 +98,20 @@
         collection_formats = {}
 
         path_params = {}
         if 'model_id' in params:
             path_params['model_id'] = params['model_id']  # noqa: E501
 
         query_params = []
+        if 'limit' in params:
+            query_params.append(('limit', params['limit']))  # noqa: E501
+        if 'cursor' in params:
+            query_params.append(('cursor', params['cursor']))  # noqa: E501
+        if 'search' in params:
+            query_params.append(('search', params['search']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -200,14 +212,111 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='Version',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def models_model_id_versions_version_id_get(self, model_id, version_id, **kwargs):  # noqa: E501
+        """Get version by ID from model  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.models_model_id_versions_version_id_get(model_id, version_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int model_id: (required)
+        :param int version_id: (required)
+        :return: Version
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.models_model_id_versions_version_id_get_with_http_info(model_id, version_id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.models_model_id_versions_version_id_get_with_http_info(model_id, version_id, **kwargs)  # noqa: E501
+            return data
+
+    def models_model_id_versions_version_id_get_with_http_info(self, model_id, version_id, **kwargs):  # noqa: E501
+        """Get version by ID from model  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.models_model_id_versions_version_id_get_with_http_info(model_id, version_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int model_id: (required)
+        :param int version_id: (required)
+        :return: Version
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['model_id', 'version_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method models_model_id_versions_version_id_get" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'model_id' is set
+        if ('model_id' not in params or
+                params['model_id'] is None):
+            raise ValueError("Missing the required parameter `model_id` when calling `models_model_id_versions_version_id_get`")  # noqa: E501
+        # verify the required parameter 'version_id' is set
+        if ('version_id' not in params or
+                params['version_id'] is None):
+            raise ValueError("Missing the required parameter `version_id` when calling `models_model_id_versions_version_id_get`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'model_id' in params:
+            path_params['model_id'] = params['model_id']  # noqa: E501
+        if 'version_id' in params:
+            path_params['version_id'] = params['version_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # Authentication setting
+        auth_settings = ['Bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/models/{model_id}/versions/{version_id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='Version',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `merlin-sdk-0.9.0.dev0/client/api_client.py` & `merlin-sdk-0.9.1/client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 """
     Merlin
 
     API Guide for accessing Merlin's model management, deployment, and serving functionalities  # noqa: E501
 
     OpenAPI spec version: 0.7.0
-
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import datetime
 import json
@@ -326,21 +326,21 @@
                                    path_params, query_params, header_params,
                                    body, post_params, files,
                                    response_type, auth_settings,
                                    _return_http_data_only, collection_formats,
                                    _preload_content, _request_timeout)
         else:
             thread = self.pool.apply_async(self.__call_api, (resource_path,
-                                           method, path_params, query_params,
-                                           header_params, body,
-                                           post_params, files,
-                                           response_type, auth_settings,
-                                           _return_http_data_only,
-                                           collection_formats,
-                                           _preload_content, _request_timeout))
+                                                             method, path_params, query_params,
+                                                             header_params, body,
+                                                             post_params, files,
+                                                             response_type, auth_settings,
+                                                             _return_http_data_only,
+                                                             collection_formats,
+                                                             _preload_content, _request_timeout))
         return thread
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
```

### Comparing `merlin-sdk-0.9.0.dev0/client/configuration.py` & `merlin-sdk-0.9.1/client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
     Merlin
 
     API Guide for accessing Merlin's model management, deployment, and serving functionalities  # noqa: E501
 
     OpenAPI spec version: 0.7.0
-
+    
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -201,15 +201,15 @@
 
         :param identifier: The identifier of apiKey.
         :return: The token for api key authentication.
         """
 
         if self.refresh_api_key_hook:
             self.refresh_api_key_hook(self)
-
+        
         key = self.api_key.get(identifier)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
```

### Comparing `merlin-sdk-0.9.0.dev0/client/models/__init__.py` & `merlin-sdk-0.9.1/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/alert_condition_metric_type.py` & `merlin-sdk-0.9.1/client/models/alert_condition_metric_type.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/alert_condition_severity.py` & `merlin-sdk-0.9.1/client/models/alert_condition_severity.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/config.py` & `merlin-sdk-0.9.1/client/models/config.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/container.py` & `merlin-sdk-0.9.1/client/models/container.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/endpoint_status.py` & `merlin-sdk-0.9.1/client/models/endpoint_status.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/env_var.py` & `merlin-sdk-0.9.1/client/models/env_var.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/environment.py` & `merlin-sdk-0.9.1/client/models/environment.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/file_format.py` & `merlin-sdk-0.9.1/client/models/file_format.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/label.py` & `merlin-sdk-0.9.1/client/models/label.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/model.py` & `merlin-sdk-0.9.1/client/models/model.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/model_endpoint.py` & `merlin-sdk-0.9.1/client/models/model_endpoint.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/model_endpoint_alert.py` & `merlin-sdk-0.9.1/client/models/model_endpoint_alert.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/model_endpoint_alert_condition.py` & `merlin-sdk-0.9.1/client/models/model_endpoint_alert_condition.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/model_endpoint_rule.py` & `merlin-sdk-0.9.1/client/models/model_endpoint_rule.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/model_endpoint_rule_destination.py` & `merlin-sdk-0.9.1/client/models/model_endpoint_rule_destination.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job.py` & `merlin-sdk-0.9.1/client/models/prediction_job.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_bigquery_sink.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config_bigquery_sink.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_bigquery_source.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config_bigquery_source.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_gcs_sink.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config_gcs_sink.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_gcs_source.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config_gcs_source.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_model.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config_model.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_config_model_result.py` & `merlin-sdk-0.9.1/client/models/prediction_job_config_model_result.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/prediction_job_resource_request.py` & `merlin-sdk-0.9.1/client/models/prediction_job_resource_request.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/project.py` & `merlin-sdk-0.9.1/client/models/project.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/resource_request.py` & `merlin-sdk-0.9.1/client/models/resource_request.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/result_type.py` & `merlin-sdk-0.9.1/client/models/result_type.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/save_mode.py` & `merlin-sdk-0.9.1/client/models/save_mode.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/secret.py` & `merlin-sdk-0.9.1/client/models/secret.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/transformer.py` & `merlin-sdk-0.9.1/client/models/transformer.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/version.py` & `merlin-sdk-0.9.1/client/models/version.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/models/version_endpoint.py` & `merlin-sdk-0.9.1/client/models/version_endpoint.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/client/rest.py` & `merlin-sdk-0.9.1/client/rest.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/Dockerfile` & `merlin-sdk-0.9.1/docs/Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/Makefile` & `merlin-sdk-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/README.md` & `merlin-sdk-0.9.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/conf.py` & `merlin-sdk-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/getting_started.rst` & `merlin-sdk-0.9.1/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/introduction.rst` & `merlin-sdk-0.9.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/sample/sample_metric.png` & `merlin-sdk-0.9.1/docs/sample/sample_metric.png`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/source/merlin.batch.rst` & `merlin-sdk-0.9.1/docs/source/merlin.batch.rst`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/source/merlin.rst` & `merlin-sdk-0.9.1/docs/source/merlin.rst`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/docs/sphinxcontrib/confluencebuilder_nbsphinx/__init__.py` & `merlin-sdk-0.9.1/docs/sphinxcontrib/confluencebuilder_nbsphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/__init__.py` & `merlin-sdk-0.9.1/merlin/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/batch/__init__.py` & `merlin-sdk-0.9.1/merlin/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/batch/big_query_util.py` & `merlin-sdk-0.9.1/merlin/batch/big_query_util.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/batch/config.py` & `merlin-sdk-0.9.1/merlin/batch/config.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/batch/job.py` & `merlin-sdk-0.9.1/merlin/batch/job.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/batch/sink.py` & `merlin-sdk-0.9.1/merlin/batch/sink.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/batch/source.py` & `merlin-sdk-0.9.1/merlin/batch/source.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/client.py` & `merlin-sdk-0.9.1/merlin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         """
         env_list = self._env_api.environments_get()
         envs = []
         for env in env_list:
             envs.append(Environment(env))
         return envs
 
+
     def get_environment(self, env_name: str) -> Optional[Environment]:
         """
         Get environment for given env name
 
         :return: Environment or None
         """
         env_list = self._env_api.environments_get()
```

### Comparing `merlin-sdk-0.9.0.dev0/merlin/docker/__init__.py` & `merlin-sdk-0.9.1/merlin/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/docker/docker.py` & `merlin-sdk-0.9.1/merlin/docker/docker.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/docker/pyfunc.Dockerfile` & `merlin-sdk-0.9.1/merlin/docker/pyfunc.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/docker/standard.Dockerfile` & `merlin-sdk-0.9.1/merlin/docker/standard.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/endpoint.py` & `merlin-sdk-0.9.1/merlin/endpoint.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/environment.py` & `merlin-sdk-0.9.1/merlin/environment.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/fluent.py` & `merlin-sdk-0.9.1/merlin/fluent.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/merlin.py` & `merlin-sdk-0.9.1/merlin/merlin.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/model.py` & `merlin-sdk-0.9.1/merlin/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import pathlib
 import re
 from abc import abstractmethod
 from datetime import datetime
 from enum import Enum
 from time import sleep
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, Tuple
 
 import docker
 import mlflow
 import numpy
 import pandas
 import pyprind
 from docker import APIClient
@@ -44,14 +44,15 @@
 from merlin.resource_request import ResourceRequest
 from merlin.transformer import Transformer
 from merlin.util import autostr, download_files_from_gcs, guess_mlp_ui_url, valid_name_check
 from merlin.validation import validate_model_dir
 from merlin.version import VERSION
 
 DEFAULT_MODEL_PATH = "model"
+DEFAULT_MODEL_VERSION_LIMIT = 50
 V1 = "v1"
 PREDICTION_JOB = "PredictionJob"
 
 
 @autostr
 class Project:
     def __init__(self, project: client.Project, mlp_url: str,
@@ -157,24 +158,25 @@
         :return:
         """
         secret_api = SecretApi(self._api_client)
         secret_api.projects_project_id_secrets_post(project_id=int(self.id),
                                                     body={
                                                         "name": name,
                                                         "data": data
-                                                    })
+        })
 
     def list_secret(self) -> List[str]:
         """
         List all secret name within the project
 
         :return:
         """
         secret_api = SecretApi(self._api_client)
-        secrets = secret_api.projects_project_id_secrets_get(project_id=int(self.id))
+        secrets = secret_api.projects_project_id_secrets_get(
+            project_id=int(self.id))
         secret_names = []
         for s in secrets:
             secret_names.append(s.name)
         return secret_names
 
     def update_secret(self, name: str, data: str):
         """
@@ -184,19 +186,20 @@
         :param data: new secret data
         :return:
         """
         secret_api = SecretApi(self._api_client)
         match = self._find_secret(name)
 
         secret_api.projects_project_id_secrets_secret_id_patch(project_id=int(self.id),
-                                                               secret_id=int(match.id),
+                                                               secret_id=int(
+                                                                   match.id),
                                                                body={
                                                                    "name": name,
                                                                    "data": data
-                                                               })
+        })
 
     def delete_secret(self, name: str):
         """
         Delete secret with given name
 
         :param name: secret to be removed
         :return:
@@ -205,21 +208,23 @@
         match = self._find_secret(name)
 
         secret_api.projects_project_id_secrets_secret_id_delete(project_id=int(self.id),
                                                                 secret_id=int(match.id))
 
     def _find_secret(self, name: str):
         secret_api = SecretApi(self._api_client)
-        secrets = secret_api.projects_project_id_secrets_get(project_id=int(self.id))
+        secrets = secret_api.projects_project_id_secrets_get(
+            project_id=int(self.id))
         match = None
         for s in secrets:
             if s.name == name:
                 match = s
         if match is None:
-            raise ValueError(f"unable to find secret {name} in project {self.name}")
+            raise ValueError(
+                f"unable to find secret {name} in project {self.name}")
         return match
 
 
 class ModelType(Enum):
     """
     Model type supported by merlin
     """
@@ -329,20 +334,40 @@
     def list_version(self) -> List['ModelVersion']:
         """
         List all version of the model
         List all version of the model
 
         :return: list of ModelVersion
         """
+        result: List['ModelVersion'] = []
+        versions, cursor = self._list_version_pagination()
+        result = result + versions
+        while cursor != "":
+            versions, cursor = self._list_version_pagination(cursor=cursor)
+            result = result + versions
+        return result
+
+    def _list_version_pagination(self, limit=DEFAULT_MODEL_VERSION_LIMIT, cursor="", search="") -> Tuple[List['ModelVersion'], str]:
+        """
+        List version of the model with pagination
+        :param limit: integer, max number of rows will be returned
+        :param cursor: text, indicator where backend will start to look up the data
+        :param search: text
+
+        :return: list of ModelVersion
+        :return: next cursor to fetch next page of version
+        """
         version_api = VersionApi(self._api_client)
-        v_list = version_api.models_model_id_versions_get(int(self.id))
+        (versions, _, headers) = version_api.models_model_id_versions_get_with_http_info(
+            int(self.id), limit=limit, cursor=cursor, search=search)
+        next_cursor = headers.get("Next-Cursor") or ""
         result = []
-        for v in v_list:
+        for v in versions:
             result.append(ModelVersion(v, self, self._api_client))
-        return result
+        return result, next_cursor
 
     def new_model_version(self) -> 'ModelVersion':
         """
         Create a new version of this model
 
         :return:  new ModelVersion
         """
@@ -518,24 +543,24 @@
             }, model_id=int(self.id))
             return ModelEndpoint(ep)
         else:
             def_model_endpoint = self.endpoint
             # GET and PUT
             ep = model_endpoint_api \
                 .models_model_id_endpoints_model_endpoint_id_get(
-                model_id=int(self.id),
-                model_endpoint_id=def_model_endpoint.id)
+                    model_id=int(self.id),
+                    model_endpoint_id=def_model_endpoint.id)
             ep.rule.destinations[0] \
                 .version_endpoint_id = def_version_endpoint.id
             ep.rule.destinations[0].weight = 100
             ep = model_endpoint_api \
                 .models_model_id_endpoints_model_endpoint_id_put(
-                model_id=int(self.id),
-                model_endpoint_id=def_model_endpoint.id,
-                body=ep.to_dict())
+                    model_id=int(self.id),
+                    model_endpoint_id=def_model_endpoint.id,
+                    body=ep.to_dict())
 
         return ModelEndpoint(ep)
 
 
 @autostr
 class ModelVersion:
     """
@@ -581,15 +606,15 @@
         environment
 
         :return: Endpoint or None
         """
         endpoint_api = EndpointApi(self._api_client)
         ep_list = endpoint_api. \
             models_model_id_versions_version_id_endpoint_get(
-            model_id=self.model.id, version_id=self.id)
+                model_id=self.model.id, version_id=self.id)
 
         for endpoint in ep_list:
             if endpoint.environment.is_default:
                 return VersionEndpoint(endpoint)
 
         return None
 
@@ -792,15 +817,16 @@
 
         :param model_instance: instance of python function model
         :param conda_env: path to conda env.yaml file
         :param code_dir: additional code directory that will be loaded with ModelType.PYFUNC model
         :param artifacts: dictionary of artifact that will be stored together with the model. This will be passed to PythonModel.initialize. Example: {"config" : "config/staging.yaml"}
         """
         if self._model.type != ModelType.PYFUNC and self._model.type != ModelType.PYFUNC_V2:
-            raise ValueError("log_pyfunc_model is only for PyFunc and PyFuncV2 model")
+            raise ValueError(
+                "log_pyfunc_model is only for PyFunc and PyFuncV2 model")
 
         validate_model_dir(self._model.type, ModelType.PYFUNC, None)
         mlflow.pyfunc.log_model(DEFAULT_MODEL_PATH,
                                 python_model=model_instance,
                                 code_path=code_dir,
                                 conda_env=conda_env,
                                 artifacts=artifacts)
@@ -816,16 +842,15 @@
             raise ValueError("log_pytorch_model is only for PyTorch model")
 
         validate_model_dir(self._model.type, ModelType.PYTORCH, model_dir)
         mlflow.log_artifacts(model_dir, DEFAULT_MODEL_PATH)
         if model_class_name is not None:
             version_api = VersionApi(self._api_client)
             version_api.models_model_id_versions_version_id_patch(
-                int(self.model.id), int(self.id), body=
-                {"properties": {
+                int(self.model.id), int(self.id), body={"properties": {
                     "pytorch_class_name": model_class_name
                 }
                 })
 
     def log_model(self, model_dir=None):
         """
         Upload model to artifact storage.
@@ -848,15 +873,15 @@
         Return all endpoint deployment for this particular model version
 
         :return: List of VersionEndpoint
         """
         endpoint_api = EndpointApi(self._api_client)
         ep_list = endpoint_api. \
             models_model_id_versions_version_id_endpoint_get(
-            model_id=self.model.id, version_id=self.id)
+                model_id=self.model.id, version_id=self.id)
 
         endpoints = []
         for ep in ep_list:
             endpoints.append(VersionEndpoint(ep))
         return endpoints
 
     def deploy(self, environment_name: str = None,
@@ -911,19 +936,21 @@
             if env_vars is not None:
                 if not isinstance(env_vars, dict):
                     raise ValueError(
                         f"env_vars should be dictionary, got: {type(env_vars)}")
 
                 if len(env_vars) > 0:
                     for name, value in env_vars.items():
-                        target_env_vars.append(client.EnvVar(str(name), str(value)))
+                        target_env_vars.append(
+                            client.EnvVar(str(name), str(value)))
 
         target_transformer = None
         if transformer is not None:
-            target_transformer = self.create_transformer_spec(transformer, target_env_name)
+            target_transformer = self.create_transformer_spec(
+                transformer, target_env_name)
 
         model = self._model
         endpoint_api = EndpointApi(self._api_client)
         endpoint = client.VersionEndpoint(environment_name=target_env_name,
                                           resource_request=target_resource_request,
                                           env_vars=target_env_vars,
                                           transformer=target_transformer)
@@ -934,17 +961,17 @@
         bar = pyprind.ProgBar(100, track_time=True,
                               title=f"Deploying model {model.name} version "
                                     f"{self.id}")
 
         while endpoint.status == "pending":
             endpoint = endpoint_api \
                 .models_model_id_versions_version_id_endpoint_endpoint_id_get(
-                model_id=int(model.id),
-                version_id=int(self.id),
-                endpoint_id=endpoint.id)
+                    model_id=int(model.id),
+                    version_id=int(self.id),
+                    endpoint_id=endpoint.id)
             bar.update()
             sleep(5)
         bar.stop()
 
         if endpoint.status != "running":
             raise ValueError(
                 f"Failed deploying model {model.name} version {self.id}")
@@ -981,15 +1008,16 @@
         if transformer.env_vars is not None:
             if not isinstance(transformer.env_vars, dict):
                 raise ValueError(
                     f"transformer.env_vars should be dictionary, got: {type(transformer.env_vars)}")
 
             if len(transformer.env_vars) > 0:
                 for name, value in transformer.env_vars.items():
-                    target_env_vars.append(client.EnvVar(str(name), str(value)))
+                    target_env_vars.append(
+                        client.EnvVar(str(name), str(value)))
 
         return client.Transformer(
             transformer.enabled, transformer.image,
             transformer.command, transformer.args,
             target_resource_request, target_env_vars)
 
     def undeploy(self, environment_name: str = None):
@@ -1035,15 +1063,16 @@
         Create and run prediction job with given config using this model version
 
         :param sync: boolean to set synchronicity of job. The default is set to True.
         :param job_config: prediction job config
         :return: prediction job
         """
         if self.model.type != ModelType.PYFUNC_V2:
-            raise ValueError(f"model type is not supported for prediction job: {self.model.type}")
+            raise ValueError(
+                f"model type is not supported for prediction job: {self.model.type}")
 
         job_cfg = client.PredictionJobConfig(version=V1, kind=PREDICTION_JOB, model={
             "type": self.model.type.value.upper(),
             "uri": os.path.join(self.artifact_uri, DEFAULT_MODEL_PATH),
             "result": {
                 "type": job_config.result_type.value,
                 "item_type": job_config.item_type.value
@@ -1145,38 +1174,43 @@
         :return:
         """
         if tmp_dir is None:
             tmp_dir = "/tmp"
         artifact_path = f"{tmp_dir}/merlin/{self.model.project.name}/{self.model.name}/{self.id}/{DEFAULT_MODEL_PATH}"
         pathlib.Path(artifact_path).mkdir(parents=True, exist_ok=True)
         if len(os.listdir(artifact_path)) < 1:
-            print(f"Downloading model artifact for model {self.model.name} version {self.id}")
+            print(
+                f"Downloading model artifact for model {self.model.name} version {self.id}")
             self.download_artifact(artifact_path)
 
         # stop all previous containers to avoid port conflict
         client = docker.from_env()
         if kill_existing_server:
-            started_containers = client.containers.list(filters={"name": self._container_name()})
+            started_containers = client.containers.list(
+                filters={"name": self._container_name()})
             for started_container in started_containers:
                 print(f"Stopping model server {started_container.name}")
                 started_container.remove(force=True)
 
         model_type = self.model.type
         if model_type == ModelType.PYFUNC:
-            self._run_pyfunc_local_server(artifact_path, env_vars, port, pyfunc_base_image)
+            self._run_pyfunc_local_server(
+                artifact_path, env_vars, port, pyfunc_base_image)
             return
 
         if model_type == ModelType.TENSORFLOW \
                 or model_type == ModelType.XGBOOST \
                 or model_type == ModelType.SKLEARN \
                 or model_type == ModelType.PYTORCH:
-            self._run_standard_model_local_server(artifact_path, env_vars, port, build_image)
+            self._run_standard_model_local_server(
+                artifact_path, env_vars, port, build_image)
             return
 
-        raise ValueError(f"running local model server is not supported for model type: {model_type}")
+        raise ValueError(
+            f"running local model server is not supported for model type: {model_type}")
 
     def _create_launch_command(self):
         model_type = self.model.type
         print(f"model type: {model_type}")
         if model_type == ModelType.SKLEARN or model_type == ModelType.XGBOOST or model_type == ModelType.PYTORCH:
             return f"--port=9000 --rest_api_port=8080 --model_name={self.model.name}-{self.id} --model_dir=/mnt/models"
 
@@ -1199,15 +1233,16 @@
                 print(f"Building {self.model.type} image: {image_tag}")
                 logs = apiClient.build(path=artifact_path,
                                        tag=image_tag,
                                        buildargs={
                                            "BASE_IMAGE": image_name,
                                            "MODEL_PATH": artifact_path
                                        },
-                                       dockerfile=os.path.basename(dockerfile_path),
+                                       dockerfile=os.path.basename(
+                                           dockerfile_path),
                                        decode=True
                                        )
                 self._wait_build_complete(logs)
                 image_name = image_tag
 
             print(f"Starting model server {container_name} at port: {port}")
             print(f"This process might take several minutes to complete")
@@ -1311,15 +1346,16 @@
 
     def predict(self, model_input, **kwargs):
         if self._use_kwargs_infer:
             try:
                 return self.infer(model_input, **kwargs)
             except TypeError as e:
                 if "infer() got an unexpected keyword argument" in str(e):
-                    print('Fallback to the old infer() method, got TypeError exception: {}'.format(e))
+                    print(
+                        'Fallback to the old infer() method, got TypeError exception: {}'.format(e))
                     self._use_kwargs_infer = False
                 else:
                     raise e
 
         return self.infer(model_input)
 
     @abstractmethod
```

### Comparing `merlin-sdk-0.9.0.dev0/merlin/resource_request.py` & `merlin-sdk-0.9.1/merlin/resource_request.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/transformer.py` & `merlin-sdk-0.9.1/merlin/transformer.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/util.py` & `merlin-sdk-0.9.1/merlin/util.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/validation.py` & `merlin-sdk-0.9.1/merlin/validation.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin/version.py` & `merlin-sdk-0.9.1/merlin/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = "0.9.0.dev0"
+VERSION = "0.9.1"
```

### Comparing `merlin-sdk-0.9.0.dev0/merlin_cli.gif` & `merlin-sdk-0.9.1/merlin_cli.gif`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/merlin_sdk.egg-info/SOURCES.txt` & `merlin-sdk-0.9.1/merlin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/setup.py` & `merlin-sdk-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/__init__.py` & `merlin-sdk-0.9.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/batch/big_query_util_test.py` & `merlin-sdk-0.9.1/test/batch/big_query_util_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/batch/sink_unit_test.py` & `merlin-sdk-0.9.1/test/batch/sink_unit_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/batch/source_unit_test.py` & `merlin-sdk-0.9.1/test/batch/source_unit_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/batch_integration_test.py` & `merlin-sdk-0.9.1/test/batch_integration_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/cli_integration_test.py` & `merlin-sdk-0.9.1/test/cli_integration_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/client_test.py` & `merlin-sdk-0.9.1/test/client_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/conftest.py` & `merlin-sdk-0.9.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/docker/docker_test.py` & `merlin-sdk-0.9.1/test/docker/docker_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/integration_test.py` & `merlin-sdk-0.9.1/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/onnx-model-invalid/invalid.onnx` & `merlin-sdk-0.9.1/test/invalid-models/onnx-model-invalid/invalid.onnx`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/pyfunc-model-invalid/invalid_model.pkl` & `merlin-sdk-0.9.1/test/invalid-models/pyfunc-model-invalid/invalid_model.pkl`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/pytorch-model-invalid/invalid.pt` & `merlin-sdk-0.9.1/test/invalid-models/pytorch-model-invalid/invalid.pt`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/sklearn-model-invalid/invalid.joblib` & `merlin-sdk-0.9.1/test/invalid-models/sklearn-model-invalid/invalid.joblib`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/invalid_model.pb` & `merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/invalid_model.pb`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/tensorflow-model-invalid/1/variables/variables.data-00001-of-00002` & `merlin-sdk-0.9.1/test/invalid-models/tensorflow-model-invalid/1/variables/variables.data-00001-of-00002`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/invalid-models/xgboost-model-invalid/invalid.bst` & `merlin-sdk-0.9.1/test/invalid-models/xgboost-model-invalid/invalid.bst`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/local_server_test.py` & `merlin-sdk-0.9.1/test/local_server_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/merlin_test.py` & `merlin-sdk-0.9.1/test/merlin_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/model_test.py` & `merlin-sdk-0.9.1/test/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,47 +422,49 @@
         assert j.name == job_1.name
 
 class TestModel:
     v1 = cl.Version(id=1, model_id=1)
     v2 = cl.Version(id=2, model_id=1)
 
     @responses.activate
-    def test_get_version(self, model):
-        responses.add("GET", "/v1/models/1/versions",
-                      body=json.dumps([self.v1.to_dict(), self.v2.to_dict()]),
+    def test_list_version(self, model):
+        responses.add("GET", "/v1/models/1/versions?limit=50&cursor=&search=",
+                      match_querystring=True,
+                      body=json.dumps([self.v1.to_dict()]),
                       status=200,
+                      adding_headers={"Next-Cursor": "abcdef"},
                       content_type='application/json')
-        v = model.get_version(1)
-        assert v.id == 1
-        assert model.get_version(3) is None
+        responses.add("GET", "/v1/models/1/versions?limit=50&cursor=abcdef&search=",
+                      match_querystring=True,
+                      body=json.dumps([self.v2.to_dict()]),
+                      status=200,
+                      content_type='application/json')
+        versions = model.list_version()
+        assert len(versions) == 2
+        assert versions[0].id == 1
+        assert versions[1].id == 2
 
 
         @responses.activate
-        def test_endpoint(self, model):
-            responses.add("GET", '/v1/models/1/endpoints',
-                          body=json.dumps([mdl_endpoint_2.to_dict()]),
-                          status=200,
-                          content_type='application/json')
-
-            ep = model.endpoint
-            assert ep is None
-            responses.reset()
-
+        def test_list_endpoint(self, model):
             responses.add("GET", '/v1/models/1/endpoints',
                           body=json.dumps(
                               [mdl_endpoint_1.to_dict(),
                                mdl_endpoint_2.to_dict()]),
                           status=200,
                           content_type='application/json')
 
-            ep = model.endpoint
-            assert ep.id == str(mdl_endpoint_1.id)
-            assert ep.status.value == mdl_endpoint_1.status
-            assert ep.environment_name == mdl_endpoint_1.environment_name
-            assert ep.url.startswith(f"http://{mdl_endpoint_1.url}")
+            endpoints = model.list_endpoint()
+            assert len(endpoints) == 2
+            assert endpoints[0].id == str(mdl_endpoint_1.id)
+            assert endpoints[1].id == str(mdl_endpoint_2.id)
+
+            v = model.get_version(1)
+            assert v.id == 1
+            assert model.get_version(3) is None
 
         @responses.activate
         def test_list_endpoint(self, model):
             responses.add("GET", '/v1/models/1/endpoints',
                           body=json.dumps(
                               [mdl_endpoint_1.to_dict(),
                                mdl_endpoint_2.to_dict()]),
```

### Comparing `merlin-sdk-0.9.0.dev0/test/model_validation_test.py` & `merlin-sdk-0.9.1/test/model_validation_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/onnx-model/model.onnx` & `merlin-sdk-0.9.1/test/onnx-model/model.onnx`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/pyfunc/model_1.bst` & `merlin-sdk-0.9.1/test/pyfunc/model_1.bst`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/pyfunc/model_2.joblib` & `merlin-sdk-0.9.1/test/pyfunc/model_2.joblib`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/pyfunc_integration_test.py` & `merlin-sdk-0.9.1/test/pyfunc_integration_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/pytorch-model/model.pt` & `merlin-sdk-0.9.1/test/pytorch-model/model.pt`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/pytorch-model/model.py` & `merlin-sdk-0.9.1/test/pytorch-model/model.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/resource_request_test.py` & `merlin-sdk-0.9.1/test/resource_request_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/sklearn-model/model.joblib` & `merlin-sdk-0.9.1/test/sklearn-model/model.joblib`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/saved_model.pb` & `merlin-sdk-0.9.1/test/tensorflow-model/1/saved_model.pb`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/tensorflow-model/1/variables/variables.data-00001-of-00002` & `merlin-sdk-0.9.1/test/tensorflow-model/1/variables/variables.data-00001-of-00002`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/transformer/cifar10.py` & `merlin-sdk-0.9.1/test/transformer/cifar10.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/transformer/input.json` & `merlin-sdk-0.9.1/test/transformer/input.json`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/transformer/model.pt` & `merlin-sdk-0.9.1/test/transformer/model.pt`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/utils.py` & `merlin-sdk-0.9.1/test/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/utils_unit_test.py` & `merlin-sdk-0.9.1/test/utils_unit_test.py`

 * *Files identical despite different names*

### Comparing `merlin-sdk-0.9.0.dev0/test/xgboost-model/model.bst` & `merlin-sdk-0.9.1/test/xgboost-model/model.bst`

 * *Files identical despite different names*

