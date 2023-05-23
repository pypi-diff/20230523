# Comparing `tmp/gordo-5.0.1.tar.gz` & `tmp/gordo-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gordo-5.0.1.tar", last modified: Mon May 15 11:34:01 2023, max compression
+gzip compressed data, was "gordo-5.0.2.tar", last modified: Tue May 23 14:15:31 2023, max compression
```

## Comparing `gordo-5.0.1.tar` & `gordo-5.0.2.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.045832 gordo-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 11:31:49.000000 gordo-5.0.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 11:31:49.000000 gordo-5.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 11:31:49.000000 gordo-5.0.1/.github/dependabot.yml 
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-15 11:31:49.000000 gordo-5.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-15 11:31:49.000000 gordo-5.0.1/.github/workflows/master-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-15 11:31:49.000000 gordo-5.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-15 11:31:49.000000 gordo-5.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 11:31:49.000000 gordo-5.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/.trivyignore
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-15 11:31:49.000000 gordo-5.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-15 11:31:49.000000 gordo-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-15 11:31:49.000000 gordo-5.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-15 11:34:01.045832 gordo-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-15 11:31:49.000000 gordo-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-15 11:31:49.000000 gordo-5.0.1/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/benchmarks/load_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-15 11:31:49.000000 gordo-5.0.1/benchmarks/load_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-15 11:31:49.000000 gordo-5.0.1/benchmarks/load_test/load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-15 11:31:49.000000 gordo-5.0.1/benchmarks/load_test/task_set.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-15 11:31:49.000000 gordo-5.0.1/benchmarks/test_ml_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-15 11:31:49.000000 gordo-5.0.1/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/_static/Gordo_C4.README
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/_static/Gordo_C4.svg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/_static/_placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/_static/endpoint-metadata.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/docs/components/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.025832 gordo-5.0.1/docs/components/machine/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/docs/components/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/model/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/model/model-factories.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/model/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/model/transformer-funcs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/model/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/machine/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/serializer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/docs/components/server/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/server/anomaly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/server/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/server/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/components/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/docs/general/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/general/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/general/endpoints.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/general/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-15 11:31:49.000000 gordo-5.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-05-15 11:31:49.000000 gordo-5.0.1/examples/Gordo-Workflow-High-Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-15 11:31:49.000000 gordo-5.0.1/examples/Pipelines-with-Gordo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-15 11:31:49.000000 gordo-5.0.1/examples/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-15 11:31:49.000000 gordo-5.0.1/functions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/builder/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/builder/local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/cli/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/cli/exceptions_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/cli/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/anomaly/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/anomaly/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/machine/model/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/factories/feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/factories/lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/factories/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/machine/model/transformer_funcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/transformer_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/transformer_funcs/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/machine/model/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/transformers/imputer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/machine/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/reporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/reporters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/reporters/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/reporters/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/serializer/from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/serializer/into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/serializer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/server/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/blueprints/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/blueprints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/model_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/server/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/prometheus/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/prometheus/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/util/disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/util/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/util/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.033832 gordo-5.0.1/gordo/workflow/config_elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/config_elements/normalized_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/config_elements/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/gordo/workflow/workflow_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/workflow_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/workflow_generator/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/gordo/workflow/workflow_generator/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/workflow_generator/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-15 11:31:49.000000 gordo-5.0.1/gordo/workflow/workflow_generator/workflow_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.029832 gordo-5.0.1/gordo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:34:00.000000 gordo-5.0.1/gordo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 11:31:49.000000 gordo-5.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-15 11:31:49.000000 gordo-5.0.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/docs_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/full_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/mlflow_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/postgres_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/test_requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-15 11:31:49.000000 gordo-5.0.1/requirements/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.021832 gordo-5.0.1/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.021832 gordo-5.0.1/resources/grafana/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/resources/grafana/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-05-15 11:31:49.000000 gordo-5.0.1/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-15 11:31:49.000000 gordo-5.0.1/resources/grafana/dashboards/how_to_modify_dashboard.md
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-15 11:31:49.000000 gordo-5.0.1/resources/grafana/dashboards/machines.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-15 11:31:49.000000 gordo-5.0.1/run_workflow_and_argo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-15 11:31:49.000000 gordo-5.0.1/scripts/download_argo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-15 11:31:49.000000 gordo-5.0.1/scripts/github_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-15 11:31:49.000000 gordo-5.0.1/scripts/tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-15 11:31:49.000000 gordo-5.0.1/scripts/trivy_scan.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:34:01.045832 gordo-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-15 11:31:49.000000 gordo-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/config-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/gordo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/gordo/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/builder/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/builder/test_local_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/builder/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/gordo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/cli/test_exception_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/gordo/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/client/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/gordo/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.037832 gordo-5.0.1/tests/gordo/machine/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/metadata/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/machine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/machine/model/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_factories_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_feedforward_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_lstm_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_raw_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/model/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/reporters/test_mlflow_reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/reporters/test_postgres_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/serializer/definition_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/serializer/test_serializer_from_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/serializer/test_serializer_into_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/serializer/test_serializer_load_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/test_anomaly_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/test_base_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/test_gordo_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/test_model_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/test_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/server/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/util/test_disk_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/util/test_sensor_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/util/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_config_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_normalized_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.041833 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:34:01.045832 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/mocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-15 11:31:49.000000 gordo-5.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 14:13:17.000000 gordo-5.0.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 14:13:17.000000 gordo-5.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/dependabot.yml 
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/workflows/master-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-23 14:13:17.000000 gordo-5.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-23 14:13:17.000000 gordo-5.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 14:13:17.000000 gordo-5.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/.trivyignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-23 14:13:17.000000 gordo-5.0.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-05-23 14:13:17.000000 gordo-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-23 14:13:17.000000 gordo-5.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-23 14:15:31.007681 gordo-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-23 14:13:17.000000 gordo-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/benchmarks/load_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/load_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/load_test/load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/load_test/task_set.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 14:13:17.000000 gordo-5.0.2/benchmarks/test_ml_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 14:13:17.000000 gordo-5.0.2/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.983681 gordo-5.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/Gordo_C4.README
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/Gordo_C4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/_placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   162857 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/_static/endpoint-metadata.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/model-factories.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/transformer-funcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/model/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/machine/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/serializer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/components/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/server/anomaly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/server/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/server/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/components/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/docs/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/general/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/general/endpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/general/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-23 14:13:17.000000 gordo-5.0.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-05-23 14:13:17.000000 gordo-5.0.2/examples/Gordo-Workflow-High-Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-23 14:13:17.000000 gordo-5.0.2/examples/Pipelines-with-Gordo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-23 14:13:17.000000 gordo-5.0.2/examples/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 14:13:17.000000 gordo-5.0.2/functions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/exceptions_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19987 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/cli/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/anomaly/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/anomaly/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/factories/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/transformer_funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformer_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformer_funcs/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/machine/model/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/transformers/imputer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/machine/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16222 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/reporters/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/serializer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.991681 gordo-5.0.2/gordo/server/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/blueprints/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/blueprints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/model_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/server/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/prometheus/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/config_elements/normalized_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/config_elements/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/workflow_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/gordo/workflow/workflow_generator/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70702 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-23 14:13:17.000000 gordo-5.0.2/gordo/workflow/workflow_generator/workflow_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.987681 gordo-5.0.2/gordo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:15:30.000000 gordo-5.0.2/gordo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 14:13:17.000000 gordo-5.0.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-23 14:13:17.000000 gordo-5.0.2/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/docs_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/full_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/mlflow_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/postgres_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/test_requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-23 14:13:17.000000 gordo-5.0.2/requirements/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.979681 gordo-5.0.2/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.979681 gordo-5.0.2/resources/grafana/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/resources/grafana/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-05-23 14:13:17.000000 gordo-5.0.2/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 14:13:17.000000 gordo-5.0.2/resources/grafana/dashboards/how_to_modify_dashboard.md
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-05-23 14:13:17.000000 gordo-5.0.2/resources/grafana/dashboards/machines.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-05-23 14:13:17.000000 gordo-5.0.2/run_workflow_and_argo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.995681 gordo-5.0.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/download_argo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/github_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 14:13:17.000000 gordo-5.0.2/scripts/trivy_scan.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:15:31.007681 gordo-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-23 14:13:17.000000 gordo-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/config-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/test_local_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/builder/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/cli/test_exception_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:30.999681 gordo-5.0.2/tests/gordo/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/client/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/metadata/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/machine/model/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_factories_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_feedforward_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_lstm_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_raw_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/model/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/reporters/test_mlflow_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/reporters/test_postgres_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.003682 gordo-5.0.2/tests/gordo/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/definition_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/test_serializer_from_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/test_serializer_into_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/serializer/test_serializer_load_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_anomaly_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_base_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_gordo_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/server/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/test_disk_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/test_sensor_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_normalized_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:15:31.007681 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-empty-default-data-provider.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone-quoted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-missing-timezone.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-simple.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/mocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-23 14:13:17.000000 gordo-5.0.2/tests/utils.py
```

### Comparing `gordo-5.0.1/.github/workflows/main.yml` & `gordo-5.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/.github/workflows/master-ci.yml` & `gordo-5.0.2/.github/workflows/master-ci.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/.github/workflows/release.yml` & `gordo-5.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/.gitignore` & `gordo-5.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/Dockerfile` & `gordo-5.0.2/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 RUN cp ${HOME}/build.sh /usr/bin/build \
     && chmod a+x /usr/bin/build
 
 # Run things from gordo's home to have write access when needed (e.g. Catboost tmp files)
 WORKDIR ${HOME}
 
 #download & install argo
