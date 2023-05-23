# Comparing `tmp/kolena-0.69.0.tar.gz` & `tmp/kolena-0.70.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena-0.69.0.tar", max compression
+gzip compressed data, was "kolena-0.70.0.tar", max compression
```

## Comparing `kolena-0.69.0.tar` & `kolena-0.70.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0    11346 2023-05-16 21:43:37.336470 kolena-0.69.0/LICENSE
--rw-r--r--   0        0        0      556 2023-05-16 21:43:37.336470 kolena-0.69.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1546 2023-05-16 21:43:37.336470 kolena-0.69.0/README.md
--rw-r--r--   0        0        0     1349 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     8201 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5540 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      783 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4970 2023-05-16 21:43:37.336470 kolena-0.69.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5481 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3235 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15591 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3578 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     2645 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4138 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8572 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13515 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12407 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    12957 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     4716 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20512 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9319 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14479 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12196 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16929 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15301 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3544 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/initialize.py
--rw-r--r--   0        0        0     4550 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-05-16 21:43:37.340470 kolena-0.69.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     7794 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    15849 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0     9318 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      846 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0    14420 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7592 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13372 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22779 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9155 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    14458 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9326 2023-05-16 21:43:37.344470 kolena-0.69.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     2553 2023-05-16 21:43:52.688630 kolena-0.69.0/pyproject.toml
--rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 kolena-0.69.0/setup.py
--rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 kolena-0.69.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-23 21:36:32.093116 kolena-0.70.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-05-23 21:36:32.093116 kolena-0.70.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1546 2023-05-23 21:36:32.093116 kolena-0.70.0/README.md
+-rw-r--r--   0        0        0     1349 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     8201 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5540 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      783 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4970 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-05-23 21:36:32.097116 kolena-0.70.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5481 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15677 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3566 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3237 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4468 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8566 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13755 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12341 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13033 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5327 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20512 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9316 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14583 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12193 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16915 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15376 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3544 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4550 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     8158 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    15849 2023-05-23 21:36:32.101117 kolena-0.70.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    10725 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      846 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0    14420 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7589 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13369 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22768 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     9155 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    14458 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9349 2023-05-23 21:36:32.105116 kolena-0.70.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     2553 2023-05-23 21:36:45.469266 kolena-0.70.0/pyproject.toml
+-rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 kolena-0.70.0/setup.py
+-rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 kolena-0.70.0/PKG-INFO
```

### Comparing `kolena-0.69.0/LICENSE` & `kolena-0.70.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/LICENSE_HEADER` & `kolena-0.70.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/README.md` & `kolena-0.70.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/__init__.py` & `kolena-0.70.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/__init__.py` & `kolena-0.70.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/__init__.py` & `kolena-0.70.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/batched_load.py` & `kolena-0.70.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/client_log.py` & `kolena-0.70.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/core.py` & `kolena-0.70.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/detection.py` & `kolena-0.70.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/fr.py` & `kolena-0.70.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/generic.py` & `kolena-0.70.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/repository.py` & `kolena-0.70.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/token.py` & `kolena-0.70.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_api/v1/workflow.py` & `kolena-0.70.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/__init__.py` & `kolena-0.70.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/asset_path_mapper.py` & `kolena-0.70.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/batched_load.py` & `kolena-0.70.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/cli.py` & `kolena-0.70.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/consts.py` & `kolena-0.70.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/dataframes/__init__.py` & `kolena-0.70.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/dataframes/validators.py` & `kolena-0.70.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/datatypes.py` & `kolena-0.70.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/endpoints.py` & `kolena-0.70.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/frozen.py` & `kolena-0.70.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/geometry.py` & `kolena-0.70.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/inference_validators.py` & `kolena-0.70.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/instrumentation.py` & `kolena-0.70.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/krequests.py` & `kolena-0.70.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/log.py` & `kolena-0.70.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/repository.py` & `kolena-0.70.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/serde.py` & `kolena-0.70.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/serializable.py` & `kolena-0.70.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/state.py` & `kolena-0.70.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/uninstantiable.py` & `kolena-0.70.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/_utils/validators.py` & `kolena-0.70.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/__init__.py` & `kolena-0.70.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/metadata.py` & `kolena-0.70.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/model.py` & `kolena-0.70.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/multiclass/__init__.py` & `kolena-0.70.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/multiclass/_utils.py` & `kolena-0.70.0/kolena/classification/multiclass/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
 from typing import Optional
 from typing import Tuple
+from typing import Union
 
 import numpy as np
 
 from kolena._utils import log
 from kolena.classification.multiclass import InferenceLabel
+from kolena.workflow.annotation import ScoredClassificationLabel
 
 
-def get_label_confidence(label: str, inference_labels: List[InferenceLabel]) -> float:
+def get_label_confidence(label: str, inference_labels: List[Union[ScoredClassificationLabel, InferenceLabel]]) -> float:
     for inf_label in inference_labels:
         if inf_label.label == label:
-            return inf_label.confidence
+            return inf_label.score
     return 0
 
 
 def roc_curve(y_true: List[int], y_score: List[float]) -> Tuple[List[float], List[float]]:
     # Convert inputs to numpy arrays
     y_true = np.array(y_true)
     y_score = np.array(y_score)
```

### Comparing `kolena-0.69.0/kolena/classification/multiclass/evaluator.py` & `kolena-0.70.0/kolena/classification/multiclass/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Type
+from typing import Union
 
 import numpy as np
 
 from kolena._utils import log
 from kolena.classification.multiclass._utils import get_histogram_range
 from kolena.classification.multiclass._utils import get_label_confidence
 from kolena.classification.multiclass._utils import roc_curve
@@ -42,14 +43,15 @@
 from kolena.workflow import ConfusionMatrix
 from kolena.workflow import Curve
 from kolena.workflow import CurvePlot
 from kolena.workflow import EvaluationResults
 from kolena.workflow import Histogram
 from kolena.workflow import Plot
 from kolena.workflow import TestCases
+from kolena.workflow.annotation import ScoredClassificationLabel
 
 Result = Tuple[TestSample, GroundTruth, Inference]
 
 
 def _compute_test_sample_metric(
     threshold_configuration: ThresholdConfiguration,
     ground_truth: GroundTruth,
@@ -59,21 +61,21 @@
         classification=None,
         margin=None,
         is_correct=False,
     )
     if len(inference.inferences) == 0:
         return empty_metrics
 
-    sorted_indices = np.argsort([label.confidence for label in inference.inferences])
+    sorted_indices = np.argsort([label.score for label in inference.inferences])
     match = inference.inferences[sorted_indices[-1]]
-    predicted_label, confidence_score = match.label, match.confidence
+    predicted_label, confidence_score = match.label, match.score
     margin: Optional[float] = None
     if len(sorted_indices) > 1:
