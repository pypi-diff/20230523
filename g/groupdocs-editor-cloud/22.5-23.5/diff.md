# Comparing `tmp/groupdocs-editor-cloud-22.5.tar.gz` & `tmp/groupdocs-editor-cloud-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-editor-cloud-22.5.tar", last modified: Wed May 25 06:35:19 2022, max compression
+gzip compressed data, was "dist\groupdocs-editor-cloud-23.5.tar", last modified: Tue May 23 07:20:15 2023, max compression
```

## Comparing `groupdocs-editor-cloud-22.5.tar` & `groupdocs-editor-cloud-23.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/
--rw-rw-rw-   0        0        0     1105 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/LICENSE
--rw-rw-rw-   0        0        0     3295 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/PKG-INFO
--rw-rw-rw-   0        0        0     2464 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/README.md
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/
--rw-rw-rw-   0        0        0     3594 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/__init__.py
--rw-rw-rw-   0        0        0    26221 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/
--rw-rw-rw-   0        0        0      439 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    13920 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/edit_api.py
--rw-rw-rw-   0        0        0    38644 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36254 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    11838 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     6594 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0    26570 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0     3303 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/auth.py
--rw-rw-rw-   0        0        0     7677 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/
--rw-rw-rw-   0        0        0     2504 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     5129 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     8949 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/delimited_text_load_options.py
--rw-rw-rw-   0        0        0     8663 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/delimited_text_save_options.py
--rw-rw-rw-   0        0        0     5187 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     4098 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/document_result.py
--rw-rw-rw-   0        0        0     6291 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     6370 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5409 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     4897 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/format.py
--rw-rw-rw-   0        0        0     4211 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0     7579 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/info_result.py
--rw-rw-rw-   0        0        0     3687 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/load_options.py
--rw-rw-rw-   0        0        0     5029 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/load_result.py
--rw-rw-rw-   0        0        0     5178 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     4925 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/options.py
--rw-rw-rw-   0        0        0     6472 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/pdf_save_options.py
--rw-rw-rw-   0        0        0     6210 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/presentation_load_options.py
--rw-rw-rw-   0        0        0     4572 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/presentation_save_options.py
--rw-rw-rw-   0        0        0     5879 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/save_options.py
--rw-rw-rw-   0        0        0     6575 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/spreadsheet_load_options.py
--rw-rw-rw-   0        0        0     7160 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/spreadsheet_save_options.py
--rw-rw-rw-   0        0        0     4276 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0    10290 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/text_load_options.py
--rw-rw-rw-   0        0        0     7088 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/text_save_options.py
--rw-rw-rw-   0        0        0     8470 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/word_processing_load_options.py
--rw-rw-rw-   0        0        0    12545 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/word_processing_save_options.py
--rw-rw-rw-   0        0        0    11779 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/xml_load_options.py
--rw-rw-rw-   0        0        0    13735 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/
--rw-rw-rw-   0        0        0     3295 2022-05-25 06:35:18.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2712 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-25 06:35:18.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/setup.cfg
--rw-rw-rw-   0        0        0     1679 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/test/
--rw-rw-rw-   0        0        0        0 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-25 06:35:19.000000 groupdocs-editor-cloud-22.5/test/apis/
--rw-rw-rw-   0        0        0        0 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3005 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0    13391 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_editor_api.py
--rw-rw-rw-   0        0        0     2028 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_editor_formats_api.py
--rw-rw-rw-   0        0        0     2280 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_editor_get_info_api.py
--rw-rw-rw-   0        0        0     3806 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3136 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     2735 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     4769 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/test_context.py
--rw-rw-rw-   0        0        0     3826 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/test_file.py
--rw-rw-rw-   0        0        0     1702 2022-05-25 06:34:57.000000 groupdocs-editor-cloud-22.5/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/
+-rw-rw-rw-   0        0        0     1105 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/LICENSE
+-rw-rw-rw-   0        0        0     3295 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2464 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/
+-rw-rw-rw-   0        0        0     3594 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/__init__.py
+-rw-rw-rw-   0        0        0    26221 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/
+-rw-rw-rw-   0        0        0      439 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    13920 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/edit_api.py
+-rw-rw-rw-   0        0        0    38644 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36254 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    11838 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     6594 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0    26570 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0     3303 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/auth.py
+-rw-rw-rw-   0        0        0     7677 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/
+-rw-rw-rw-   0        0        0     2504 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     5129 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     8949 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/delimited_text_load_options.py
+-rw-rw-rw-   0        0        0     8663 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/delimited_text_save_options.py
+-rw-rw-rw-   0        0        0     5187 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     4098 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/document_result.py
+-rw-rw-rw-   0        0        0     6291 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     6370 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5409 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     4897 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4211 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0     7579 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/info_result.py
+-rw-rw-rw-   0        0        0     3687 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/load_options.py
+-rw-rw-rw-   0        0        0     5029 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/load_result.py
+-rw-rw-rw-   0        0        0     5178 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     4925 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/options.py
+-rw-rw-rw-   0        0        0     6472 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/pdf_save_options.py
+-rw-rw-rw-   0        0        0     6210 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/presentation_load_options.py
+-rw-rw-rw-   0        0        0     4572 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/presentation_save_options.py
+-rw-rw-rw-   0        0        0     5879 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/save_options.py
+-rw-rw-rw-   0        0        0     6575 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/spreadsheet_load_options.py
+-rw-rw-rw-   0        0        0     7160 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/spreadsheet_save_options.py
+-rw-rw-rw-   0        0        0     4276 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0    10290 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/text_load_options.py
+-rw-rw-rw-   0        0        0     7088 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/text_save_options.py
+-rw-rw-rw-   0        0        0     8470 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/word_processing_load_options.py
+-rw-rw-rw-   0        0        0    12545 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/word_processing_save_options.py
+-rw-rw-rw-   0        0        0    11779 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/xml_load_options.py
+-rw-rw-rw-   0        0        0    13735 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/
+-rw-rw-rw-   0        0        0     3295 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2712 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/test/
+-rw-rw-rw-   0        0        0        0 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:20:15.000000 groupdocs-editor-cloud-23.5/test/apis/
+-rw-rw-rw-   0        0        0        0 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3005 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0    13391 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_editor_api.py
+-rw-rw-rw-   0        0        0     2028 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_editor_formats_api.py
+-rw-rw-rw-   0        0        0     2280 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_editor_get_info_api.py
+-rw-rw-rw-   0        0        0     3806 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3136 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     2735 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     4769 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/test_context.py
+-rw-rw-rw-   0        0        0     3826 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/test_file.py
+-rw-rw-rw-   0        0        0     1702 2023-05-23 07:19:51.000000 groupdocs-editor-cloud-23.5/test/test_settings.py
```

### Comparing `groupdocs-editor-cloud-22.5/LICENSE` & `groupdocs-editor-cloud-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-editor-cloud-22.5/PKG-INFO` & `groupdocs-editor-cloud-23.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-editor-cloud
-Version: 22.5
+Version: 23.5
 Summary: GroupDocs.Editor Cloud Python SDK
 Home-page: http://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,editor,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-editor-cloud-22.5/README.md` & `groupdocs-editor-cloud-23.5/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/__init__.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/api_client.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_client.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '22.5'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.5'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 22.5'
