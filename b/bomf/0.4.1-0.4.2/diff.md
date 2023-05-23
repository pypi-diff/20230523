# Comparing `tmp/bomf-0.4.1.tar.gz` & `tmp/bomf-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.4.1.tar", last modified: Thu May  4 07:55:32 2023, max compression
+gzip compressed data, was "bomf-0.4.2.tar", last modified: Tue May 23 12:12:47 2023, max compression
```

## Comparing `bomf-0.4.1.tar` & `bomf-0.4.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.431872 bomf-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-04 07:55:24.000000 bomf-0.4.1/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-04 07:55:24.000000 bomf-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 07:55:24.000000 bomf-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-04 07:55:24.000000 bomf-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:55:32.431872 bomf-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-04 07:55:24.000000 bomf-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-04 07:55:24.000000 bomf-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:55:24.000000 bomf-0.4.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-04 07:55:24.000000 bomf-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 07:55:32.431872 bomf-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 07:55:24.000000 bomf-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.431872 bomf-0.4.1/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 07:55:24.000000 bomf-0.4.1/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.427872 bomf-0.4.1/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 07:55:32.000000 bomf-0.4.1/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-04 07:55:24.000000 bomf-0.4.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:55:32.431872 bomf-0.4.1/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-05-04 07:55:24.000000 bomf-0.4.1/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.842965 bomf-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 12:12:40.000000 bomf-0.4.2/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-23 12:12:40.000000 bomf-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 12:12:40.000000 bomf-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-23 12:12:40.000000 bomf-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-23 12:12:47.846964 bomf-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-23 12:12:40.000000 bomf-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-23 12:12:40.000000 bomf-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 12:12:40.000000 bomf-0.4.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 12:12:40.000000 bomf-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-23 12:12:47.846964 bomf-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 12:12:40.000000 bomf-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.834964 bomf-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.842965 bomf-0.4.2/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.842965 bomf-0.4.2/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.842965 bomf-0.4.2/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.842965 bomf-0.4.2/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-23 12:12:40.000000 bomf-0.4.2/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.838964 bomf-0.4.2/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-23 12:12:47.000000 bomf-0.4.2/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-23 12:12:47.000000 bomf-0.4.2/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:12:47.000000 bomf-0.4.2/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:12:47.000000 bomf-0.4.2/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 12:12:47.000000 bomf-0.4.2/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 12:12:47.000000 bomf-0.4.2/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-23 12:12:40.000000 bomf-0.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:12:47.842965 bomf-0.4.2/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-05-23 12:12:40.000000 bomf-0.4.2/unittests/test_validation.py
```

### Comparing `bomf-0.4.1/.github/dependabot.yml` & `bomf-0.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/black.yml` & `bomf-0.4.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/codeql-analysis.yml` & `bomf-0.4.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/coverage.yml` & `bomf-0.4.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/packaging_test.yml` & `bomf-0.4.2/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/python-publish.yml` & `bomf-0.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/pythonlint.yml` & `bomf-0.4.2/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.github/workflows/unittests.yml` & `bomf-0.4.2/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.gitignore` & `bomf-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/.pre-commit-config.yaml` & `bomf-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/LICENSE` & `bomf-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/PKG-INFO` & `bomf-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.4.1
+Version: 0.4.2
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.4.1/README.md` & `bomf-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/pyproject.toml` & `bomf-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/requirements.txt` & `bomf-0.4.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/setup.cfg` & `bomf-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/__init__.py` & `bomf-0.4.2/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/filter/__init__.py` & `bomf-0.4.2/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.4.2/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/loader/entityloader.py` & `bomf-0.4.2/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/mapper/__init__.py` & `bomf-0.4.2/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/model/__init__.py` & `bomf-0.4.2/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/provider/__init__.py` & `bomf-0.4.2/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/core/analysis.py` & `bomf-0.4.2/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/core/errors.py` & `bomf-0.4.2/src/bomf/validation/core/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,16 @@
             message += f"\n\tParameter information: \n{formatted_param_infos}"
         super().__init__(message)
         self.cause = cause
         self.data_set = data_set
         self.mapped_validator = mapped_validator
         self.validator_set = validation_manager
         self.error_id = error_id
+        self.message_detail = message_detail
+        self.provided_params = provided_params
 
 
 # pylint: disable=too-few-public-methods
 class ErrorHandler(Generic[DataSetT]):
     """
     This class provides functionality to easily log any occurring error.
     It can save one exception for each validator function.
```

### Comparing `bomf-0.4.1/src/bomf/validation/core/execution.py` & `bomf-0.4.2/src/bomf/validation/core/execution.py`

 * *Files 5% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                     self._execute_async_validator(mapped_validator, running_dependencies)
                 )
             else:
                 assert is_sync(mapped_validator)  # Should never fail, but makes mypy happy
                 self.info.tasks[mapped_validator] = self.info.current_task
                 await self._execute_sync_validator(mapped_validator)
 
-    async def validate(self, *data_sets: DataSetT) -> ValidationResult[DataSetT]:
+    async def validate(self, *data_sets: DataSetT, log_summary: bool = False) -> ValidationResult[DataSetT]:
         """
         Validates each of the provided data set instances onto the registered validators.
         Any errors occurring during validation will be collected the validation process will not be cancelled.
         The returned `ValidationSummary` object supports several analytical methods - most importantly the property
         `succeeded_data_sets` to retrieve the positively validated data sets (without errors).
         """
         error_handlers: dict[DataSetT, ErrorHandler[DataSetT]] = {}
@@ -351,8 +351,17 @@
             # sadly, networkx is not carefully typed. topological_sort returns a generator of nodes
             if any(is_async(mapped_validator) for mapped_validator in self.validators):
                 async with asyncio.TaskGroup() as task_group:
                     await self._execute_validators(validator_execution_order, task_group=task_group)
             else:
                 await self._execute_validators(validator_execution_order)
 
-        return ValidationResult(self, error_handlers)
+        validation_result = ValidationResult(self, error_handlers)
+        if log_summary:
+            validation_logger.info(
+                "Validation Summary: %i succeeded, %i failed, %i errors. %s",
+                validation_result.num_succeeds,
+                validation_result.num_fails,
+                validation_result.num_errors_total,
+                str(validation_result.num_errors_per_id),
+            )
+        return validation_result
```

### Comparing `bomf-0.4.1/src/bomf/validation/core/types.py` & `bomf-0.4.2/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/core/utils.py` & `bomf-0.4.2/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/core/validator.py` & `bomf-0.4.2/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/path_map.py` & `bomf-0.4.2/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/query_map.py` & `bomf-0.4.2/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf/validation/utils.py` & `bomf-0.4.2/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/src/bomf.egg-info/PKG-INFO` & `bomf-0.4.2/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.4.1
+Version: 0.4.2
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.4.1/src/bomf.egg-info/SOURCES.txt` & `bomf-0.4.2/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/tox.ini` & `bomf-0.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_bo4e_data_set.py` & `bomf-0.4.2/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_entity_loader.py` & `bomf-0.4.2/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_filter.py` & `bomf-0.4.2/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_mapper.py` & `bomf-0.4.2/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_migration.py` & `bomf-0.4.2/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_source_data_provider.py` & `bomf-0.4.2/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.4.1/unittests/test_validation.py` & `bomf-0.4.2/unittests/test_validation.py`

 * *Files identical despite different names*

