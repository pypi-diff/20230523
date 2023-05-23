# Comparing `tmp/foundry-dev-tools-1.0.8.tar.gz` & `tmp/foundry-dev-tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry-dev-tools-1.0.8.tar", last modified: Mon Apr 17 13:53:10 2023, max compression
+gzip compressed data, was "foundry-dev-tools-1.0.9.tar", last modified: Thu Apr 27 12:23:55 2023, max compression
```

## Comparing `foundry-dev-tools-1.0.8.tar` & `foundry-dev-tools-1.0.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/blank_issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/Configuration_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/FoundryFileSystem_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/FoundryRestClient_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/SSO_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/docs/pictures/
--rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/tpa_config.png
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/usage_and_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-17 13:53:10.894557 foundry-dev-tools-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    86868 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/foundry_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/fsspec_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/metadata_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/spark_caches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/foundry_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/transforms/api/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/foundry_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_cached_foundry_client_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/tests/test_data/binary_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_data/binary_dataset/bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/tests/test_data/iris/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_data/iris/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)    29242 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_local_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_spark_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_sql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_fsspec_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_multipass_tpa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_spark_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_transforms_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.788965 foundry-dev-tools-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.740965 foundry-dev-tools-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.740965 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/blank_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.744965 foundry-dev-tools-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-27 12:23:55.788965 foundry-dev-tools-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.752965 foundry-dev-tools-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/Configuration_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/FoundryFileSystem_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/FoundryRestClient_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/SSO_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.752965 foundry-dev-tools-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.756965 foundry-dev-tools-1.0.9/docs/pictures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/pictures/tpa_config.png
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/docs/usage_and_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 12:23:55.788965 foundry-dev-tools-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.756965 foundry-dev-tools-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.760965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86863 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/foundry_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/fsspec_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.764965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.768965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/metadata_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/spark_caches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.768965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/foundry_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.768965 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.764965 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 12:23:55.000000 foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.772965 foundry-dev-tools-1.0.9/src/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.772965 foundry-dev-tools-1.0.9/src/transforms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/src/transforms/api/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.784965 foundry-dev-tools-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/foundry_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_cached_foundry_client_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.732965 foundry-dev-tools-1.0.9/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.784965 foundry-dev-tools-1.0.9/tests/test_data/binary_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_data/binary_dataset/bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:23:55.784965 foundry-dev-tools-1.0.9/tests/test_data/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_data/iris/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29252 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_local_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_spark_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_foundry_sql_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_fsspec_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_multipass_tpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_spark_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/test_transforms_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-27 12:21:47.000000 foundry-dev-tools-1.0.9/tox.ini
```

### Comparing `foundry-dev-tools-1.0.8/.coveragerc` & `foundry-dev-tools-1.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/blank_issue.yml` & `foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/blank_issue.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/feature_request.yml` & `foundry-dev-tools-1.0.9/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.github/pull_request_template.md` & `foundry-dev-tools-1.0.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.github/workflows/ci.yml` & `foundry-dev-tools-1.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.github/workflows/docs.yml` & `foundry-dev-tools-1.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.gitignore` & `foundry-dev-tools-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/.pre-commit-config.yaml` & `foundry-dev-tools-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/LICENSE` & `foundry-dev-tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/PKG-INFO` & `foundry-dev-tools-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Home-page: https://github.com/emdgroup/foundry-dev-tools
 Author: Nicolas Renkamp, Jonas Wunderlich
 Author-email: nicolas.renkamp@merckgroup.com, jonas.wunderlich@merckgroup.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.9 Summary:
 Seamlessly run your Palantir Foundry Repository transforms code on your local
 machine. Home-page: https://github.com/emdgroup/foundry-dev-tools Author:
 Nicolas Renkamp, Jonas Wunderlich Author-email: nicolas.renkamp@merckgroup.com,
 jonas.wunderlich@merckgroup.com License: Apache License, Version 2.0 Project-
 URL: Documentation, https://emdgroup.github.io/foundry-dev-tools Project-URL:
 Source, https://github.com/emdgroup/foundry-dev-tools Project-URL: Tracker,
 https://github.com/emdgroup/foundry-dev-tools/issues Project-URL: Changelog,
```

### Comparing `foundry-dev-tools-1.0.8/README.md` & `foundry-dev-tools-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/Configuration_usage.md` & `foundry-dev-tools-1.0.9/docs/Configuration_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/FoundryFileSystem_usage.md` & `foundry-dev-tools-1.0.9/docs/FoundryFileSystem_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/FoundryRestClient_usage.md` & `foundry-dev-tools-1.0.9/docs/FoundryRestClient_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/SSO_usage.md` & `foundry-dev-tools-1.0.9/docs/SSO_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/architecture.md` & `foundry-dev-tools-1.0.9/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/changelog.md` & `foundry-dev-tools-1.0.9/docs/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog],
 and this project adheres to [Semantic Versioning].
 