+        self.user_agent = 'python sdk 23.5'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/api_exception.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/api_exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="api_exception.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/edit_api.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/edit_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="editor_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -271,15 +271,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="load_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -307,15 +307,15 @@
     def __init__(self, load_options):
         """Initializes new instance of LoadRequest."""  # noqa: E501
         self.load_options = load_options
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="save_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/file_api.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="editor_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -634,15 +634,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -678,15 +678,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -718,15 +718,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="download_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -758,15 +758,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -802,15 +802,15 @@
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="upload_file_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/folder_api.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="editor_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -610,15 +610,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="copy_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -652,15 +652,15 @@
         self.dest_path = dest_path
         self.src_storage_name = src_storage_name
         self.dest_storage_name = dest_storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="create_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -690,15 +690,15 @@
         """Initializes new instance of CreateFolderRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="delete_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -730,15 +730,15 @@
         self.path = path
         self.storage_name = storage_name
         self.recursive = recursive
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_files_list_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -768,15 +768,15 @@
         """Initializes new instance of GetFilesListRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="move_folder_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/info_api.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/info_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="editor_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -265,15 +265,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_info_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/license_api.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/license_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="editor_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/apis/storage_api.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/apis/storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="editor_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -471,15 +471,15 @@
         else:
             return s[0].lower() + s[1:]
 
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_disc_usage_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -507,15 +507,15 @@
     def __init__(self, storage_name=None):
         """Initializes new instance of GetDiscUsageRequest."""  # noqa: E501
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="get_file_versions_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -545,15 +545,15 @@
         """Initializes new instance of GetFileVersionsRequest."""  # noqa: E501
         self.path = path
         self.storage_name = storage_name
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="object_exists_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -585,15 +585,15 @@
         self.path = path
         self.storage_name = storage_name
         self.version_id = version_id
 # coding: utf-8
 
 # --------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="storage_exists_request.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/auth.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="auth.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/configuration.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="configuration.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 22.5\n"\
