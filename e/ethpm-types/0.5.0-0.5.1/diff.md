# Comparing `tmp/ethpm-types-0.5.0.tar.gz` & `tmp/ethpm-types-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.5.0.tar", last modified: Thu May  4 12:52:30 2023, max compression
+gzip compressed data, was "ethpm-types-0.5.1.tar", last modified: Tue May 23 13:43:33 2023, max compression
```

## Comparing `ethpm-types-0.5.0.tar` & `ethpm-types-0.5.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:52:29.000000 ethpm-types-0.5.0/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.989127 ethpm-types-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.985127 ethpm-types-0.5.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/tests/data/Compiled/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/HasError.json
--rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)   220464 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Compiled/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:29.997127 ethpm-types-0.5.0/tests/data/Sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/data/Sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-04 12:52:05.000000 ethpm-types-0.5.0/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.815462 ethpm-types-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.815462 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.819462 ethpm-types-0.5.1/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.823462 ethpm-types-0.5.1/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 13:43:33.000000 ethpm-types-0.5.1/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 13:43:33.835461 ethpm-types-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.823462 ethpm-types-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.811462 ethpm-types-0.5.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/tests/data/Compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)   220464 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Compiled/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:43:33.831462 ethpm-types-0.5.1/tests/data/Sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/data/Sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-23 13:43:02.000000 ethpm-types-0.5.1/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.5.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/release-drafter.yml` & `ethpm-types-0.5.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/workflows/commitlint.yaml` & `ethpm-types-0.5.1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/workflows/docs.yaml` & `ethpm-types-0.5.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/workflows/prtitle.yaml` & `ethpm-types-0.5.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/workflows/publish.yaml` & `ethpm-types-0.5.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.github/workflows/test.yaml` & `ethpm-types-0.5.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.gitignore` & `ethpm-types-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/.pre-commit-config.yaml` & `ethpm-types-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/CONTRIBUTING.md` & `ethpm-types-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/LICENSE` & `ethpm-types-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/PKG-INFO` & `ethpm-types-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.5.0
+Version: 0.5.1
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.5.0/README.md` & `ethpm-types-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/build_docs.py` & `ethpm-types-0.5.1/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/docs/_static/custom.css` & `ethpm-types-0.5.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/docs/_static/custom.js` & `ethpm-types-0.5.1/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/docs/_templates/layout.html` & `ethpm-types-0.5.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/docs/conf.py` & `ethpm-types-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/docs/favicon.ico` & `ethpm-types-0.5.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/docs/logo.gif` & `ethpm-types-0.5.1/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/__init__.py` & `ethpm-types-0.5.1/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/abi.py` & `ethpm-types-0.5.1/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/ast.py` & `ethpm-types-0.5.1/ethpm_types/ast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Iterator, List, Optional, Union
+from typing import Dict, Iterator, List, Optional, Union
 
 from pydantic import root_validator
 
 from ethpm_types.base import BaseModel
 from ethpm_types.sourcemap import SourceMapItem
 from ethpm_types.utils import SourceLocation
 
