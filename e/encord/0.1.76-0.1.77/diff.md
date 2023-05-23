# Comparing `tmp/encord-0.1.76.tar.gz` & `tmp/encord-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.76.tar", max compression
+gzip compressed data, was "encord-0.1.77.tar", max compression
```

## Comparing `encord-0.1.76.tar` & `encord-0.1.77.tar`

### file list

```diff
@@ -1,75 +1,74 @@
--rw-r--r--   0        0        0    11330 2023-05-22 16:10:18.357820 encord-0.1.76/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-22 16:10:18.357820 encord-0.1.76/README.md
--rw-r--r--   0        0        0       84 2023-05-22 16:10:18.357820 encord-0.1.76/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-05-22 16:10:18.377820 encord-0.1.76/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-05-22 16:10:18.377820 encord-0.1.76/encord/_version.py
--rw-r--r--   0        0        0    49178 2023-05-22 16:10:18.377820 encord-0.1.76/encord/client.py
--rw-r--r--   0        0        0    10825 2023-05-22 16:10:18.377820 encord-0.1.76/encord/configs.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/enums.py
--rw-r--r--   0        0        0     3211 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-05-22 16:10:18.377820 encord-0.1.76/encord/dataset.py
--rw-r--r--   0        0        0     6302 2023-05-22 16:10:18.377820 encord-0.1.76/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/__init__.py
--rw-r--r--   0        0        0     5329 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/limits.py
--rw-r--r--   0        0        0     7875 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/__init__.py
--rw-r--r--   0        0        0      145 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/classification.py
--rw-r--r--   0        0        0    29709 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/common.py
--rw-r--r--   0        0        0      172 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   139903 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      137 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      148 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-05-22 16:10:18.377820 encord-0.1.76/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/api_key.py
--rw-r--r--   0        0        0     5377 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32206 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      188 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/model.py
--rw-r--r--   0        0        0      745 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/ontology.py
--rw-r--r--   0        0        0     8844 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    39203 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27840 2023-05-22 16:10:18.381820 encord-0.1.76/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1685 2023-05-22 16:10:18.381820 encord-0.1.76/pyproject.toml
--rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encord-0.1.76/setup.py
--rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 encord-0.1.76/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-05-23 12:12:07.482519 encord-0.1.77/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-23 12:12:07.482519 encord-0.1.77/README.md
+-rw-r--r--   0        0        0       84 2023-05-23 12:12:07.482519 encord-0.1.77/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-23 12:12:07.498519 encord-0.1.77/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-23 12:12:07.498519 encord-0.1.77/encord/_version.py
+-rw-r--r--   0        0        0    49201 2023-05-23 12:12:07.498519 encord-0.1.77/encord/client.py
+-rw-r--r--   0        0        0    10825 2023-05-23 12:12:07.498519 encord-0.1.77/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/enums.py
+-rw-r--r--   0        0        0     3211 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-05-23 12:12:07.498519 encord-0.1.77/encord/dataset.py
+-rw-r--r--   0        0        0     6363 2023-05-23 12:12:07.498519 encord-0.1.77/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/__init__.py
+-rw-r--r--   0        0        0     5329 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/limits.py
+-rw-r--r--   0        0        0     7875 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/classification.py
+-rw-r--r--   0        0        0    29709 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/common.py
+-rw-r--r--   0        0        0      172 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   139937 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      137 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      148 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-05-23 12:12:07.498519 encord-0.1.77/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5377 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32206 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      188 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/model.py
+-rw-r--r--   0        0        0      745 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8844 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    39203 2023-05-23 12:12:07.498519 encord-0.1.77/encord/project.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-23 12:12:07.498519 encord-0.1.77/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    27840 2023-05-23 12:12:07.502519 encord-0.1.77/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1685 2023-05-23 12:12:07.502519 encord-0.1.77/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 encord-0.1.77/PKG-INFO
```

### Comparing `encord-0.1.76/LICENSE` & `encord-0.1.77/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/README.md` & `encord-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/client.py` & `encord-0.1.77/encord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,44 +41,52 @@
 import time
 import typing
 import uuid
 from datetime import datetime
 from math import ceil
 from pathlib import Path
 from typing import Iterable, List, Optional, Tuple, Union
+
 import requests
+
 import encord.exceptions
 from encord.configs import ENCORD_DOMAIN, ApiKeyConfig, Config, EncordConfig
