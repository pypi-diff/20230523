# Comparing `tmp/cognite_power_ops-0.5.0.tar.gz` & `tmp/cognite_power_ops-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.5.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.6.0.tar", max compression
```

## Comparing `cognite_power_ops-0.5.0.tar` & `cognite_power_ops-0.6.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    10758 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/LICENSE
--rw-r--r--   0        0        0      250 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/README.md
--rw-r--r--   0        0        0       76 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0       65 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0     6203 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/asset_apis.py
--rw-r--r--   0        0        0      601 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2037 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0     1883 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm_apis.py
--rw-r--r--   0        0        0     2294 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0     2990 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/shop_api.py
--rw-r--r--   0        0        0    26552 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/asset_lists.py
--rw-r--r--   0        0        0     3057 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0      129 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/config_model.py
--rw-r--r--   0        0        0     3630 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/core.py
--rw-r--r--   0        0        0      128 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/generators.py
--rw-r--r--   0        0        0     1482 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16698 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0       99 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/price_area.py
--rw-r--r--   0        0        0     5114 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0      180 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/reservoirs.py
--rw-r--r--   0        0        0     1609 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0      163 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/shared.py
--rw-r--r--   0        0        0     2171 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     5039 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/version.py
--rw-r--r--   0        0        0     1434 2023-05-16 11:32:00.034569 cognite_power_ops-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/README.md
+-rw-r--r--   0        0        0       76 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10362 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0       65 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6203 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2037 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0     1883 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/dm_apis.py
+-rw-r--r--   0        0        0     2294 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0     2990 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/client/shop_api.py
+-rw-r--r--   0        0        0    27013 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0     3057 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0      128 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/generators.py
+-rw-r--r--   0        0        0     1482 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16698 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-22 12:26:52.378082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0     1609 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0      163 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2171 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1323 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     5039 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1434 2023-05-22 12:26:52.382082 cognite_power_ops-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.6.0/PKG-INFO
```

### Comparing `cognite_power_ops-0.5.0/LICENSE` & `cognite_power_ops-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.6.0/cognite/powerops/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 from pathlib import Path
 from typing import List, Optional
 
 from cognite.client import CogniteClient
 
 from cognite.powerops.config import (
     BidMatrixGeneratorConfig,
@@ -151,15 +152,18 @@
         "https://shop-production.az-inso-powerops.cognite.ai/submit-run"
         if cognite_project.endswith("-prod")
         else "https://shop-staging.az-inso-powerops.cognite.ai/submit-run"
     )
 
 
 def _load_config(path: Path) -> BootstrapConfig:
-    return BootstrapConfig.from_yamls(path)
+    config = BootstrapConfig.from_yamls(path)
+    if os.environ.get("COGNITE_PROJECT"):
+        config.cdf.from_env()
+    return config
 
 
 def _transform(
     config: BootstrapConfig,
     path: Path,
     market: str = "Dayahead",
 ) -> BootstrapResourceCollection:
```

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/asset_apis.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/asset_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/dm/client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.6.0/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/dm/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/dm_apis.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/dm_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/client/shop_api.py` & `cognite_power_ops-0.6.0/cognite/powerops/client/shop_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/config.py` & `cognite_power_ops-0.6.0/cognite/powerops/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import ast
 import json
+import os
 import typing
 from collections import defaultdict
 from pathlib import Path
-from typing import ClassVar, Dict, Generator, List, Optional, Tuple, Union
+from typing import ClassVar, Dict, Generator, List, Optional, Tuple
 
 from cognite.client.data_classes import Asset, Label, Sequence
 from pydantic import BaseModel, Field, root_validator, validator
 
 from cognite.powerops.data_classes.benchmarking_config import BenchmarkingConfig
 from cognite.powerops.data_classes.cdf_resource_collection import (
     BootstrapResourceCollection,
@@ -395,24 +396,34 @@
 
 MARKET_BY_PRICE_AREA = {"NO2": "Dayahead", "NO1": "1", "NO3": "1", "NO5": "1"}
 
 
 class CDFConfig(BaseModel):
     TENANT_ID: str
     CLIENT_ID: str
-    CLIENT_SECRET_ENV: Union[str, None] = None
     CDF_CLUSTER: str
     COGNITE_PROJECT: str
     SPACE_ID: str
     DATA_MODEL: str
     SCHEMA_VERSION: str
 
     @classmethod
-    def from_yaml(cls, yaml_path: Path) -> "CDFConfig":
-        return cls(**load_yaml(yaml_path))
+    def from_env(cls) -> "CDFConfig":
+        return cls(
+            **{
+                "TENANT_ID": os.environ.get("TENANT_ID"),
+                "CLIENT_ID": os.environ.get("CLIENT_ID"),
+                "CLIENT_SECRET_ENV": os.environ.get("CLIENT_SECRET_ENV"),
+                "CDF_CLUSTER": os.environ.get("CDF_CLUSTER"),
+                "COGNITE_PROJECT": os.environ.get("COGNITE_PROJECT"),
+                "SPACE_ID": os.environ.get("SPACE_ID"),
+                "DATA_MODEL": os.environ.get("DATA_MODEL"),
+                "SCHEMA_VERSION": os.environ.get("SCHEMA_VERSION"),
+            }
+        )
 
 
 class ReserveScenarios(BaseModel):
     volumes: list[int]
     auction: Auction
     product: Product
     block: Block
```

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/asset_lists.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/asset_lists.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/core.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/market_config.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.6.0/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/logger.py` & `cognite_power_ops-0.6.0/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/main.py` & `cognite_power_ops-0.6.0/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/cdf_auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,19 @@
 def get_client(parameters: dict) -> CogniteClient:
     client_name = "power-ops-bootstrap"
 
     client_id = parameters.get("CLIENT_ID")
     cluster = parameters.get("CDF_CLUSTER")
     project = parameters.get("COGNITE_PROJECT")
     tenant_id = parameters.get("TENANT_ID")
-    client_secret_env = parameters.get("CLIENT_SECRET_ENV")
 
     base_url = f"https://{cluster}.cognitedata.com"
     scopes = [f"https://{cluster}.cognitedata.com/.default"]
 
-    client_secret = os.getenv(client_secret_env) if client_secret_env else None
-
-    if client_secret:
+    if client_secret := os.getenv("POWER_OPS_CLIENT_SECRET"):
         token_url = f"https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token"
         creds = OAuthClientCredentials(
             token_url=token_url,
             client_id=client_id,
             client_secret=client_secret,
             scopes=scopes,
         )
```

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/common.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/files.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.6.0/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.5.0/pyproject.toml` & `cognite_power_ops-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.5.0"
+version = "0.6.0"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
```

### Comparing `cognite_power_ops-0.5.0/PKG-INFO` & `cognite_power_ops-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.5.0
+Version: 0.6.0
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