+## [1.0.9] - 2023-04-27
+
+### Fixed
+
+- file upload for files greater than 2GB (#16)
+
 ## [1.0.8] - 2023-04-17
 
 ### Added
 
 - python 3.11 support, as pyspark 3.4 gained support for it (#13)
 - conda-forge badges to the README (#13)
 
@@ -92,14 +98,15 @@
 
 ## [1.0] - 2023-02-28 [YANKED]
 
 - First public Open Source Release of Foundry DevTools.
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/spec/v2.0.0.html
+[1.0.9]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.8...v1.0.9
 [1.0.8]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.7...v1.0.8
 [1.0.7]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.6...v1.0.7
 [1.0.6]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.5...v1.0.6
 [1.0.5]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.4...v1.0.5
 [1.0.4]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.3...v1.0.4
 [1.0.3]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.2...v1.0.3
 [1.0.2]: https://github.com/emdgroup/foundry-dev-tools/releases/tag/v1.0.2
```

### Comparing `foundry-dev-tools-1.0.8/docs/conf.py` & `foundry-dev-tools-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/develop.md` & `foundry-dev-tools-1.0.9/docs/develop.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/index.md` & `foundry-dev-tools-1.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/installation.md` & `foundry-dev-tools-1.0.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-dark.svg` & `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-light.svg` & `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-already-cached-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-dark.svg` & `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-light.svg` & `foundry-dev-tools-1.0.9/docs/pictures/mermaid-diagram-new-transaction-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/pictures/tpa_config.png` & `foundry-dev-tools-1.0.9/docs/pictures/tpa_config.png`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/docs/usage_and_examples.md` & `foundry-dev-tools-1.0.9/docs/usage_and_examples.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/setup.cfg` & `foundry-dev-tools-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/setup.py` & `foundry-dev-tools-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/__init__.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/cached_foundry_client.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/cached_foundry_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/config.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/foundry_api_client.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/foundry_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         self.multipass = f"{api_base}/multipass/api"
         self._api_base = api_base
         self._requests_verify_value = _determine_requests_verify_value(self._config)
 
     def _headers(self):
         return {
             "User-Agent": requests.utils.default_user_agent(
-                f"Foundry DevTools/{fdt_version}/python-requests"
+                f"foundry-dev-tools/{fdt_version}/python-requests"
             ),
             "Content-Type": "application/json",
             "Authorization": f"Bearer {_get_auth_token(self._config)}",
         }
 
     def _verify(self):
         return self._requests_verify_value
@@ -546,15 +546,15 @@
         )
         with open(path_or_buf, "rb") as file:
             response = _request(
                 "POST",
                 f"{self.data_proxy}/dataproxy/datasets/{dataset_rid}/"
                 f"transactions/{transaction_rid}/putFile",
                 params={"logicalPath": path_in_foundry_dataset},
-                data=file.read(),
+                data=file,
                 headers={
                     "Content-Type": "application/octet-stream",
                     "Authorization": self._headers()["Authorization"],
                 },
             )
         builtins.open = original_open
         _raise_for_status_verbose(response)
@@ -1707,15 +1707,15 @@
         self._headers = self._get_initial_headers(
             session_authorization=self.session_auth_token
         )
 
     def _get_initial_headers(self, session_authorization=None):
         return {
             "User-Agent": requests.utils.default_user_agent(
-                f"Foundry DevTools/{fdt_version}/python-requests"
+                f"foundry-dev-tools/{fdt_version}/python-requests"
             ),
             "Accept": "application/json",
             "Accept-Encoding": "gzip, deflate, br",
             "Content-Type": "application/json",
             "Session-Authorization": session_authorization,
             "Authorization": f"Bearer {_get_auth_token(self._config)}",
         }
@@ -2044,15 +2044,15 @@
             'expires_in': 3600,
             'token_type': 'bearer'
        }
 
     """
     headers = {
         "User-Agent": requests.utils.default_user_agent(
-            f"Foundry DevTools/{fdt_version}/python-requests"
+            f"foundry-dev-tools/{fdt_version}/python-requests"
         ),
         "Authorization": "Basic "
         + base64.b64encode(bytes(client_id + ":" + client_secret, "ISO-8859-1")).decode(
             "ascii"
         ),
         "Content-Type": "application/x-www-form-urlencoded",
     }
@@ -2069,15 +2069,14 @@
 
 
 @lru_with_ttl(ttl_seconds=3600)
 def _get_palantir_oauth_token(
     foundry_url: str, client_id: str, client_secret: str = None
 ) -> str:
     if oauth_provider := _is_palantir_oauth_client_installed():
-
         credentials = oauth_provider.get_user_credentials(
             scopes=[
                 "offline_access",
                 "compass:view",
                 "compass:edit",
                 "compass:discover",
                 "api:write-data",
```

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/fsspec_impl.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/metadata_store.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/metadata_store.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/spark_caches.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/caches/spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/foundry_spark.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/converter/foundry_spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/importer.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/importer.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/spark.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/PKG-INFO` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Home-page: https://github.com/emdgroup/foundry-dev-tools
 Author: Nicolas Renkamp, Jonas Wunderlich
 Author-email: nicolas.renkamp@merckgroup.com, jonas.wunderlich@merckgroup.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.9 Summary:
 Seamlessly run your Palantir Foundry Repository transforms code on your local
 machine. Home-page: https://github.com/emdgroup/foundry-dev-tools Author:
 Nicolas Renkamp, Jonas Wunderlich Author-email: nicolas.renkamp@merckgroup.com,
 jonas.wunderlich@merckgroup.com License: Apache License, Version 2.0 Project-
 URL: Documentation, https://emdgroup.github.io/foundry-dev-tools Project-URL:
 Source, https://github.com/emdgroup/foundry-dev-tools Project-URL: Tracker,
 https://github.com/emdgroup/foundry-dev-tools/issues Project-URL: Changelog,
```

### Comparing `foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/SOURCES.txt` & `foundry-dev-tools-1.0.9/src/foundry_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/transforms/api/__init__.py` & `foundry-dev-tools-1.0.9/src/transforms/api/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/transforms/api/_configure.py` & `foundry-dev-tools-1.0.9/src/transforms/api/_configure.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/transforms/api/_dataset.py` & `foundry-dev-tools-1.0.9/src/transforms/api/_dataset.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/transforms/api/_decorators.py` & `foundry-dev-tools-1.0.9/src/transforms/api/_decorators.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/src/transforms/api/_transform.py` & `foundry-dev-tools-1.0.9/src/transforms/api/_transform.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/conftest.py` & `foundry-dev-tools-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/foundry_mock_client.py` & `foundry-dev-tools-1.0.9/tests/foundry_mock_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_cached_foundry_client.py` & `foundry-dev-tools-1.0.9/tests/test_cached_foundry_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_cached_foundry_client_integration.py` & `foundry-dev-tools-1.0.9/tests/test_cached_foundry_client_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_config.py` & `foundry-dev-tools-1.0.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_data/binary_dataset/bin` & `foundry-dev-tools-1.0.9/tests/test_data/binary_dataset/bin`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_data/iris/iris.csv` & `foundry-dev-tools-1.0.9/tests/test_data/iris/iris.csv`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_foundry_api.py` & `foundry-dev-tools-1.0.9/tests/test_foundry_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         mock_get_user_credentials = mocker.patch(
             "palantir_oauth_client.get_user_credentials"
         )
         mock_get_user_credentials.return_value.token = "access-token"
 
         assert client._headers()["Authorization"] == "Bearer access-token"
-        assert "Foundry DevTools" in client._headers()["User-Agent"]
+        assert client._headers()["User-Agent"].startswith("foundry-dev-tools")
 
 
 @pytest.mark.integration
 def test_monster_integration_test(client):
     BRANCH = "master/with/slash"
     rnd = "".join(choice(ascii_uppercase) for i in range(5))
     dataset_path = str(INTEGRATION_TEST_COMPASS_ROOT_PATH / f"test_api_{rnd}")
```

### Comparing `foundry-dev-tools-1.0.8/tests/test_foundry_local_deprecation.py` & `foundry-dev-tools-1.0.9/tests/test_foundry_local_deprecation.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_foundry_mock.py` & `foundry-dev-tools-1.0.9/tests/test_foundry_mock.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_foundry_spark_converters.py` & `foundry-dev-tools-1.0.9/tests/test_foundry_spark_converters.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_foundry_sql_client.py` & `foundry-dev-tools-1.0.9/tests/test_foundry_sql_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_fsspec_impl.py` & `foundry-dev-tools-1.0.9/tests/test_fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_multipass_tpa.py` & `foundry-dev-tools-1.0.9/tests/test_multipass_tpa.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_spark_caches.py` & `foundry-dev-tools-1.0.9/tests/test_spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_token_provider.py` & `foundry-dev-tools-1.0.9/tests/test_token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_transforms.py` & `foundry-dev-tools-1.0.9/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/test_transforms_integration.py` & `foundry-dev-tools-1.0.9/tests/test_transforms_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tests/utils.py` & `foundry-dev-tools-1.0.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.8/tox.ini` & `foundry-dev-tools-1.0.9/tox.ini`

 * *Files identical despite different names*