-        second_closest: InferenceLabel = inference.inferences[sorted_indices[-2]]
-        margin = confidence_score - second_closest.confidence
+        second_closest: Union[ScoredClassificationLabel, InferenceLabel] = inference.inferences[sorted_indices[-2]]
+        margin = confidence_score - second_closest.score
 
     if threshold_configuration.threshold is not None and confidence_score < threshold_configuration.threshold:
         return empty_metrics
 
     is_correct = predicted_label == ground_truth.classification.label
     return TestSampleMetrics(
         classification=match,
@@ -132,41 +134,41 @@
 ) -> List[Histogram]:
     if confidence_range is None:
         log.warn(
             f"skipping confidence histograms for {test_case_name}: unsupported confidence range",
         )
         return []
 
-    confidence_all = [mts.classification.confidence for mts in metrics if mts.classification is not None]
+    confidence_all = [mts.classification.score for mts in metrics if mts.classification is not None]
     confidence_correct = [
-        mts.classification.confidence for mts in metrics if mts.classification is not None and mts.is_correct
+        mts.classification.score for mts in metrics if mts.classification is not None and mts.is_correct
     ]
     confidence_incorrect = [
-        mts.classification.confidence for mts in metrics if mts.classification is not None and not mts.is_correct
+        mts.classification.score for mts in metrics if mts.classification is not None and not mts.is_correct
     ]
 
     plots = [
-        _as_confidence_histogram("Confidence Distribution (All)", confidence_all, confidence_range),
-        _as_confidence_histogram("Confidence Distribution (Correct)", confidence_correct, confidence_range),
-        _as_confidence_histogram("Confidence Distribution (Incorrect)", confidence_incorrect, confidence_range),
+        _as_confidence_histogram("Score Distribution (All)", confidence_all, confidence_range),
+        _as_confidence_histogram("Score Distribution (Correct)", confidence_correct, confidence_range),
+        _as_confidence_histogram("Score Distribution (Incorrect)", confidence_incorrect, confidence_range),
     ]
     return plots
 
 
 def _compute_test_case_plots(
     test_case_name: str,
     labels: List[str],
     ground_truths: List[GroundTruth],
     inferences: List[Inference],
     metrics: List[TestSampleMetrics],
     metrics_by_label: Dict[str, AggregatedMetrics],
     confidence_range: Optional[Tuple[float, float, int]],
 ) -> List[Plot]:
     gt_labels = {gt.classification.label for gt in ground_truths}
-    plots = [
+    plots: List[Plot] = [
         _as_class_metric_plot(field.name, metrics_by_label, labels)
         for field in dataclasses.fields(AggregatedMetrics)
         if len(gt_labels) > 2
         or field.name not in ["Precision", "Recall"]  # Omit single-class TC from precision and recall plots
     ]
 
     plots.extend(_compute_confidence_histograms(test_case_name, metrics, confidence_range))
@@ -358,15 +360,15 @@
     labels = sorted(labels_set)
 
     metrics_test_sample: List[Tuple[TestSample, TestSampleMetrics]] = [
         (ts, _compute_test_sample_metric(configuration, gt, inf))
         for ts, gt, inf in zip(test_samples, ground_truths, inferences)
     ]
     test_sample_metrics: List[TestSampleMetrics] = [mts for _, mts in metrics_test_sample]
-    confidence_scores = [mts.classification.confidence for mts in test_sample_metrics if mts.classification is not None]
+    confidence_scores = [mts.classification.score for mts in test_sample_metrics if mts.classification is not None]
     confidence_range = get_histogram_range(confidence_scores)
 
     metrics_test_case: List[Tuple[TestCase, TestCaseMetrics]] = []
     plots_test_case: List[Tuple[TestCase, List[Plot]]] = []
     for tc, tc_samples, tc_gts, tc_infs, tc_metrics in test_cases.iter(
         test_samples,
         ground_truths,
```

### Comparing `kolena-0.69.0/kolena/classification/multiclass/test_run.py` & `kolena-0.70.0/kolena/classification/multiclass/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 from kolena._utils.validators import ValidatorConfig
 from kolena.classification.multiclass import Model
 from kolena.classification.multiclass import MulticlassClassificationEvaluator
 from kolena.classification.multiclass import TestSuite
 from kolena.classification.multiclass.workflow import ThresholdConfiguration
 from kolena.workflow import EvaluatorConfiguration
-from kolena.workflow.test_run import test as generic_test
-from kolena.workflow.test_run import TestRun as GenericTestRun
+from kolena.workflow.test_run import test as base_test
+from kolena.workflow.test_run import TestRun as BaseTestRun
 
 
-class TestRun(GenericTestRun):
+class TestRun(BaseTestRun):
     """
     Convenience alias for :class:`kolena.workflow.test_run.TestRun`, configured for the
     `kolena.classification.multiclass` workflow and evaluator.
 
     Interface to run tests for a :class:`kolena.classification.multiclass.Model` on a set of
     :class:`kolena.classification.multiclass.TestSuite` suites.
 
@@ -79,14 +79,14 @@
     :param test_suite: the test suite on which to test the model.
     :param configurations: an optional list of configurations to use when running the evaluator. Defaults to selecting
         the max confidence label (with no thresholding) if unset.
     :param reset: overwrites existing inferences if set.
     """
     if configurations is None:
         configurations = [ThresholdConfiguration()]
-    generic_test(
+    base_test(
         model=model,
         test_suite=test_suite,
         evaluator=MulticlassClassificationEvaluator,
         configurations=configurations,
         reset=reset,
     )
```

### Comparing `kolena-0.69.0/kolena/classification/multiclass/workflow.py` & `kolena-0.70.0/kolena/classification/multiclass/workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,56 +9,72 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
 from typing import Optional
+from typing import Union
 
+from deprecation import deprecated
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from kolena.workflow import define_workflow
 from kolena.workflow import EvaluatorConfiguration
 from kolena.workflow import GroundTruth as BaseGroundTruth
 from kolena.workflow import Image
 from kolena.workflow import Inference as BaseInference
 from kolena.workflow import Metadata
 from kolena.workflow import MetricsTestCase
 from kolena.workflow import MetricsTestSample
 from kolena.workflow import MetricsTestSuite
 from kolena.workflow.annotation import ClassificationLabel
+from kolena.workflow.annotation import ScoredClassificationLabel
 
 
 @dataclass(frozen=True)
 class TestSample(Image):
     metadata: Metadata = Field(default_factory=dict)
 
 
 @dataclass(frozen=True)
 class GroundTruth(BaseGroundTruth):
     classification: ClassificationLabel
 
 
 @dataclass(frozen=True)
 class InferenceLabel(ClassificationLabel):
+    """
+    :class:`InferenceLabel` is deprecated and preserved for compatibility only. Please use
+    :class:`ScoredClassificationLabel` instead.
+    """
+
     confidence: float
 
+    @deprecated(details="use :class:`kolena.workflow.annotation.ScoredClassificationLabel`", deprecated_in="0.70.0")
+    def __post_init__(self) -> None:
+        ...
+
+    @property
+    def score(self) -> float:
+        return self.confidence
+
 
 @dataclass(frozen=True)
 class Inference(BaseInference):
-    inferences: List[InferenceLabel]
+    inferences: List[Union[ScoredClassificationLabel, InferenceLabel]]
 
 
 _workflow, TestCase, TestSuite, Model = define_workflow("Multiclass Classification", TestSample, GroundTruth, Inference)
 
 
 @dataclass(frozen=True)
 class TestSampleMetrics(MetricsTestSample):
-    classification: Optional[InferenceLabel]
+    classification: Optional[Union[ScoredClassificationLabel, InferenceLabel]]
     margin: Optional[float]
     is_correct: bool
 
 
 @dataclass(frozen=True)
 class AggregatedMetrics:
     F1: float
```

### Comparing `kolena-0.69.0/kolena/classification/test_case.py` & `kolena-0.70.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/test_config.py` & `kolena-0.70.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/test_image.py` & `kolena-0.70.0/kolena/classification/test_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,7 +98,14 @@
     def _to_detection(self) -> detection.TestImage:
         return detection.TestImage(
             locator=self.locator,
             dataset=self.dataset,
             ground_truths=[ClassificationLabel(label) for label in self.labels],
             metadata=self.metadata,
         )
+
+    # TODO: remove implementation in favor of Frozen.__eq__ once label ordering is ensured upstream
+    def __eq__(self, other: Any) -> bool:
+        return isinstance(other, type(self)) and {**self.__dict__, "labels": sorted(self.labels)} == {
+            **other.__dict__,
+            "labels": sorted(other.labels),
+        }
```

### Comparing `kolena-0.69.0/kolena/classification/test_run.py` & `kolena-0.70.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/classification/test_suite.py` & `kolena-0.70.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/__init__.py` & `kolena-0.70.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_datatypes.py` & `kolena-0.70.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/__init__.py` & `kolena-0.70.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/datatypes.py` & `kolena-0.70.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/ground_truth.py` & `kolena-0.70.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/inference.py` & `kolena-0.70.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/metadata.py` & `kolena-0.70.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/model.py` & `kolena-0.70.0/kolena/detection/_internal/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         params = dict(model_id=self._id, batch_size=batch_size, **{test_id_key: test_object._id})
         init_request = API.InitLoadInferencesRequest(**params)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_INFERENCES.value,
             df_class=self._LoadInferencesDataFrameClass,
         )
-        log.success(f"loaded inferences from model '{self.name}' on {test_object_display_name}")
+        log.info(f"loaded inferences from model '{self.name}' on {test_object_display_name}")
 
     @validate_arguments(config=ValidatorConfig)
     def load_inferences_by_test_case(
         self,
         test_suite: _TestSuiteClass,
     ) -> Dict[int, List[SampleInferences[_TestImageClass, _InferenceClass]]]:
         """Retrieve the uploaded inferences of a test suite for each image, grouped by test case."""
@@ -177,12 +177,12 @@
         params = dict(model_id=self._id, batch_size=batch_size, test_suite_id=test_suite._id)
         init_request = API.InitLoadInferencesByTestCaseRequest(**params)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_INFERENCES_BY_TEST_CASE.value,
             df_class=self._LoadInferencesDataFrameClass,
         )
-        log.success(f"loaded inferences from model '{self.name}' on test suite '{test_suite.name}'")
+        log.info(f"loaded inferences from model '{self.name}' on test suite '{test_suite.name}'")
 
     @abstractmethod
     def _inferences_from_record(self, record: Any) -> Tuple[_TestImageClass, Optional[List[_InferenceClass]]]:
         ...
```

### Comparing `kolena-0.69.0/kolena/detection/_internal/test_case.py` & `kolena-0.70.0/kolena/detection/_internal/test_case.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,28 +127,29 @@
     ) -> "BaseTestCase":
         """Create a new test case with the provided name."""
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
+        log.info(f"created test case '{name}' (v{obj.version})")
         if images is not None:
             obj._hydrate(images)