@@ -33,71 +33,88 @@
     """
 
     src: SourceMapItem
     """
     The source offset item.
     """
 
-    lineno: int
+    lineno: int = -1
     """
     The start line number in the source.
     """
 
-    end_lineno: int
+    end_lineno: int = -1
     """
     The line number where the AST node ends.
     """
 
-    col_offset: int
+    col_offset: int = -1
     """
     The offset of the column start.
     """
 
-    end_col_offset: int
+    end_col_offset: int = -1
     """
     The offset when the column ends.
     """
 
     children: List["ASTNode"] = []
     """
     All sub-AST nodes within this one.
     """
 
     @root_validator(pre=True)
-    def validate_src(cls, val):
-        src = val.get("src")
-        if src and isinstance(src, str):
-            src = SourceMapItem.parse_str(src)
-
-        def find_children(node):
-            children = []
-
-            def add_child(data):
-                data["children"] = find_children(data)
-                child = ASTNode.parse_obj(data)
-                children.append(child)
-
-            for value in node.values():
-                if isinstance(value, dict) and "ast_type" in value:
-                    add_child(value)
-
-                elif isinstance(value, list):
-                    for _val in value:
-                        if isinstance(_val, dict) and "ast_type" in _val:
-                            add_child(_val)
+    def validate_node(cls, val):
+        src = cls._validate_src(val)
 
-            return children
+        # Handle `ast_type`.
+        if "nodeType" in val and "ast_type" not in val:
+            val["ast_type"] = val.pop("nodeType")
 
         return {
             "doc_str": val.get("doc_string"),
-            "children": find_children(val),
+            "children": cls.find_children(val),
             **val,
             "src": src,
         }
 
+    @classmethod
+    def _validate_src(cls, val: Dict) -> SourceMapItem:
+        src = val.get("src")
+        if src and isinstance(src, str):
+            src = SourceMapItem.parse_str(src)
+
+        elif isinstance(src, dict):
+            src = SourceMapItem.parse_obj(src)
+
+        elif not isinstance(src, SourceMapItem):
+            raise TypeError(type(src))
+
+        return src
+
+    @classmethod
+    def find_children(cls, node) -> List["ASTNode"]:
+        children = []
+
+        def add_child(data):
+            data["children"] = cls.find_children(data)
+            child = cls.parse_obj(data)
+            children.append(child)
+
+        for value in node.values():
+            if isinstance(value, dict) and ("ast_type" in value or "nodeType" in value):
+                add_child(value)
+
+            elif isinstance(value, list):
+                for _val in value:
+                    if isinstance(_val, dict) and ("ast_type" in _val or "nodeType" in _val):
+                        add_child(_val)
+
+        return children
+
     @property
     def line_numbers(self) -> SourceLocation:
         """
         The values needed for constructing the line numbers for this node
         in the form ``[lineno, col_offset, end_lineno, end_col_offset]``.
         """
```

### Comparing `ethpm-types-0.5.0/ethpm_types/base.py` & `ethpm-types-0.5.1/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/contract_type.py` & `ethpm-types-0.5.1/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/manifest.py` & `ethpm-types-0.5.1/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/source.py` & `ethpm-types-0.5.1/ethpm_types/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Dict, Iterator, List, Optional, Tuple, Union
+from typing import Dict, Iterator, List, Optional, Set, Tuple, Union
 
 import requests
 from cid import make_cid  # type: ignore
 from pydantic import root_validator, validator
 
 from ethpm_types.ast import ASTClassification, ASTNode, SourceLocation
 from ethpm_types.base import BaseModel
@@ -402,14 +402,22 @@
 class Statement(BaseModel):
     """
     A class representing an item in a control flow, either a source statement
     or implicit compiler code.
     """
 
     type: str
+    """
+    The type of statement it is, such as `source` or a virtual identifier.
+    """
+
+    pcs: Set[int] = set()
+    """
+    The PC value for the statement.
+    """
 
     def __repr__(self) -> str:
         return f"<Statement type={self.type}>"
 
 
 class SourceStatement(Statement):
     """
```

### Comparing `ethpm-types-0.5.0/ethpm_types/sourcemap.py` & `ethpm-types-0.5.1/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types/utils.py` & `ethpm-types-0.5.1/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.5.1/ethpm_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.5.0
+Version: 0.5.1
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.5.0/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.5.1/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.5.1/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/pyproject.toml` & `ethpm-types-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/setup.py` & `ethpm-types-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/conftest.py` & `ethpm-types-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Compiled/HasError.json` & `ethpm-types-0.5.1/tests/data/Compiled/HasError.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Compiled/OpenZeppelinContracts.json` & `ethpm-types-0.5.1/tests/data/Compiled/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Compiled/SolidityContract.json` & `ethpm-types-0.5.1/tests/data/Compiled/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Compiled/TestStrategy.srcmap` & `ethpm-types-0.5.1/tests/data/Compiled/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Compiled/VyperContract.json` & `ethpm-types-0.5.1/tests/data/Compiled/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Sources/SolidityContract.sol` & `ethpm-types-0.5.1/tests/data/Sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/data/Sources/VyperContract.vy` & `ethpm-types-0.5.1/tests/data/Sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_cairo.py` & `ethpm-types-0.5.1/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_contract_type.py` & `ethpm-types-0.5.1/tests/test_contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_hexbytes.py` & `ethpm-types-0.5.1/tests/test_hexbytes.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_package_manifest.py` & `ethpm-types-0.5.1/tests/test_package_manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_pc_map.py` & `ethpm-types-0.5.1/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_schema_fuzzing.py` & `ethpm-types-0.5.1/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_source.py` & `ethpm-types-0.5.1/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.5.0/tests/test_sourcemap.py` & `ethpm-types-0.5.1/tests/test_sourcemap.py`

 * *Files identical despite different names*