+from encord.constants.enums import DataType
 from encord.constants.model import AutomationModels, Device
 from encord.constants.string_constants import *
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
 from encord.http.utils import (
     CloudUploadSettings,
     upload_images_to_encord,
     upload_to_signed_url_list,
     upload_video_to_encord,
 )
 from encord.orm.api_key import ApiKeyMeta
 from encord.orm.cloud_integration import CloudIntegration
-from encord.orm.dataset import DEFAULT_DATASET_ACCESS_SETTINGS, AddPrivateDataResponse
-from encord.orm.dataset import Dataset as OrmDataset, DataRows, DataRow
 from encord.orm.dataset import (
-    DatasetDataLongPolling,
-    LongPollingStatus,
+    DEFAULT_DATASET_ACCESS_SETTINGS,
+    AddPrivateDataResponse,
+    DataRow,
+    DataRows,
+)
+from encord.orm.dataset import Dataset as OrmDataset
+from encord.orm.dataset import (
     DatasetAccessSettings,
     DatasetData,
+    DatasetDataLongPolling,
     DatasetUser,
     DatasetUserRole,
     DatasetUsers,
     DicomSeries,
     Image,
     ImageGroup,
     ImageGroupOCR,
     Images,
+    LongPollingStatus,
     ReEncodeVideoTask,
     SingleImage,
     Video,
 )
 from encord.orm.label_log import LabelLog
 from encord.orm.label_row import (
     AnnotationTaskStatus,
@@ -117,15 +125,14 @@
     ProjectUsers,
 )
 from encord.project_ontology.classification_type import ClassificationType
 from encord.project_ontology.object_type import ObjectShape
 from encord.project_ontology.ontology import Ontology
 from encord.utilities.client_utilities import optional_set_to_list, parse_datetime
 from encord.utilities.project_user import ProjectUser, ProjectUserRole
-from encord.constants.enums import DataType
 
 LONG_POLLING_RESPONSE_RETRY_N = 3
 LONG_POLLING_SLEEP_ON_FAILURE_SECONDS = 3
 LONG_POLLING_MAX_REQUEST_TIME_SECONDS = 60
 
 logger = logging.getLogger(__name__)
```

### Comparing `encord-0.1.76/encord/configs.py` & `encord-0.1.77/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/constants/enums.py` & `encord-0.1.77/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/constants/model.py` & `encord-0.1.77/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/constants/model_weights.py` & `encord-0.1.77/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/constants/string_constants.py` & `encord-0.1.77/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/constants/test/test_enums.py` & `encord-0.1.77/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/dataset.py` & `encord-0.1.77/encord/dataset.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from pathlib import Path
 from datetime import datetime
+from pathlib import Path
 from typing import Dict, Iterable, List, Optional, TextIO, Union
 
 from encord.client import EncordClientDataset
+from encord.constants.enums import DataType
 from encord.http.utils import CloudUploadSettings
 from encord.orm.cloud_integration import CloudIntegration
 from encord.orm.dataset import AddPrivateDataResponse, DataRow
 from encord.orm.dataset import Dataset as OrmDataset
 from encord.orm.dataset import (
-    DatasetDataLongPolling,
     DatasetAccessSettings,
+    DatasetDataLongPolling,
     DatasetUser,
     DatasetUserRole,
     Image,
     ImageGroupOCR,
     StorageLocation,
 )
-from encord.constants.enums import DataType
 
 
 class Dataset:
     """
     Access dataset related data and manipulate the dataset.
     """
```

### Comparing `encord-0.1.76/encord/exceptions.py` & `encord-0.1.77/encord/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 import time
-from datetime import datetime, timezone
 from dataclasses import dataclass, field, fields
+from datetime import datetime, timezone
 from typing import Optional
 
 
 @dataclass
 class ExceptionContext:
     timestamp: datetime = field(default_factory=lambda: datetime.now(tz=timezone.utc).isoformat())
 
@@ -244,16 +244,16 @@
 
 
 class MultiLabelLimitError(EncordException):
     """
     Too many labels were requested
     """
 
-    def __init__(self, message, maximum_labels_allowed: int):
-        super().__init__(message=message)
+    def __init__(self, message, maximum_labels_allowed: int, context: Optional[ExceptionContext] = None):
+        super().__init__(message=message, context=context)
         self.maximum_labels_allowed = maximum_labels_allowed
 
 
 class LabelRowError(EncordException):
     """An error thrown when the construction of a LabelRow class is invalid."""
 
     pass