-        log.info(f"created test case '{name}'")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> CoreAPI.EntityData:
         """Load an existing test case with the provided name."""
         request = CoreAPI.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
-        log.info(f"loaded test case '{name}'")
-        return from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        obj = from_dict(data_class=CoreAPI.EntityData, data=res.json())
+        log.info(f"loaded test case '{name}' (v{obj.version})")
+        return obj
 
     @validate_arguments(config=ValidatorConfig)
     def _hydrate(self, images: List[_TestImageClass], description: Optional[str] = None) -> None:
         if len(images) == 0:
             log.warn("no images provided, unable to populate test case")
             return
         with self.edit(reset=True) as editor:
@@ -166,24 +167,24 @@
     def load_images(self) -> List[_TestImageClass]:
         """Load all test images with their associated ground truths in this test case."""
         return list(self.iter_images())
 
     @validate_arguments(config=ValidatorConfig)
     def iter_images(self) -> Iterator[_TestImageClass]:
         """Iterate through all images with their associated ground truths in this test case."""
-        log.info(f"loading test images for test case '{self.name}'")
+        log.info(f"loading test images for test case '{self.name}' (v{self.version})")
         init_request = CoreAPI.InitLoadContentsRequest(batch_size=BatchSize.LOAD_SAMPLES.value, test_case_id=self._id)
         for df in _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_IMAGES.value,
             df_class=self._TestImageDataFrameClass,
         ):
             for record in df.itertuples():
                 yield self._TestImageClass._from_record(record)
