# Comparing `tmp/lusid-configuration-sdk-preview-0.1.430.tar.gz` & `tmp/lusid-configuration-sdk-preview-0.1.431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-configuration-sdk-preview-0.1.430.tar", last modified: Thu Apr 20 15:19:35 2023, max compression
+gzip compressed data, was "dist/lusid-configuration-sdk-preview-0.1.431.tar", last modified: Tue May 23 12:02:04 2023, max compression
```

## Comparing `lusid-configuration-sdk-preview-0.1.430.tar` & `lusid-configuration-sdk-preview-0.1.431.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8423 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/
--rw-r--r--   0 root         (0) root         (0)     3344 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api/
--rw-r--r--   0 root         (0) root         (0)      251 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6858 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)   146162 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api/configuration_sets_api.py
--rw-r--r--   0 root         (0) root         (0)    27443 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16648 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5106 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/
--rw-r--r--   0 root         (0) root         (0)     2240 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7271 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9034 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7239 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    16888 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_item.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_item_summary.py
--rw-r--r--   0 root         (0) root         (0)    13793 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_set.py
--rw-r--r--   0 root         (0) root         (0)     6233 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_set_summary.py
--rw-r--r--   0 root         (0) root         (0)    11674 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/create_configuration_item.py
--rw-r--r--   0 root         (0) root         (0)     6977 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/create_configuration_set.py
--rw-r--r--   0 root         (0) root         (0)     8032 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9521 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9547 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10712 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     9198 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/personal_access_token.py
--rw-r--r--   0 root         (0) root         (0)     6106 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7782 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7586 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_configuration_item.py
--rw-r--r--   0 root         (0) root         (0)     7558 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_configuration_set.py
--rw-r--r--   0 root         (0) root         (0)     7754 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_configuration_set_summary.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/update_configuration_item.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/update_configuration_set.py
--rw-r--r--   0 root         (0) root         (0)    13568 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/utilities/
--rw-r--r--   0 root         (0) root         (0)       66 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2027 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 15:19:35.000000 lusid-configuration-sdk-preview-0.1.430/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2291 2023-04-20 15:17:49.000000 lusid-configuration-sdk-preview-0.1.430/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8423 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6858 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)   146162 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api/configuration_sets_api.py
+-rw-r--r--   0 root         (0) root         (0)    27443 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16648 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7271 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9034 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7239 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    16888 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_item.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_item_summary.py
+-rw-r--r--   0 root         (0) root         (0)    13793 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_set.py
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_set_summary.py
+-rw-r--r--   0 root         (0) root         (0)    11674 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/create_configuration_item.py
+-rw-r--r--   0 root         (0) root         (0)     6977 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/create_configuration_set.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9521 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10712 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     9198 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/personal_access_token.py
+-rw-r--r--   0 root         (0) root         (0)     6106 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7782 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7586 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_configuration_item.py
+-rw-r--r--   0 root         (0) root         (0)     7558 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_configuration_set.py
+-rw-r--r--   0 root         (0) root         (0)     7754 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_configuration_set_summary.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/update_configuration_item.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/update_configuration_set.py
+-rw-r--r--   0 root         (0) root         (0)    13568 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/utilities/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:02:04.000000 lusid-configuration-sdk-preview-0.1.431/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-23 11:59:34.000000 lusid-configuration-sdk-preview-0.1.431/setup.py
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/README.md` & `lusid-configuration-sdk-preview-0.1.431/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.430
-- Package version: 0.1.430
+- API version: 0.1.431
+- Package version: 0.1.431
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/__init__.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.430"
+__version__ = "0.1.431"
 
 # import apis into sdk package
 from lusid_configuration.api.application_metadata_api import ApplicationMetadataApi
 from lusid_configuration.api.configuration_sets_api import ConfigurationSetsApi
 
 # import ApiClient
 from lusid_configuration.api_client import ApiClient
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api/application_metadata_api.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api/configuration_sets_api.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api/configuration_sets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -227,15 +227,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ConfigurationSet",
             400: "LusidValidationProblemDetails",
@@ -359,15 +359,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -516,15 +516,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ConfigurationSet",
             400: "LusidValidationProblemDetails",
@@ -647,15 +647,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -858,15 +858,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -1050,15 +1050,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -1185,15 +1185,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PersonalAccessToken",
             400: "LusidValidationProblemDetails",
@@ -1406,15 +1406,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ConfigurationItem",
             400: "LusidValidationProblemDetails",
@@ -1609,15 +1609,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ConfigurationSet",
             400: "LusidValidationProblemDetails",
@@ -1786,15 +1786,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfConfigurationItem",
             400: "LusidValidationProblemDetails",
@@ -1944,15 +1944,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfConfigurationSet",
             400: "LusidValidationProblemDetails",
@@ -2098,15 +2098,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfConfigurationSetSummary",
             400: "LusidValidationProblemDetails",
@@ -2326,15 +2326,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ConfigurationItem",
             400: "LusidValidationProblemDetails",
@@ -2536,15 +2536,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.430'
+        header_params['X-LUSID-SDK-Version'] = '0.1.431'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ConfigurationSet",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/api_client.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.430/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.431/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/configuration.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.430\n"\
-               "SDK Package Version: 0.1.430".\
+               "Version of the API: 0.1.431\n"\
+               "SDK Package Version: 0.1.431".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/exceptions.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/__init__.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/access_controlled_action.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/access_controlled_resource.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/action_id.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_item.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_item_summary.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_item_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_set.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/configuration_set_summary.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/configuration_set_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/create_configuration_item.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/create_configuration_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/create_configuration_set.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/create_configuration_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/id_selector_definition.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/identifier_part_schema.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/link.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/lusid_problem_details.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/lusid_validation_problem_details.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/personal_access_token.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/personal_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_id.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_access_controlled_resource.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_configuration_item.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_configuration_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_configuration_set.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_configuration_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/resource_list_of_configuration_set_summary.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/resource_list_of_configuration_set_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/update_configuration_item.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/update_configuration_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/models/update_configuration_set.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/models/update_configuration_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/rest.py` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE ConfigurationService API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.430
+    The version of the OpenAPI document: 0.1.431
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration/utilities/config_keys.json` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-configuration-sdk-preview-0.1.430/lusid_configuration_sdk_preview.egg-info/SOURCES.txt` & `lusid-configuration-sdk-preview-0.1.431/lusid_configuration_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-configuration-sdk-preview-0.1.430/setup.py` & `lusid-configuration-sdk-preview-0.1.431/setup.py`

 * *Files identical despite different names*