```

### Comparing `encord-0.1.76/encord/http/bundle.py` & `encord-0.1.77/encord/http/bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
-from typing import Callable, TypeVar, Optional, List, Dict, Tuple, Generic, Generator
 from dataclasses import asdict, dataclass, field
 from functools import reduce
+from typing import Callable, Dict, Generator, Generic, List, Optional, Tuple, TypeVar
 
 log = logging.getLogger(__name__)
 
 T = TypeVar("T")
 R = TypeVar("R")
```

### Comparing `encord-0.1.76/encord/http/constants.py` & `encord-0.1.77/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/http/error_utils.py` & `encord-0.1.77/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/http/querier.py` & `encord-0.1.77/encord/http/querier.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 import dataclasses
 import logging
 import platform
-import uuid
 import random
+import uuid
 from contextlib import contextmanager
-from typing import Any, List, Tuple, Optional, Type, TypeVar, Generator
+from typing import Any, Generator, List, Optional, Tuple, Type, TypeVar
 
 import requests
 import requests.exceptions
-from requests import Session, Response
+from requests import Response, Session
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
+from encord._version import __version__ as encord_version
 from encord.configs import BaseConfig
 from encord.exceptions import *
 from encord.http.error_utils import check_error_response
 from encord.http.query_methods import QueryMethods
 from encord.http.request import Request
 from encord.orm.formatter import Formatter
-from encord._version import __version__ as encord_version
 
 logger = logging.getLogger(__name__)
 
 HEADER_USER_AGENT = "User-Agent"
 HEADER_CLOUD_TRACE_CONTEXT = "X-Cloud-Trace-Context"
```

### Comparing `encord-0.1.76/encord/http/query_methods.py` & `encord-0.1.77/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/http/request.py` & `encord-0.1.77/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/http/utils.py` & `encord-0.1.77/encord/http/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import mimetypes
 import os.path
 from dataclasses import dataclass
-from typing import List, Optional, Type, TypeVar, Union, Iterable
+from typing import Iterable, List, Optional, Type, TypeVar, Union
 
 from tqdm import tqdm
 
 from encord.configs import BaseConfig
 from encord.exceptions import CloudUploadError
 from encord.http.querier import Querier, create_new_session
 from encord.orm.dataset import (
```

### Comparing `encord-0.1.76/encord/objects/common.py` & `encord-0.1.77/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/objects/coordinates.py` & `encord-0.1.77/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/objects/frames.py` & `encord-0.1.77/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/objects/internal_helpers.py` & `encord-0.1.77/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/objects/ontology_labels_impl.py` & `encord-0.1.77/encord/objects/ontology_labels_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,24 @@
     Union,
     overload,
 )
 from uuid import uuid4
 
 from dateutil.parser import parse
 
-from encord.client import EncordClientProject, LabelRow as OrmLabelRow
+from encord.client import EncordClientProject
+from encord.client import LabelRow as OrmLabelRow
 from encord.constants.enums import DataType
-from encord.exceptions import LabelRowError, OntologyError
+from encord.exceptions import LabelRowError, OntologyError, WrongProjectTypeError
+from encord.http.bundle import Bundle, BundleResultHandler, BundleResultMapper
+from encord.http.limits import (
+    LABEL_ROW_BUNDLE_CREATE_LIMIT,
+    LABEL_ROW_BUNDLE_GET_LIMIT,
+    LABEL_ROW_BUNDLE_SAVE_LIMIT,
+)
 from encord.objects.common import (
     Attribute,
     AttributeClasses,
     AttributeTypes,
     ChecklistAttribute,
     FlatOption,
     NestableOption,
@@ -85,18 +92,20 @@
     check_email,
     check_type,
     does_type_match,
     filter_by_type,
     short_uuid_str,
 )
 from encord.orm.formatter import Formatter