-        log.success(f"loaded test images for test case '{self.name}'")
+        log.info(f"loaded test images for test case '{self.name}' (v{self.version})")
 
     @classmethod
     def create(
         cls,
         name: str,
         description: Optional[str] = None,
         images: Optional[List[_TestImageClass]] = None,
@@ -211,14 +212,15 @@
         return cls._create_from_data(data)
 
     class Editor:
         """
         Interface to edit a test case. Create with :meth:`TestCase.edit`.
         """
 
+        _TestImageClass: Type[BaseTestImage] = BaseTestImage
         _images: Dict[str, BaseTestImage]
         _reset: bool
         _description: str
         _initial_description: str
 
         def __init__(self, description: str, reset: bool) -> None:
             self._edited = False
@@ -236,15 +238,15 @@
             """
             if self._description == description:
                 return
             self._description = description
             self._edited = True
 
         @validate_arguments(config=ValidatorConfig)
-        def add(self, image: BaseTestImage) -> None:
+        def add(self, image: _TestImageClass) -> None:
             """
             Add a test image to the test case, targeting the ``ground_truths`` held by the image.
             When the test image already exists in the test case, its ground truth
             is overwritten.
 
             To filter the ground truths associated with a test image, see :meth:`kolena.detection.TestImage.filter`.
 
@@ -253,15 +255,15 @@
             if image == self._images.get(image.locator, None):
                 log.info(f"no op: {image.locator} already in test case")
                 return
             self._images[image.locator] = image
             self._edited = True
 
         @validate_arguments(config=ValidatorConfig)
-        def remove(self, image: BaseTestImage) -> None:
+        def remove(self, image: _TestImageClass) -> None:
             """
             Remove the image from the test case.
 
             :param image: the test image to remove
             :raises KeyError: if the image is not in the test case
             """
             if image.locator not in self._images.keys():
@@ -291,26 +293,27 @@
                 editor.remove(...)
 
         Changes are committed to the Kolena platform when the context is exited.
 
         :param reset: clear any and all test samples currently in the test case.
         """
         editor = self.Editor(self.description, reset)
+        editor._TestImageClass = self._TestImageClass
         if not reset:
             for image in self.iter_images():
                 editor.add(image)
             editor._edited = False
 
         yield editor
 
         # no-op contexts have no effect, do not bump version
         if not editor._edited:
             return
 
-        log.info(f"editing test case '{self.name}'")
+        log.info(f"editing test case '{self.name}' (v{self.version})")
         init_response = init_upload()
         df = self._to_data_frame(list(editor._images.values()))
         df_serialized = df.as_serializable()
         upload_data_frame(df=df_serialized, batch_size=BatchSize.UPLOAD_RECORDS.value, load_uuid=init_response.uuid)
 
         request = CoreAPI.CompleteEditRequest(
             test_case_id=self._id,
@@ -322,8 +325,8 @@
         complete_res = krequests.put(
             endpoint_path=API.Path.COMPLETE_EDIT.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=CoreAPI.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
-        log.success(f"edited test case '{self.name}'")
+        log.success(f"edited test case '{self.name}' (v{self.version})")
```

### Comparing `kolena-0.69.0/kolena/detection/_internal/test_config.py` & `kolena-0.70.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/test_image.py` & `kolena-0.70.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/_internal/test_run.py` & `kolena-0.70.0/kolena/detection/_internal/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from kolena.detection._internal import BaseTestImage
 from kolena.detection._internal import BaseTestSuite
 from kolena.detection._internal import Inference
 from kolena.detection._internal.model import SampleInferences
 from kolena.errors import CustomMetricsException
 from kolena.errors import IncorrectUsageError
 from kolena.errors import InputValidationError
+from kolena.errors import WorkflowMismatchError
 
 _ImageDataFrame = Union[pa.typing.DataFrame, LoadableDataFrame]
 InferenceType = TypeVar("InferenceType")
 CustomMetricsCallback = Callable[[List[SampleInferences]], CustomMetrics]
 
 
 class BaseTestRun(ABC, Frozen, WithTelemetry):
@@ -79,22 +80,22 @@
         model: BaseModel,
         test_suite: BaseTestSuite,
         config: Optional[Metrics.RunConfig] = None,
         custom_metrics_callback: Optional[CustomMetricsCallback[_TestImageClass, _InferenceClass]] = None,
         reset: bool = False,
     ):
         if model._workflow != test_suite._workflow:
-            raise ValueError(
+            raise WorkflowMismatchError(
                 f"mismatching test suite workflow for model of type '{model._workflow}': '{test_suite._workflow}'",
             )
 
         if reset:
             log.warn("overwriting existing inferences from this model (reset=True)")
         else:
-            log.info("reset flag is disabled. update existing inferences by enabling the reset flag")
+            log.info("not overwriting any existing inferences from this model (reset=False)")
 
         request = API.CreateOrRetrieveRequest(
             model_id=model._id,
             test_suite_ids=[test_suite._id],
             config=config,
         )
         res = krequests.post(
@@ -160,17 +161,15 @@
             else:
                 context_image_inferences.extend(inferences)
                 self._n_inferences += len(inferences)
 
             self._inferences[image_id] = context_image_inferences
 
         if self._n_inferences >= BatchSize.UPLOAD_RESULTS.value:
-            log.info(f"uploading batch of '{self._n_inferences}' inference results")
             self._upload_chunk()
-            log.success(f"uploaded batch of '{self._n_inferences}' inference results")
 
     @validate_arguments(config=ValidatorConfig)
     def iter_images(self) -> Iterator[_TestImageClass]:
         """
         Returns an iterator of all remaining images that need inferences evaluated.
         """
         self._assert_active()
@@ -190,15 +189,15 @@
         self._assert_active()
         log.info("loading batch of images for test run")
         try:
             df_image_batch = next(self._iter_image_batch(batch_size=batch_size))
         except StopIteration:
             # no more images
             return []
-        log.success("loaded batch of images for test run")
+        log.info("loaded batch of images for test run")
         return [self._image_from_load_image_record(record) for record in df_image_batch.itertuples()]
 
     @validate_arguments(config=ValidatorConfig)
     def _iter_image_batch(
         self,
         batch_size: int = BatchSize.LOAD_SAMPLES.value,
     ) -> Iterator[_LoadTestImagesDataFrameClass]:
@@ -216,30 +215,31 @@
         )
 
     @validate_arguments(config=ValidatorConfig)
     def _upload_chunk(self) -> None:
         if self._n_inferences == 0:
             # Bail if this happens to being run by fencepost immediately after being run by add_inference
             return
-        log.info("streaming inference upload for test run")
+
+        log.info(f"uploading {self._n_inferences} inferences for test run")
         if self._upload_uuid is None:
             init_response = init_upload()
             self._upload_uuid = init_response.uuid
 
         df_chunk = self._ImageResultDataFrameClass.from_image_inference_mapping(
             self._id,
             self._model._id,
             self._inferences,
             self._ignored_image_ids,
         )
         df_chunk_serializable = df_chunk.as_serializable()
         upload_data_frame_chunk(df_chunk_serializable, load_uuid=self._upload_uuid)
         self._n_inferences = 0
         self._inferences = OrderedDict()
-        log.success("streamed inference upload for test run")
+        log.success(f"uploaded {self._n_inferences} inferences for test run")
 
     def _finalize_upload(self) -> None:
         if self._upload_uuid is None:
             # nothing was uploaded
             return
 
         log.info("finalizing inference upload for test run")
@@ -288,16 +288,16 @@
         log.success("computed custom metrics for test run")
         return custom_metrics
 
     def _submit_custom_metrics(self) -> None:
         if self._custom_metrics_callback is None:
             return
 
-        log.info("submitting custom metrics for test run")
+        log.info("computing and uploading custom metrics for test run")
         custom_metrics = self._compute_custom_metrics()
         request = API.UpdateCustomMetricsRequest(model_id=self._model._id, metrics=custom_metrics)
         res = krequests.put(
             endpoint_path=API.Path.UPLOAD_CUSTOM_METRICS.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
-        log.success("submitted custom metrics for test run")
+        log.success("computed and uploaded custom metrics for test run")
```

### Comparing `kolena-0.69.0/kolena/detection/_internal/test_suite.py` & `kolena-0.70.0/kolena/detection/_internal/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,17 @@
     ) -> "BaseTestSuite":
         """Create a new test suite with the provided name."""
         request = CoreAPI.TestSuite.CreateRequest(name=name, description=description or "", workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
         obj = cls._create_from_data(data)
+        log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         if test_cases is not None:
             obj._hydrate(test_cases)
-        log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     @validate_arguments(config=ValidatorConfig)
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> CoreAPI.TestSuite.EntityData:
         """Retrieve the existing test suite with the provided name."""
         request = CoreAPI.TestSuite.LoadByNameRequest(name=name, version=version)
@@ -178,15 +178,15 @@
         :param name: the name of the test suite to load.
         :param version: optionally specify a particular version of the test suite to load. Defaults to the latest
             version when unset.
         :return: the loaded test suite.
         """
         data = cls._load_by_name(name, version)
         obj = cls._create_from_data(data)
-        log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
+        log.info(f"loaded test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         return obj
 
     class Editor:
         """
         Interface to edit a test suite. Create with :meth:`TestSuite.edit`.
         """
 
@@ -232,15 +232,15 @@
             Remove the provided :class:`kolena.detection.TestCase` from the test suite. Any version of this test
             case in this test suite will be removed; the version does not need to match exactly.
 
             :param test_case: the test case to be removed from the test suite
             """
             name = test_case.name
             if name not in self._test_cases.keys():
-                raise KeyError(f"test case '{name}' not in suite")
+                raise KeyError(f"test case '{name}' not in test suite")
             self._test_cases.pop(name)
 
         @deprecated(details="use :meth:`add` instead", deprecated_in="0.56.0")
         @validate_arguments(config=ValidatorConfig)
         def merge(self, test_case: BaseTestCase) -> None:
             """
             Add the provided :class:`kolena.detection.TestCase` to the test suite, replacing any previous version
@@ -285,25 +285,25 @@
 
         yield editor
 
         if not editor._edited():
             log.info("no op: nothing edited")
             return
 
-        log.info(f"edited test suite '{self.name}'")
+        log.info(f"editing test suite '{self.name}' (v{self.version})")
         request = CoreAPI.TestSuite.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             test_case_ids=list(editor._test_cases.values()),
         )
         data = json.dumps(dataclasses.asdict(request))
         res = krequests.post(endpoint_path=API.Path.EDIT.value, data=data)
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
-        log.success(f"edited test suite '{self.name}' ({get_test_suite_url(test_suite_data.id)})")
+        log.success(f"edited test suite '{self.name}' (v{self.version}) ({get_test_suite_url(test_suite_data.id)})")
         with self._unfrozen():
             self.version = test_suite_data.version
             self.description = test_suite_data.description
             self.test_cases = [self._test_case_from(tc) for tc in test_suite_data.test_cases]
             self._id = test_suite_data.id
```

### Comparing `kolena-0.69.0/kolena/detection/ground_truth.py` & `kolena-0.70.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/inference.py` & `kolena-0.70.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/metadata.py` & `kolena-0.70.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/model.py` & `kolena-0.70.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/test_case.py` & `kolena-0.70.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/test_config.py` & `kolena-0.70.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/test_image.py` & `kolena-0.70.0/kolena/detection/test_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import json
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -76,14 +77,25 @@
             metadata=_from_dict(record.metadata),
         )
 
     @classmethod
     def _to_record(cls, image: "TestImage") -> Tuple[str, Optional[str], List[Dict[str, Any]], Dict[str, Any]]:
         return (image.locator, image.dataset, [gt._to_dict() for gt in image.ground_truths], _to_dict(image.metadata))
 