-ENV ARGO_VERSIONS="[{\"number\":3,\"version\":\"3.4.3\"},{\"number\":2,\"version\":\"2.12.13\"}]"
+ENV ARGO_VERSIONS="[{\"number\":3,\"version\":\"3.4.7\"}]"
 COPY scripts/download_argo.py ./download_argo.py
 RUN python3 ./download_argo.py -o /usr/local/bin
 
 # Cleanup
 RUN dpkg -r curl && rm ./download_argo.py
 
 # Make gordo own all in its home
```

### Comparing `gordo-5.0.1/LICENSE` & `gordo-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/Makefile` & `gordo-5.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/PKG-INFO` & `gordo-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.1
+Version: 5.0.2
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.1 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.0.2 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
 Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-Extra:
```

### Comparing `gordo-5.0.1/README.md` & `gordo-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/benchmarks/load_test/README.md` & `gordo-5.0.2/benchmarks/load_test/README.md`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/benchmarks/load_test/load_test.py` & `gordo-5.0.2/benchmarks/load_test/load_test.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/benchmarks/test_ml_server.py` & `gordo-5.0.2/benchmarks/test_ml_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/Makefile` & `gordo-5.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/_static/Gordo_C4.svg` & `gordo-5.0.2/docs/_static/Gordo_C4.svg`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/_static/endpoint-metadata.png` & `gordo-5.0.2/docs/_static/endpoint-metadata.png`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/machine/machine.rst` & `gordo-5.0.2/docs/components/machine/machine.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/machine/metadata.rst` & `gordo-5.0.2/docs/components/machine/metadata.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/machine/model/anomaly.rst` & `gordo-5.0.2/docs/components/machine/model/anomaly.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/machine/model/model-factories.rst` & `gordo-5.0.2/docs/components/machine/model/model-factories.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/machine/model/model.rst` & `gordo-5.0.2/docs/components/machine/model/model.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/serializer.rst` & `gordo-5.0.2/docs/components/serializer.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/server/server.rst` & `gordo-5.0.2/docs/components/server/server.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/components/workflow.rst` & `gordo-5.0.2/docs/components/workflow.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/conf.py` & `gordo-5.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/general/endpoints.rst` & `gordo-5.0.2/docs/general/endpoints.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/general/quickstart.rst` & `gordo-5.0.2/docs/general/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/docs/index.rst` & `gordo-5.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/examples/Gordo-Workflow-High-Level.ipynb` & `gordo-5.0.2/examples/Gordo-Workflow-High-Level.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/examples/Pipelines-with-Gordo.ipynb` & `gordo-5.0.2/examples/Pipelines-with-Gordo.ipynb`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/examples/config.yaml` & `gordo-5.0.2/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/functions.sh` & `gordo-5.0.2/functions.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/__init__.py` & `gordo-5.0.2/gordo/__init__.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/builder/build_model.py` & `gordo-5.0.2/gordo/builder/build_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/builder/local_build.py` & `gordo-5.0.2/gordo/builder/local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/builder/utils.py` & `gordo-5.0.2/gordo/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/cli/cli.py` & `gordo-5.0.2/gordo/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/cli/custom_types.py` & `gordo-5.0.2/gordo/cli/custom_types.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/cli/exceptions_reporter.py` & `gordo-5.0.2/gordo/cli/exceptions_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/cli/workflow_generator.py` & `gordo-5.0.2/gordo/cli/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/encoders.py` & `gordo-5.0.2/gordo/machine/encoders.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/loader.py` & `gordo-5.0.2/gordo/machine/loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/machine.py` & `gordo-5.0.2/gordo/machine/machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/metadata/metadata.py` & `gordo-5.0.2/gordo/machine/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/anomaly/base.py` & `gordo-5.0.2/gordo/machine/model/anomaly/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/anomaly/diff.py` & `gordo-5.0.2/gordo/machine/model/anomaly/diff.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/base.py` & `gordo-5.0.2/gordo/machine/model/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/factories/feedforward_autoencoder.py` & `gordo-5.0.2/gordo/machine/model/factories/feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/factories/lstm_autoencoder.py` & `gordo-5.0.2/gordo/machine/model/factories/lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/factories/utils.py` & `gordo-5.0.2/gordo/machine/model/factories/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/models.py` & `gordo-5.0.2/gordo/machine/model/models.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/register.py` & `gordo-5.0.2/gordo/machine/model/register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/transformer_funcs/general.py` & `gordo-5.0.2/gordo/machine/model/transformer_funcs/general.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/transformers/imputer.py` & `gordo-5.0.2/gordo/machine/model/transformers/imputer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/model/utils.py` & `gordo-5.0.2/gordo/machine/model/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/machine/validators.py` & `gordo-5.0.2/gordo/machine/validators.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/reporters/base.py` & `gordo-5.0.2/gordo/reporters/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/reporters/mlflow.py` & `gordo-5.0.2/gordo/reporters/mlflow.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/reporters/postgres.py` & `gordo-5.0.2/gordo/reporters/postgres.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/serializer/from_definition.py` & `gordo-5.0.2/gordo/serializer/from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/serializer/into_definition.py` & `gordo-5.0.2/gordo/serializer/into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/serializer/serializer.py` & `gordo-5.0.2/gordo/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/serializer/utils.py` & `gordo-5.0.2/gordo/serializer/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/blueprints/anomaly.py` & `gordo-5.0.2/gordo/server/blueprints/anomaly.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/blueprints/base.py` & `gordo-5.0.2/gordo/server/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/model_io.py` & `gordo-5.0.2/gordo/server/model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/prometheus/metrics.py` & `gordo-5.0.2/gordo/server/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/prometheus/server.py` & `gordo-5.0.2/gordo/server/prometheus/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/properties.py` & `gordo-5.0.2/gordo/server/properties.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/server.py` & `gordo-5.0.2/gordo/server/server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/server/utils.py` & `gordo-5.0.2/gordo/server/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/util/disk_registry.py` & `gordo-5.0.2/gordo/util/disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/util/utils.py` & `gordo-5.0.2/gordo/util/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/util/version.py` & `gordo-5.0.2/gordo/util/version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/utils.py` & `gordo-5.0.2/gordo/utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/workflow/config_elements/normalized_config.py` & `gordo-5.0.2/gordo/workflow/config_elements/normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/workflow/config_elements/schemas.py` & `gordo-5.0.2/gordo/workflow/config_elements/schemas.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/workflow/workflow_generator/helpers.py` & `gordo-5.0.2/gordo/workflow/workflow_generator/helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template` & `gordo-5.0.2/gordo/workflow/workflow_generator/resources/argo-workflow.yml.template`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo/workflow/workflow_generator/workflow_generator.py` & `gordo-5.0.2/gordo/workflow/workflow_generator/workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo.egg-info/PKG-INFO` & `gordo-5.0.2/gordo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo
-Version: 5.0.1
+Version: 5.0.2
 Summary: Train and build models for Argo / Kubernetes
 Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 License: AGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gordo Version: 5.0.1 Summary: Train and build
+Metadata-Version: 2.1 Name: gordo Version: 5.0.2 Summary: Train and build
 models for Argo / Kubernetes Home-page: https://github.com/equinor/gordo
 Author: Equinor ASA Author-email: fg_gpl@equinor.com License: AGPLv3
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
 Extra: docs Provides-Extra: mlflow Provides-Extra: postgres Provides-Extra:
```