-               "SDK Package Version: 22.5".\
+               "Version of the API: 23.5\n"\
+               "SDK Package Version: 23.5".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/__init__.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/consumption_result.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/consumption_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ConsumptionResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/delimited_text_load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/delimited_text_load_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DelimitedTextLoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/delimited_text_save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/delimited_text_save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DelimitedTextSaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/disc_usage.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/disc_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DiscUsage.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/document_result.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/document_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="DocumentResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/error.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Error.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/error_details.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/error_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ErrorDetails.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/file_info.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileInfo.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/file_version.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/file_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersion.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/file_versions.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/file_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FileVersions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/files_list.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/files_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesList.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/files_upload_result.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/files_upload_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FilesUploadResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/format.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Format.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/formats_result.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/formats_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="FormatsResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/info_result.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/info_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="InfoResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/load_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="LoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/load_result.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/load_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="LoadResult.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/object_exist.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/object_exist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="ObjectExist.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="Options.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/pdf_save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/pdf_save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PdfSaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/presentation_load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/presentation_load_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PresentationLoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/presentation_save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/presentation_save_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="PresentationSaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/spreadsheet_load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/spreadsheet_load_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SpreadsheetLoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/spreadsheet_save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/spreadsheet_save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="SpreadsheetSaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/storage_exist.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/storage_exist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageExist.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/storage_file.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/storage_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="StorageFile.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/text_load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/text_load_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextLoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/text_save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/text_save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="TextSaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/word_processing_load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/word_processing_load_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="WordProcessingLoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/word_processing_save_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/word_processing_save_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="WordProcessingSaveOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/models/xml_load_options.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/models/xml_load_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="XmlLoadOptions.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud/rest.py` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="rest.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/PKG-INFO` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-editor-cloud
-Version: 22.5
+Version: 23.5
 Summary: GroupDocs.Editor Cloud Python SDK
 Home-page: http://github.com/groupdocs-editor-cloud/groupdocs-editor-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,editor,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-editor-cloud-22.5/groupdocs_editor_cloud.egg-info/SOURCES.txt` & `groupdocs-editor-cloud-23.5/groupdocs_editor_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupdocs-editor-cloud-22.5/setup.py` & `groupdocs-editor-cloud-23.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-editor-cloud"
-VERSION = "22.5"
+VERSION = "23.5"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_auth_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_auth_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_auth_api.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_editor_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_editor_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_editor_formats_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_editor_formats_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_editor_get_info_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_editor_get_info_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_file_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_folder_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_folder_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/apis/test_storage_api.py` & `groupdocs-editor-cloud-23.5/test/apis/test_storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/test_context.py` & `groupdocs-editor-cloud-23.5/test/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/test_file.py` & `groupdocs-editor-cloud-23.5/test/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_file.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

### Comparing `groupdocs-editor-cloud-22.5/test/test_settings.py` & `groupdocs-editor-cloud-23.5/test/test_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
 # <copyright company="Aspose Pty Ltd" file="test_context.py">
-#   Copyright (c) 2003-2022 Aspose Pty Ltd
+#   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
```