+    # TODO: remove implementation in favor of Frozen.__eq__ once ground_truth ordering is ensured upstream
+    def __eq__(self, other: Any) -> bool:
+        return isinstance(other, type(self)) and {
+            **self.__dict__,
+            "ground_truths": self._sort_ground_truths(self.ground_truths),
+        } == {**other.__dict__, "ground_truths": self._sort_ground_truths(other.ground_truths)}
+
+    @staticmethod
+    def _sort_ground_truths(ground_truths: List[GroundTruth]) -> List[GroundTruth]:
+        return sorted(ground_truths, key=lambda gt: json.dumps(gt._to_dict(), sort_keys=True))
+
 
 @deprecated(details="use :class:`kolena.detection.TestCase.load_images`", deprecated_in="0.26.0")
 @validate_arguments(config=ValidatorConfig)
 def load_images(dataset: Optional[str] = None) -> List[TestImage]:
     """
     Load a list of :class:`kolena.detection.TestImage` samples registered in the Kolena platform.
```

### Comparing `kolena-0.69.0/kolena/detection/test_run.py` & `kolena-0.70.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/detection/test_suite.py` & `kolena-0.70.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/errors.py` & `kolena-0.70.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/fr/__init__.py` & `kolena-0.70.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/fr/_utils.py` & `kolena-0.70.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/fr/datatypes.py` & `kolena-0.70.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/fr/model.py` & `kolena-0.70.0/kolena/fr/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         base_load_request = dataclasses.asdict(self._get_load_pair_results_request(test_object))
         init_request = API.InitLoadPairResultsRequest(batch_size=batch_size, **base_load_request)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_PAIR_RESULTS.value,
             df_class=LoadedPairResultDataFrame,
         )
-        log.success(f"loaded pair results from model '{self.data.name}' on {test_object_display_name}")
+        log.info(f"loaded pair results from model '{self.data.name}' on {test_object_display_name}")
 
 
 class InferenceModel(Model):
     """
     A :class:`kolena.fr.Model` capable of running tests via :meth:`kolena.fr.test`.
 
     Currently supports extracting a single embedding per image. To extract multiple embeddings per image, see
```

### Comparing `kolena-0.69.0/kolena/fr/test_case.py` & `kolena-0.70.0/kolena/fr/test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,17 +125,17 @@
         :return: the newly created test case.
         """
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
+        log.info(f"created test case '{name}' (v{obj.version})")
         if test_samples is not None:
             obj._hydrate(test_samples)
-        log.info(f"created test case '{name}'")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
@@ -161,15 +161,15 @@
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestCase":
         request = API.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
-        log.info(f"loaded test case '{name}'")
+        log.info(f"loaded test case '{name}' (v{data.version})")
         return cls._create_from_data(data)
 
     def load_data(self) -> TestCaseDataFrame:
         """
         Load all pairs data for a test case.
 
         :return: a DataFrame containing all pairs defined in this test case