-from encord.orm.label_row import AnnotationTaskStatus, LabelRowMetadata, LabelStatus, WorkflowGraphNode
-from encord.exceptions import WrongProjectTypeError
-from encord.http.bundle import Bundle, BundleResultHandler, BundleResultMapper
-from encord.http.limits import LABEL_ROW_BUNDLE_GET_LIMIT, LABEL_ROW_BUNDLE_CREATE_LIMIT, LABEL_ROW_BUNDLE_SAVE_LIMIT
+from encord.orm.label_row import (
+    AnnotationTaskStatus,
+    LabelRowMetadata,
+    LabelStatus,
+    WorkflowGraphNode,
+)
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Object:
     """
```

### Comparing `encord-0.1.76/encord/objects/project.py` & `encord-0.1.77/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/objects/utils.py` & `encord-0.1.77/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/ontology.py` & `encord-0.1.77/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/api_key.py` & `encord-0.1.77/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/base_orm.py` & `encord-0.1.77/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/dataset.py` & `encord-0.1.77/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/dataset_with_user_role.py` & `encord-0.1.77/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/label_log.py` & `encord-0.1.77/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/label_row.py` & `encord-0.1.77/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/labeling_algorithm.py` & `encord-0.1.77/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/model.py` & `encord-0.1.77/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/ontology.py` & `encord-0.1.77/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/project.py` & `encord-0.1.77/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/project_api_key.py` & `encord-0.1.77/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/project_with_user_role.py` & `encord-0.1.77/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/orm/test/test_dataset.py` & `encord-0.1.77/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/project.py` & `encord-0.1.77/encord/project.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 from typing import Iterable, List, Optional, Set, Tuple, Union
 
 from encord.client import EncordClientProject
 from encord.constants.model import AutomationModels, Device
+from encord.http.bundle import Bundle
 from encord.objects import LabelRowV2
+from encord.ontology import Ontology
 from encord.orm.cloud_integration import CloudIntegration
 from encord.orm.dataset import Image, Video
 from encord.orm.label_log import LabelLog
 from encord.orm.label_row import (
     AnnotationTaskStatus,
     LabelRow,
     LabelRowMetadata,
@@ -17,16 +19,14 @@
 from encord.orm.model import ModelConfiguration, ModelTrainingWeights, TrainingMetadata
 from encord.orm.project import CopyDatasetOptions, CopyLabelsOptions
 from encord.orm.project import Project as OrmProject
 from encord.project_ontology.classification_type import ClassificationType
 from encord.project_ontology.object_type import ObjectShape
 from encord.project_ontology.ontology import Ontology as LegacyOntology
 from encord.utilities.project_user import ProjectUser, ProjectUserRole
-from encord.ontology import Ontology
-from encord.http.bundle import Bundle
 
 
 class Project:
     """
     Access project related data and manipulate the project.
     """
```

### Comparing `encord-0.1.76/encord/project_ontology/classification_attribute.py` & `encord-0.1.77/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/project_ontology/classification_option.py` & `encord-0.1.77/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/project_ontology/ontology.py` & `encord-0.1.77/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/project_ontology/ontology_classification.py` & `encord-0.1.77/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/project_ontology/ontology_object.py` & `encord-0.1.77/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/user_client.py` & `encord-0.1.77/encord/user_client.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import base64
-from datetime import datetime
 import logging
+from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import dateutil
 
 # add this for backward compatible class comparisons
```

### Comparing `encord-0.1.76/encord/utilities/client_utilities.py` & `encord-0.1.77/encord/utilities/client_utilities.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-from datetime import datetime
 import pprint
 from dataclasses import dataclass
+from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Set, TypeVar, Union
 
 from dateutil import parser as datetime_parser
 
 
 def pretty_print(data):
```

### Comparing `encord-0.1.76/encord/utilities/label_utilities.py` & `encord-0.1.77/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/encord/utilities/project_user.py` & `encord-0.1.77/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.76/pyproject.toml` & `encord-0.1.77/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.76"
+version = "0.1.77"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.76/setup.py` & `encord-0.1.77/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,103 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: encord
+Version: 0.1.77
+Summary: Encord Python SDK Client
+Home-page: https://github.com/encord-team/encord-client-python
+License: Apache Software License
+Keywords: cord,encord
+Author: Cord Technologies Limited
+Author-email: hello@encord.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=3.4.8,<4.0.0)
+Requires-Dist: importlib_metadata (>=6.1.0,<7.0.0) ; python_version < "3.8"
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.25.0,<3.0.0)
+Requires-Dist: tqdm (>=4.32.1,<5.0.0)
+Project-URL: Documentation, https://python.docs.encord.com/
+Project-URL: Repository, https://github.com/encord-team/encord-client-python
+Description-Content-Type: text/markdown
 
-packages = \
-['cord',
- 'encord',
- 'encord.constants',
- 'encord.constants.test',
- 'encord.http',
- 'encord.objects',
- 'encord.orm',
- 'encord.orm.test',
- 'encord.project_ontology',
- 'encord.utilities']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cryptography>=3.4.8,<4.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'requests>=2.25.0,<3.0.0',
- 'tqdm>=4.32.1,<5.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']}
-
-setup_kwargs = {
-    'name': 'encord',
-    'version': '0.1.76',
-    'description': 'Encord Python SDK Client',
-    'long_description': '<h1 align="center">\n  <p align="center">Encord Python API Client</p>\n  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>\n</h1>\n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer vision***\n\n## 💻 Features\n\n- Minimal low-level Python client that allows you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`\n\n## ✨ Relevant Links\n* [Encord website](https://encord.com)\n* [Encord web app](https://app.encord.com)\n* [Encord documentation](https://docs.encord.com)\n\n## 💡 Getting Started\n\nFor full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).\n\nFirst, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:\n\n```bash\npip install encord\n```\n\nThen, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.\n\n```bash\nexport ENCORD_PROJECT_ID="<project_id>"\nexport ENCORD_API_KEY="<project_api_key>"\n```\n\nPassing the resource ID and API key as environment variables, you can initialise the Encord client directly.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\n```\n\nIf you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise("<resource_id>", "<resource_api_key>")\n```\n\nIf you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.\n\n```py\nfrom encord.client import EncordClient\nfrom encord.client import EncordConfig\n\nconfig = EncordConfig("<resource_id>", "<resource_api_key>")\nclient = EncordClient.initialise_with_config(config)\n```\n\nOnce you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.\n\n```py\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\nproject = client.get_project()\n```\n\n## 🐛 Troubleshooting\n\nPlease report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.\n',
-    'author': 'Cord Technologies Limited',
-    'author_email': 'hello@encord.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/encord-team/encord-client-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+<h1 align="center">
+  <p align="center">Encord Python API Client</p>
+  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>
+</h1>
 
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+***The data engine for computer vision***
+
+## 💻 Features
+
+- Minimal low-level Python client that allows you to interact with Encord's API
+- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`
+
+## ✨ Relevant Links
+* [Encord website](https://encord.com)
+* [Encord web app](https://app.encord.com)
+* [Encord documentation](https://docs.encord.com)
+
+## 💡 Getting Started
+
+For full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).
+
+First, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
+
+```bash
+pip install encord
+```
+
+Then, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.
+
+```bash
+export ENCORD_PROJECT_ID="<project_id>"
+export ENCORD_API_KEY="<project_api_key>"
+```
+
+Passing the resource ID and API key as environment variables, you can initialise the Encord client directly.
+
+```python
+from encord.client import EncordClient
+
+client = EncordClient.initialise()
+```
+
+If you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.
+
+```python
+from encord.client import EncordClient
+
+client = EncordClient.initialise("<resource_id>", "<resource_api_key>")
+```
+
+If you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.
+
+```py
+from encord.client import EncordClient
+from encord.client import EncordConfig
+
+config = EncordConfig("<resource_id>", "<resource_api_key>")
+client = EncordClient.initialise_with_config(config)
+```
+
+Once you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.
+
+```py
+from encord.client import EncordClient
+
+client = EncordClient.initialise()
+project = client.get_project()
+```
+
+## 🐛 Troubleshooting
+
+Please report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,48 +1,48 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['cord',
-'encord', 'encord.constants', 'encord.constants.test', 'encord.http',
-'encord.objects', 'encord.orm', 'encord.orm.test', 'encord.project_ontology',
-'encord.utilities'] package_data = \ {'': ['*']} install_requires = \
-['cryptography>=3.4.8,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0',
-'requests>=2.25.0,<3.0.0', 'tqdm>=4.32.1,<5.0.0'] extras_require = \ {':
-python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']} setup_kwargs =
-{ 'name': 'encord', 'version': '0.1.76', 'description': 'Encord Python SDK
-Client', 'long_description': '
-           ****** \nEncord Python API Client\n [Cord_logo]\n ******
-\n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)]
-(https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer
-vision***\n\n## ð» Features\n\n- Minimal low-level Python client that allows
-you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and
-`3.10`\n\n## â¨ Relevant Links\n* [Encord website](https://encord.com)\n*
-[Encord web app](https://app.encord.com)\n* [Encord documentation](https://
-docs.encord.com)\n\n## ð¡ Getting Started\n\nFor full documentation, please
-visit [Encord Python SDK](https://python.docs.encord.com/).\n\nFirst, install
-Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/
-installing) package manager:\n\n```bash\npip install encord\n```\n\nThen,
-create an API key for authentication via the [Encord web app](https://
-app.encord.com). Pass the resource ID and API key as environment variables or
-pass them explicitly when you initialise the EncordClient
-object.\n\n```bash\nexport ENCORD_PROJECT_ID=""\nexport
-ENCORD_API_KEY=""\n```\n\nPassing the resource ID and API key as environment
-variables, you can initialise the Encord client directly.\n\n```python\nfrom
-encord.client import EncordClient\n\nclient = EncordClient.initialise
-()\n```\n\nIf you want to avoid setting environment variables, you can
-initialise the Encord client by passing the resource ID and API key as
-strings.\n\n```python\nfrom encord.client import EncordClient\n\nclient =
-EncordClient.initialise("", "")\n```\n\nIf you wish to instantiate several
-client objects and avoid passing parameters each time, you can instantiate a
-EncordConfig object, pass the resource ID and API key as strings, and
-initialise the client with the config object.\n\n```py\nfrom encord.client
-import EncordClient\nfrom encord.client import EncordConfig\n\nconfig =
-EncordConfig("", "")\nclient = EncordClient.initialise_with_config
-(config)\n```\n\nOnce you have instantiated an Encord client, it is easy to
-fetch information associated with the given resource ID.\n\n```py\nfrom
-encord.client import EncordClient\n\nclient = EncordClient.initialise
-()\nproject = client.get_project()\n```\n\n## ð Troubleshooting\n\nPlease
-report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-
-python/issues). Just make sure you read the [Encord documentation](https://
-docs.encord.com) and search for related issues first.\n', 'author': 'Cord
-Technologies Limited', 'author_email': 'hello@encord.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/encord-team/
-encord-client-python', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: encord Version: 0.1.77 Summary: Encord Python SDK
+Client Home-page: https://github.com/encord-team/encord-client-python License:
+Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
+Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
+:: OSI Approved :: Apache Software License Classifier: License :: Other/
+Proprietary License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: cryptography (>=3.4.8,<4.0.0) Requires-Dist: importlib_metadata
+(>=6.1.0,<7.0.0) ; python_version < "3.8" Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm
+(>=4.32.1,<5.0.0) Project-URL: Documentation, https://python.docs.encord.com/
+Project-URL: Repository, https://github.com/encord-team/encord-client-python
+Description-Content-Type: text/markdown
+               ****** Encord Python API Client[Cord_logo] ******
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
+//opensource.org/licenses/Apache-2.0) ***The data engine for computer vision***
+## ð» Features - Minimal low-level Python client that allows you to interact
+with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, and `3.10` ## â¨
+Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
+//app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
+Getting Started For full documentation, please visit [Encord Python SDK](https:
+//python.docs.encord.com/). First, install Encord Python API Client using the
+[pip](https://pip.pypa.io/en/stable/installing) package manager: ```bash pip
+install encord ``` Then, create an API key for authentication via the [Encord
+web app](https://app.encord.com). Pass the resource ID and API key as
+environment variables or pass them explicitly when you initialise the
+EncordClient object. ```bash export ENCORD_PROJECT_ID="" export
+ENCORD_API_KEY="" ``` Passing the resource ID and API key as environment
+variables, you can initialise the Encord client directly. ```python from
+encord.client import EncordClient client = EncordClient.initialise() ``` If you
+want to avoid setting environment variables, you can initialise the Encord
+client by passing the resource ID and API key as strings. ```python from
+encord.client import EncordClient client = EncordClient.initialise("", "") ```
+If you wish to instantiate several client objects and avoid passing parameters
+each time, you can instantiate a EncordConfig object, pass the resource ID and
+API key as strings, and initialise the client with the config object. ```py
+from encord.client import EncordClient from encord.client import EncordConfig
+config = EncordConfig("", "") client = EncordClient.initialise_with_config
+(config) ``` Once you have instantiated an Encord client, it is easy to fetch
+information associated with the given resource ID. ```py from encord.client
+import EncordClient client = EncordClient.initialise() project =
+client.get_project() ``` ## ð Troubleshooting Please report bugs to [GitHub
+Issues](https://github.com/encord-team/encord-client-python/issues). Just make
+sure you read the [Encord documentation](https://docs.encord.com) and search
+for related issues first.
```