### Comparing `gordo-5.0.1/gordo.egg-info/SOURCES.txt` & `gordo-5.0.2/gordo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/gordo.egg-info/requires.txt` & `gordo-5.0.2/gordo.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 six==1.16.0
 sniffio==1.3.0
 soupsieve==2.3.2.post1
 stack-data==0.6.0
 terminado==0.17.0
 tinycss2==1.2.1
 tomli==1.2.3
-tornado==6.2
+tornado==6.3.2
 traitlets==5.5.0
 types-mock==4.0.15.2
 types-python-dateutil==2.8.19.2
 types-pytz==2022.6.0.1
 types-pyyaml==6.0.12.1
 types-requests==2.28.11.2
 types-setuptools==65.5.0.2
```

### Comparing `gordo-5.0.1/pytest.ini` & `gordo-5.0.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/requirements/full_requirements.txt` & `gordo-5.0.2/requirements/full_requirements.txt`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/requirements/test_requirements.txt` & `gordo-5.0.2/requirements/test_requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     # via nbconvert
 tomli==1.2.3
     # via
     #   black
     #   coverage
     #   mypy
     #   pytest
-tornado==6.2
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
```

### Comparing `gordo-5.0.1/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json` & `gordo-5.0.2/resources/grafana/dashboards/Gordo_servers-VictoriaMetrics.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/resources/grafana/dashboards/machines.json` & `gordo-5.0.2/resources/grafana/dashboards/machines.json`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/run_workflow_and_argo.sh` & `gordo-5.0.2/run_workflow_and_argo.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/scripts/download_argo.py` & `gordo-5.0.2/scripts/download_argo.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/scripts/github_docker.py` & `gordo-5.0.2/scripts/github_docker.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/scripts/tests.sh` & `gordo-5.0.2/scripts/tests.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/scripts/trivy_scan.sh` & `gordo-5.0.2/scripts/trivy_scan.sh`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/setup.py` & `gordo-5.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/config-test.yaml` & `gordo-5.0.2/tests/config-test.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/conftest.py` & `gordo-5.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/builder/test_builder.py` & `gordo-5.0.2/tests/gordo/builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/builder/test_local_build.py` & `gordo-5.0.2/tests/gordo/builder/test_local_build.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/builder/test_utils.py` & `gordo-5.0.2/tests/gordo/builder/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/cli/test_cli.py` & `gordo-5.0.2/tests/gordo/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/cli/test_exception_reporter.py` & `gordo-5.0.2/tests/gordo/cli/test_exception_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/client/test_client.py` & `gordo-5.0.2/tests/gordo/client/test_client.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/metadata/test_metadata.py` & `gordo-5.0.2/tests/gordo/machine/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py` & `gordo-5.0.2/tests/gordo/machine/model/anomaly/test_anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_factories_utils.py` & `gordo-5.0.2/tests/gordo/machine/model/test_factories_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_feedforward_autoencoder.py` & `gordo-5.0.2/tests/gordo/machine/model/test_feedforward_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_lstm_autoencoder.py` & `gordo-5.0.2/tests/gordo/machine/model/test_lstm_autoencoder.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_model.py` & `gordo-5.0.2/tests/gordo/machine/model/test_model.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_raw_keras.py` & `gordo-5.0.2/tests/gordo/machine/model/test_raw_keras.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_register.py` & `gordo-5.0.2/tests/gordo/machine/model/test_register.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_transformers.py` & `gordo-5.0.2/tests/gordo/machine/model/test_transformers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/model/test_utils.py` & `gordo-5.0.2/tests/gordo/machine/model/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/test_descriptors.py` & `gordo-5.0.2/tests/gordo/machine/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/test_loader.py` & `gordo-5.0.2/tests/gordo/machine/test_loader.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/machine/test_machine.py` & `gordo-5.0.2/tests/gordo/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/reporters/test_mlflow_reporter.py` & `gordo-5.0.2/tests/gordo/reporters/test_mlflow_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/reporters/test_postgres_reporter.py` & `gordo-5.0.2/tests/gordo/reporters/test_postgres_reporter.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/serializer/test_serializer_from_definition.py` & `gordo-5.0.2/tests/gordo/serializer/test_serializer_from_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/serializer/test_serializer_into_definition.py` & `gordo-5.0.2/tests/gordo/serializer/test_serializer_into_definition.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/serializer/test_serializer_load_dump.py` & `gordo-5.0.2/tests/gordo/serializer/test_serializer_load_dump.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/server/test_anomaly_blueprint.py` & `gordo-5.0.2/tests/gordo/server/test_anomaly_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/server/test_base_blueprint.py` & `gordo-5.0.2/tests/gordo/server/test_base_blueprint.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/server/test_gordo_server.py` & `gordo-5.0.2/tests/gordo/server/test_gordo_server.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/server/test_model_io.py` & `gordo-5.0.2/tests/gordo/server/test_model_io.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/server/test_prometheus.py` & `gordo-5.0.2/tests/gordo/server/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/server/test_utils.py` & `gordo-5.0.2/tests/gordo/server/test_utils.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/test_version.py` & `gordo-5.0.2/tests/gordo/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/util/test_disk_registry.py` & `gordo-5.0.2/tests/gordo/util/test_disk_registry.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/util/test_version.py` & `gordo-5.0.2/tests/gordo/util/test_version.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_config_elements.py` & `gordo-5.0.2/tests/gordo/workflow/test_config_elements.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_helpers.py` & `gordo-5.0.2/tests/gordo/workflow/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_normalized_config.py` & `gordo-5.0.2/tests/gordo/workflow/test_normalized_config.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-allowed-timestamps.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-datasource.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-disable-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-empty-tag-list.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-failing-resource-format.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-model-builder-spec.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-quotes.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-images.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-labels.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-runtime-resource.yaml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-selective-influx.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-1.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-2.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-timestamp-3.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-log-key.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/data/config-test-with-models.yml`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py` & `gordo-5.0.2/tests/gordo/workflow/test_workflow_generator/test_workflow_generator.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/test_examples.py` & `gordo-5.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gordo-5.0.1/tests/utils.py` & `gordo-5.0.2/tests/utils.py`

 * *Files identical despite different names*