@@ -308,15 +308,15 @@
 
         yield editor
 
         # no-op contexts have no effect, do not bump version
         if not editor._edited():
             return
 
-        log.info(f"editing test case '{self.name}'")
+        log.info(f"editing test case '{self.name}' (v{self.version})")
         init_response = init_upload()
         df = pd.DataFrame(editor._samples.values(), columns=TEST_CASE_COLUMNS)
         df_validated = validate_df_schema(df, TestCaseDataFrameSchema)
 
         upload_data_frame(df=df_validated, batch_size=BatchSize.UPLOAD_RECORDS.value, load_uuid=init_response.uuid)
         request = API.CompleteEditRequest(
             test_case_id=self._id,
@@ -328,25 +328,25 @@
         complete_res = krequests.post(
             endpoint_path=API.Path.COMPLETE_EDIT.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(complete_res)
         test_case_data = from_dict(data_class=API.EntityData, data=complete_res.json())
         self._populate_from_other(self._create_from_data(test_case_data))
-        log.success(f"edited test case '{self.name}'")
+        log.success(f"edited test case '{self.name}' (v{self.version})")
 
     @validate_arguments
     def iter_data(self, batch_size: int = 10_000_000) -> Iterator[TestCaseDataFrame]:
         """
         Iterator of DataFrames describing all pairs data for a test case.
 
         :param batch_size: optionally specify maximum number of rows to be returned in a single DataFrame. By default,
             limits row count to 10_000_000.
         """
-        log.info(f"loading image pairs in test case '{self.name}'")
+        log.info(f"loading image pairs in test case '{self.name}' (v{self.version})")
         init_request = API.InitLoadDataRequest(batch_size=batch_size, test_case_id=self._id)
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_DATA.value,
             df_class=TestCaseDataFrame,
         )
-        log.success(f"loaded image pairs in test case '{self.name}'")
+        log.info(f"loaded image pairs in test case '{self.name}' (v{self.version})")
```

### Comparing `kolena-0.69.0/kolena/fr/test_images.py` & `kolena-0.70.0/kolena/fr/test_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
             batch_size=batch_size,
         )
         yield from _BatchedLoader.iter_data(
             init_request=init_request,
             endpoint_path=API.Path.INIT_LOAD_REQUEST.value,
             df_class=TestImageDataFrame,
         )
-        log.success(f"loaded test images{from_extra}")
+        log.info(f"loaded test images{from_extra}")
 
     @staticmethod
     def _data_source_display_name(
         data_source: Optional[Union[str, TestSuite, TestSuite.Data, TestCase, TestCase.Data]],
         include_augmented: bool,
     ) -> Optional[str]:
         if isinstance(data_source, str):
```

### Comparing `kolena-0.69.0/kolena/fr/test_run.py` & `kolena-0.70.0/kolena/fr/test_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         model: Model.Data
         test_suites: List[TestSuite.Data]
 
     def __init__(self, model: Model, test_suite: TestSuite, reset: bool = False):
         if reset:
             log.warn("overwriting existing inferences from this model (reset=True)")
         else:
-            log.info("reset flag is disabled. update existing inferences by enabling the reset flag")
+            log.info("not overwriting any existing inferences from this model (reset=False)")
 
         request = API.CreateOrRetrieveRequest(model_id=model.data.id, test_suite_ids=[test_suite._id], reset=reset)
         res = krequests.post(
             endpoint_path=API.Path.CREATE_OR_RETRIEVE.value,
             data=json.dumps(dataclasses.asdict(request)),
         )
         krequests.raise_for_status(res)
@@ -139,15 +139,15 @@
             load_uuid = None
             try:
                 dfs: List[ImageDataFrame] = []
                 for line in init_res.iter_lines():
                     partial_response = from_dict(data_class=LoadAPI.InitDownloadPartialResponse, data=json.loads(line))
                     load_uuid = partial_response.uuid
                     dfs.append(_BatchedLoader.load_path(partial_response.path, ImageDataFrame))
-                log.success("loaded remaining images for test run")
+                log.info("loaded remaining images for test run")
                 return _BatchedLoader.concat(dfs, ImageDataFrame)
             finally:
                 _BatchedLoader.complete_load(load_uuid)
 
     def upload_image_results(self, df_image_result: ImageResultDataFrame) -> int:
         """
         Upload inference results for a batch of images.
@@ -245,15 +245,15 @@
                     load_uuid_embedding = partial_response.embeddings.uuid
                     dfs_embedding.append(_BatchedLoader.load_path(partial_response.embeddings.path, EmbeddingDataFrame))
                     load_uuid_pair = partial_response.pairs.uuid
                     dfs_pair.append(_BatchedLoader.load_path(partial_response.pairs.path, PairDataFrame))
 
                 df_embedding = _BatchedLoader.concat(dfs_embedding, EmbeddingDataFrame)
                 df_pair = _BatchedLoader.concat(dfs_pair, PairDataFrame)
-                log.success("loaded batch of image pairs for test run")
+                log.info("loaded batch of image pairs for test run")
                 return df_embedding, df_pair
             finally:
                 for uuid in [load_uuid_embedding, load_uuid_pair]:
                     _BatchedLoader.complete_load(uuid)
 
     def upload_pair_results(self, df_pair_result: PairResultDataFrame) -> int:
         """
```

### Comparing `kolena-0.69.0/kolena/fr/test_suite.py` & `kolena-0.70.0/kolena/fr/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,16 @@
         :return: the newly created test suite.
         """
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
+        log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         obj._hydrate(baseline_test_cases, non_baseline_test_cases)
-        log.info(f"created test suite '{name}' ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
         Load an existing test suite with the provided name.
 
@@ -160,15 +160,15 @@
 
     @classmethod
     def _load_by_name(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         request = API.LoadByNameRequest(name=name, version=version)
         res = krequests.put(endpoint_path=API.Path.LOAD_BY_NAME.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._create_from_data(from_dict(data_class=API.EntityData, data=res.json()))
-        log.info(f"loaded test suite '{name}' ({get_test_suite_url(obj._id)})")
+        log.info(f"loaded test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         return obj
 
     def _populate_from_other(self, other: "TestSuite") -> None:
         with self._unfrozen():
             self._id = other._id
             self.name = other.name
             self.version = other.version
@@ -276,15 +276,15 @@
             """
             name = test_case.name
             if name in self._baseline_test_cases.keys():
                 self._baseline_test_cases.pop(name)
             elif name in self._non_baseline_test_cases.keys():
                 self._non_baseline_test_cases.pop(name)
             else:
