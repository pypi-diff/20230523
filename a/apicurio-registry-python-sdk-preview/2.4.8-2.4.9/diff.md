# Comparing `tmp/apicurio_registry_python_sdk_preview-2.4.8.tar.gz` & `tmp/apicurio_registry_python_sdk_preview-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.8.tar", max compression
+gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.9.tar", max compression
```

## Comparing `apicurio_registry_python_sdk_preview-2.4.8.tar` & `apicurio_registry_python_sdk_preview-2.4.9.tar`

### file list

```diff
@@ -1,5 +1,86 @@
--rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurio_registry_python_sdk_preview-2.4.8/README.md
--rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurio_registry_python_sdk_preview-2.4.8/apicurioregistrysdk/__init__.py
--rw-r--r--   0        0        0     2233 2023-05-18 14:39:08.122837 apicurio_registry_python_sdk_preview-2.4.8/kiota-gen.py
--rw-r--r--   0        0        0     1117 2023-05-18 15:26:40.288604 apicurio_registry_python_sdk_preview-2.4.8/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurio_registry_python_sdk_preview-2.4.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/__init__.py
+-rw-r--r--   0        0        0     6316 2023-05-18 15:26:48.351512 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/admin_request_builder.py
+-rw-r--r--   0        0        0     4141 2023-05-18 15:26:48.336614 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py
+-rw-r--r--   0        0        0     2509 2023-05-18 15:26:48.342182 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/config/config_request_builder.py
+-rw-r--r--   0        0        0     9895 2023-05-18 15:26:48.345382 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
+-rw-r--r--   0        0        0     4230 2023-05-18 15:26:48.343445 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py
+-rw-r--r--   0        0        0     4497 2023-05-18 15:26:48.350037 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/export/export_request_builder.py
+-rw-r--r--   0        0        0     4016 2023-05-18 15:26:48.356132 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/import_/import_request_builder.py
+-rw-r--r--   0        0        0     9210 2023-05-18 15:26:48.338950 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py
+-rw-r--r--   0        0        0     3970 2023-05-18 15:26:48.340039 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py
+-rw-r--r--   0        0        0     9490 2023-05-18 15:26:48.348644 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
+-rw-r--r--   0        0        0     6823 2023-05-18 15:26:48.346663 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py
+-rw-r--r--   0        0        0     9847 2023-05-18 15:26:48.353602 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0     9029 2023-05-18 15:26:48.355219 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/admin/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     7675 2023-05-18 15:26:48.442874 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/groups_request_builder.py
+-rw-r--r--   0        0        0    17933 2023-05-18 15:26:48.446922 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0    12567 2023-05-18 15:26:48.449529 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6977 2023-05-18 15:26:48.471504 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
+-rw-r--r--   0        0        0    11150 2023-05-18 15:26:48.467673 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0    10297 2023-05-18 15:26:48.469665 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     4942 2023-05-18 15:26:48.475808 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py
+-rw-r--r--   0        0        0     6104 2023-05-18 15:26:48.472644 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py
+-rw-r--r--   0        0        0    10548 2023-05-18 15:26:48.457784 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6008 2023-05-18 15:26:48.453000 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4767 2023-05-18 15:26:48.451445 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
+-rw-r--r--   0        0        0    10171 2023-05-18 15:26:48.455153 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
+-rw-r--r--   0        0        0     9632 2023-05-18 15:26:48.459654 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
+-rw-r--r--   0        0        0    16487 2023-05-18 15:26:48.474837 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
+-rw-r--r--   0        0        0     7662 2023-05-18 15:26:48.444555 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py
+-rw-r--r--   0        0        0     1299 2023-05-18 15:26:48.436389 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py
+-rw-r--r--   0        0        0     4122 2023-05-18 15:26:48.434237 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4828 2023-05-18 15:26:48.435602 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
+-rw-r--r--   0        0        0     1287 2023-05-18 15:26:48.425900 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py
+-rw-r--r--   0        0        0     4108 2023-05-18 15:26:48.427518 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4820 2023-05-18 15:26:48.428601 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py
+-rw-r--r--   0        0        0     1283 2023-05-18 15:26:48.432550 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py
+-rw-r--r--   0        0        0     4807 2023-05-18 15:26:48.430095 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     5362 2023-05-18 15:26:48.431773 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py
+-rw-r--r--   0        0        0     4913 2023-05-18 15:26:48.437780 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/ids/ids_request_builder.py
+-rw-r--r--   0        0        0     1159 2023-05-18 15:26:48.527852 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/kiota-lock.json
+-rw-r--r--   0        0        0     4573 2023-05-18 15:26:48.398394 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_content.py
+-rw-r--r--   0        0        0    15041 2023-05-18 15:26:48.392622 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_meta_data.py
+-rw-r--r--   0        0        0     3253 2023-05-18 15:26:48.369986 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_owner.py
+-rw-r--r--   0        0        0     5461 2023-05-18 15:26:48.387558 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_reference.py
+-rw-r--r--   0        0        0     4781 2023-05-18 15:26:48.385280 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_search_results.py
+-rw-r--r--   0        0        0      134 2023-05-18 15:26:48.383910 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_state.py
+-rw-r--r--   0        0        0     3192 2023-05-18 15:26:48.393923 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/artifact_type_info.py
+-rw-r--r--   0        0        0     5921 2023-05-18 15:26:48.380761 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/configuration_property.py
+-rw-r--r--   0        0        0     4961 2023-05-18 15:26:48.408154 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/create_group_meta_data.py
+-rw-r--r--   0        0        0     3989 2023-05-18 15:26:48.418017 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/download_ref.py
+-rw-r--r--   0        0        0     5719 2023-05-18 15:26:48.400789 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/editable_meta_data.py
+-rw-r--r--   0        0        0     5777 2023-05-18 15:26:48.404147 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/error.py
+-rw-r--r--   0        0        0     8023 2023-05-18 15:26:48.407052 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/group_meta_data.py
+-rw-r--r--   0        0        0     4661 2023-05-18 15:26:48.410154 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/group_search_results.py
+-rw-r--r--   0        0        0    14563 2023-05-18 15:26:48.402780 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/limits.py
+-rw-r--r--   0        0        0     2597 2023-05-18 15:26:48.404921 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/log_configuration.py
+-rw-r--r--   0        0        0      281 2023-05-18 15:26:48.385763 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/log_level.py
+-rw-r--r--   0        0        0     3217 2023-05-18 15:26:48.399788 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/named_log_configuration.py
+-rw-r--r--   0        0        0     2605 2023-05-18 15:26:48.368799 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/properties.py
+-rw-r--r--   0        0        0     4978 2023-05-18 15:26:48.416418 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/role_mapping.py
+-rw-r--r--   0        0        0      125 2023-05-18 15:26:48.403180 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/role_type.py
+-rw-r--r--   0        0        0     3964 2023-05-18 15:26:48.378596 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/rule.py
+-rw-r--r--   0        0        0      110 2023-05-18 15:26:48.376838 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/rule_type.py
+-rw-r--r--   0        0        0     2301 2023-05-18 15:26:48.399109 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/rule_violation_error.py
+-rw-r--r--   0        0        0    11035 2023-05-18 15:26:48.367443 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/searched_artifact.py
+-rw-r--r--   0        0        0     7087 2023-05-18 15:26:48.395639 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/searched_group.py
+-rw-r--r--   0        0        0    12237 2023-05-18 15:26:48.374572 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/searched_version.py
+-rw-r--r--   0        0        0     5359 2023-05-18 15:26:48.409195 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/system_info.py
+-rw-r--r--   0        0        0     3263 2023-05-18 15:26:48.383337 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/update_configuration_property.py
+-rw-r--r--   0        0        0     3322 2023-05-18 15:26:48.371100 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/update_role.py
+-rw-r--r--   0        0        0     3712 2023-05-18 15:26:48.405687 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/update_state.py
+-rw-r--r--   0        0        0     6096 2023-05-18 15:26:48.422107 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/user_info.py
+-rw-r--r--   0        0        0    12512 2023-05-18 15:26:48.414552 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/version_meta_data.py
+-rw-r--r--   0        0        0     4748 2023-05-18 15:26:48.382254 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/models/version_search_results.py
+-rw-r--r--   0        0        0     4683 2023-05-18 15:26:48.424784 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/registry_client.py
+-rw-r--r--   0        0        0    10097 2023-05-18 15:26:48.439961 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0     1669 2023-05-18 15:26:48.441023 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/search/search_request_builder.py
+-rw-r--r--   0        0        0     3945 2023-05-18 15:26:48.334090 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/system/info/info_request_builder.py
+-rw-r--r--   0        0        0     3913 2023-05-18 15:26:48.334930 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/system/limits/limits_request_builder.py
+-rw-r--r--   0        0        0     1973 2023-05-18 15:26:48.332919 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/system/system_request_builder.py
+-rw-r--r--   0        0        0     3793 2023-05-18 15:26:48.331483 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/users/me/me_request_builder.py
+-rw-r--r--   0        0        0     1609 2023-05-18 15:26:48.319948 apicurio_registry_python_sdk_preview-2.4.9/apicurioregistrysdk/client/users/users_request_builder.py
+-rw-r--r--   0        0        0     2233 2023-05-18 14:39:08.122837 apicurio_registry_python_sdk_preview-2.4.9/kiota-gen.py
+-rw-r--r--   0        0        0     1122 2023-05-18 15:27:31.671878 apicurio_registry_python_sdk_preview-2.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.9/PKG-INFO
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.8/kiota-gen.py` & `apicurio_registry_python_sdk_preview-2.4.9/kiota-gen.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.8/pyproject.toml` & `apicurio_registry_python_sdk_preview-2.4.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "apicurio-registry-python-sdk-preview"
-version = "2.4.8"
+version = "2.4.9"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "apicurioregistrysdk"}]
 include = [
-    { path = "apicurioregistrysdk/client" },
+    { path = "apicurioregistrysdk/client/**/*" },
 ]
 license = "Apache 2.0"
 homepage = "https://github.com/apicurio/apicurio-registry"
 repository = "https://github.com/apicurio/apicurio-registry"
 keywords = ["apicurio", "registry"]
 
 [tool.poetry.dependencies]
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.8/PKG-INFO` & `apicurio_registry_python_sdk_preview-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicurio-registry-python-sdk-preview
-Version: 2.4.8
+Version: 2.4.9
 Summary: 
 Home-page: https://github.com/apicurio/apicurio-registry
 License: Apache 2.0
 Keywords: apicurio,registry
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.9,<4.0
```