-                raise KeyError(f"test case '{name}' not in suite")
+                raise KeyError(f"test case '{name}' not in test suite")
             self._edited = True
 
         @deprecated(details="use :meth:`add` instead", deprecated_in="0.57.0")
         @validate_arguments(config=ValidatorConfig)
         def merge(self, test_case: TestCase, is_baseline: Optional[bool] = None) -> None:
             """
             Add the :class:`kolena.fr.TestCase` to the suite. If a test case by this name already exists in the suite,
@@ -323,21 +323,21 @@
 
         yield editor
 
         # no-op contexts have no effect, do not bump version
         if not editor._edited:
             return
 
-        log.info(f"editing test suite '{self.name}'")
+        log.info(f"editing test suite '{self.name}' (v{self.version})")
         request = API.EditRequest(
             test_suite_id=self._id,
             current_version=self.version,
             name=self.name,
             description=editor._description,
             baseline_test_case_ids=list(editor._baseline_test_cases.values()),
             non_baseline_test_case_ids=list(editor._non_baseline_test_cases.values()),
         )
         res = krequests.post(endpoint_path=API.Path.EDIT.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         test_suite_data = from_dict(data_class=API.EntityData, data=res.json())
         self._populate_from_other(self._create_from_data(test_suite_data))
-        log.success(f"edited test suite '{self.name}' ({get_test_suite_url(self._id)})")
+        log.success(f"edited test suite '{self.name}' (v{self.version}) ({get_test_suite_url(self._id)})")
```

### Comparing `kolena-0.69.0/kolena/initialize.py` & `kolena-0.70.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/__init__.py` & `kolena-0.70.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/_datatypes.py` & `kolena-0.70.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/_helpers.py` & `kolena-0.70.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/_validators.py` & `kolena-0.70.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/annotation.py` & `kolena-0.70.0/kolena/workflow/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,20 +243,34 @@
     label: str
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.CLASSIFICATON_LABEL
 
 
+@dataclass(frozen=True, config=ValidatorConfig)
+class ScoredClassificationLabel(ClassificationLabel):
+    """Classification label with accompanying score."""
+
+    score: float
+
+
 _ANNOTATION_TYPES = [
     BoundingBox,
     LabeledBoundingBox,
+    ScoredBoundingBox,
+    ScoredLabeledBoundingBox,
     Polygon,
     LabeledPolygon,
+    ScoredPolygon,
+    ScoredLabeledPolygon,
     Keypoints,
     Polyline,
     BoundingBox3D,
     LabeledBoundingBox3D,
+    ScoredBoundingBox3D,
+    ScoredLabeledBoundingBox3D,
     SegmentationMask,
     BitmapMask,
     ClassificationLabel,
+    ScoredClassificationLabel,
 ]
```

### Comparing `kolena-0.69.0/kolena/workflow/asset.py` & `kolena-0.70.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/evaluator.py` & `kolena-0.70.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/evaluator_function.py` & `kolena-0.70.0/kolena/workflow/evaluator_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,14 +98,40 @@
     [List[TestSample], List[GroundTruth], List[Inference], TestCases],
     Optional[EvaluationResults],
 ]
 #: ``kolena.workflow.BasicEvaluatorFunction`` introduces a function based evaluator implementation that takes
 #: the inferences for all test samples in a test suite and a :class:`kolena.workflow.TestCases` as input, and computes
 #: the corresponding test-sample-level, test-case-level, and test-suite-level metrics (and optionally plots) as output.
 #:
+#: Example implementation, relying on ``compute_per_sample`` and ``compute_aggregate`` functions implemented elsewhere:
+#:
+#: .. code-block:: python
+#:
+#:     def evaluate(
+#:         test_samples: List[TestSample],
+#:         ground_truths: List[GroundTruth],
+#:         inferences: List[Inference],
+#:         test_cases: TestCases,
+#:     ) -> EvaluationResults:
+#:         # compute per-sample metrics for each test sample
+#:         per_sample_metrics = [compute_per_sample(gt, inf) for gt, inf in zip(ground_truths, inferences)]
+#:
+#:         # compute aggregate metrics across all test cases using `test_cases.iter(...)`
+#:         aggregate_metrics: List[Tuple[TestCase, MetricsTestCase]] = []
+#:         for test_case, *s in test_cases.iter(test_samples, ground_truths, inferences, per_sample_metrics):
+#:             # subset of `test_samples`/`ground_truths`/`inferences`/`test_sample_metrics` in given test case
+#:             tc_test_samples, tc_ground_truths, tc_inferences, tc_per_sample_metrics = s
+#:             aggregate_metrics.append((test_case, compute_aggregate(tc_per_sample_metrics)))
+#:
+#:         # if desired, compute and add `plots_test_case` and `metrics_test_suite`
+#:         return EvaluationResults(
+#:             metrics_test_sample=list(zip(test_samples, per_sample_metrics)),
+#:             metrics_test_case=aggregate_metrics,
+#:         )
+#:
 #: The control flow is in general more streamlined than with :class:`kolena.workflow.Evaluator`, but requires a couple
 #: of assumptions to hold:
 #:
 #: - Test-sample-level metrics do not vary by test case
 #: - Ground truths corresponding to a given test sample do not vary by test case
 #:
 #: This ``BasicEvaluatorFunction`` is provided to the test run at runtime, and is expected to have the
@@ -167,15 +193,15 @@
     def _update_progress(self, test_case: TestCase) -> None:
         if not is_client_initialized():
             return
 
         config_description = (
             f" {_configuration_description(self._wip_configuration)}" if self._wip_configuration else ""
         )
-        message = f"Computed metrics for test case {test_case.name}{config_description}"
+        message = f"Computed metrics for test case '{test_case.name}' (v{test_case.version}){config_description}"
         progress = self._n_test_cases_processed / self._n_test_cases_and_configurations
 
         log.info(message)
         request = API.UpdateMetricsStatusRequest(
             test_run_id=self._test_run_id,
             progress=progress,
             message=message,
```

### Comparing `kolena-0.69.0/kolena/workflow/ground_truth.py` & `kolena-0.70.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/inference.py` & `kolena-0.70.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/metrics/__init__.py` & `kolena-0.70.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/metrics/_geometry.py` & `kolena-0.70.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/model.py` & `kolena-0.70.0/kolena/workflow/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             df_class=TestSampleDataFrame,
         ):
             for record in df_batch.itertuples():
                 test_sample = self.workflow.test_sample_type._from_dict(record.test_sample)
                 ground_truth = self.workflow.ground_truth_type._from_dict(record.ground_truth)
                 inference = self.workflow.inference_type._from_dict(record.inference)
                 yield test_sample, ground_truth, inference
-        log.success(f"loaded inferences from model '{self.name}' on test case '{test_case.name}'")
+        log.info(f"loaded inferences from model '{self.name}' on test case '{test_case.name}'")
 
     @classmethod
     def _from_data_with_infer(
         cls,
         data: CoreAPI.EntityData,
         infer: Optional[Callable[[TestSample], Inference]] = None,
     ) -> "Model":
```

### Comparing `kolena-0.69.0/kolena/workflow/test_case.py` & `kolena-0.70.0/kolena/workflow/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,17 @@
         """
         cls._validate_test_samples(test_samples)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
+        log.info(f"created test case '{name}' (v{obj.version})")
         if test_samples is not None:
             obj._hydrate(test_samples)
-        log.info(f"created test case '{name}' (v{obj.version})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestCase":
         """
         Load an existing test case with the provided name.
 
@@ -200,15 +200,15 @@
         ):
             has_metadata = "test_sample_metadata" in df.columns
             for record in df.itertuples():
                 metadata_field = record.test_sample_metadata if has_metadata else {}
                 test_sample = test_sample_type._from_dict({**record.test_sample, "metadata": metadata_field})
                 ground_truth = ground_truth_type._from_dict(record.ground_truth)
                 yield test_sample, ground_truth
-        log.success(f"loaded test samples in test case '{self.name}' (v{self.version})")
+        log.info(f"loaded test samples in test case '{self.name}' (v{self.version})")
 
     class Editor:
         @dataclass(frozen=True)
         class _Edit:
             test_sample: TestSample
             ground_truth: Optional[GroundTruth] = None
             remove: bool = False
```

### Comparing `kolena-0.69.0/kolena/workflow/test_run.py` & `kolena-0.70.0/kolena/workflow/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             raise WorkflowMismatchError(
                 f"model workflow ({model.workflow}) does not match test suite workflow ({test_suite.workflow})",
             )
 
         if reset:
             log.warn("overwriting existing inferences from this model (reset=True)")
         else:
-            log.info("reset flag is disabled. update existing inferences by enabling the reset flag")
+            log.info("not overwriting any existing inferences from this model (reset=False)")
 
         self.model = model
         self.test_suite = test_suite
         self.evaluator = evaluator
         self.configurations = self.evaluator.configurations if isinstance(evaluator, Evaluator) else configurations
         self.reset = reset
 
@@ -216,15 +216,15 @@
             df_class=TestSampleDataFrame,
         ):
             for record in df_batch.itertuples():
                 test_sample = self.test_suite.workflow.test_sample_type._from_dict(record.test_sample)
                 ground_truth = self.test_suite.workflow.ground_truth_type._from_dict(record.ground_truth)
                 inference = self.test_suite.workflow.inference_type._from_dict(record.inference)
                 yield test_sample, ground_truth, inference
-        log.success(f"loaded inferences from model '{self.model.name}' on test suite '{self.test_suite.name}'")
+        log.info(f"loaded inferences from model '{self.model.name}' on test suite '{self.test_suite.name}'")
 
     @validate_arguments(config=ValidatorConfig)
     def upload_inferences(self, inferences: List[Tuple[TestSample, Inference]]) -> None:
         """
         Upload inferences from a model.
 
         :param inferences: the inferences, paired with their corresponding test samples, to upload.
```

### Comparing `kolena-0.69.0/kolena/workflow/test_sample.py` & `kolena-0.70.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena-0.69.0/kolena/workflow/test_suite.py` & `kolena-0.70.0/kolena/workflow/test_suite.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -185,17 +185,17 @@
         cls._validate_workflow()
         cls._validate_test_cases(test_cases)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name, tags=tags)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
+        log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         if test_cases is not None:
             obj._hydrate(test_cases)
-        log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         return obj
 
     @classmethod
     def load(cls, name: str, version: Optional[int] = None) -> "TestSuite":
         """
         Load an existing test suite with the provided name.
```

### Comparing `kolena-0.69.0/kolena/workflow/workflow.py` & `kolena-0.70.0/kolena/workflow/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     #: role_arn to be assume-into
     assume_role_arn: str
 
 
 @dataclass(frozen=True)
 class RemoteEvaluator:
     """
-    Remote evaluator for generic workflows.
+    Remote evaluator for workflows built with ``kolena.workflow``.
     """
 
     #: The name of the workflow
     workflow: str
 
     #: The name of the evaluator
     name: str
```

### Comparing `kolena-0.69.0/pyproject.toml` & `kolena-0.70.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena"
-version = "0.69.0"  # version is automatically set to latest git tag during release process
+version = "0.70.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena-0.69.0/setup.py` & `kolena-0.70.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                                                           'pandas>=1.1,<1.6']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena',
-    'version': '0.69.0',
+    'version': '0.70.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
     'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena"><img src="https://img.shields.io/pypi/v/kolena" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena" /></a>\n  <a href="https://github.com/kolenaIO/kolena/actions"><img src="https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk" /></a>\n  <a href="https://codecov.io/gh/kolenaIO/kolena" ><img src="https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/badge.svg?token=8WOY5I8SF1"/></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/resource-docs-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\nThis `kolena` package contains the Python client library for programmatic interaction with the Kolena ML testing\nplatform.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 'pandera>=0.9.0', 'pyarrow>=8', 'pydantic>=1.8', 'requests-toolbelt',
 'requests>=2.20,<2.30', 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0',
 'tqdm>=4,<5'] extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata<5.0', 'typing-extensions>=4.5.0,<5.0.0'], ':python_version >= "3.11"':
 ['numpy>=1.23', 'pandas>=1.5,<1.6'], ':python_version >= "3.7" and
 python_version < "3.11"': ['numpy>=1.19', 'pandas>=1.1,<1.6']} entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']} setup_kwargs =
-{ 'name': 'kolena', 'version': '0.69.0', 'description': "Client for Kolena's
+{ 'name': 'kolena', 'version': '0.70.0', 'description': "Client for Kolena's
 machine learning (ML) testing and debugging platform.", 'long_description': '
                                  \n [Kolena]\n
 \n\n
 \n [https://img.shields.io/pypi/v/kolena]\n [https://img.shields.io/pypi/l/
 kolena]\n [https://img.shields.io/github/checks-status/kolenaIO/kolena/trunk]\n
 [https://codecov.io/gh/kolenaIO/kolena/branch/trunk/graph/
 badge.svg?token=8WOY5I8SF1]\n [https://img.shields.io/badge/resource-docs-
```

### Comparing `kolena-0.69.0/PKG-INFO` & `kolena-0.70.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena
-Version: 0.69.0
+Version: 0.70.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena Version: 0.69.0 Summary: Client for Kolena's
+Metadata-Version: 2.1 Name: kolena Version: 0.70.0 Summary: Client for Kolena's
 machine learning (ML) testing and debugging platform. Home-page: https://
 kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena
 Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

