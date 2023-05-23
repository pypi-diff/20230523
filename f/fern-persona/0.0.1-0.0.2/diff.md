# Comparing `tmp/fern_persona-0.0.1.tar.gz` & `tmp/fern_persona-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_persona-0.0.1.tar", max compression
+gzip compressed data, was "fern_persona-0.0.2.tar", max compression
```

## Comparing `fern_persona-0.0.1.tar` & `fern_persona-0.0.2.tar`

### file list

```diff
@@ -1,302 +1,913 @@
--rw-r--r--   0        0        0     1683 2023-05-23 13:19:16.338314 fern_persona-0.0.1/README.md
--rw-r--r--   0        0        0      374 2023-05-23 13:19:16.338314 fern_persona-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    26887 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/__init__.py
--rw-r--r--   0        0        0     4284 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/client.py
--rw-r--r--   0        0        0      348 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      163 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/environment.py
--rw-r--r--   0        0        0      355 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/errors/conflict_error.py
--rw-r--r--   0        0        0      246 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/errors/not_found_error.py
--rw-r--r--   0        0        0      341 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/py.typed
--rw-r--r--   0        0        0      598 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/accounts/__init__.py
--rw-r--r--   0        0        0    17150 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/api_logs/__init__.py
--rw-r--r--   0        0        0     4855 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/api_logs/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/database_verifications/__init__.py
--rw-r--r--   0        0        0     3185 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/database_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/document_verifications/__init__.py
--rw-r--r--   0        0        0     7863 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/document_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/documents/__init__.py
--rw-r--r--   0        0        0    10928 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/events/__init__.py
--rw-r--r--   0        0        0     6122 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/events/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/government_id_verifications/__init__.py
--rw-r--r--   0        0        0     3404 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/government_id_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/importers/__init__.py
--rw-r--r--   0        0        0    21225 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/importers/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/inquiries/__init__.py
--rw-r--r--   0        0        0    21099 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/inquiries/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/phone_number_verifications/__init__.py
--rw-r--r--   0        0        0     3390 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/phone_number_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/reports/__init__.py
--rw-r--r--   0        0        0     4265 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/reports/client.py
--rw-r--r--   0        0        0       65 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/verifications/__init__.py
--rw-r--r--   0        0        0     2258 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/resources/verifications/client.py
--rw-r--r--   0        0        0    41687 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_consolidate_request_meta.py
--rw-r--r--   0        0        0      903 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_request_data.py
--rw-r--r--   0        0        0     3570 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_request_data_attributes.py
--rw-r--r--   0        0        0     1226 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_request_data_attributes_selfie_photo.py
--rw-r--r--   0        0        0     1112 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_request_data_attributes_selfie_photo_data.py
--rw-r--r--   0        0        0      866 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_response.py
--rw-r--r--   0        0        0      967 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_response_data.py
--rw-r--r--   0        0        0     1028 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_create_response_data_attributes.py
--rw-r--r--   0        0        0     1029 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_list_all_response.py
--rw-r--r--   0        0        0      989 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_list_all_response_data_item.py
--rw-r--r--   0        0        0     1040 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_list_all_response_data_item_attributes.py
--rw-r--r--   0        0        0      817 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_list_all_response_links.py
--rw-r--r--   0        0        0      866 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_redact_response.py
--rw-r--r--   0        0        0      967 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_redact_response_data.py
--rw-r--r--   0        0        0     1895 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_redact_response_data_attributes.py
--rw-r--r--   0        0        0      874 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_retrieve_response.py
--rw-r--r--   0        0        0      975 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_retrieve_response_data.py
--rw-r--r--   0        0        0     1030 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_retrieve_response_data_attributes.py
--rw-r--r--   0        0        0      903 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_request_data.py
--rw-r--r--   0        0        0     3571 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_request_data_attributes.py
--rw-r--r--   0        0        0     1226 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_request_data_attributes_selfie_photo.py
--rw-r--r--   0        0        0     1112 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_request_data_attributes_selfie_photo_data.py
--rw-r--r--   0        0        0      866 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_response.py
--rw-r--r--   0        0        0      967 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_response_data.py
--rw-r--r--   0        0        0     1079 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/accounts_update_response_data_attributes.py
--rw-r--r--   0        0        0      871 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response.py
--rw-r--r--   0        0        0      972 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data.py
--rw-r--r--   0        0        0     1249 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes.py
--rw-r--r--   0        0        0     1720 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request.py
--rw-r--r--   0        0        0     1013 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_get_params.py
--rw-r--r--   0        0        0      818 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_get_params_filter.py
--rw-r--r--   0        0        0      897 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_headers.py
--rw-r--r--   0        0        0      773 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_post_params.py
--rw-r--r--   0        0        0     1067 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_response.py
--rw-r--r--   0        0        0      892 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_response_headers.py
--rw-r--r--   0        0        0      919 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/database_verifications_create_response.py
--rw-r--r--   0        0        0     1242 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data.py
--rw-r--r--   0        0        0     1649 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data_attributes.py
--rw-r--r--   0        0        0     1010 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data_relationships.py
--rw-r--r--   0        0        0      817 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      956 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_request_data.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_request_data_attributes.py
--rw-r--r--   0        0        0      919 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response.py
--rw-r--r--   0        0        0     1242 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data.py
--rw-r--r--   0        0        0     1439 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_attributes.py
--rw-r--r--   0        0        0     1252 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships.py
--rw-r--r--   0        0        0     1031 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_document.py
--rw-r--r--   0        0        0      844 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_document_data.py
--rw-r--r--   0        0        0     1027 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      919 2023-05-23 13:19:16.338314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response.py
--rw-r--r--   0        0        0     1242 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data.py
--rw-r--r--   0        0        0     1425 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_attributes.py
--rw-r--r--   0        0        0     1252 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships.py
--rw-r--r--   0        0        0     1031 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_document.py
--rw-r--r--   0        0        0      844 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_document_data.py
--rw-r--r--   0        0        0     1027 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      907 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_request_data.py
--rw-r--r--   0        0        0      966 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_request_data_attributes.py
--rw-r--r--   0        0        0      870 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response.py
--rw-r--r--   0        0        0     1147 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response_data.py
--rw-r--r--   0        0        0     1227 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response_data_attributes.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      952 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response_data_relationships.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_create_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      878 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response.py
--rw-r--r--   0        0        0     1161 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data.py
--rw-r--r--   0        0        0     1308 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_attributes.py
--rw-r--r--   0        0        0      833 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      960 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_relationships.py
--rw-r--r--   0        0        0      986 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      833 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      870 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response.py
--rw-r--r--   0        0        0     1147 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response_data.py
--rw-r--r--   0        0        0     1227 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response_data_attributes.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      952 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response_data_relationships.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_submit_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      907 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_request_data.py
--rw-r--r--   0        0        0      894 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_request_data_attributes.py
--rw-r--r--   0        0        0      870 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response.py
--rw-r--r--   0        0        0     1147 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response_data.py
--rw-r--r--   0        0        0     1227 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response_data_attributes.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      952 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response_data_relationships.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/documents_update_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      740 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/events_list_all_response.py
--rw-r--r--   0        0        0      741 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/events_retrieve_response.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data.py
--rw-r--r--   0        0        0     2190 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes.py
--rw-r--r--   0        0        0     1368 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_back_photo.py
--rw-r--r--   0        0        0     1171 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_back_photo_data.py
--rw-r--r--   0        0        0     1373 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_front_photo.py
--rw-r--r--   0        0        0     1172 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_front_photo_data.py
--rw-r--r--   0        0        0      936 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response.py
--rw-r--r--   0        0        0     1281 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data.py
--rw-r--r--   0        0        0     2569 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_attributes.py
--rw-r--r--   0        0        0     1282 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships.py
--rw-r--r--   0        0        0     1048 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships_document.py
--rw-r--r--   0        0        0      848 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships_document_data.py
--rw-r--r--   0        0        0      821 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      912 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_account_request_data.py
--rw-r--r--   0        0        0      928 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_account_request_data_file.py
--rw-r--r--   0        0        0      899 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_account_response.py
--rw-r--r--   0        0        0     1000 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_account_response_data.py
--rw-r--r--   0        0        0     1248 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_account_response_data_attributes.py
--rw-r--r--   0        0        0      987 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_request_data.py
--rw-r--r--   0        0        0     1118 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_request_data_attributes.py
--rw-r--r--   0        0        0      948 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      941 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_response.py
--rw-r--r--   0        0        0     1051 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_response_data.py
--rw-r--r--   0        0        0     1258 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_response_data_attributes.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_request_data.py
--rw-r--r--   0        0        0     1113 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_request_data_attributes.py
--rw-r--r--   0        0        0      947 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      936 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_response.py
--rw-r--r--   0        0        0     1046 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_response_data.py
--rw-r--r--   0        0        0     1257 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_response_data_attributes.py
--rw-r--r--   0        0        0     1012 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_request_data.py
--rw-r--r--   0        0        0     1143 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_request_data_attributes.py
--rw-r--r--   0        0        0      954 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      975 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_response.py
--rw-r--r--   0        0        0     1076 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_response_data.py
--rw-r--r--   0        0        0     1264 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_response_data_attributes.py
--rw-r--r--   0        0        0      975 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_request_data.py
--rw-r--r--   0        0        0     1106 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_request_data_attributes.py
--rw-r--r--   0        0        0      945 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      929 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_response.py
--rw-r--r--   0        0        0     1039 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_response_data.py
--rw-r--r--   0        0        0     1255 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_response_data_attributes.py
--rw-r--r--   0        0        0      945 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_name_lists_request_data.py
--rw-r--r--   0        0        0     1076 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_name_lists_request_data_attributes.py
--rw-r--r--   0        0        0      940 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_name_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      908 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_name_lists_response.py
--rw-r--r--   0        0        0     1009 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_name_lists_response_data.py
--rw-r--r--   0        0        0     1250 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_name_lists_response_data_attributes.py
--rw-r--r--   0        0        0      983 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_request_data.py
--rw-r--r--   0        0        0     1114 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_request_data_attributes.py
--rw-r--r--   0        0        0      947 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      937 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_response.py
--rw-r--r--   0        0        0     1047 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_response_data.py
--rw-r--r--   0        0        0     1257 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_response_data_attributes.py
--rw-r--r--   0        0        0      878 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_retrieve_response.py
--rw-r--r--   0        0        0      979 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_retrieve_response_data.py
--rw-r--r--   0        0        0     1243 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/importers_retrieve_response_data_attributes.py
--rw-r--r--   0        0        0      848 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_request_meta.py
--rw-r--r--   0        0        0      874 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response.py
--rw-r--r--   0        0        0     1154 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data.py
--rw-r--r--   0        0        0     1196 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_attributes.py
--rw-r--r--   0        0        0     1578 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_account.py
--rw-r--r--   0        0        0      832 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      819 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_reports.py
--rw-r--r--   0        0        0      986 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_template.py
--rw-r--r--   0        0        0      833 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1032 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      842 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      907 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_request_data.py
--rw-r--r--   0        0        0     3292 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_request_data_attributes.py
--rw-r--r--   0        0        0     2262 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_request_data_attributes_fields.py
--rw-r--r--   0        0        0      870 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response.py
--rw-r--r--   0        0        0     1147 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data.py
--rw-r--r--   0        0        0     1202 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_attributes.py
--rw-r--r--   0        0        0     1565 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_reports.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1028 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      848 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_request_meta.py
--rw-r--r--   0        0        0      874 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response.py
--rw-r--r--   0        0        0     1154 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data.py
--rw-r--r--   0        0        0     1196 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_attributes.py
--rw-r--r--   0        0        0     1578 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_account.py
--rw-r--r--   0        0        0      832 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      819 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_reports.py
--rw-r--r--   0        0        0      986 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_template.py
--rw-r--r--   0        0        0      833 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1032 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      842 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0     1036 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response.py
--rw-r--r--   0        0        0     1186 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item.py
--rw-r--r--   0        0        0     1200 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_attributes.py
--rw-r--r--   0        0        0     1887 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships.py
--rw-r--r--   0        0        0     1000 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_account.py
--rw-r--r--   0        0        0      836 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_account_data.py
--rw-r--r--   0        0        0      823 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_reports.py
--rw-r--r--   0        0        0     1030 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_sessions.py
--rw-r--r--   0        0        0      841 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_sessions_data_item.py
--rw-r--r--   0        0        0     1004 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_template.py
--rw-r--r--   0        0        0      837 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_template_data.py
--rw-r--r--   0        0        0     1050 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_verifications.py
--rw-r--r--   0        0        0      846 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      818 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_links.py
--rw-r--r--   0        0        0      870 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response.py
--rw-r--r--   0        0        0     1147 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_attributes.py
--rw-r--r--   0        0        0     1565 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_reports.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1028 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      997 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response.py
--rw-r--r--   0        0        0     1147 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_attributes.py
--rw-r--r--   0        0        0     1565 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_reports.py
--rw-r--r--   0        0        0      982 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1028 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      873 2023-05-23 13:19:16.342314 fern_persona-0.0.1/src/persona/types/inquiries_resume_response_meta.py
--rw-r--r--   0        0        0     1053 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response.py
--rw-r--r--   0        0        0     1161 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data.py
--rw-r--r--   0        0        0     2309 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes.py
--rw-r--r--   0        0        0     2068 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_behaviours.py
--rw-r--r--   0        0        0     1362 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_fields.py
--rw-r--r--   0        0        0      837 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_fields_name_first.py
--rw-r--r--   0        0        0      836 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_fields_name_last.py
--rw-r--r--   0        0        0     1793 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships.py
--rw-r--r--   0        0        0      986 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_account.py
--rw-r--r--   0        0        0      833 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      820 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_reports.py
--rw-r--r--   0        0        0     1016 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_sessions.py
--rw-r--r--   0        0        0      838 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_sessions_data_item.py
--rw-r--r--   0        0        0      990 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_template.py
--rw-r--r--   0        0        0      834 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1036 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      843 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0     1012 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_included_item.py
--rw-r--r--   0        0        0     1782 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_included_item_attributes.py
--rw-r--r--   0        0        0      907 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_update_request_data.py
--rw-r--r--   0        0        0     2047 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/inquiries_update_request_data_attributes.py
--rw-r--r--   0        0        0      978 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_request_data.py
--rw-r--r--   0        0        0     1485 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_request_data_attributes.py
--rw-r--r--   0        0        0      932 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response.py
--rw-r--r--   0        0        0     1042 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response_data.py
--rw-r--r--   0        0        0     1844 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response_data_attributes.py
--rw-r--r--   0        0        0      779 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response_data_attributes_metadata.py
--rw-r--r--   0        0        0      862 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/reports_redact_response.py
--rw-r--r--   0        0        0      963 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/reports_redact_response_data.py
--rw-r--r--   0        0        0     1225 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/reports_redact_response_data_attributes.py
--rw-r--r--   0        0        0      870 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/reports_retrieve_response.py
--rw-r--r--   0        0        0      971 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/reports_retrieve_response_data.py
--rw-r--r--   0        0        0     1815 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/reports_retrieve_response_data_attributes.py
--rw-r--r--   0        0        0      925 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/unprocessable_entity_error_body.py
--rw-r--r--   0        0        0      824 2023-05-23 13:19:16.346314 fern_persona-0.0.1/src/persona/types/unprocessable_entity_error_body_errors_item.py
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 fern_persona-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1683 2023-05-23 16:50:24.961418 fern_persona-0.0.2/README.md
+-rw-r--r--   0        0        0      374 2023-05-23 16:50:24.961418 fern_persona-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    89351 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/__init__.py
+-rw-r--r--   0        0        0     9082 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/client.py
+-rw-r--r--   0        0        0      348 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      163 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/environment.py
+-rw-r--r--   0        0        0      355 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/conflict_error.py
+-rw-r--r--   0        0        0      246 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/not_found_error.py
+-rw-r--r--   0        0        0      341 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/py.typed
+-rw-r--r--   0        0        0     1282 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    27071 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/api_keys/__init__.py
+-rw-r--r--   0        0        0    12850 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/api_keys/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/api_logs/__init__.py
+-rw-r--r--   0        0        0     4924 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/api_logs/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/cases/__init__.py
+-rw-r--r--   0        0        0    19144 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/cases/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/database_verifications/__init__.py
+-rw-r--r--   0        0        0     7986 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/document_verifications/__init__.py
+-rw-r--r--   0        0        0     8038 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/document_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/documents/__init__.py
+-rw-r--r--   0        0        0    11036 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/email_address_verifications/__init__.py
+-rw-r--r--   0        0        0    11147 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/email_address_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/events/__init__.py
+-rw-r--r--   0        0        0     6189 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/events/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_documents/__init__.py
+-rw-r--r--   0        0        0     9367 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_verifications/__init__.py
+-rw-r--r--   0        0        0    11578 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/graph_queries/__init__.py
+-rw-r--r--   0        0        0     4115 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/graph_queries/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/importers/__init__.py
+-rw-r--r--   0        0        0    23039 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/importers/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/inquiries/__init__.py
+-rw-r--r--   0        0        0    34666 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/inquiries/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/list_items/__init__.py
+-rw-r--r--   0        0        0    47166 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/list_items/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/lists/__init__.py
+-rw-r--r--   0        0        0    39214 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/lists/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_carrier_database_verifications/__init__.py
+-rw-r--r--   0        0        0     9207 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_carrier_database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_number_verifications/__init__.py
+-rw-r--r--   0        0        0    11061 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_number_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/print_verifications/__init__.py
+-rw-r--r--   0        0        0     2140 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/print_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/reports/__init__.py
+-rw-r--r--   0        0        0    31595 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/reports/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/selfie_verifications/__init__.py
+-rw-r--r--   0        0        0     8611 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/selfie_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/serpo_database_verifications/__init__.py
+-rw-r--r--   0        0        0     8878 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/serpo_database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/tin_database_verifications/__init__.py
+-rw-r--r--   0        0        0     9240 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/tin_database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/user_audit_logs/__init__.py
+-rw-r--r--   0        0        0     5057 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/user_audit_logs/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/verifications/__init__.py
+-rw-r--r--   0        0        0     2302 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/workflows/__init__.py
+-rw-r--r--   0        0        0     3702 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/workflows/client.py
+-rw-r--r--   0        0        0   141824 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/__init__.py
+-rw-r--r--   0        0        0      855 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_a_tag_1_request_meta.py
+-rw-r--r--   0        0        0      854 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_a_tag_request_meta.py
+-rw-r--r--   0        0        0      965 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_request_meta.py
+-rw-r--r--   0        0        0      879 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response.py
+-rw-r--r--   0        0        0     1163 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data.py
+-rw-r--r--   0        0        0     1835 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_attributes.py
+-rw-r--r--   0        0        0     1994 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      825 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0     1008 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      838 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0     1021 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      839 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      848 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_request_meta.py
+-rw-r--r--   0        0        0      875 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response.py
+-rw-r--r--   0        0        0     1156 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1196 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1033 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      842 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      950 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response.py
+-rw-r--r--   0        0        0     1306 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data.py
+-rw-r--r--   0        0        0     1187 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1041 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      824 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      921 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response.py
+-rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data.py
+-rw-r--r--   0        0        0     1303 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      817 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      951 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response.py
+-rw-r--r--   0        0        0     1308 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data.py
+-rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1042 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      824 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      739 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_list_response.py
+-rw-r--r--   0        0        0      893 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response.py
+-rw-r--r--   0        0        0     1188 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data.py
+-rw-r--r--   0        0        0     1287 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0      984 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      810 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      930 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response.py
+-rw-r--r--   0        0        0     1271 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data.py
+-rw-r--r--   0        0        0     1256 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1021 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      956 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_request_meta.py
+-rw-r--r--   0        0        0      855 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response.py
+-rw-r--r--   0        0        0     1121 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data.py
+-rw-r--r--   0        0        0     1836 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1871 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      984 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0      997 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      989 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      999 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data.py
+-rw-r--r--   0        0        0      954 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data_attributes.py
+-rw-r--r--   0        0        0     1866 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data_attributes_query.py
+-rw-r--r--   0        0        0      896 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response.py
+-rw-r--r--   0        0        0      997 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data.py
+-rw-r--r--   0        0        0     1506 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes.py
+-rw-r--r--   0        0        0     1316 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_query.py
+-rw-r--r--   0        0        0     3441 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item.py
+-rw-r--r--   0        0        0     1209 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_addresses_item.py
+-rw-r--r--   0        0        0     1069 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent.py
+-rw-r--r--   0        0        0     1208 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent_address.py
+-rw-r--r--   0        0        0      851 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_identifiers_item.py
+-rw-r--r--   0        0        0      973 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_industry_codes_item.py
+-rw-r--r--   0        0        0     1335 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item.py
+-rw-r--r--   0        0        0     1215 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item_address.py
+-rw-r--r--   0        0        0     1102 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration.py
+-rw-r--r--   0        0        0     1215 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration_address.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_source.py
+-rw-r--r--   0        0        0      988 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_request_data.py
+-rw-r--r--   0        0        0      890 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_request_data_attributes.py
+-rw-r--r--   0        0        0      942 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response.py
+-rw-r--r--   0        0        0     1052 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data.py
+-rw-r--r--   0        0        0     1778 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes.py
+-rw-r--r--   0        0        0      781 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data.py
+-rw-r--r--   0        0        0      889 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response.py
+-rw-r--r--   0        0        0     1047 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data.py
+-rw-r--r--   0        0        0     1849 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      780 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0     1027 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/consolidate_into_an_account_request_meta.py
+-rw-r--r--   0        0        0      992 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_request_data.py
+-rw-r--r--   0        0        0     1102 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      946 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response.py
+-rw-r--r--   0        0        0     1299 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data.py
+-rw-r--r--   0        0        0     1193 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1037 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      975 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_request_data.py
+-rw-r--r--   0        0        0      854 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_request_data_attributes.py
+-rw-r--r--   0        0        0      756 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_response.py
+-rw-r--r--   0        0        0      892 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_request_data.py
+-rw-r--r--   0        0        0      938 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_request_data_attributes.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_request_meta.py
+-rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response.py
+-rw-r--r--   0        0        0     1121 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data.py
+-rw-r--r--   0        0        0     1857 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1871 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      984 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0      997 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      814 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0     1179 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item.py
+-rw-r--r--   0        0        0     1970 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_attributes.py
+-rw-r--r--   0        0        0      766 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_attributes_fields.py
+-rw-r--r--   0        0        0     2699 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships.py
+-rw-r--r--   0        0        0      996 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_account.py
+-rw-r--r--   0        0        0      835 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_account_data.py
+-rw-r--r--   0        0        0     1030 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents_data_item.py
+-rw-r--r--   0        0        0      824 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_inquiry_template_version.py
+-rw-r--r--   0        0        0      822 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_reports.py
+-rw-r--r--   0        0        0     1022 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies.py
+-rw-r--r--   0        0        0      839 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies_data_item.py
+-rw-r--r--   0        0        0     1026 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions.py
+-rw-r--r--   0        0        0      840 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_template.py
+-rw-r--r--   0        0        0      836 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_template_data.py
+-rw-r--r--   0        0        0     1046 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_verifications.py
+-rw-r--r--   0        0        0      845 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      921 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_country_list_request_data.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_country_list_request_data_attributes.py
+-rw-r--r--   0        0        0      745 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_country_list_response.py
+-rw-r--r--   0        0        0      934 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_county_list_item_request_data.py
+-rw-r--r--   0        0        0     1114 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_county_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      925 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response.py
+-rw-r--r--   0        0        0     1262 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data.py
+-rw-r--r--   0        0        0     1629 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_attributes.py
+-rw-r--r--   0        0        0     1016 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      920 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data.py
+-rw-r--r--   0        0        0     1649 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1011 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      817 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_request_data.py
+-rw-r--r--   0        0        0      966 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_request_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data.py
+-rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      953 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      957 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_request_data.py
+-rw-r--r--   0        0        0      978 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      920 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data.py
+-rw-r--r--   0        0        0     1439 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1254 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1032 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      844 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      926 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data.py
+-rw-r--r--   0        0        0     1220 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      940 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes_face_photo.py
+-rw-r--r--   0        0        0      909 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data.py
+-rw-r--r--   0        0        0      840 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data_attributes.py
+-rw-r--r--   0        0        0      742 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_response.py
+-rw-r--r--   0        0        0      954 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_request_data.py
+-rw-r--r--   0        0        0     1401 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      917 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response.py
+-rw-r--r--   0        0        0     1239 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data.py
+-rw-r--r--   0        0        0     1309 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1008 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      816 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_request_data.py
+-rw-r--r--   0        0        0      847 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_request_data_attributes.py
+-rw-r--r--   0        0        0      749 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_response.py
+-rw-r--r--   0        0        0      946 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data.py
+-rw-r--r--   0        0        0     2143 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes.py
+-rw-r--r--   0        0        0     1341 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1164 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1346 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1165 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      909 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response.py
+-rw-r--r--   0        0        0     1216 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data.py
+-rw-r--r--   0        0        0     2562 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1235 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1021 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0      814 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      958 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data.py
+-rw-r--r--   0        0        0     1767 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes.py
+-rw-r--r--   0        0        0     1353 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1167 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1358 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1168 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      921 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response.py
+-rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data.py
+-rw-r--r--   0        0        0     2186 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      993 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_request_data.py
+-rw-r--r--   0        0        0     1305 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      947 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response.py
+-rw-r--r--   0        0        0     1301 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data.py
+-rw-r--r--   0        0        0     1303 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1038 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      976 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_request_data.py
+-rw-r--r--   0        0        0      854 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_request_data_attributes.py
+-rw-r--r--   0        0        0      756 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_response.py
+-rw-r--r--   0        0        0      917 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data.py
+-rw-r--r--   0        0        0     1146 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data_attributes.py
+-rw-r--r--   0        0        0     1295 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data_attributes_variable_map.py
+-rw-r--r--   0        0        0      926 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_request_data.py
+-rw-r--r--   0        0        0     1266 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      889 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response.py
+-rw-r--r--   0        0        0     1181 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data.py
+-rw-r--r--   0        0        0     1293 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0      980 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      809 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      909 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data.py
+-rw-r--r--   0        0        0     1098 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data_attributes.py
+-rw-r--r--   0        0        0      742 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_response.py
+-rw-r--r--   0        0        0     2149 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_request_attributes.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response.py
+-rw-r--r--   0        0        0     1341 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data.py
+-rw-r--r--   0        0        0     1571 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1061 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      829 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      955 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data.py
+-rw-r--r--   0        0        0     1065 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      938 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_request_data.py
+-rw-r--r--   0        0        0      847 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_request_data_attributes.py
+-rw-r--r--   0        0        0      749 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_response.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data.py
+-rw-r--r--   0        0        0     1485 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      933 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response.py
+-rw-r--r--   0        0        0     1043 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data.py
+-rw-r--r--   0        0        0     1845 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      779 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      900 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_report_request_data.py
+-rw-r--r--   0        0        0     2563 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_report_request_data_attributes.py
+-rw-r--r--   0        0        0      949 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data.py
+-rw-r--r--   0        0        0     2190 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes.py
+-rw-r--r--   0        0        0     1077 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo.py
+-rw-r--r--   0        0        0      920 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo_data.py
+-rw-r--r--   0        0        0     1067 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo.py
+-rw-r--r--   0        0        0      918 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo_data.py
+-rw-r--r--   0        0        0     1072 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo.py
+-rw-r--r--   0        0        0      919 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo_data.py
+-rw-r--r--   0        0        0      912 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response.py
+-rw-r--r--   0        0        0     1221 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data.py
+-rw-r--r--   0        0        0     2064 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1003 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      769 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_request_attributes.py
+-rw-r--r--   0        0        0      945 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data.py
+-rw-r--r--   0        0        0     1565 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1290 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      822 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships_selfie.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_request_data.py
+-rw-r--r--   0        0        0     1634 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_request_data_attributes.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response.py
+-rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data.py
+-rw-r--r--   0        0        0     1563 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_attributes.py
+-rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1126 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_request_data.py
+-rw-r--r--   0        0        0     1429 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_request_data_attributes.py
+-rw-r--r--   0        0        0      884 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response.py
+-rw-r--r--   0        0        0     1172 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data.py
+-rw-r--r--   0        0        0      998 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_attributes.py
+-rw-r--r--   0        0        0     1540 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships.py
+-rw-r--r--   0        0        0      808 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      996 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow.py
+-rw-r--r--   0        0        0      835 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_data.py
+-rw-r--r--   0        0        0     1025 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version.py
+-rw-r--r--   0        0        0      842 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version_data.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data.py
+-rw-r--r--   0        0        0     3575 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes.py
+-rw-r--r--   0        0        0     1231 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo.py
+-rw-r--r--   0        0        0     1113 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo_data.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_response_data.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      905 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_request_data.py
+-rw-r--r--   0        0        0     1804 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_request_data_attributes.py
+-rw-r--r--   0        0        0      868 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_response.py
+-rw-r--r--   0        0        0      969 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      963 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_request_data.py
+-rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      926 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response.py
+-rw-r--r--   0        0        0     1264 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data.py
+-rw-r--r--   0        0        0     1262 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      946 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_request_data.py
+-rw-r--r--   0        0        0      849 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_request_data_attributes.py
+-rw-r--r--   0        0        0      751 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_response.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_request_data.py
+-rw-r--r--   0        0        0     1487 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      941 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response.py
+-rw-r--r--   0        0        0     1051 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data.py
+-rw-r--r--   0        0        0     1855 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      781 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data.py
+-rw-r--r--   0        0        0     3293 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes.py
+-rw-r--r--   0        0        0     2262 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes_fields.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1202 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      951 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_item_request_data.py
+-rw-r--r--   0        0        0     1098 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      934 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_request_data.py
+-rw-r--r--   0        0        0      846 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_request_data_attributes.py
+-rw-r--r--   0        0        0      748 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_response.py
+-rw-r--r--   0        0        0      848 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_request_meta.py
+-rw-r--r--   0        0        0      875 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response.py
+-rw-r--r--   0        0        0     1156 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1196 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1033 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      842 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      903 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data.py
+-rw-r--r--   0        0        0     1622 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data_attributes.py
+-rw-r--r--   0        0        0      780 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data_attributes_dismiss_type.py
+-rw-r--r--   0        0        0      866 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response.py
+-rw-r--r--   0        0        0     1140 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data.py
+-rw-r--r--   0        0        0     1271 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_attributes.py
+-rw-r--r--   0        0        0     1467 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships.py
+-rw-r--r--   0        0        0      804 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_account.py
+-rw-r--r--   0        0        0      804 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1003 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      959 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_request_meta.py
+-rw-r--r--   0        0        0      868 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_response.py
+-rw-r--r--   0        0        0      969 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      903 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_request_meta.py
+-rw-r--r--   0        0        0     1038 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response.py
+-rw-r--r--   0        0        0     1188 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data.py
+-rw-r--r--   0        0        0     3746 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes.py
+-rw-r--r--   0        0        0     2163 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_behaviors.py
+-rw-r--r--   0        0        0     4475 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields.py
+-rw-r--r--   0        0        0      849 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_city.py
+-rw-r--r--   0        0        0      855 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_postal_code.py
+-rw-r--r--   0        0        0      852 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_1.py
+-rw-r--r--   0        0        0      852 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_2.py
+-rw-r--r--   0        0        0      856 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_subdivision.py
+-rw-r--r--   0        0        0      847 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_birthdate.py
+-rw-r--r--   0        0        0      850 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_email_address.py
+-rw-r--r--   0        0        0      858 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_identification_number.py
+-rw-r--r--   0        0        0      847 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_first.py
+-rw-r--r--   0        0        0      846 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_last.py
+-rw-r--r--   0        0        0      848 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_middle.py
+-rw-r--r--   0        0        0      849 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_phone_number.py
+-rw-r--r--   0        0        0     3265 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships.py
+-rw-r--r--   0        0        0     1001 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account.py
+-rw-r--r--   0        0        0      836 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0     1035 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_documents.py
+-rw-r--r--   0        0        0      842 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_documents_data_item.py
+-rw-r--r--   0        0        0     1034 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template.py
+-rw-r--r--   0        0        0      844 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_data.py
+-rw-r--r--   0        0        0     1063 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version.py
+-rw-r--r--   0        0        0      851 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version_data.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      811 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_reviewer.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_selfies.py
+-rw-r--r--   0        0        0     1031 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0      811 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_template.py
+-rw-r--r--   0        0        0     1051 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      846 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      970 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_meta.py
+-rw-r--r--   0        0        0      884 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_request_data.py
+-rw-r--r--   0        0        0      921 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_request_data_file.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      941 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data.py
+-rw-r--r--   0        0        0     1072 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      939 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      904 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_response.py
+-rw-r--r--   0        0        0     1005 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data.py
+-rw-r--r--   0        0        0     1249 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_request_data.py
+-rw-r--r--   0        0        0     1152 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      941 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes_image_files_item.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      936 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data.py
+-rw-r--r--   0        0        0     1067 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      938 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      899 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response.py
+-rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data.py
+-rw-r--r--   0        0        0     1248 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      975 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data.py
+-rw-r--r--   0        0        0     1106 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      945 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      929 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response.py
+-rw-r--r--   0        0        0     1039 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data.py
+-rw-r--r--   0        0        0     1255 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      929 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data.py
+-rw-r--r--   0        0        0     1060 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      936 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      892 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response.py
+-rw-r--r--   0        0        0      993 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data.py
+-rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_request_data.py
+-rw-r--r--   0        0        0     1039 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      931 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data.py
+-rw-r--r--   0        0        0     1068 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      938 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      900 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response.py
+-rw-r--r--   0        0        0     1001 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data.py
+-rw-r--r--   0        0        0     1248 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data_attributes.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response.py
+-rw-r--r--   0        0        0      989 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item.py
+-rw-r--r--   0        0        0     1040 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item_attributes.py
+-rw-r--r--   0        0        0      817 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response_links.py
+-rw-r--r--   0        0        0     1024 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response.py
+-rw-r--r--   0        0        0      986 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_data_item.py
+-rw-r--r--   0        0        0     1554 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_data_item_attributes.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_links.py
+-rw-r--r--   0        0        0     1008 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response.py
+-rw-r--r--   0        0        0     1158 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item.py
+-rw-r--r--   0        0        0     1779 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_attributes.py
+-rw-r--r--   0        0        0     1089 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships.py
+-rw-r--r--   0        0        0     1005 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template_data.py
+-rw-r--r--   0        0        0      821 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_links.py
+-rw-r--r--   0        0        0      740 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_events_response.py
+-rw-r--r--   0        0        0     1036 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response.py
+-rw-r--r--   0        0        0     1186 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item.py
+-rw-r--r--   0        0        0     1200 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_attributes.py
+-rw-r--r--   0        0        0     1887 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships.py
+-rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account.py
+-rw-r--r--   0        0        0      836 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account_data.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_reports.py
+-rw-r--r--   0        0        0     1030 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0     1004 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template_data.py
+-rw-r--r--   0        0        0     1050 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications.py
+-rw-r--r--   0        0        0      846 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_links.py
+-rw-r--r--   0        0        0      739 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_lists_response.py
+-rw-r--r--   0        0        0      863 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_a_report_response.py
+-rw-r--r--   0        0        0      964 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_a_report_response_data.py
+-rw-r--r--   0        0        0     1225 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_a_report_response_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_account_response_data.py
+-rw-r--r--   0        0        0     1896 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      858 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/remove_a_tag_1_request_meta.py
+-rw-r--r--   0        0        0      857 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/remove_a_tag_request_meta.py
+-rw-r--r--   0        0        0      961 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response.py
+-rw-r--r--   0        0        0     1325 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data.py
+-rw-r--r--   0        0        0     1294 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_attributes.py
+-rw-r--r--   0        0        0     1724 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships.py
+-rw-r--r--   0        0        0      827 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_account.py
+-rw-r--r--   0        0        0      827 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1098 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      860 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      905 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response.py
+-rw-r--r--   0        0        0     1209 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data.py
+-rw-r--r--   0        0        0     1280 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_attributes.py
+-rw-r--r--   0        0        0     1584 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships.py
+-rw-r--r--   0        0        0      813 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_account.py
+-rw-r--r--   0        0        0      813 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1042 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      846 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      965 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response.py
+-rw-r--r--   0        0        0     1332 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data.py
+-rw-r--r--   0        0        0     1295 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_attributes.py
+-rw-r--r--   0        0        0     1734 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships.py
+-rw-r--r--   0        0        0      828 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_account.py
+-rw-r--r--   0        0        0      828 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1102 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      861 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      861 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_request_meta.py
+-rw-r--r--   0        0        0      868 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response.py
+-rw-r--r--   0        0        0     1144 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data.py
+-rw-r--r--   0        0        0     1875 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_attributes.py
+-rw-r--r--   0        0        0     1473 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships.py
+-rw-r--r--   0        0        0      804 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_account.py
+-rw-r--r--   0        0        0      804 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1005 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      864 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_request_meta.py
+-rw-r--r--   0        0        0      880 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response.py
+-rw-r--r--   0        0        0     1165 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data.py
+-rw-r--r--   0        0        0     1878 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_attributes.py
+-rw-r--r--   0        0        0     1503 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships.py
+-rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_account.py
+-rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      840 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      877 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_request_meta.py
+-rw-r--r--   0        0        0      880 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response.py
+-rw-r--r--   0        0        0     1165 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data.py
+-rw-r--r--   0        0        0     1878 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_attributes.py
+-rw-r--r--   0        0        0     1503 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships.py
+-rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_account.py
+-rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      840 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      999 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      873 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_meta.py
+-rw-r--r--   0        0        0      928 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response.py
+-rw-r--r--   0        0        0     1267 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data.py
+-rw-r--r--   0        0        0     1821 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1164 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      788 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1019 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      879 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response.py
+-rw-r--r--   0        0        0     1163 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data.py
+-rw-r--r--   0        0        0     1309 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      961 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      945 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data.py
+-rw-r--r--   0        0        0     1767 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      782 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0     1036 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      945 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data.py
+-rw-r--r--   0        0        0     3024 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1181 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      792 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1142 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_photo_urls_item.py
+-rw-r--r--   0        0        0     1298 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1057 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      850 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      740 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_list_response.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response.py
+-rw-r--r--   0        0        0     1355 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data.py
+-rw-r--r--   0        0        0     1788 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1221 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0     1001 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1069 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      941 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response.py
+-rw-r--r--   0        0        0     1290 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data.py
+-rw-r--r--   0        0        0     1839 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      781 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0     1032 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      822 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_report_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data.py
+-rw-r--r--   0        0        0     1815 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data_attributes.py
+-rw-r--r--   0        0        0      920 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data.py
+-rw-r--r--   0        0        0     2216 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1156 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      786 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1011 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      817 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      953 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response.py
+-rw-r--r--   0        0        0     1311 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data.py
+-rw-r--r--   0        0        0     1763 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1196 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      794 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1304 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      825 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      824 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_selfie.py
+-rw-r--r--   0        0        0      945 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response.py
+-rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data.py
+-rw-r--r--   0        0        0     1755 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes.py
+-rw-r--r--   0        0        0     1188 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      792 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1036 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      879 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_account_response.py
+-rw-r--r--   0        0        0      980 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_account_response_data.py
+-rw-r--r--   0        0        0     1031 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      876 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response.py
+-rw-r--r--   0        0        0      977 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1584 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      876 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response.py
+-rw-r--r--   0        0        0      977 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data.py
+-rw-r--r--   0        0        0     1258 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes.py
+-rw-r--r--   0        0        0     1733 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request.py
+-rw-r--r--   0        0        0     1018 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params_filter.py
+-rw-r--r--   0        0        0      898 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_headers.py
+-rw-r--r--   0        0        0      774 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_post_params.py
+-rw-r--r--   0        0        0     1072 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response.py
+-rw-r--r--   0        0        0      893 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response_headers.py
+-rw-r--r--   0        0        0      742 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_event_response.py
+-rw-r--r--   0        0        0      883 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response.py
+-rw-r--r--   0        0        0      984 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data.py
+-rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data_attributes.py
+-rw-r--r--   0        0        0     1055 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response.py
+-rw-r--r--   0        0        0     1163 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     2311 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     2068 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_behaviours.py
+-rw-r--r--   0        0        0     1364 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_first.py
+-rw-r--r--   0        0        0      836 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_last.py
+-rw-r--r--   0        0        0     1798 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      820 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions.py
+-rw-r--r--   0        0        0      838 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0      991 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      834 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1037 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item.py
+-rw-r--r--   0        0        0     1782 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item_attributes.py
+-rw-r--r--   0        0        0      901 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response.py
+-rw-r--r--   0        0        0     1002 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data.py
+-rw-r--r--   0        0        0     1022 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data_attributes.py
+-rw-r--r--   0        0        0     1018 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response.py
+-rw-r--r--   0        0        0     1126 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data.py
+-rw-r--r--   0        0        0     1775 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1882 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships.py
+-rw-r--r--   0        0        0      996 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_accounts_data_item.py
+-rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments_data_item.py
+-rw-r--r--   0        0        0      987 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      834 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      815 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      992 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item.py
+-rw-r--r--   0        0        0     1092 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item_attributes.py
+-rw-r--r--   0        0        0      892 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_request_data.py
+-rw-r--r--   0        0        0      876 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_request_data_attributes.py
+-rw-r--r--   0        0        0      855 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response.py
+-rw-r--r--   0        0        0      956 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response_data.py
+-rw-r--r--   0        0        0     1682 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes.py
+-rw-r--r--   0        0        0      760 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      884 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_request_data.py
+-rw-r--r--   0        0        0      874 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_request_data_attributes.py
+-rw-r--r--   0        0        0      847 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response.py
+-rw-r--r--   0        0        0      948 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response_data.py
+-rw-r--r--   0        0        0     1750 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes.py
+-rw-r--r--   0        0        0      758 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_all_tags_1_request_meta.py
+-rw-r--r--   0        0        0      870 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_all_tags_request_meta.py
+-rw-r--r--   0        0        0      781 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_request_meta.py
+-rw-r--r--   0        0        0      881 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response.py
+-rw-r--r--   0        0        0     1167 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data.py
+-rw-r--r--   0        0        0     1842 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     2013 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      825 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0     1010 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      838 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0     1023 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      839 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0     1015 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      837 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data.py
+-rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      953 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      920 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data.py
+-rw-r--r--   0        0        0     1425 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1254 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1032 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      844 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      921 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response.py
+-rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data.py
+-rw-r--r--   0        0        0     2186 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response.py
+-rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data.py
+-rw-r--r--   0        0        0     2555 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1284 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1049 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      848 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0      821 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response.py
+-rw-r--r--   0        0        0     1341 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data.py
+-rw-r--r--   0        0        0     1557 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1061 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      829 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      912 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response.py
+-rw-r--r--   0        0        0     1221 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data.py
+-rw-r--r--   0        0        0     2043 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1003 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      945 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data.py
+-rw-r--r--   0        0        0     1551 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1290 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      822 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_selfie.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response.py
+-rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data.py
+-rw-r--r--   0        0        0     1549 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_attributes.py
+-rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      925 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body.py
+-rw-r--r--   0        0        0      824 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body_errors_item.py
+-rw-r--r--   0        0        0      892 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data.py
+-rw-r--r--   0        0        0     1128 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes.py
+-rw-r--r--   0        0        0      943 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_attachments_item.py
+-rw-r--r--   0        0        0     1055 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_fields.py
+-rw-r--r--   0        0        0      855 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response.py
+-rw-r--r--   0        0        0     1121 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data.py
+-rw-r--r--   0        0        0     1836 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1871 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      819 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      984 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      832 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0      997 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      833 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      989 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_request_data.py
+-rw-r--r--   0        0        0      894 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_request_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response.py
+-rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data.py
+-rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      953 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      831 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      958 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data.py
+-rw-r--r--   0        0        0     1561 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes.py
+-rw-r--r--   0        0        0     1353 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1167 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1358 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1168 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      921 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response.py
+-rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data.py
+-rw-r--r--   0        0        0     2186 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships.py
+-rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      983 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data.py
+-rw-r--r--   0        0        0     1589 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes.py
+-rw-r--r--   0        0        0     1369 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1171 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1374 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1172 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      937 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response.py
+-rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data.py
+-rw-r--r--   0        0        0     3080 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1045 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      847 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data.py
+-rw-r--r--   0        0        0     3576 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes.py
+-rw-r--r--   0        0        0     1231 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo.py
+-rw-r--r--   0        0        0     1113 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo_data.py
+-rw-r--r--   0        0        0      871 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_response_data.py
+-rw-r--r--   0        0        0     1080 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      905 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data.py
+-rw-r--r--   0        0        0     1804 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data_attributes.py
+-rw-r--r--   0        0        0      868 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_response.py
+-rw-r--r--   0        0        0      969 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1589 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      908 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data.py
+-rw-r--r--   0        0        0     2047 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data_attributes.py
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 fern_persona-0.0.2/PKG-INFO
```

### Comparing `fern_persona-0.0.1/README.md` & `fern_persona-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.1/src/persona/core/datetime_utils.py` & `fern_persona-0.0.2/src/persona/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.1/src/persona/core/jsonable_encoder.py` & `fern_persona-0.0.2/src/persona/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.1/src/persona/resources/__init__.py` & `fern_persona-0.0.2/src/persona/resources/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,59 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from . import (
     accounts,
+    api_keys,
     api_logs,
+    cases,
     database_verifications,
     document_verifications,
     documents,
+    email_address_verifications,
     events,
+    government_id_documents,
     government_id_verifications,
+    graph_queries,
     importers,
     inquiries,
+    list_items,
+    lists,
+    phone_carrier_database_verifications,
     phone_number_verifications,
+    print_verifications,
     reports,
+    selfie_verifications,
+    serpo_database_verifications,
+    tin_database_verifications,
+    user_audit_logs,
     verifications,
+    workflows,
 )
 
 __all__ = [
     "accounts",
+    "api_keys",
     "api_logs",
+    "cases",
     "database_verifications",
     "document_verifications",
     "documents",
+    "email_address_verifications",
     "events",
+    "government_id_documents",
     "government_id_verifications",
+    "graph_queries",
     "importers",
     "inquiries",
+    "list_items",
+    "lists",
+    "phone_carrier_database_verifications",
     "phone_number_verifications",
+    "print_verifications",
     "reports",
+    "selfie_verifications",
+    "serpo_database_verifications",
+    "tin_database_verifications",
+    "user_audit_logs",
     "verifications",
+    "workflows",
 ]
```

### Comparing `fern_persona-0.0.1/src/persona/resources/accounts/client.py` & `fern_persona-0.0.2/src/persona/resources/cases/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,366 +8,378 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
 from ...errors.bad_request_error import BadRequestError
-from ...errors.conflict_error import ConflictError
-from ...errors.not_found_error import NotFoundError
-from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.accounts_consolidate_request_meta import AccountsConsolidateRequestMeta
-from ...types.accounts_create_request_data import AccountsCreateRequestData
-from ...types.accounts_create_response import AccountsCreateResponse
-from ...types.accounts_list_all_response import AccountsListAllResponse
-from ...types.accounts_redact_response import AccountsRedactResponse
-from ...types.accounts_retrieve_response import AccountsRetrieveResponse
-from ...types.accounts_update_request_data import AccountsUpdateRequestData
-from ...types.accounts_update_response import AccountsUpdateResponse
-from ...types.unprocessable_entity_error_body import UnprocessableEntityErrorBody
+from ...types.add_persona_objects_request_meta import AddPersonaObjectsRequestMeta
+from ...types.add_persona_objects_response import AddPersonaObjectsResponse
+from ...types.assign_a_case_request_meta import AssignACaseRequestMeta
+from ...types.assign_a_case_response import AssignACaseResponse
+from ...types.create_a_case_request_data import CreateACaseRequestData
+from ...types.create_a_case_request_meta import CreateACaseRequestMeta
+from ...types.create_a_case_response import CreateACaseResponse
+from ...types.list_all_cases_response import ListAllCasesResponse
+from ...types.retrieve_case_response import RetrieveCaseResponse
+from ...types.set_status_for_a_case_request_meta import SetStatusForACaseRequestMeta
+from ...types.set_status_for_a_case_response import SetStatusForACaseResponse
+from ...types.update_a_case_request_data import UpdateACaseRequestData
+from ...types.update_a_case_response import UpdateACaseResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class AccountsClient:
+class CasesClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def retrieve(self, account_id: str, *, key_inflection: typing.Optional[str] = None) -> AccountsRetrieveResponse:
+    def list_all_cases(
+        self,
+        *,
+        page_after: typing.Optional[str] = None,
+        page_before: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        filter_status: typing.Optional[str] = None,
+        filter_resolution: typing.Optional[str] = None,
+        filter_case_template_id: typing.Optional[str] = None,
+        filter_account_id: typing.Optional[str] = None,
+        filter_inquiry_id: typing.Optional[str] = None,
+        filter_report_id: typing.Optional[str] = None,
+        key_inflection: typing.Optional[str] = None,
+    ) -> ListAllCasesResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            urllib.parse.urljoin(f"{self._environment.value}/", "cases"),
+            params={
+                "page[after]": page_after,
+                "page[before]": page_before,
+                "page[size]": page_size,
+                "filter[status]": filter_status,
+                "filter[resolution]": filter_resolution,
+                "filter[case-template-id]": filter_case_template_id,
+                "filter[account-id]": filter_account_id,
+                "filter[inquiry-id]": filter_inquiry_id,
+                "filter[report-id]": filter_report_id,
+            },
+            headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsRetrieveResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(ListAllCasesResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
-        self,
-        account_id: str,
-        *,
-        data: typing.Optional[AccountsUpdateRequestData] = OMIT,
-        key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> AccountsUpdateResponse:
-        _request: typing.Dict[str, typing.Any] = {}
-        if data is not OMIT:
-            _request["data"] = data
+    def create_a_case(
+        self, *, data: CreateACaseRequestData, meta: typing.Optional[CreateACaseRequestMeta] = OMIT
+    ) -> CreateACaseResponse:
+        _request: typing.Dict[str, typing.Any] = {"data": data}
+        if meta is not OMIT:
+            _request["meta"] = meta
         _response = httpx.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "cases"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsUpdateResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(CreateACaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def redact(self, account_id: str, *, persona_version: typing.Optional[str] = None) -> AccountsRedactResponse:
+    def retrieve_case(self, case_id: str, *, key_inflection: typing.Optional[str] = None) -> RetrieveCaseResponse:
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-            headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
+            headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsRedactResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveCaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list_all(
-        self,
-        *,
-        page_before: typing.Optional[str] = None,
-        page_after: typing.Optional[str] = None,
-        page_size: typing.Optional[str] = None,
-        filter_reference_id: typing.Optional[str] = None,
-        key_inflection: typing.Optional[str] = None,
-    ) -> AccountsListAllResponse:
+    def update_a_case(
+        self, case_id: str, *, data: typing.Optional[UpdateACaseRequestData] = OMIT
+    ) -> UpdateACaseResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
-            params={
-                "page[before]": page_before,
-                "page[after]": page_after,
-                "page[size]": page_size,
-                "filter[reference-id]": filter_reference_id,
-            },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
+            json=jsonable_encoder(_request),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsListAllResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UpdateACaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(
-        self,
-        *,
-        data: typing.Optional[AccountsCreateRequestData] = OMIT,
-        key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> AccountsCreateResponse:
+    def add_persona_objects(
+        self, case_id: str, *, meta: typing.Optional[AddPersonaObjectsRequestMeta] = OMIT
+    ) -> AddPersonaObjectsResponse:
         _request: typing.Dict[str, typing.Any] = {}
-        if data is not OMIT:
-            _request["data"] = data
+        if meta is not OMIT:
+            _request["meta"] = meta
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/add-objects"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsCreateResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(AddPersonaObjectsResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def consolidate(
-        self,
-        account_id: str,
-        *,
-        meta: typing.Optional[AccountsConsolidateRequestMeta] = OMIT,
-        key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> None:
+    def assign_a_case(self, case_id: str, *, meta: AssignACaseRequestMeta) -> AssignACaseResponse:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/assign"),
+            json=jsonable_encoder({"meta": meta}),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(AssignACaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def set_status_for_a_case(
+        self, case_id: str, *, meta: typing.Optional[SetStatusForACaseRequestMeta] = OMIT
+    ) -> SetStatusForACaseResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/consolidate"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/set-status"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
-            ),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(SetStatusForACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(
-                pydantic.parse_obj_as(UnprocessableEntityErrorBody, _response.json())  # type: ignore
-            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncAccountsClient:
+class AsyncCasesClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def retrieve(
-        self, account_id: str, *, key_inflection: typing.Optional[str] = None
-    ) -> AccountsRetrieveResponse:
+    async def list_all_cases(
+        self,
+        *,
+        page_after: typing.Optional[str] = None,
+        page_before: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        filter_status: typing.Optional[str] = None,
+        filter_resolution: typing.Optional[str] = None,
+        filter_case_template_id: typing.Optional[str] = None,
+        filter_account_id: typing.Optional[str] = None,
+        filter_inquiry_id: typing.Optional[str] = None,
+        filter_report_id: typing.Optional[str] = None,
+        key_inflection: typing.Optional[str] = None,
+    ) -> ListAllCasesResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                urllib.parse.urljoin(f"{self._environment.value}/", "cases"),
+                params={
+                    "page[after]": page_after,
+                    "page[before]": page_before,
+                    "page[size]": page_size,
+                    "filter[status]": filter_status,
+                    "filter[resolution]": filter_resolution,
+                    "filter[case-template-id]": filter_case_template_id,
+                    "filter[account-id]": filter_account_id,
+                    "filter[inquiry-id]": filter_inquiry_id,
+                    "filter[report-id]": filter_report_id,
+                },
+                headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsRetrieveResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(ListAllCasesResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self,
-        account_id: str,
-        *,
-        data: typing.Optional[AccountsUpdateRequestData] = OMIT,
-        key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> AccountsUpdateResponse:
-        _request: typing.Dict[str, typing.Any] = {}
-        if data is not OMIT:
-            _request["data"] = data
+    async def create_a_case(
+        self, *, data: CreateACaseRequestData, meta: typing.Optional[CreateACaseRequestMeta] = OMIT
+    ) -> CreateACaseResponse:
+        _request: typing.Dict[str, typing.Any] = {"data": data}
+        if meta is not OMIT:
+            _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", "cases"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers(
-                    {
-                        "Key-Inflection": key_inflection,
-                        "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
-                    }
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsUpdateResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(CreateACaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def redact(self, account_id: str, *, persona_version: typing.Optional[str] = None) -> AccountsRedactResponse:
+    async def retrieve_case(self, case_id: str, *, key_inflection: typing.Optional[str] = None) -> RetrieveCaseResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-                headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
+                headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsRedactResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveCaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list_all(
-        self,
-        *,
-        page_before: typing.Optional[str] = None,
-        page_after: typing.Optional[str] = None,
-        page_size: typing.Optional[str] = None,
-        filter_reference_id: typing.Optional[str] = None,
-        key_inflection: typing.Optional[str] = None,
-    ) -> AccountsListAllResponse:
+    async def update_a_case(
+        self, case_id: str, *, data: typing.Optional[UpdateACaseRequestData] = OMIT
+    ) -> UpdateACaseResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
-                params={
-                    "page[before]": page_before,
-                    "page[after]": page_after,
-                    "page[size]": page_size,
-                    "filter[reference-id]": filter_reference_id,
-                },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                "PATCH",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
+                json=jsonable_encoder(_request),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsListAllResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UpdateACaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(
-        self,
-        *,
-        data: typing.Optional[AccountsCreateRequestData] = OMIT,
-        key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> AccountsCreateResponse:
+    async def add_persona_objects(
+        self, case_id: str, *, meta: typing.Optional[AddPersonaObjectsRequestMeta] = OMIT
+    ) -> AddPersonaObjectsResponse:
         _request: typing.Dict[str, typing.Any] = {}
-        if data is not OMIT:
-            _request["data"] = data
+        if meta is not OMIT:
+            _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/add-objects"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers(
-                    {
-                        "Key-Inflection": key_inflection,
-                        "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
-                    }
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(AddPersonaObjectsResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def assign_a_case(self, case_id: str, *, meta: AssignACaseRequestMeta) -> AssignACaseResponse:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/assign"),
+                json=jsonable_encoder({"meta": meta}),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AccountsCreateResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(AssignACaseResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def consolidate(
-        self,
-        account_id: str,
-        *,
-        meta: typing.Optional[AccountsConsolidateRequestMeta] = OMIT,
-        key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> None:
+    async def set_status_for_a_case(
+        self, case_id: str, *, meta: typing.Optional[SetStatusForACaseRequestMeta] = OMIT
+    ) -> SetStatusForACaseResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/consolidate"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/set-status"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers(
-                    {
-                        "Key-Inflection": key_inflection,
-                        "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
-                    }
-                ),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(SetStatusForACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
-        if _response.status_code == 422:
-            raise UnprocessableEntityError(
-                pydantic.parse_obj_as(UnprocessableEntityErrorBody, _response.json())  # type: ignore
-            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/api_logs/client.py` & `fern_persona-0.0.2/src/persona/resources/api_logs/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
 from ...errors.not_found_error import NotFoundError
-from ...types.api_logs_retrieve_response import ApiLogsRetrieveResponse
+from ...types.retrieve_an_api_log_response import RetrieveAnApiLogResponse
 
 
 class ApiLogsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def list(
+    def list_all_api_logs(
         self,
         *,
         page_before: typing.Optional[str] = None,
         page_after: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         key_inflection: typing.Optional[str] = None,
     ) -> None:
@@ -38,38 +38,40 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, api_log_id: str, *, key_inflection: typing.Optional[str] = None) -> ApiLogsRetrieveResponse:
+    def retrieve_an_api_log(
+        self, api_log_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnApiLogResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api-logs/{api_log_id}"),
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiLogsRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnApiLogResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncApiLogsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def list(
+    async def list_all_api_logs(
         self,
         *,
         page_before: typing.Optional[str] = None,
         page_after: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         key_inflection: typing.Optional[str] = None,
     ) -> None:
@@ -85,26 +87,26 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(
+    async def retrieve_an_api_log(
         self, api_log_id: str, *, key_inflection: typing.Optional[str] = None
-    ) -> ApiLogsRetrieveResponse:
+    ) -> RetrieveAnApiLogResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api-logs/{api_log_id}"),
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ApiLogsRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnApiLogResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/document_verifications/client.py` & `fern_persona-0.0.2/src/persona/resources/document_verifications/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,74 +8,76 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
 from ...errors.bad_request_error import BadRequestError
-from ...types.document_verifications_create_request_data import DocumentVerificationsCreateRequestData
-from ...types.document_verifications_create_response import DocumentVerificationsCreateResponse
-from ...types.document_verifications_submit_response import DocumentVerificationsSubmitResponse
+from ...types.create_a_document_verification_request_data import CreateADocumentVerificationRequestData
+from ...types.create_a_document_verification_response import CreateADocumentVerificationResponse
+from ...types.submit_a_document_verification_response import SubmitADocumentVerificationResponse
 
 
 class DocumentVerificationsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def create(
+    def create_a_document_verification(
         self,
         *,
-        data: DocumentVerificationsCreateRequestData,
+        data: CreateADocumentVerificationRequestData,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentVerificationsCreateResponse:
+    ) -> CreateADocumentVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/documents"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentVerificationsCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateADocumentVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def submit(
+    def submit_a_document_verification(
         self,
         verification_id: str,
         *,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentVerificationsSubmitResponse:
+    ) -> SubmitADocumentVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}/submit"),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentVerificationsSubmitResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SubmitADocumentVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, verification_id: str, *, key_inflection: typing.Optional[str] = None) -> None:
+    def retrieve_a_document_verification(
+        self, verification_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}"),
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -90,21 +92,21 @@
 
 
 class AsyncDocumentVerificationsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def create(
+    async def create_a_document_verification(
         self,
         *,
-        data: DocumentVerificationsCreateRequestData,
+        data: CreateADocumentVerificationRequestData,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentVerificationsCreateResponse:
+    ) -> CreateADocumentVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/documents"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
@@ -112,52 +114,54 @@
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentVerificationsCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateADocumentVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def submit(
+    async def submit_a_document_verification(
         self,
         verification_id: str,
         *,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentVerificationsSubmitResponse:
+    ) -> SubmitADocumentVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentVerificationsSubmitResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SubmitADocumentVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(self, verification_id: str, *, key_inflection: typing.Optional[str] = None) -> None:
+    async def retrieve_a_document_verification(
+        self, verification_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}"),
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
```

### Comparing `fern_persona-0.0.1/src/persona/resources/documents/client.py` & `fern_persona-0.0.2/src/persona/resources/documents/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,155 +8,157 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
 from ...errors.bad_request_error import BadRequestError
-from ...types.documents_create_request_data import DocumentsCreateRequestData
-from ...types.documents_create_response import DocumentsCreateResponse
-from ...types.documents_retrieve_response import DocumentsRetrieveResponse
-from ...types.documents_submit_response import DocumentsSubmitResponse
-from ...types.documents_update_request_data import DocumentsUpdateRequestData
-from ...types.documents_update_response import DocumentsUpdateResponse
+from ...types.create_a_document_request_data import CreateADocumentRequestData
+from ...types.create_a_document_response import CreateADocumentResponse
+from ...types.retrieve_a_document_response import RetrieveADocumentResponse
+from ...types.submit_a_document_response import SubmitADocumentResponse
+from ...types.update_a_document_request_data import UpdateADocumentRequestData
+from ...types.update_a_document_response import UpdateADocumentResponse
 
 
 class DocumentsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def retrieve(self, document_id: str, *, key_inflection: typing.Optional[str] = None) -> DocumentsRetrieveResponse:
+    def retrieve_a_document(
+        self, document_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveADocumentResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"documents/{document_id}"),
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(
+    def create_a_document(
         self,
         *,
-        data: DocumentsCreateRequestData,
+        data: CreateADocumentRequestData,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentsCreateResponse:
+    ) -> CreateADocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "document/generics"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
+    def update_a_document(
         self,
         document_id: str,
         *,
-        data: DocumentsUpdateRequestData,
+        data: UpdateADocumentRequestData,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentsUpdateResponse:
+    ) -> UpdateADocumentResponse:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsUpdateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UpdateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def submit(
+    def submit_a_document(
         self,
         document_id: str,
         *,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentsSubmitResponse:
+    ) -> SubmitADocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}/submit"),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsSubmitResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SubmitADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDocumentsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def retrieve(
+    async def retrieve_a_document(
         self, document_id: str, *, key_inflection: typing.Optional[str] = None
-    ) -> DocumentsRetrieveResponse:
+    ) -> RetrieveADocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"documents/{document_id}"),
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(
+    async def create_a_document(
         self,
         *,
-        data: DocumentsCreateRequestData,
+        data: CreateADocumentRequestData,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentsCreateResponse:
+    ) -> CreateADocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "document/generics"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
@@ -164,31 +166,31 @@
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
+    async def update_a_document(
         self,
         document_id: str,
         *,
-        data: DocumentsUpdateRequestData,
+        data: UpdateADocumentRequestData,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentsUpdateResponse:
+    ) -> UpdateADocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
@@ -196,45 +198,45 @@
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsUpdateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UpdateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def submit(
+    async def submit_a_document(
         self,
         document_id: str,
         *,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> DocumentsSubmitResponse:
+    ) -> SubmitADocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(DocumentsSubmitResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SubmitADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/events/client.py` & `fern_persona-0.0.2/src/persona/resources/events/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
 from ...errors.bad_request_error import BadRequestError
-from ...types.events_list_all_response import EventsListAllResponse
-from ...types.events_retrieve_response import EventsRetrieveResponse
+from ...types.list_all_events_response import ListAllEventsResponse
+from ...types.retrieve_an_event_response import RetrieveAnEventResponse
 
 
 class EventsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def list_all(
+    def list_all_events(
         self,
         *,
         page_before: typing.Optional[str] = None,
         page_after: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         filter_name: typing.Optional[str] = None,
         filter_object_id: typing.Optional[str] = None,
         filter_id: typing.Optional[str] = None,
         key_inflection: typing.Optional[str] = None,
-    ) -> EventsListAllResponse:
+    ) -> ListAllEventsResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "events"),
             params={
                 "page[before]": page_before,
                 "page[after]": page_after,
                 "page[size]": page_size,
@@ -42,57 +42,59 @@
                 "filter[object_id]": filter_object_id,
                 "filter[id]": filter_id,
             },
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EventsListAllResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListAllEventsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, event_id: str, *, key_inflection: typing.Optional[str] = None) -> EventsRetrieveResponse:
+    def retrieve_an_event(
+        self, event_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnEventResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"events/{event_id}"),
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EventsRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnEventResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncEventsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def list_all(
+    async def list_all_events(
         self,
         *,
         page_before: typing.Optional[str] = None,
         page_after: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         filter_name: typing.Optional[str] = None,
         filter_object_id: typing.Optional[str] = None,
         filter_id: typing.Optional[str] = None,
         key_inflection: typing.Optional[str] = None,
-    ) -> EventsListAllResponse:
+    ) -> ListAllEventsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "events"),
                 params={
                     "page[before]": page_before,
                     "page[after]": page_after,
@@ -101,33 +103,35 @@
                     "filter[object_id]": filter_object_id,
                     "filter[id]": filter_id,
                 },
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EventsListAllResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListAllEventsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(self, event_id: str, *, key_inflection: typing.Optional[str] = None) -> EventsRetrieveResponse:
+    async def retrieve_an_event(
+        self, event_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnEventResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"events/{event_id}"),
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EventsRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnEventResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/government_id_verifications/client.py` & `fern_persona-0.0.2/src/persona/resources/workflows/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,74 +7,80 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
-from ...types.government_id_verifications_create_request_data import GovernmentIdVerificationsCreateRequestData
-from ...types.government_id_verifications_create_response import GovernmentIdVerificationsCreateResponse
+from ...errors.bad_request_error import BadRequestError
+from ...types.create_a_workflow_run_request_data import CreateAWorkflowRunRequestData
+from ...types.create_a_workflow_run_response import CreateAWorkflowRunResponse
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
-class GovernmentIdVerificationsClient:
+
+class WorkflowsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def create(
+    def create_a_workflow_run(
         self,
+        workflow_id: str,
         *,
-        data: GovernmentIdVerificationsCreateRequestData,
+        data: typing.Optional[CreateAWorkflowRunRequestData] = OMIT,
         key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> GovernmentIdVerificationsCreateResponse:
+    ) -> CreateAWorkflowRunResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "verification/government-ids"),
-            json=jsonable_encoder({"data": data}),
-            headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
-            ),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"workflows/{workflow_id}/trigger"),
+            json=jsonable_encoder(_request),
+            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GovernmentIdVerificationsCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateAWorkflowRunResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncGovernmentIdVerificationsClient:
+class AsyncWorkflowsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def create(
+    async def create_a_workflow_run(
         self,
+        workflow_id: str,
         *,
-        data: GovernmentIdVerificationsCreateRequestData,
+        data: typing.Optional[CreateAWorkflowRunRequestData] = OMIT,
         key_inflection: typing.Optional[str] = None,
-        idempotency_key: typing.Optional[str] = None,
-    ) -> GovernmentIdVerificationsCreateResponse:
+    ) -> CreateAWorkflowRunResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "verification/government-ids"),
-                json=jsonable_encoder({"data": data}),
-                headers=remove_none_from_headers(
-                    {
-                        "Key-Inflection": key_inflection,
-                        "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
-                    }
-                ),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"workflows/{workflow_id}/trigger"),
+                json=jsonable_encoder(_request),
+                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GovernmentIdVerificationsCreateResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateAWorkflowRunResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/importers/client.py` & `fern_persona-0.0.2/src/persona/resources/importers/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,403 +8,444 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
 from ...errors.bad_request_error import BadRequestError
-from ...types.importers_import_account_request_data import ImportersImportAccountRequestData
-from ...types.importers_import_account_response import ImportersImportAccountResponse
-from ...types.importers_import_email_address_lists_request_data import ImportersImportEmailAddressListsRequestData
-from ...types.importers_import_email_address_lists_response import ImportersImportEmailAddressListsResponse
-from ...types.importers_import_geolocation_lists_request_data import ImportersImportGeolocationListsRequestData
-from ...types.importers_import_geolocation_lists_response import ImportersImportGeolocationListsResponse
-from ...types.importers_import_government_id_number_lists_request_data import (
-    ImportersImportGovernmentIdNumberListsRequestData,
-)
-from ...types.importers_import_government_id_number_lists_response import ImportersImportGovernmentIdNumberListsResponse
-from ...types.importers_import_ip_address_lists_request_data import ImportersImportIpAddressListsRequestData
-from ...types.importers_import_ip_address_lists_response import ImportersImportIpAddressListsResponse
-from ...types.importers_import_name_lists_request_data import ImportersImportNameListsRequestData
-from ...types.importers_import_name_lists_response import ImportersImportNameListsResponse
-from ...types.importers_import_phone_number_lists_request_data import ImportersImportPhoneNumberListsRequestData
-from ...types.importers_import_phone_number_lists_response import ImportersImportPhoneNumberListsResponse
-from ...types.importers_retrieve_response import ImportersRetrieveResponse
+from ...types.import_an_account_request_data import ImportAnAccountRequestData
+from ...types.import_an_account_response import ImportAnAccountResponse
+from ...types.import_email_address_lists_request_data import ImportEmailAddressListsRequestData
+from ...types.import_email_address_lists_response import ImportEmailAddressListsResponse
+from ...types.import_face_lists_request_data import ImportFaceListsRequestData
+from ...types.import_face_lists_response import ImportFaceListsResponse
+from ...types.import_geolocation_lists_request_data import ImportGeolocationListsRequestData
+from ...types.import_geolocation_lists_response import ImportGeolocationListsResponse
+from ...types.import_government_id_number_lists_request_data import ImportGovernmentIdNumberListsRequestData
+from ...types.import_government_id_number_lists_response import ImportGovernmentIdNumberListsResponse
+from ...types.import_ip_address_lists_request_data import ImportIpAddressListsRequestData
+from ...types.import_ip_address_lists_response import ImportIpAddressListsResponse
+from ...types.import_name_lists_request_data import ImportNameListsRequestData
+from ...types.import_name_lists_response import ImportNameListsResponse
+from ...types.import_phone_number_lists_request_data import ImportPhoneNumberListsRequestData
+from ...types.import_phone_number_lists_response import ImportPhoneNumberListsResponse
+from ...types.retrieve_an_importer_response import RetrieveAnImporterResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ImportersClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def retrieve(self, importer_id: str) -> ImportersRetrieveResponse:
+    def retrieve_an_importer(self, importer_id: str) -> RetrieveAnImporterResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"importers/{importer_id}"),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnImporterResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def import_account(
-        self, *, data: typing.Optional[ImportersImportAccountRequestData] = OMIT
-    ) -> ImportersImportAccountResponse:
+    def import_an_account(self, *, data: typing.Optional[ImportAnAccountRequestData] = OMIT) -> ImportAnAccountResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/accounts"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportAccountResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def import_email_address_lists(
-        self, *, data: typing.Optional[ImportersImportEmailAddressListsRequestData] = OMIT
-    ) -> ImportersImportEmailAddressListsResponse:
+        self, *, data: typing.Optional[ImportEmailAddressListsRequestData] = OMIT
+    ) -> ImportEmailAddressListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/email-addresses"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportEmailAddressListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportEmailAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def import_geolocation_lists(
-        self, *, data: typing.Optional[ImportersImportGeolocationListsRequestData] = OMIT
-    ) -> ImportersImportGeolocationListsResponse:
+        self, *, data: typing.Optional[ImportGeolocationListsRequestData] = OMIT
+    ) -> ImportGeolocationListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/geolocations"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportGeolocationListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportGeolocationListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def import_government_id_number_lists(
-        self, *, data: typing.Optional[ImportersImportGovernmentIdNumberListsRequestData] = OMIT
-    ) -> ImportersImportGovernmentIdNumberListsResponse:
+        self, *, data: typing.Optional[ImportGovernmentIdNumberListsRequestData] = OMIT
+    ) -> ImportGovernmentIdNumberListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/government-id-numbers"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportGovernmentIdNumberListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportGovernmentIdNumberListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def import_ip_address_lists(
-        self, *, data: typing.Optional[ImportersImportIpAddressListsRequestData] = OMIT
-    ) -> ImportersImportIpAddressListsResponse:
+        self, *, data: typing.Optional[ImportIpAddressListsRequestData] = OMIT
+    ) -> ImportIpAddressListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/ip-addresses"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportIpAddressListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportIpAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def import_name_lists(
-        self, *, data: typing.Optional[ImportersImportNameListsRequestData] = OMIT
-    ) -> ImportersImportNameListsResponse:
+    def import_name_lists(self, *, data: typing.Optional[ImportNameListsRequestData] = OMIT) -> ImportNameListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/names"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportNameListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportNameListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def import_phone_number_lists(
-        self, *, data: typing.Optional[ImportersImportPhoneNumberListsRequestData] = OMIT
-    ) -> ImportersImportPhoneNumberListsResponse:
+        self, *, data: typing.Optional[ImportPhoneNumberListsRequestData] = OMIT
+    ) -> ImportPhoneNumberListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/phone-numbers"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportPhoneNumberListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportPhoneNumberListsResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def import_face_lists(self, *, data: typing.Optional[ImportFaceListsRequestData] = OMIT) -> ImportFaceListsResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/faces"),
+            json=jsonable_encoder(_request),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ImportFaceListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncImportersClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def retrieve(self, importer_id: str) -> ImportersRetrieveResponse:
+    async def retrieve_an_importer(self, importer_id: str) -> RetrieveAnImporterResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"importers/{importer_id}"),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersRetrieveResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnImporterResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def import_account(
-        self, *, data: typing.Optional[ImportersImportAccountRequestData] = OMIT
-    ) -> ImportersImportAccountResponse:
+    async def import_an_account(
+        self, *, data: typing.Optional[ImportAnAccountRequestData] = OMIT
+    ) -> ImportAnAccountResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/accounts"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportAccountResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def import_email_address_lists(
-        self, *, data: typing.Optional[ImportersImportEmailAddressListsRequestData] = OMIT
-    ) -> ImportersImportEmailAddressListsResponse:
+        self, *, data: typing.Optional[ImportEmailAddressListsRequestData] = OMIT
+    ) -> ImportEmailAddressListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/email-addresses"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportEmailAddressListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportEmailAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def import_geolocation_lists(
-        self, *, data: typing.Optional[ImportersImportGeolocationListsRequestData] = OMIT
-    ) -> ImportersImportGeolocationListsResponse:
+        self, *, data: typing.Optional[ImportGeolocationListsRequestData] = OMIT
+    ) -> ImportGeolocationListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/geolocations"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportGeolocationListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportGeolocationListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def import_government_id_number_lists(
-        self, *, data: typing.Optional[ImportersImportGovernmentIdNumberListsRequestData] = OMIT
-    ) -> ImportersImportGovernmentIdNumberListsResponse:
+        self, *, data: typing.Optional[ImportGovernmentIdNumberListsRequestData] = OMIT
+    ) -> ImportGovernmentIdNumberListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/government-id-numbers"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportGovernmentIdNumberListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportGovernmentIdNumberListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def import_ip_address_lists(
-        self, *, data: typing.Optional[ImportersImportIpAddressListsRequestData] = OMIT
-    ) -> ImportersImportIpAddressListsResponse:
+        self, *, data: typing.Optional[ImportIpAddressListsRequestData] = OMIT
+    ) -> ImportIpAddressListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/ip-addresses"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportIpAddressListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportIpAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def import_name_lists(
-        self, *, data: typing.Optional[ImportersImportNameListsRequestData] = OMIT
-    ) -> ImportersImportNameListsResponse:
+        self, *, data: typing.Optional[ImportNameListsRequestData] = OMIT
+    ) -> ImportNameListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/names"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportNameListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportNameListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def import_phone_number_lists(
-        self, *, data: typing.Optional[ImportersImportPhoneNumberListsRequestData] = OMIT
-    ) -> ImportersImportPhoneNumberListsResponse:
+        self, *, data: typing.Optional[ImportPhoneNumberListsRequestData] = OMIT
+    ) -> ImportPhoneNumberListsResponse:
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/phone-numbers"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ImportersImportPhoneNumberListsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ImportPhoneNumberListsResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def import_face_lists(
+        self, *, data: typing.Optional[ImportFaceListsRequestData] = OMIT
+    ) -> ImportFaceListsResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/faces"),
+                json=jsonable_encoder(_request),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ImportFaceListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/inquiries/client.py` & `fern_persona-0.0.2/src/persona/resources/accounts/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,449 +7,602 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
+from ...errors.bad_request_error import BadRequestError
 from ...errors.conflict_error import ConflictError
 from ...errors.not_found_error import NotFoundError
-from ...types.inquiries_approve_request_meta import InquiriesApproveRequestMeta
-from ...types.inquiries_approve_response import InquiriesApproveResponse
-from ...types.inquiries_create_request_data import InquiriesCreateRequestData
-from ...types.inquiries_create_response import InquiriesCreateResponse
-from ...types.inquiries_decline_request_meta import InquiriesDeclineRequestMeta
-from ...types.inquiries_decline_response import InquiriesDeclineResponse
-from ...types.inquiries_list_all_response import InquiriesListAllResponse
-from ...types.inquiries_redact_response import InquiriesRedactResponse
-from ...types.inquiries_resume_response import InquiriesResumeResponse
-from ...types.inquiries_retrieve_response import InquiriesRetrieveResponse
-from ...types.inquiries_update_request_data import InquiriesUpdateRequestData
+from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.add_a_tag_1_request_meta import AddATag1RequestMeta
+from ...types.consolidate_into_an_account_request_meta import ConsolidateIntoAnAccountRequestMeta
+from ...types.create_an_account_request_data import CreateAnAccountRequestData
+from ...types.create_an_account_response import CreateAnAccountResponse
+from ...types.list_all_accounts_response import ListAllAccountsResponse
+from ...types.redact_an_account_response import RedactAnAccountResponse
+from ...types.remove_a_tag_1_request_meta import RemoveATag1RequestMeta
+from ...types.retrieve_an_account_response import RetrieveAnAccountResponse
+from ...types.set_all_tags_1_request_meta import SetAllTags1RequestMeta
+from ...types.unprocessable_entity_error_body import UnprocessableEntityErrorBody
+from ...types.update_an_account_request_data import UpdateAnAccountRequestData
+from ...types.update_an_account_response import UpdateAnAccountResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class InquiriesClient:
+class AccountsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def resume(
+    def retrieve_an_account(
+        self, account_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnAccountResponse:
+        _response = httpx.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(RetrieveAnAccountResponse, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def update_an_account(
         self,
-        inquiry_id: str,
+        account_id: str,
         *,
+        data: typing.Optional[UpdateAnAccountRequestData] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesResumeResponse:
+    ) -> UpdateAnAccountResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/resume"),
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesResumeResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(UpdateAnAccountResponse, _response.json())  # type: ignore
+        if _response.status_code == 409:
+            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None) -> InquiriesRetrieveResponse:
+    def redact_an_account(
+        self, account_id: str, *, persona_version: typing.Optional[str] = None
+    ) -> RedactAnAccountResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+            headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesRetrieveResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(RedactAnAccountResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
-        self, inquiry_id: str, *, data: InquiriesUpdateRequestData, key_inflection: typing.Optional[str] = None
-    ) -> None:
+    def list_all_accounts(
+        self,
+        *,
+        page_before: typing.Optional[str] = None,
+        page_after: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        filter_reference_id: typing.Optional[str] = None,
+        key_inflection: typing.Optional[str] = None,
+    ) -> ListAllAccountsResponse:
         _response = httpx.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-            json=jsonable_encoder({"data": data}),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            params={
+                "page[before]": page_before,
+                "page[after]": page_after,
+                "page[size]": page_size,
+                "filter[reference-id]": filter_reference_id,
+            },
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(ListAllAccountsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def redact(self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None) -> InquiriesRedactResponse:
+    def create_an_account(
+        self,
+        *,
+        data: typing.Optional[CreateAnAccountRequestData] = OMIT,
+        key_inflection: typing.Optional[str] = None,
+        idempotency_key: typing.Optional[str] = None,
+    ) -> CreateAnAccountResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+            json=jsonable_encoder(_request),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesRedactResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateAnAccountResponse, _response.json())  # type: ignore
+        if _response.status_code == 409:
+            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def approve(
+    def consolidate_into_an_account(
         self,
-        inquiry_id: str,
+        account_id: str,
         *,
-        meta: typing.Optional[InquiriesApproveRequestMeta] = OMIT,
+        meta: typing.Optional[ConsolidateIntoAnAccountRequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesApproveResponse:
+    ) -> None:
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/approve"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/consolidate"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesApproveResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(UnprocessableEntityErrorBody, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def decline(
+    def add_a_tag_1(
         self,
-        inquiry_id: str,
+        account_id: str,
         *,
-        meta: typing.Optional[InquiriesDeclineRequestMeta] = OMIT,
+        meta: typing.Optional[AddATag1RequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesDeclineResponse:
+    ) -> None:
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/decline"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/add-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesDeclineResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list_all(
+    def remove_a_tag_1(
         self,
+        account_id: str,
         *,
-        page_after: typing.Optional[str] = None,
-        page_before: typing.Optional[str] = None,
-        page_size: typing.Optional[str] = None,
-        filter_account_id: typing.Optional[str] = None,
-        filter_reference_id: typing.Optional[str] = None,
+        meta: typing.Optional[RemoveATag1RequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
-    ) -> InquiriesListAllResponse:
+        idempotency_key: typing.Optional[str] = None,
+    ) -> None:
+        _request: typing.Dict[str, typing.Any] = {}
+        if meta is not OMIT:
+            _request["meta"] = meta
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "inquiries"),
-            params={
-                "page[after]": page_after,
-                "page[before]": page_before,
-                "page[size]": page_size,
-                "filter[account-id]": filter_account_id,
-                "filter[reference-id]": filter_reference_id,
-            },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/remove-tag"),
+            json=jsonable_encoder(_request),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesListAllResponse, _response.json())  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(
+    def set_all_tags_1(
         self,
+        account_id: str,
         *,
-        data: InquiriesCreateRequestData,
+        meta: typing.Optional[SetAllTags1RequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesCreateResponse:
+    ) -> None:
+        _request: typing.Dict[str, typing.Any] = {}
+        if meta is not OMIT:
+            _request["meta"] = meta
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "inquiries"),
-            json=jsonable_encoder({"data": data}),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/set-tags"),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesCreateResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def print_an_inquiry_pdf(self, inquiry_id: str) -> None:
+        _response = httpx.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/print"),
+            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncInquiriesClient:
+class AsyncAccountsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def resume(
+    async def retrieve_an_account(
+        self, account_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnAccountResponse:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(RetrieveAnAccountResponse, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def update_an_account(
         self,
-        inquiry_id: str,
+        account_id: str,
         *,
+        data: typing.Optional[UpdateAnAccountRequestData] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesResumeResponse:
+    ) -> UpdateAnAccountResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/resume"),
+                "PATCH",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesResumeResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(UpdateAnAccountResponse, _response.json())  # type: ignore
+        if _response.status_code == 409:
+            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(
-        self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
-    ) -> InquiriesRetrieveResponse:
+    async def redact_an_account(
+        self, account_id: str, *, persona_version: typing.Optional[str] = None
+    ) -> RedactAnAccountResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
+                headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesRetrieveResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(RedactAnAccountResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self, inquiry_id: str, *, data: InquiriesUpdateRequestData, key_inflection: typing.Optional[str] = None
-    ) -> None:
+    async def list_all_accounts(
+        self,
+        *,
+        page_before: typing.Optional[str] = None,
+        page_after: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        filter_reference_id: typing.Optional[str] = None,
+        key_inflection: typing.Optional[str] = None,
+    ) -> ListAllAccountsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-                json=jsonable_encoder({"data": data}),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+                params={
+                    "page[before]": page_before,
+                    "page[after]": page_after,
+                    "page[size]": page_size,
+                    "filter[reference-id]": filter_reference_id,
+                },
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return pydantic.parse_obj_as(ListAllAccountsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def redact(self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None) -> InquiriesRedactResponse:
+    async def create_an_account(
+        self,
+        *,
+        data: typing.Optional[CreateAnAccountRequestData] = OMIT,
+        key_inflection: typing.Optional[str] = None,
+        idempotency_key: typing.Optional[str] = None,
+    ) -> CreateAnAccountResponse:
+        _request: typing.Dict[str, typing.Any] = {}
+        if data is not OMIT:
+            _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
+                json=jsonable_encoder(_request),
+                headers=remove_none_from_headers(
+                    {
+                        "Key-Inflection": key_inflection,
+                        "Idempotency-Key": idempotency_key,
+                        "Authorization": self.api_key,
+                    }
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesRedactResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateAnAccountResponse, _response.json())  # type: ignore
+        if _response.status_code == 409:
+            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def approve(
+    async def consolidate_into_an_account(
         self,
-        inquiry_id: str,
+        account_id: str,
         *,
-        meta: typing.Optional[InquiriesApproveRequestMeta] = OMIT,
+        meta: typing.Optional[ConsolidateIntoAnAccountRequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesApproveResponse:
+    ) -> None:
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/approve"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/consolidate"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesApproveResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(
+                pydantic.parse_obj_as(UnprocessableEntityErrorBody, _response.json())  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def decline(
+    async def add_a_tag_1(
         self,
-        inquiry_id: str,
+        account_id: str,
         *,
-        meta: typing.Optional[InquiriesDeclineRequestMeta] = OMIT,
+        meta: typing.Optional[AddATag1RequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesDeclineResponse:
+    ) -> None:
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/decline"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/add-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesDeclineResponse, _response.json())  # type: ignore
-        if _response.status_code == 409:
-            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list_all(
+    async def remove_a_tag_1(
         self,
+        account_id: str,
         *,
-        page_after: typing.Optional[str] = None,
-        page_before: typing.Optional[str] = None,
-        page_size: typing.Optional[str] = None,
-        filter_account_id: typing.Optional[str] = None,
-        filter_reference_id: typing.Optional[str] = None,
+        meta: typing.Optional[RemoveATag1RequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
-    ) -> InquiriesListAllResponse:
+        idempotency_key: typing.Optional[str] = None,
+    ) -> None:
+        _request: typing.Dict[str, typing.Any] = {}
+        if meta is not OMIT:
+            _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "inquiries"),
-                params={
-                    "page[after]": page_after,
-                    "page[before]": page_before,
-                    "page[size]": page_size,
-                    "filter[account-id]": filter_account_id,
-                    "filter[reference-id]": filter_reference_id,
-                },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/remove-tag"),
+                json=jsonable_encoder(_request),
+                headers=remove_none_from_headers(
+                    {
+                        "Key-Inflection": key_inflection,
+                        "Idempotency-Key": idempotency_key,
+                        "Authorization": self.api_key,
+                    }
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesListAllResponse, _response.json())  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(
+    async def set_all_tags_1(
         self,
+        account_id: str,
         *,
-        data: InquiriesCreateRequestData,
+        meta: typing.Optional[SetAllTags1RequestMeta] = OMIT,
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
-    ) -> InquiriesCreateResponse:
+    ) -> None:
+        _request: typing.Dict[str, typing.Any] = {}
+        if meta is not OMIT:
+            _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "inquiries"),
-                json=jsonable_encoder({"data": data}),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/set-tags"),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
                         "Authorization": self.api_key,
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InquiriesCreateResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+            return
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def print_an_inquiry_pdf(self, inquiry_id: str) -> None:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/print"),
+                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/reports/client.py` & `fern_persona-0.0.2/src/persona/resources/user_audit_logs/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,83 +6,107 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import PersonaEnvironment
-from ...types.reports_redact_response import ReportsRedactResponse
-from ...types.reports_retrieve_response import ReportsRetrieveResponse
+from ...errors.not_found_error import NotFoundError
+from ...types.retrieve_an_user_audit_log_response import RetrieveAnUserAuditLogResponse
 
 
-class ReportsClient:
+class UserAuditLogsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def retrieve(self, report_id: str, *, key_inflection: typing.Optional[str] = None) -> ReportsRetrieveResponse:
+    def list_all_user_audit_logs(
+        self,
+        *,
+        page_before: typing.Optional[str] = None,
+        page_after: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        key_inflection: typing.Optional[str] = None,
+    ) -> None:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "user-audit-logs"),
+            params={"page[before]": page_before, "page[after]": page_after, "page[size]": page_size},
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ReportsRetrieveResponse, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def redact(self, report_id: str, *, persona_version: typing.Optional[str] = None) -> ReportsRedactResponse:
+    def retrieve_an_user_audit_log(
+        self, user_audit_log_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnUserAuditLogResponse:
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
-            headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+            "GET",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"user-audit-logs/{user_audit_log_id}"),
+            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ReportsRedactResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnUserAuditLogResponse, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncReportsClient:
+class AsyncUserAuditLogsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def retrieve(self, report_id: str, *, key_inflection: typing.Optional[str] = None) -> ReportsRetrieveResponse:
+    async def list_all_user_audit_logs(
+        self,
+        *,
+        page_before: typing.Optional[str] = None,
+        page_after: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        key_inflection: typing.Optional[str] = None,
+    ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "user-audit-logs"),
+                params={"page[before]": page_before, "page[after]": page_after, "page[size]": page_size},
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ReportsRetrieveResponse, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def redact(self, report_id: str, *, persona_version: typing.Optional[str] = None) -> ReportsRedactResponse:
+    async def retrieve_an_user_audit_log(
+        self, user_audit_log_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> RetrieveAnUserAuditLogResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
-                headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+                "GET",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"user-audit-logs/{user_audit_log_id}"),
+                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ReportsRedactResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RetrieveAnUserAuditLogResponse, _response.json())  # type: ignore
+        if _response.status_code == 404:
+            raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `fern_persona-0.0.1/src/persona/resources/verifications/client.py` & `fern_persona-0.0.2/src/persona/resources/verifications/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class VerificationsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def retrieve(self, verification_id: str, *, key_inflection: typing.Optional[str] = None) -> None:
+    def retrieve_a_verification(self, verification_id: str, *, key_inflection: typing.Optional[str] = None) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/{verification_id}"),
             headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -33,15 +33,17 @@
 
 
 class AsyncVerificationsClient:
     def __init__(self, *, environment: PersonaEnvironment = PersonaEnvironment.DEFAULT, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def retrieve(self, verification_id: str, *, key_inflection: typing.Optional[str] = None) -> None:
+    async def retrieve_a_verification(
+        self, verification_id: str, *, key_inflection: typing.Optional[str] = None
+    ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/{verification_id}"),
                 headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
                 timeout=60,
             )
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_consolidate_request_meta.py` & `fern_persona-0.0.2/src/persona/types/consolidate_into_an_account_request_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsConsolidateRequestMeta(pydantic.BaseModel):
+class ConsolidateIntoAnAccountRequestMeta(pydantic.BaseModel):
     source_account_ids: typing.Optional[typing.List[str]] = pydantic.Field(
         alias="source-account-ids",
         description=("A list of Account IDs that need to be consolidated into the destination Account.\n"),
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_request_data.py` & `fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_create_request_data_attributes import AccountsCreateRequestDataAttributes
+from .dismiss_matches_request_data_attributes import DismissMatchesRequestDataAttributes
 
 
-class AccountsCreateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[AccountsCreateRequestDataAttributes]
+class DismissMatchesRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[DismissMatchesRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_create_request_data_attributes_selfie_photo import AccountsCreateRequestDataAttributesSelfiePhoto
+from .create_an_account_request_data_attributes_selfie_photo import CreateAnAccountRequestDataAttributesSelfiePhoto
 
 
-class AccountsCreateRequestDataAttributes(pydantic.BaseModel):
+class CreateAnAccountRequestDataAttributes(pydantic.BaseModel):
     reference_id: typing.Optional[str] = pydantic.Field(
         alias="reference-id", description=("Reference ID on Account, refers to an entity in your user model\n")
     )
     name_first: typing.Optional[str] = pydantic.Field(alias="name-first", description=("Given or first name.\n"))
     name_middle: typing.Optional[str] = pydantic.Field(alias="name-middle", description=("Middle name.\n"))
     name_last: typing.Optional[str] = pydantic.Field(alias="name-last", description=("Family or last name.\n"))
     birthdate: typing.Optional[str] = pydantic.Field(description=('Birthdate, must be in the format "YYYY-MM-DD".\n'))
@@ -47,15 +47,15 @@
     phone_number: typing.Optional[str] = pydantic.Field(alias="phone-number", description=("Phone number.\n"))
     social_security_number: typing.Optional[str] = pydantic.Field(
         alias="social-security-number", description=("Social security number.\n")
     )
     tags: typing.Optional[typing.List[str]] = pydantic.Field(
         description=("A list of tag names that are associated to an Account.\n")
     )
-    selfie_photo: typing.Optional[AccountsCreateRequestDataAttributesSelfiePhoto] = pydantic.Field(
+    selfie_photo: typing.Optional[CreateAnAccountRequestDataAttributesSelfiePhoto] = pydantic.Field(
         alias="selfie-photo", description=("Selfie photo.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_request_data_attributes_selfie_photo.py` & `fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_create_request_data_attributes_selfie_photo_data import (
-    AccountsCreateRequestDataAttributesSelfiePhotoData,
+from .update_an_account_request_data_attributes_selfie_photo_data import (
+    UpdateAnAccountRequestDataAttributesSelfiePhotoData,
 )
 
 
-class AccountsCreateRequestDataAttributesSelfiePhoto(pydantic.BaseModel):
+class UpdateAnAccountRequestDataAttributesSelfiePhoto(pydantic.BaseModel):
     """
     Selfie photo.
     """
 
-    data: typing.Optional[AccountsCreateRequestDataAttributesSelfiePhotoData] = pydantic.Field(
+    data: typing.Optional[UpdateAnAccountRequestDataAttributesSelfiePhotoData] = pydantic.Field(
         description=(
             "Selfie photo data, must be an image. Can also be provided as an uploaded file such as with multipart/form-data requests instead of this object.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_request_data_attributes_selfie_photo_data.py` & `fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsCreateRequestDataAttributesSelfiePhotoData(pydantic.BaseModel):
+class CreateAnAccountRequestDataAttributesSelfiePhotoData(pydantic.BaseModel):
     """
     Selfie photo data, must be an image. Can also be provided as an uploaded file such as with multipart/form-data requests instead of this object.
     """
 
     data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded image\n"))
     filename: typing.Optional[str] = pydantic.Field(description=("Name of the image\n"))
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_response.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_create_response_data import AccountsCreateResponseData
+from .create_an_inquiry_response_data import CreateAnInquiryResponseData
 
 
-class AccountsCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[AccountsCreateResponseData]
+class CreateAnInquiryResponse(pydantic.BaseModel):
+    data: typing.Optional[CreateAnInquiryResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_create_response_data_attributes import AccountsCreateResponseDataAttributes
+from .list_all_accounts_response_data_item_attributes import ListAllAccountsResponseDataItemAttributes
 
 
-class AccountsCreateResponseData(pydantic.BaseModel):
+class ListAllAccountsResponseDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[AccountsCreateResponseDataAttributes]
+    attributes: typing.Optional[ListAllAccountsResponseDataItemAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsCreateResponseDataAttributes(pydantic.BaseModel):
-    reference_id: typing.Optional[str] = pydantic.Field(alias="reference-id")
+class ListAllAccountsResponseDataItemAttributes(pydantic.BaseModel):
+    reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_list_all_response.py` & `fern_persona-0.0.2/src/persona/types/list_all_accounts_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_list_all_response_data_item import AccountsListAllResponseDataItem
-from .accounts_list_all_response_links import AccountsListAllResponseLinks
+from .list_all_accounts_response_data_item import ListAllAccountsResponseDataItem
+from .list_all_accounts_response_links import ListAllAccountsResponseLinks
 
 
-class AccountsListAllResponse(pydantic.BaseModel):
-    data: typing.Optional[typing.List[AccountsListAllResponseDataItem]]
-    links: typing.Optional[AccountsListAllResponseLinks]
+class ListAllAccountsResponse(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ListAllAccountsResponseDataItem]]
+    links: typing.Optional[ListAllAccountsResponseLinks]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_list_all_response_data_item.py` & `fern_persona-0.0.2/src/persona/types/redact_an_account_response_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_list_all_response_data_item_attributes import AccountsListAllResponseDataItemAttributes
+from .redact_an_account_response_data_attributes import RedactAnAccountResponseDataAttributes
 
 
-class AccountsListAllResponseDataItem(pydantic.BaseModel):
+class RedactAnAccountResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[AccountsListAllResponseDataItemAttributes]
+    attributes: typing.Optional[RedactAnAccountResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_list_all_response_data_item_attributes.py` & `fern_persona-0.0.2/src/persona/types/update_an_account_response_data_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsListAllResponseDataItemAttributes(pydantic.BaseModel):
-    reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
+class UpdateAnAccountResponseDataAttributes(pydantic.BaseModel):
+    reference_id: typing.Optional[str] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
+    tags: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_list_all_response_links.py` & `fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_links.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsListAllResponseLinks(pydantic.BaseModel):
+class ListAllApiKeysResponseLinks(pydantic.BaseModel):
     prev: typing.Optional[typing.Any]
-    next: typing.Optional[str]
+    next: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_redact_response.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_redact_response_data import AccountsRedactResponseData
 
 
-class AccountsRedactResponse(pydantic.BaseModel):
-    data: typing.Optional[AccountsRedactResponseData]
+class ApproveAnInquiryResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_redact_response_data.py` & `fern_persona-0.0.2/src/persona/types/update_an_account_response_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_redact_response_data_attributes import AccountsRedactResponseDataAttributes
+from .update_an_account_response_data_attributes import UpdateAnAccountResponseDataAttributes
 
 
-class AccountsRedactResponseData(pydantic.BaseModel):
+class UpdateAnAccountResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[AccountsRedactResponseDataAttributes]
+    attributes: typing.Optional[UpdateAnAccountResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_redact_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/redact_an_account_response_data_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsRedactResponseDataAttributes(pydantic.BaseModel):
+class RedactAnAccountResponseDataAttributes(pydantic.BaseModel):
     reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
     name_first: typing.Optional[typing.Any] = pydantic.Field(alias="name-first")
     name_middle: typing.Optional[typing.Any] = pydantic.Field(alias="name-middle")
     name_last: typing.Optional[typing.Any] = pydantic.Field(alias="name-last")
     address_street_1: typing.Optional[typing.Any] = pydantic.Field(alias="address-street-1")
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_retrieve_response_data import AccountsRetrieveResponseData
+from .expire_an_inquiry_response_data import ExpireAnInquiryResponseData
 
 
-class AccountsRetrieveResponse(pydantic.BaseModel):
-    data: typing.Optional[AccountsRetrieveResponseData]
+class ExpireAnInquiryResponse(pydantic.BaseModel):
+    data: typing.Optional[ExpireAnInquiryResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_retrieve_response_data.py` & `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_retrieve_response_data_attributes import AccountsRetrieveResponseDataAttributes
 
 
-class AccountsRetrieveResponseData(pydantic.BaseModel):
+class UpdateAGovernmentIdVerificationResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[AccountsRetrieveResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_retrieve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsRetrieveResponseDataAttributes(pydantic.BaseModel):
-    reference_id: typing.Optional[str] = pydantic.Field(alias="reference-id")
+class RetrieveAnUserAuditLogResponseDataAttributes(pydantic.BaseModel):
+    method: typing.Optional[str]
+    path: typing.Optional[str]
+    ip_address: typing.Optional[str] = pydantic.Field(alias="ip-address")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_request_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_report_request_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_update_request_data_attributes import AccountsUpdateRequestDataAttributes
+from .create_a_report_request_data_attributes import CreateAReportRequestDataAttributes
 
 
-class AccountsUpdateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[AccountsUpdateRequestDataAttributes]
+class CreateAReportRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[CreateAReportRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_update_request_data_attributes_selfie_photo import AccountsUpdateRequestDataAttributesSelfiePhoto
+from .update_an_account_request_data_attributes_selfie_photo import UpdateAnAccountRequestDataAttributesSelfiePhoto
 
 
-class AccountsUpdateRequestDataAttributes(pydantic.BaseModel):
+class UpdateAnAccountRequestDataAttributes(pydantic.BaseModel):
     reference_id: typing.Optional[str] = pydantic.Field(
         alias="reference-id", description=("Reference ID on Account, refers to an entity in your user model.\n")
     )
     name_first: typing.Optional[str] = pydantic.Field(alias="name-first", description=("Given or first name.\n"))
     name_middle: typing.Optional[str] = pydantic.Field(alias="name-middle", description=("Middle name.\n"))
     name_last: typing.Optional[str] = pydantic.Field(alias="name-last", description=("Family or last name.\n"))
     birthdate: typing.Optional[str] = pydantic.Field(description=('Birthdate, must be in the format "YYYY-MM-DD".\n'))
@@ -47,15 +47,15 @@
     phone_number: typing.Optional[str] = pydantic.Field(alias="phone-number", description=("Phone number.\n"))
     social_security_number: typing.Optional[str] = pydantic.Field(
         alias="social-security-number", description=("Social security number.\n")
     )
     tags: typing.Optional[typing.List[str]] = pydantic.Field(
         description=("A list of tag names that are associated to an Account.\n")
     )
-    selfie_photo: typing.Optional[AccountsUpdateRequestDataAttributesSelfiePhoto] = pydantic.Field(
+    selfie_photo: typing.Optional[UpdateAnAccountRequestDataAttributesSelfiePhoto] = pydantic.Field(
         alias="selfie-photo", description=("Selfie photo.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_request_data_attributes_selfie_photo.py` & `fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes_image_files_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_update_request_data_attributes_selfie_photo_data import (
-    AccountsUpdateRequestDataAttributesSelfiePhotoData,
-)
 
 
-class AccountsUpdateRequestDataAttributesSelfiePhoto(pydantic.BaseModel):
-    """
-    Selfie photo.
-    """
-
-    data: typing.Optional[AccountsUpdateRequestDataAttributesSelfiePhotoData] = pydantic.Field(
-        description=(
-            "Selfie photo data, must be an image. Can also be provided as an uploaded file such as with multipart/form-data requests instead of this object.\n"
-        )
-    )
+class ImportFaceListsRequestDataAttributesImageFilesItem(pydantic.BaseModel):
+    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
+    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_request_data_attributes_selfie_photo_data.py` & `fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsUpdateRequestDataAttributesSelfiePhotoData(pydantic.BaseModel):
-    """
-    Selfie photo data, must be an image. Can also be provided as an uploaded file such as with multipart/form-data requests instead of this object.
-    """
-
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded image\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of the image\n"))
+class ImportEmailAddressListsRequestDataAttributesFile(pydantic.BaseModel):
+    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
+    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_response.py` & `fern_persona-0.0.2/src/persona/types/create_a_name_list_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_update_response_data import AccountsUpdateResponseData
 
 
-class AccountsUpdateResponse(pydantic.BaseModel):
-    data: typing.Optional[AccountsUpdateResponseData]
-
+class CreateANameListResponse(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes_files_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .accounts_update_response_data_attributes import AccountsUpdateResponseDataAttributes
 
 
-class AccountsUpdateResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[AccountsUpdateResponseDataAttributes]
+class CreateADocumentResponseDataAttributesFilesItem(pydantic.BaseModel):
+    filename: typing.Optional[str]
+    url: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/accounts_update_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsUpdateResponseDataAttributes(pydantic.BaseModel):
-    reference_id: typing.Optional[str] = pydantic.Field(alias="reference-id")
+class CreateAWorkflowRunResponseDataAttributes(pydantic.BaseModel):
+    status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
-    tags: typing.Optional[typing.List[typing.Any]]
+    completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .api_logs_retrieve_response_data import ApiLogsRetrieveResponseData
+from .retrieve_an_api_log_response_data import RetrieveAnApiLogResponseData
 
 
-class ApiLogsRetrieveResponse(pydantic.BaseModel):
-    data: typing.Optional[ApiLogsRetrieveResponseData]
+class RetrieveAnApiLogResponse(pydantic.BaseModel):
+    data: typing.Optional[RetrieveAnApiLogResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .api_logs_retrieve_response_data_attributes import ApiLogsRetrieveResponseDataAttributes
+from .retrieve_an_api_key_response_data_attributes import RetrieveAnApiKeyResponseDataAttributes
 
 
-class ApiLogsRetrieveResponseData(pydantic.BaseModel):
+class RetrieveAnApiKeyResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ApiLogsRetrieveResponseDataAttributes]
+    attributes: typing.Optional[RetrieveAnApiKeyResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_attributes.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .api_logs_retrieve_response_data_attributes_request import ApiLogsRetrieveResponseDataAttributesRequest
-from .api_logs_retrieve_response_data_attributes_response import ApiLogsRetrieveResponseDataAttributesResponse
 
 
-class ApiLogsRetrieveResponseDataAttributes(pydantic.BaseModel):
-    request: typing.Optional[ApiLogsRetrieveResponseDataAttributesRequest]
-    response: typing.Optional[ApiLogsRetrieveResponseDataAttributesResponse]
+class ListAllInquiriesResponseDataItemAttributes(pydantic.BaseModel):
+    status: typing.Optional[str]
+    subject: typing.Optional[typing.Any]
+    reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
+    completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
+    expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .api_logs_retrieve_response_data_attributes_request_get_params import (
-    ApiLogsRetrieveResponseDataAttributesRequestGetParams,
+from .retrieve_an_api_log_response_data_attributes_request_get_params import (
+    RetrieveAnApiLogResponseDataAttributesRequestGetParams,
 )
-from .api_logs_retrieve_response_data_attributes_request_headers import (
-    ApiLogsRetrieveResponseDataAttributesRequestHeaders,
+from .retrieve_an_api_log_response_data_attributes_request_headers import (
+    RetrieveAnApiLogResponseDataAttributesRequestHeaders,
 )
-from .api_logs_retrieve_response_data_attributes_request_post_params import (
-    ApiLogsRetrieveResponseDataAttributesRequestPostParams,
+from .retrieve_an_api_log_response_data_attributes_request_post_params import (
+    RetrieveAnApiLogResponseDataAttributesRequestPostParams,
 )
 
 
-class ApiLogsRetrieveResponseDataAttributesRequest(pydantic.BaseModel):
+class RetrieveAnApiLogResponseDataAttributesRequest(pydantic.BaseModel):
     method: typing.Optional[str]
     path: typing.Optional[str]
-    headers: typing.Optional[ApiLogsRetrieveResponseDataAttributesRequestHeaders]
-    get_params: typing.Optional[ApiLogsRetrieveResponseDataAttributesRequestGetParams] = pydantic.Field(
+    headers: typing.Optional[RetrieveAnApiLogResponseDataAttributesRequestHeaders]
+    get_params: typing.Optional[RetrieveAnApiLogResponseDataAttributesRequestGetParams] = pydantic.Field(
         alias="get-params"
     )
-    post_params: typing.Optional[ApiLogsRetrieveResponseDataAttributesRequestPostParams] = pydantic.Field(
+    post_params: typing.Optional[RetrieveAnApiLogResponseDataAttributesRequestPostParams] = pydantic.Field(
         alias="post-params"
     )
     ip_address: typing.Optional[str] = pydantic.Field(alias="ip-address")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_get_params.py` & `fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .api_logs_retrieve_response_data_attributes_request_get_params_filter import (
-    ApiLogsRetrieveResponseDataAttributesRequestGetParamsFilter,
-)
 
 
-class ApiLogsRetrieveResponseDataAttributesRequestGetParams(pydantic.BaseModel):
-    filter: typing.Optional[ApiLogsRetrieveResponseDataAttributesRequestGetParamsFilter]
-
+class SendAnEmailResponseDataAttributesMetadata(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_get_params_filter.py` & `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes_files_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ApiLogsRetrieveResponseDataAttributesRequestGetParamsFilter(pydantic.BaseModel):
-    reference_id: typing.Optional[str]
+class UpdateADocumentResponseDataAttributesFilesItem(pydantic.BaseModel):
+    filename: typing.Optional[str]
+    url: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_headers.py` & `fern_persona-0.0.2/src/persona/types/set_all_tags_1_request_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ApiLogsRetrieveResponseDataAttributesRequestHeaders(pydantic.BaseModel):
-    authorization: typing.Optional[str] = pydantic.Field(alias="Authorization")
+class SetAllTags1RequestMeta(pydantic.BaseModel):
+    tag_name: typing.Optional[typing.List[str]] = pydantic.Field(alias="tag-name")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_request_post_params.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ApiLogsRetrieveResponseDataAttributesRequestPostParams(pydantic.BaseModel):
+class CreateAPhoneNumberVerificationResponseDataAttributesMetadata(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_response.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .api_logs_retrieve_response_data_attributes_response_headers import (
-    ApiLogsRetrieveResponseDataAttributesResponseHeaders,
-)
+from .retrieve_an_api_log_response_data_attributes import RetrieveAnApiLogResponseDataAttributes
 
 
-class ApiLogsRetrieveResponseDataAttributesResponse(pydantic.BaseModel):
-    status: typing.Optional[int]
-    headers: typing.Optional[ApiLogsRetrieveResponseDataAttributesResponseHeaders]
-    body: typing.Optional[typing.List[typing.Any]]
+class RetrieveAnApiLogResponseData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
+    attributes: typing.Optional[RetrieveAnApiLogResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/api_logs_retrieve_response_data_attributes_response_headers.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ApiLogsRetrieveResponseDataAttributesResponseHeaders(pydantic.BaseModel):
+class RetrieveAnApiLogResponseDataAttributesResponseHeaders(pydantic.BaseModel):
     request_id: typing.Optional[str] = pydantic.Field(alias="Request-Id")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/database_verifications_create_response.py` & `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .database_verifications_create_response_data import DatabaseVerificationsCreateResponseData
 
 
-class DatabaseVerificationsCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[DatabaseVerificationsCreateResponseData]
+class DeclineAnInquiryResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .database_verifications_create_response_data_attributes import DatabaseVerificationsCreateResponseDataAttributes
-from .database_verifications_create_response_data_relationships import (
-    DatabaseVerificationsCreateResponseDataRelationships,
+from .create_a_phone_carrier_database_verification_response_data_attributes import (
+    CreateAPhoneCarrierDatabaseVerificationResponseDataAttributes,
+)
+from .create_a_phone_carrier_database_verification_response_data_relationships import (
+    CreateAPhoneCarrierDatabaseVerificationResponseDataRelationships,
 )
 
 
-class DatabaseVerificationsCreateResponseData(pydantic.BaseModel):
+class CreateAPhoneCarrierDatabaseVerificationResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[DatabaseVerificationsCreateResponseDataAttributes]
-    relationships: typing.Optional[DatabaseVerificationsCreateResponseDataRelationships]
+    attributes: typing.Optional[CreateAPhoneCarrierDatabaseVerificationResponseDataAttributes]
+    relationships: typing.Optional[CreateAPhoneCarrierDatabaseVerificationResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DatabaseVerificationsCreateResponseDataAttributes(pydantic.BaseModel):
+class CreateADatabaseVerificationResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     created_at_ts: typing.Optional[int] = pydantic.Field(alias="created-at-ts")
     submitted_at: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at")
     submitted_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at-ts")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     completed_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at-ts")
```

### Comparing `fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .database_verifications_create_response_data_relationships_inquiry import (
-    DatabaseVerificationsCreateResponseDataRelationshipsInquiry,
+from .create_a_phone_carrier_database_verification_response_data_relationships_inquiry import (
+    CreateAPhoneCarrierDatabaseVerificationResponseDataRelationshipsInquiry,
 )
 
 
-class DatabaseVerificationsCreateResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DatabaseVerificationsCreateResponseDataRelationshipsInquiry]
+class CreateAPhoneCarrierDatabaseVerificationResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[CreateAPhoneCarrierDatabaseVerificationResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/database_verifications_create_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships_inquiry.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DatabaseVerificationsCreateResponseDataRelationshipsInquiry(pydantic.BaseModel):
+class CreateASelfieVerificationResponseDataRelationshipsInquiry(pydantic.BaseModel):
     data: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_request_data.py` & `fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_create_request_data_attributes import DocumentVerificationsCreateRequestDataAttributes
+from .update_an_api_key_request_data_attributes import UpdateAnApiKeyRequestDataAttributes
 
 
-class DocumentVerificationsCreateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[DocumentVerificationsCreateRequestDataAttributes]
+class UpdateAnApiKeyRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[UpdateAnApiKeyRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data_attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsCreateRequestDataAttributes(pydantic.BaseModel):
-    inquiry_id: str = pydantic.Field(alias="inquiry-id")
-    document_id: str = pydantic.Field(alias="document-id", description=("ID of the document to verify\n"))
+class CreateANameListRequestDataAttributes(pydantic.BaseModel):
+    name: typing.Optional[str] = pydantic.Field(description=("Name of the list\n"))
+    allow_fuzzy_name_first: typing.Optional[bool] = pydantic.Field(
+        alias="allow-fuzzy-name-first",
+        description=("Flag to determine if the list should use fuzzy matching for first name\n"),
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_create_response_data import DocumentVerificationsCreateResponseData
+from .create_a_document_verification_response_data import CreateADocumentVerificationResponseData
 
 
-class DocumentVerificationsCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[DocumentVerificationsCreateResponseData]
+class CreateADocumentVerificationResponse(pydantic.BaseModel):
+    data: typing.Optional[CreateADocumentVerificationResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_create_response_data_attributes import DocumentVerificationsCreateResponseDataAttributes
-from .document_verifications_create_response_data_relationships import (
-    DocumentVerificationsCreateResponseDataRelationships,
+from .create_a_gov_id_verification_response_data_relationships_document_data import (
+    CreateAGovIdVerificationResponseDataRelationshipsDocumentData,
 )
 
 
-class DocumentVerificationsCreateResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[DocumentVerificationsCreateResponseDataAttributes]
-    relationships: typing.Optional[DocumentVerificationsCreateResponseDataRelationships]
+class CreateAGovIdVerificationResponseDataRelationshipsDocument(pydantic.BaseModel):
+    data: typing.Optional[CreateAGovIdVerificationResponseDataRelationshipsDocumentData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsCreateResponseDataAttributes(pydantic.BaseModel):
+class CreateADocumentVerificationResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     created_at_ts: typing.Optional[int] = pydantic.Field(alias="created-at-ts")
     submitted_at: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at")
     submitted_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at-ts")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     completed_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at-ts")
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_create_response_data_relationships_document import (
-    DocumentVerificationsCreateResponseDataRelationshipsDocument,
+from .create_a_document_verification_response_data_relationships_document import (
+    CreateADocumentVerificationResponseDataRelationshipsDocument,
 )
-from .document_verifications_create_response_data_relationships_inquiry import (
-    DocumentVerificationsCreateResponseDataRelationshipsInquiry,
+from .create_a_document_verification_response_data_relationships_inquiry import (
+    CreateADocumentVerificationResponseDataRelationshipsInquiry,
 )
 
 
-class DocumentVerificationsCreateResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DocumentVerificationsCreateResponseDataRelationshipsInquiry]
-    document: typing.Optional[DocumentVerificationsCreateResponseDataRelationshipsDocument]
+class CreateADocumentVerificationResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[CreateADocumentVerificationResponseDataRelationshipsInquiry]
+    document: typing.Optional[CreateADocumentVerificationResponseDataRelationshipsDocument]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_document.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_create_response_data_relationships_document_data import (
-    DocumentVerificationsCreateResponseDataRelationshipsDocumentData,
+from .submit_a_document_verification_response_data_relationships_inquiry_data import (
+    SubmitADocumentVerificationResponseDataRelationshipsInquiryData,
 )
 
 
-class DocumentVerificationsCreateResponseDataRelationshipsDocument(pydantic.BaseModel):
-    data: typing.Optional[DocumentVerificationsCreateResponseDataRelationshipsDocumentData]
+class SubmitADocumentVerificationResponseDataRelationshipsInquiry(pydantic.BaseModel):
+    data: typing.Optional[SubmitADocumentVerificationResponseDataRelationshipsInquiryData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_document_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsCreateResponseDataRelationshipsDocumentData(pydantic.BaseModel):
+class CreateADocumentVerificationResponseDataRelationshipsDocumentData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_create_response_data_relationships_inquiry_data import (
-    DocumentVerificationsCreateResponseDataRelationshipsInquiryData,
+from .create_a_database_verification_1_response_data_relationships_inquiry import (
+    CreateADatabaseVerification1ResponseDataRelationshipsInquiry,
 )
 
 
-class DocumentVerificationsCreateResponseDataRelationshipsInquiry(pydantic.BaseModel):
-    data: typing.Optional[DocumentVerificationsCreateResponseDataRelationshipsInquiryData]
+class CreateADatabaseVerification1ResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[CreateADatabaseVerification1ResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_create_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsCreateResponseDataRelationshipsInquiryData(pydantic.BaseModel):
+class CreateADocumentVerificationResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_submit_response_data import DocumentVerificationsSubmitResponseData
+from .submit_a_document_verification_response_data import SubmitADocumentVerificationResponseData
 
 
-class DocumentVerificationsSubmitResponse(pydantic.BaseModel):
-    data: typing.Optional[DocumentVerificationsSubmitResponseData]
+class SubmitADocumentVerificationResponse(pydantic.BaseModel):
+    data: typing.Optional[SubmitADocumentVerificationResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_submit_response_data_attributes import DocumentVerificationsSubmitResponseDataAttributes
-from .document_verifications_submit_response_data_relationships import (
-    DocumentVerificationsSubmitResponseDataRelationships,
-)
+from .submit_a_document_response_data_attributes import SubmitADocumentResponseDataAttributes
+from .submit_a_document_response_data_relationships import SubmitADocumentResponseDataRelationships
 
 
-class DocumentVerificationsSubmitResponseData(pydantic.BaseModel):
+class SubmitADocumentResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[DocumentVerificationsSubmitResponseDataAttributes]
-    relationships: typing.Optional[DocumentVerificationsSubmitResponseDataRelationships]
+    attributes: typing.Optional[SubmitADocumentResponseDataAttributes]
+    relationships: typing.Optional[SubmitADocumentResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_attributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsSubmitResponseDataAttributes(pydantic.BaseModel):
+class SubmitAPhoneCarrierDatabaseVerificationResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     created_at_ts: typing.Optional[int] = pydantic.Field(alias="created-at-ts")
     submitted_at: typing.Optional[str] = pydantic.Field(alias="submitted-at")
     submitted_at_ts: typing.Optional[int] = pydantic.Field(alias="submitted-at-ts")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     completed_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at-ts")
-    country_code: typing.Optional[typing.Any] = pydantic.Field(alias="country-code")
+    country_code: typing.Optional[str] = pydantic.Field(alias="country-code")
+    name_first: typing.Optional[str] = pydantic.Field(alias="name-first")
+    checks: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_submit_response_data_relationships_document import (
-    DocumentVerificationsSubmitResponseDataRelationshipsDocument,
+from .submit_a_document_verification_response_data_relationships_document import (
+    SubmitADocumentVerificationResponseDataRelationshipsDocument,
 )
-from .document_verifications_submit_response_data_relationships_inquiry import (
-    DocumentVerificationsSubmitResponseDataRelationshipsInquiry,
+from .submit_a_document_verification_response_data_relationships_inquiry import (
+    SubmitADocumentVerificationResponseDataRelationshipsInquiry,
 )
 
 
-class DocumentVerificationsSubmitResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DocumentVerificationsSubmitResponseDataRelationshipsInquiry]
-    document: typing.Optional[DocumentVerificationsSubmitResponseDataRelationshipsDocument]
+class SubmitADocumentVerificationResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[SubmitADocumentVerificationResponseDataRelationshipsInquiry]
+    document: typing.Optional[SubmitADocumentVerificationResponseDataRelationshipsDocument]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_document.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_submit_response_data_relationships_document_data import (
-    DocumentVerificationsSubmitResponseDataRelationshipsDocumentData,
+from .submit_a_document_verification_response_data_relationships_document_data import (
+    SubmitADocumentVerificationResponseDataRelationshipsDocumentData,
 )
 
 
-class DocumentVerificationsSubmitResponseDataRelationshipsDocument(pydantic.BaseModel):
-    data: typing.Optional[DocumentVerificationsSubmitResponseDataRelationshipsDocumentData]
+class SubmitADocumentVerificationResponseDataRelationshipsDocument(pydantic.BaseModel):
+    data: typing.Optional[SubmitADocumentVerificationResponseDataRelationshipsDocumentData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_document_data.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsSubmitResponseDataRelationshipsDocumentData(pydantic.BaseModel):
+class SubmitADocumentVerificationResponseDataRelationshipsDocumentData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_verifications_submit_response_data_relationships_inquiry_data import (
-    DocumentVerificationsSubmitResponseDataRelationshipsInquiryData,
+from .create_a_database_verification_response_data_relationships_inquiry import (
+    CreateADatabaseVerificationResponseDataRelationshipsInquiry,
 )
 
 
-class DocumentVerificationsSubmitResponseDataRelationshipsInquiry(pydantic.BaseModel):
-    data: typing.Optional[DocumentVerificationsSubmitResponseDataRelationshipsInquiryData]
+class CreateADatabaseVerificationResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[CreateADatabaseVerificationResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/document_verifications_submit_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentVerificationsSubmitResponseDataRelationshipsInquiryData(pydantic.BaseModel):
+class SubmitADocumentVerificationResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_request_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_create_request_data_attributes import DocumentsCreateRequestDataAttributes
+from .create_a_name_list_request_data_attributes import CreateANameListRequestDataAttributes
 
 
-class DocumentsCreateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[DocumentsCreateRequestDataAttributes]
+class CreateANameListRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[CreateANameListRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/update_a_document_request_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsCreateRequestDataAttributes(pydantic.BaseModel):
-    inquiry_id: str = pydantic.Field(alias="inquiry-id")
-    kind: str = pydantic.Field(description=('Identifier for this document, e.g. "proof_of_employment"\n'))
+class UpdateADocumentRequestDataAttributes(pydantic.BaseModel):
+    kind: typing.Optional[str] = pydantic.Field(
+        description=('Identifier for this document, e.g. "proof_of_employment"\n')
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_create_response_data import DocumentsCreateResponseData
+from .create_a_document_response_data import CreateADocumentResponseData
 
 
-class DocumentsCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[DocumentsCreateResponseData]
+class CreateADocumentResponse(pydantic.BaseModel):
+    data: typing.Optional[CreateADocumentResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_create_response_data_attributes import DocumentsCreateResponseDataAttributes
-from .documents_create_response_data_relationships import DocumentsCreateResponseDataRelationships
+from .create_a_name_list_item_response_data_attributes import CreateANameListItemResponseDataAttributes
+from .create_a_name_list_item_response_data_relationships import CreateANameListItemResponseDataRelationships
 
 
-class DocumentsCreateResponseData(pydantic.BaseModel):
+class CreateANameListItemResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[DocumentsCreateResponseDataAttributes]
-    relationships: typing.Optional[DocumentsCreateResponseDataRelationships]
+    attributes: typing.Optional[CreateANameListItemResponseDataAttributes]
+    relationships: typing.Optional[CreateANameListItemResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_create_response_data_attributes_files_item import DocumentsCreateResponseDataAttributesFilesItem
 
 
-class DocumentsCreateResponseDataAttributes(pydantic.BaseModel):
-    kind: typing.Optional[str]
+class CreateABrowserFingerprintListItemResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
+    archived_at: typing.Optional[typing.Any] = pydantic.Field(alias="archived-at")
+    updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    processed_at: typing.Optional[typing.Any] = pydantic.Field(alias="processed-at")
-    files: typing.Optional[typing.List[DocumentsCreateResponseDataAttributesFilesItem]]
+    match_count: typing.Optional[int] = pydantic.Field(alias="match-count")
+    value: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response_data_attributes_files_item.py` & `fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsCreateResponseDataAttributesFilesItem(pydantic.BaseModel):
-    filename: typing.Optional[str]
-    url: typing.Optional[str]
+class ListAllCasesResponseDataItemRelationshipsCaseTemplateData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_create_response_data_relationships_inquiry import DocumentsCreateResponseDataRelationshipsInquiry
+from .submit_a_document_response_data_relationships_inquiry import SubmitADocumentResponseDataRelationshipsInquiry
 
 
-class DocumentsCreateResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DocumentsCreateResponseDataRelationshipsInquiry]
+class SubmitADocumentResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[SubmitADocumentResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_create_response_data_relationships_inquiry_data import (
-    DocumentsCreateResponseDataRelationshipsInquiryData,
-)
+from .create_a_document_response_data_relationships_inquiry import CreateADocumentResponseDataRelationshipsInquiry
 
 
-class DocumentsCreateResponseDataRelationshipsInquiry(pydantic.BaseModel):
-    data: typing.Optional[DocumentsCreateResponseDataRelationshipsInquiryData]
+class CreateADocumentResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[CreateADocumentResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_create_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsCreateResponseDataRelationshipsInquiryData(pydantic.BaseModel):
+class CreateADocumentResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_identifiers_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_retrieve_response_data import DocumentsRetrieveResponseData
 
 
-class DocumentsRetrieveResponse(pydantic.BaseModel):
-    data: typing.Optional[DocumentsRetrieveResponseData]
+class BusinessLookupReport1ResponseDataAttributesResultItemIdentifiersItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    value: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data.py` & `fern_persona-0.0.2/src/persona/types/update_a_document_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_retrieve_response_data_attributes import DocumentsRetrieveResponseDataAttributes
-from .documents_retrieve_response_data_relationships import DocumentsRetrieveResponseDataRelationships
+from .update_a_document_response_data_attributes import UpdateADocumentResponseDataAttributes
+from .update_a_document_response_data_relationships import UpdateADocumentResponseDataRelationships
 
 
-class DocumentsRetrieveResponseData(pydantic.BaseModel):
+class UpdateADocumentResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[DocumentsRetrieveResponseDataAttributes]
-    relationships: typing.Optional[DocumentsRetrieveResponseDataRelationships]
+    attributes: typing.Optional[UpdateADocumentResponseDataAttributes]
+    relationships: typing.Optional[UpdateADocumentResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_retrieve_response_data_attributes_files_item import DocumentsRetrieveResponseDataAttributesFilesItem
+from .retrieve_a_document_response_data_attributes_files_item import RetrieveADocumentResponseDataAttributesFilesItem
 
 
-class DocumentsRetrieveResponseDataAttributes(pydantic.BaseModel):
+class RetrieveADocumentResponseDataAttributes(pydantic.BaseModel):
     kind: typing.Optional[str]
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     processed_at: typing.Optional[str] = pydantic.Field(alias="processed-at")
-    files: typing.Optional[typing.List[DocumentsRetrieveResponseDataAttributesFilesItem]]
+    files: typing.Optional[typing.List[RetrieveADocumentResponseDataAttributesFilesItem]]
     document_type: typing.Optional[str] = pydantic.Field(alias="document-type")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_attributes_files_item.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions_data_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsRetrieveResponseDataAttributesFilesItem(pydantic.BaseModel):
-    filename: typing.Optional[str]
-    url: typing.Optional[str]
+class CreateACaseResponseIncludedItemRelationshipsSessionsDataItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_retrieve_response_data_relationships_inquiry import DocumentsRetrieveResponseDataRelationshipsInquiry
+from .submit_a_document_response_data_relationships_inquiry_data import (
+    SubmitADocumentResponseDataRelationshipsInquiryData,
+)
 
 
-class DocumentsRetrieveResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DocumentsRetrieveResponseDataRelationshipsInquiry]
+class SubmitADocumentResponseDataRelationshipsInquiry(pydantic.BaseModel):
+    data: typing.Optional[SubmitADocumentResponseDataRelationshipsInquiryData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_retrieve_response_data_relationships_inquiry_data import (
-    DocumentsRetrieveResponseDataRelationshipsInquiryData,
+from .retrieve_an_inquiry_response_data_relationships_sessions_data_item import (
+    RetrieveAnInquiryResponseDataRelationshipsSessionsDataItem,
 )
 
 
-class DocumentsRetrieveResponseDataRelationshipsInquiry(pydantic.BaseModel):
-    data: typing.Optional[DocumentsRetrieveResponseDataRelationshipsInquiryData]
+class RetrieveAnInquiryResponseDataRelationshipsSessions(pydantic.BaseModel):
+    data: typing.Optional[typing.List[RetrieveAnInquiryResponseDataRelationshipsSessionsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_retrieve_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsRetrieveResponseDataRelationshipsInquiryData(pydantic.BaseModel):
+class CreateAnInquiryResponseDataRelationshipsTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response.py` & `fern_persona-0.0.2/src/persona/types/create_a_face_list_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_submit_response_data import DocumentsSubmitResponseData
 
 
-class DocumentsSubmitResponse(pydantic.BaseModel):
-    data: typing.Optional[DocumentsSubmitResponseData]
-
+class CreateAFaceListResponse(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response_data.py` & `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_submit_response_data_attributes import DocumentsSubmitResponseDataAttributes
-from .documents_submit_response_data_relationships import DocumentsSubmitResponseDataRelationships
+from .retrieve_case_response_data_attributes import RetrieveCaseResponseDataAttributes
+from .retrieve_case_response_data_relationships import RetrieveCaseResponseDataRelationships
 
 
-class DocumentsSubmitResponseData(pydantic.BaseModel):
+class RetrieveCaseResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[DocumentsSubmitResponseDataAttributes]
-    relationships: typing.Optional[DocumentsSubmitResponseDataRelationships]
+    attributes: typing.Optional[RetrieveCaseResponseDataAttributes]
+    relationships: typing.Optional[RetrieveCaseResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_submit_response_data_attributes_files_item import DocumentsSubmitResponseDataAttributesFilesItem
+from .submit_a_document_response_data_attributes_files_item import SubmitADocumentResponseDataAttributesFilesItem
 
 
-class DocumentsSubmitResponseDataAttributes(pydantic.BaseModel):
+class SubmitADocumentResponseDataAttributes(pydantic.BaseModel):
     kind: typing.Optional[str]
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     processed_at: typing.Optional[typing.Any] = pydantic.Field(alias="processed-at")
-    files: typing.Optional[typing.List[DocumentsSubmitResponseDataAttributesFilesItem]]
+    files: typing.Optional[typing.List[SubmitADocumentResponseDataAttributesFilesItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response_data_attributes_files_item.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes_files_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsSubmitResponseDataAttributesFilesItem(pydantic.BaseModel):
+class RetrieveADocumentResponseDataAttributesFilesItem(pydantic.BaseModel):
     filename: typing.Optional[str]
     url: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_submit_response_data_relationships_inquiry import DocumentsSubmitResponseDataRelationshipsInquiry
+from .update_a_document_response_data_relationships_inquiry import UpdateADocumentResponseDataRelationshipsInquiry
 
 
-class DocumentsSubmitResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DocumentsSubmitResponseDataRelationshipsInquiry]
+class UpdateADocumentResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[UpdateADocumentResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_submit_response_data_relationships_inquiry_data import (
-    DocumentsSubmitResponseDataRelationshipsInquiryData,
+from .redact_an_inquiry_response_data_relationships_verifications_data_item import (
+    RedactAnInquiryResponseDataRelationshipsVerificationsDataItem,
 )
 
 
-class DocumentsSubmitResponseDataRelationshipsInquiry(pydantic.BaseModel):
-    data: typing.Optional[DocumentsSubmitResponseDataRelationshipsInquiryData]
+class RedactAnInquiryResponseDataRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[RedactAnInquiryResponseDataRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_submit_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsSubmitResponseDataRelationshipsInquiryData(pydantic.BaseModel):
+class SubmitADocumentResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_request_data.py` & `fern_persona-0.0.2/src/persona/types/update_a_document_request_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_update_request_data_attributes import DocumentsUpdateRequestDataAttributes
+from .update_a_document_request_data_attributes import UpdateADocumentRequestDataAttributes
 
 
-class DocumentsUpdateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[DocumentsUpdateRequestDataAttributes]
+class UpdateADocumentRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[UpdateADocumentRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_request_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsUpdateRequestDataAttributes(pydantic.BaseModel):
-    kind: typing.Optional[str] = pydantic.Field(
-        description=('Identifier for this document, e.g. "proof_of_employment"\n')
+class GenerateAOneTimeLinkRequestMeta(pydantic.BaseModel):
+    expires_in_seconds: typing.Optional[int] = pydantic.Field(
+        description=("Number of seconds from now to expire the key (minimum 0)\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response.py` & `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_update_response_data import DocumentsUpdateResponseData
 
 
-class DocumentsUpdateResponse(pydantic.BaseModel):
-    data: typing.Optional[DocumentsUpdateResponseData]
-
+class CreateABrowserFingerprintListResponse(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response_data.py` & `fern_persona-0.0.2/src/persona/types/update_a_case_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_update_response_data_attributes import DocumentsUpdateResponseDataAttributes
-from .documents_update_response_data_relationships import DocumentsUpdateResponseDataRelationships
+from .update_a_case_response_data_attributes import UpdateACaseResponseDataAttributes
+from .update_a_case_response_data_relationships import UpdateACaseResponseDataRelationships
 
 
-class DocumentsUpdateResponseData(pydantic.BaseModel):
+class UpdateACaseResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[DocumentsUpdateResponseDataAttributes]
-    relationships: typing.Optional[DocumentsUpdateResponseDataRelationships]
+    attributes: typing.Optional[UpdateACaseResponseDataAttributes]
+    relationships: typing.Optional[UpdateACaseResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_meta.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_update_response_data_attributes_files_item import DocumentsUpdateResponseDataAttributesFilesItem
 
 
-class DocumentsUpdateResponseDataAttributes(pydantic.BaseModel):
-    kind: typing.Optional[str]
-    status: typing.Optional[str]
-    created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    processed_at: typing.Optional[typing.Any] = pydantic.Field(alias="processed-at")
-    files: typing.Optional[typing.List[DocumentsUpdateResponseDataAttributesFilesItem]]
+class GenerateAOneTimeLinkResponseMeta(pydantic.BaseModel):
+    one_time_link: typing.Optional[str] = pydantic.Field(alias="one-time-link")
+    one_time_link_short: typing.Optional[str] = pydantic.Field(alias="one-time-link-short")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response_data_attributes_files_item.py` & `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports_data_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsUpdateResponseDataAttributesFilesItem(pydantic.BaseModel):
-    filename: typing.Optional[str]
-    url: typing.Optional[str]
+class AssignACaseResponseDataRelationshipsReportsDataItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_update_response_data_relationships_inquiry import DocumentsUpdateResponseDataRelationshipsInquiry
 
 
-class DocumentsUpdateResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[DocumentsUpdateResponseDataRelationshipsInquiry]
-
+class SendAnSmsResponseDataAttributesMetadata(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .documents_update_response_data_relationships_inquiry_data import (
-    DocumentsUpdateResponseDataRelationshipsInquiryData,
+from .assign_a_case_response_data_relationships_inquiries_data_item import (
+    AssignACaseResponseDataRelationshipsInquiriesDataItem,
 )
 
 
-class DocumentsUpdateResponseDataRelationshipsInquiry(pydantic.BaseModel):
-    data: typing.Optional[DocumentsUpdateResponseDataRelationshipsInquiryData]
+class AssignACaseResponseDataRelationshipsInquiries(pydantic.BaseModel):
+    data: typing.Optional[typing.List[AssignACaseResponseDataRelationshipsInquiriesDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/documents_update_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentsUpdateResponseDataRelationshipsInquiryData(pydantic.BaseModel):
+class UpdateADocumentResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/events_list_all_response.py` & `fern_persona-0.0.2/src/persona/types/list_all_events_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class EventsListAllResponse(pydantic.BaseModel):
+class ListAllEventsResponse(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/events_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/list_all_lists_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class EventsRetrieveResponse(pydantic.BaseModel):
+class ListAllListsResponse(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_request_data_attributes import (
-    GovernmentIdVerificationsCreateRequestDataAttributes,
-)
+from .create_a_phone_number_list_item_request_data_attributes import CreateAPhoneNumberListItemRequestDataAttributes
 
 
-class GovernmentIdVerificationsCreateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[GovernmentIdVerificationsCreateRequestDataAttributes]
+class CreateAPhoneNumberListItemRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[CreateAPhoneNumberListItemRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_request_data_attributes_back_photo import (
-    GovernmentIdVerificationsCreateRequestDataAttributesBackPhoto,
+from .create_a_gov_id_verification_request_data_attributes_back_photo import (
+    CreateAGovIdVerificationRequestDataAttributesBackPhoto,
 )
-from .government_id_verifications_create_request_data_attributes_front_photo import (
-    GovernmentIdVerificationsCreateRequestDataAttributesFrontPhoto,
+from .create_a_gov_id_verification_request_data_attributes_front_photo import (
+    CreateAGovIdVerificationRequestDataAttributesFrontPhoto,
 )
 
 
-class GovernmentIdVerificationsCreateRequestDataAttributes(pydantic.BaseModel):
+class CreateAGovIdVerificationRequestDataAttributes(pydantic.BaseModel):
     verification_template_id: str = pydantic.Field(
         alias="verification-template-id",
         description=(
             "ID of Verification Template. You can find your Verification Template IDs [here](https://app.withpersona.com/dashboard/verification-templates?filter=%7B%22type%22%3A%5B%22verification-template%2Fgovernment-id%22%5D%7D)\n"
         ),
     )
     country_code: typing.Optional[str] = pydantic.Field(
         alias="country-code", description=("ISO 3166-1 alpha-2 code of the ID’s issuing country.\n")
     )
     selected_id_class: typing.Optional[typing.List[str]] = pydantic.Field(
         alias="selected-id-class", description=("ID class of the input government ID.\n")
     )
-    front_photo: typing.Optional[GovernmentIdVerificationsCreateRequestDataAttributesFrontPhoto] = pydantic.Field(
+    front_photo: typing.Optional[CreateAGovIdVerificationRequestDataAttributesFrontPhoto] = pydantic.Field(
         alias="front-photo", description=("Front of ID.\n")
     )
-    back_photo: typing.Optional[GovernmentIdVerificationsCreateRequestDataAttributesBackPhoto] = pydantic.Field(
+    back_photo: typing.Optional[CreateAGovIdVerificationRequestDataAttributesBackPhoto] = pydantic.Field(
         alias="back-photo", description=("Back of ID.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_back_photo.py` & `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_request_data_attributes_back_photo_data import (
-    GovernmentIdVerificationsCreateRequestDataAttributesBackPhotoData,
+from .create_a_government_id_document_request_data_attributes_back_photo_data import (
+    CreateAGovernmentIdDocumentRequestDataAttributesBackPhotoData,
 )
 
 
-class GovernmentIdVerificationsCreateRequestDataAttributesBackPhoto(pydantic.BaseModel):
+class CreateAGovernmentIdDocumentRequestDataAttributesBackPhoto(pydantic.BaseModel):
     """
     Back of ID.
     """
 
-    data: typing.Optional[GovernmentIdVerificationsCreateRequestDataAttributesBackPhotoData] = pydantic.Field(
+    data: typing.Optional[CreateAGovernmentIdDocumentRequestDataAttributesBackPhotoData] = pydantic.Field(
         description=(
             "Government ID photo data, must be images. Can provide more than one image and we will pick the best for processing. Can also be provided as uploaded file(s) such as with multipart/form-data requests instead of this object(s).\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_back_photo_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class GovernmentIdVerificationsCreateRequestDataAttributesBackPhotoData(pydantic.BaseModel):
+class CreateAGovernmentIdDocumentRequestDataAttributesBackPhotoData(pydantic.BaseModel):
     """
     Government ID photo data, must be images. Can provide more than one image and we will pick the best for processing. Can also be provided as uploaded file(s) such as with multipart/form-data requests instead of this object(s).
     """
 
     data: str = pydantic.Field(description=("Base64 encoded file.\n"))
     filename: str = pydantic.Field(description=("Name of file.\n"))
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_front_photo.py` & `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_request_data_attributes_front_photo_data import (
-    GovernmentIdVerificationsCreateRequestDataAttributesFrontPhotoData,
+from .update_a_government_id_verification_request_data_attributes_back_photo_data import (
+    UpdateAGovernmentIdVerificationRequestDataAttributesBackPhotoData,
 )
 
 
-class GovernmentIdVerificationsCreateRequestDataAttributesFrontPhoto(pydantic.BaseModel):
+class UpdateAGovernmentIdVerificationRequestDataAttributesBackPhoto(pydantic.BaseModel):
     """
-    Front of ID.
+    Back of ID.
     """
 
-    data: typing.Optional[GovernmentIdVerificationsCreateRequestDataAttributesFrontPhotoData] = pydantic.Field(
+    data: typing.Optional[UpdateAGovernmentIdVerificationRequestDataAttributesBackPhotoData] = pydantic.Field(
         description=(
             "Government ID photo data, must be images. Can provide more than one image and we will pick the best for processing. Can also be provided as uploaded file(s) such as with multipart/form-data requests instead of this object(s).\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_request_data_attributes_front_photo_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class GovernmentIdVerificationsCreateRequestDataAttributesFrontPhotoData(pydantic.BaseModel):
+class CreateAGovernmentIdDocumentRequestDataAttributesFrontPhotoData(pydantic.BaseModel):
     """
     Government ID photo data, must be images. Can provide more than one image and we will pick the best for processing. Can also be provided as uploaded file(s) such as with multipart/form-data requests instead of this object(s).
     """
 
     data: str = pydantic.Field(description=("Base64 encoded file.\n"))
     filename: str = pydantic.Field(description=("Name of file.\n"))
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response.py` & `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_response_data import GovernmentIdVerificationsCreateResponseData
+from .update_a_government_id_verification_response_data import UpdateAGovernmentIdVerificationResponseData
 
 
-class GovernmentIdVerificationsCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[GovernmentIdVerificationsCreateResponseData]
+class UpdateAGovernmentIdVerificationResponse(pydantic.BaseModel):
+    data: typing.Optional[UpdateAGovernmentIdVerificationResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_response_data_attributes import (
-    GovernmentIdVerificationsCreateResponseDataAttributes,
+from .create_a_tin_database_verifications_response_data_attributes import (
+    CreateATinDatabaseVerificationsResponseDataAttributes,
 )
-from .government_id_verifications_create_response_data_relationships import (
-    GovernmentIdVerificationsCreateResponseDataRelationships,
+from .create_a_tin_database_verifications_response_data_relationships import (
+    CreateATinDatabaseVerificationsResponseDataRelationships,
 )
 
 
-class GovernmentIdVerificationsCreateResponseData(pydantic.BaseModel):
+class CreateATinDatabaseVerificationsResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[GovernmentIdVerificationsCreateResponseDataAttributes]
-    relationships: typing.Optional[GovernmentIdVerificationsCreateResponseDataRelationships]
+    attributes: typing.Optional[CreateATinDatabaseVerificationsResponseDataAttributes]
+    relationships: typing.Optional[CreateATinDatabaseVerificationsResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class GovernmentIdVerificationsCreateResponseDataAttributes(pydantic.BaseModel):
+class CreateAGovIdVerificationResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     created_at_ts: typing.Optional[int] = pydantic.Field(alias="created-at-ts")
     submitted_at: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at")
     submitted_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at-ts")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     completed_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at-ts")
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_response_data_relationships_document import (
-    GovernmentIdVerificationsCreateResponseDataRelationshipsDocument,
-)
-from .government_id_verifications_create_response_data_relationships_inquiry import (
-    GovernmentIdVerificationsCreateResponseDataRelationshipsInquiry,
+from .submit_a_government_id_verification_response_data_relationships_document_data import (
+    SubmitAGovernmentIdVerificationResponseDataRelationshipsDocumentData,
 )
 
 
-class GovernmentIdVerificationsCreateResponseDataRelationships(pydantic.BaseModel):
-    inquiry: typing.Optional[GovernmentIdVerificationsCreateResponseDataRelationshipsInquiry]
-    document: typing.Optional[GovernmentIdVerificationsCreateResponseDataRelationshipsDocument]
+class SubmitAGovernmentIdVerificationResponseDataRelationshipsDocument(pydantic.BaseModel):
+    data: typing.Optional[SubmitAGovernmentIdVerificationResponseDataRelationshipsDocumentData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships_document.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .government_id_verifications_create_response_data_relationships_document_data import (
-    GovernmentIdVerificationsCreateResponseDataRelationshipsDocumentData,
+from .retrieve_a_government_id_verification_response_data_relationships_document_data import (
+    RetrieveAGovernmentIdVerificationResponseDataRelationshipsDocumentData,
 )
 
 
-class GovernmentIdVerificationsCreateResponseDataRelationshipsDocument(pydantic.BaseModel):
-    data: typing.Optional[GovernmentIdVerificationsCreateResponseDataRelationshipsDocumentData]
+class RetrieveAGovernmentIdVerificationResponseDataRelationshipsDocument(pydantic.BaseModel):
+    data: typing.Optional[RetrieveAGovernmentIdVerificationResponseDataRelationshipsDocumentData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships_document_data.py` & `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries_data_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class GovernmentIdVerificationsCreateResponseDataRelationshipsDocumentData(pydantic.BaseModel):
+class AddPersonaObjectsResponseDataRelationshipsInquiriesDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/government_id_verifications_create_response_data_relationships_inquiry.py` & `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships_inquiry.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class GovernmentIdVerificationsCreateResponseDataRelationshipsInquiry(pydantic.BaseModel):
+class CreateADatabaseVerificationResponseDataRelationshipsInquiry(pydantic.BaseModel):
     data: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_account_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_account_request_data_file import ImportersImportAccountRequestDataFile
+from .import_phone_number_lists_request_data_attributes_file import ImportPhoneNumberListsRequestDataAttributesFile
 
 
-class ImportersImportAccountRequestData(pydantic.BaseModel):
-    file: typing.Optional[ImportersImportAccountRequestDataFile]
+class ImportPhoneNumberListsRequestDataAttributes(pydantic.BaseModel):
+    list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
+    file: typing.Optional[ImportPhoneNumberListsRequestDataAttributesFile]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_account_request_data_file.py` & `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportAccountRequestDataFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class CreateASelfieVerificationRequestDataAttributesLeftPhotoData(pydantic.BaseModel):
+    data: str = pydantic.Field(description=("Base64 encoded file.\n"))
+    filename: str = pydantic.Field(description=("Name of file.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_account_response.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_account_response_data import ImportersImportAccountResponseData
+from .create_a_phone_number_verification_response_data import CreateAPhoneNumberVerificationResponseData
 
 
-class ImportersImportAccountResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportAccountResponseData]
+class CreateAPhoneNumberVerificationResponse(pydantic.BaseModel):
+    data: typing.Optional[CreateAPhoneNumberVerificationResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_account_response_data.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_account_response_data_attributes import ImportersImportAccountResponseDataAttributes
+from .retrieve_an_importer_response_data_attributes import RetrieveAnImporterResponseDataAttributes
 
 
-class ImportersImportAccountResponseData(pydantic.BaseModel):
+class RetrieveAnImporterResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportAccountResponseDataAttributes]
+    attributes: typing.Optional[RetrieveAnImporterResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_account_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_an_account_response_data_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportAccountResponseDataAttributes(pydantic.BaseModel):
+class ImportAnAccountResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_email_address_lists_request_data_attributes import (
-    ImportersImportEmailAddressListsRequestDataAttributes,
-)
+from .import_ip_address_lists_response_data_attributes import ImportIpAddressListsResponseDataAttributes
 
 
-class ImportersImportEmailAddressListsRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[ImportersImportEmailAddressListsRequestDataAttributes]
+class ImportIpAddressListsResponseData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
+    attributes: typing.Optional[ImportIpAddressListsResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_email_address_lists_request_data_attributes_file import (
-    ImportersImportEmailAddressListsRequestDataAttributesFile,
-)
+from .import_email_address_lists_request_data_attributes_file import ImportEmailAddressListsRequestDataAttributesFile
 
 
-class ImportersImportEmailAddressListsRequestDataAttributes(pydantic.BaseModel):
+class ImportEmailAddressListsRequestDataAttributes(pydantic.BaseModel):
     list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
-    file: typing.Optional[ImportersImportEmailAddressListsRequestDataAttributesFile]
+    file: typing.Optional[ImportEmailAddressListsRequestDataAttributesFile]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_request_data_attributes_file.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions_data_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportEmailAddressListsRequestDataAttributesFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class RetrieveAnInquiryResponseDataRelationshipsSessionsDataItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_response.py` & `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_email_address_lists_response_data import ImportersImportEmailAddressListsResponseData
+from .import_ip_address_lists_response_data import ImportIpAddressListsResponseData
 
 
-class ImportersImportEmailAddressListsResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportEmailAddressListsResponseData]
+class ImportIpAddressListsResponse(pydantic.BaseModel):
+    data: typing.Optional[ImportIpAddressListsResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_response_data.py` & `fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_email_address_lists_response_data_attributes import (
-    ImportersImportEmailAddressListsResponseDataAttributes,
-)
+from .import_email_address_lists_response_data_attributes import ImportEmailAddressListsResponseDataAttributes
 
 
-class ImportersImportEmailAddressListsResponseData(pydantic.BaseModel):
+class ImportEmailAddressListsResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportEmailAddressListsResponseDataAttributes]
+    attributes: typing.Optional[ImportEmailAddressListsResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_email_address_lists_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportEmailAddressListsResponseDataAttributes(pydantic.BaseModel):
+class ImportEmailAddressListsResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_geolocation_lists_request_data_attributes import (
-    ImportersImportGeolocationListsRequestDataAttributes,
-)
+from .import_geolocation_lists_request_data_attributes import ImportGeolocationListsRequestDataAttributes
 
 
-class ImportersImportGeolocationListsRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[ImportersImportGeolocationListsRequestDataAttributes]
+class ImportGeolocationListsRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[ImportGeolocationListsRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_geolocation_lists_request_data_attributes_file import (
-    ImportersImportGeolocationListsRequestDataAttributesFile,
-)
+from .import_geolocation_lists_request_data_attributes_file import ImportGeolocationListsRequestDataAttributesFile
 
 
-class ImportersImportGeolocationListsRequestDataAttributes(pydantic.BaseModel):
+class ImportGeolocationListsRequestDataAttributes(pydantic.BaseModel):
     list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
-    file: typing.Optional[ImportersImportGeolocationListsRequestDataAttributesFile]
+    file: typing.Optional[ImportGeolocationListsRequestDataAttributesFile]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_request_data_attributes_file.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_request_data_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportGeolocationListsRequestDataAttributesFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class CreateADocumentRequestDataAttributes(pydantic.BaseModel):
+    inquiry_id: str = pydantic.Field(alias="inquiry-id")
+    kind: str = pydantic.Field(description=('Identifier for this document, e.g. "proof_of_employment"\n'))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_response.py` & `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_geolocation_lists_response_data import ImportersImportGeolocationListsResponseData
+from .import_geolocation_lists_response_data import ImportGeolocationListsResponseData
 
 
-class ImportersImportGeolocationListsResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportGeolocationListsResponseData]
+class ImportGeolocationListsResponse(pydantic.BaseModel):
+    data: typing.Optional[ImportGeolocationListsResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_response_data.py` & `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_geolocation_lists_response_data_attributes import (
-    ImportersImportGeolocationListsResponseDataAttributes,
-)
 
 
-class ImportersImportGeolocationListsResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportGeolocationListsResponseDataAttributes]
+class ImportIpAddressListsRequestDataAttributesFile(pydantic.BaseModel):
+    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
+    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_geolocation_lists_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportGeolocationListsResponseDataAttributes(pydantic.BaseModel):
+class ImportGeolocationListsResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_government_id_number_lists_request_data_attributes import (
-    ImportersImportGovernmentIdNumberListsRequestDataAttributes,
+from .import_government_id_number_lists_request_data_attributes_file import (
+    ImportGovernmentIdNumberListsRequestDataAttributesFile,
 )
 
 
-class ImportersImportGovernmentIdNumberListsRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[ImportersImportGovernmentIdNumberListsRequestDataAttributes]
+class ImportGovernmentIdNumberListsRequestDataAttributes(pydantic.BaseModel):
+    list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
+    file: typing.Optional[ImportGovernmentIdNumberListsRequestDataAttributesFile]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_government_id_number_lists_request_data_attributes_file import (
-    ImportersImportGovernmentIdNumberListsRequestDataAttributesFile,
+from .import_government_id_number_lists_response_data_attributes import (
+    ImportGovernmentIdNumberListsResponseDataAttributes,
 )
 
 
-class ImportersImportGovernmentIdNumberListsRequestDataAttributes(pydantic.BaseModel):
-    list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
-    file: typing.Optional[ImportersImportGovernmentIdNumberListsRequestDataAttributesFile]
+class ImportGovernmentIdNumberListsResponseData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
+    attributes: typing.Optional[ImportGovernmentIdNumberListsResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_request_data_attributes_file.py` & `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments_data_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportGovernmentIdNumberListsRequestDataAttributesFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class RetrieveCaseResponseDataRelationshipsCaseCommentsDataItem(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_response.py` & `fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_government_id_number_lists_response_data import (
-    ImportersImportGovernmentIdNumberListsResponseData,
+from .archive_a_government_id_number_list_item_response_data_relationships_creator import (
+    ArchiveAGovernmentIdNumberListItemResponseDataRelationshipsCreator,
 )
 
 
-class ImportersImportGovernmentIdNumberListsResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportGovernmentIdNumberListsResponseData]
+class ArchiveAGovernmentIdNumberListItemResponseDataRelationships(pydantic.BaseModel):
+    creator: typing.Optional[ArchiveAGovernmentIdNumberListItemResponseDataRelationshipsCreator]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_government_id_number_lists_response_data_attributes import (
-    ImportersImportGovernmentIdNumberListsResponseDataAttributes,
+from .create_a_government_id_number_list_item_response_data_relationships_creator import (
+    CreateAGovernmentIdNumberListItemResponseDataRelationshipsCreator,
 )
 
 
-class ImportersImportGovernmentIdNumberListsResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportGovernmentIdNumberListsResponseDataAttributes]
+class CreateAGovernmentIdNumberListItemResponseDataRelationships(pydantic.BaseModel):
+    creator: typing.Optional[CreateAGovernmentIdNumberListItemResponseDataRelationshipsCreator]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_government_id_number_lists_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportGovernmentIdNumberListsResponseDataAttributes(pydantic.BaseModel):
+class RetrieveAnImporterResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_ip_address_lists_request_data_attributes import (
-    ImportersImportIpAddressListsRequestDataAttributes,
-)
+from .import_ip_address_lists_request_data_attributes import ImportIpAddressListsRequestDataAttributes
 
 
-class ImportersImportIpAddressListsRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[ImportersImportIpAddressListsRequestDataAttributes]
+class ImportIpAddressListsRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[ImportIpAddressListsRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_ip_address_lists_request_data_attributes_file import (
-    ImportersImportIpAddressListsRequestDataAttributesFile,
-)
+from .import_ip_address_lists_request_data_attributes_file import ImportIpAddressListsRequestDataAttributesFile
 
 
-class ImportersImportIpAddressListsRequestDataAttributes(pydantic.BaseModel):
+class ImportIpAddressListsRequestDataAttributes(pydantic.BaseModel):
     list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
-    file: typing.Optional[ImportersImportIpAddressListsRequestDataAttributesFile]
+    file: typing.Optional[ImportIpAddressListsRequestDataAttributesFile]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_request_data_attributes_file.py` & `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportIpAddressListsRequestDataAttributesFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class BusinessLookupReport1ResponseDataAttributesResultItemSource(pydantic.BaseModel):
+    publisher: typing.Optional[str]
+    url: typing.Optional[str]
+    last_retrieved_at: typing.Optional[str] = pydantic.Field(alias="last-retrieved-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_response.py` & `fern_persona-0.0.2/src/persona/types/import_email_address_lists_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_ip_address_lists_response_data import ImportersImportIpAddressListsResponseData
+from .import_email_address_lists_response_data import ImportEmailAddressListsResponseData
 
 
-class ImportersImportIpAddressListsResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportIpAddressListsResponseData]
+class ImportEmailAddressListsResponse(pydantic.BaseModel):
+    data: typing.Optional[ImportEmailAddressListsResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_response_data.py` & `fern_persona-0.0.2/src/persona/types/import_name_lists_response_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_ip_address_lists_response_data_attributes import (
-    ImportersImportIpAddressListsResponseDataAttributes,
-)
+from .import_name_lists_response_data_attributes import ImportNameListsResponseDataAttributes
 
 
-class ImportersImportIpAddressListsResponseData(pydantic.BaseModel):
+class ImportNameListsResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportIpAddressListsResponseDataAttributes]
+    attributes: typing.Optional[ImportNameListsResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_ip_address_lists_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportIpAddressListsResponseDataAttributes(pydantic.BaseModel):
+class ImportIpAddressListsResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_name_lists_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_name_lists_request_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_name_lists_request_data_attributes import ImportersImportNameListsRequestDataAttributes
+from .import_name_lists_request_data_attributes import ImportNameListsRequestDataAttributes
 
 
-class ImportersImportNameListsRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[ImportersImportNameListsRequestDataAttributes]
+class ImportNameListsRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[ImportNameListsRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_name_lists_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_name_lists_request_data_attributes_file import ImportersImportNameListsRequestDataAttributesFile
+from .create_a_face_list_item_request_data_attributes_face_photo import (
+    CreateAFaceListItemRequestDataAttributesFacePhoto,
+)
 
 
-class ImportersImportNameListsRequestDataAttributes(pydantic.BaseModel):
-    list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
-    file: typing.Optional[ImportersImportNameListsRequestDataAttributesFile]
+class CreateAFaceListItemRequestDataAttributes(pydantic.BaseModel):
+    list_id: typing.Optional[str] = pydantic.Field(
+        alias="list-id", description=("ID of the list to add this item to. List must be a Face List.\n")
+    )
+    face_photo: typing.Optional[CreateAFaceListItemRequestDataAttributesFacePhoto] = pydantic.Field(alias="face-photo")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_name_lists_request_data_attributes_file.py` & `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_request_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportNameListsRequestDataAttributesFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class SetStatusForACaseRequestMeta(pydantic.BaseModel):
+    status: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_name_lists_response.py` & `fern_persona-0.0.2/src/persona/types/update_an_account_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_name_lists_response_data import ImportersImportNameListsResponseData
+from .update_an_account_response_data import UpdateAnAccountResponseData
 
 
-class ImportersImportNameListsResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportNameListsResponseData]
+class UpdateAnAccountResponse(pydantic.BaseModel):
+    data: typing.Optional[UpdateAnAccountResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_name_lists_response_data.py` & `fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_attachments_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_name_lists_response_data_attributes import ImportersImportNameListsResponseDataAttributes
 
 
-class ImportersImportNameListsResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportNameListsResponseDataAttributes]
+class UpdateACaseRequestDataAttributesAttachmentsItem(pydantic.BaseModel):
+    data: typing.Optional[str] = pydantic.Field(description=("base 64 encoded file\n"))
+    filename: typing.Optional[str] = pydantic.Field(description=("Name of the file\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_name_lists_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_name_lists_response_data_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportNameListsResponseDataAttributes(pydantic.BaseModel):
+class ImportNameListsResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_request_data.py` & `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_phone_number_lists_request_data_attributes import (
-    ImportersImportPhoneNumberListsRequestDataAttributes,
+from .import_government_id_number_lists_request_data_attributes import (
+    ImportGovernmentIdNumberListsRequestDataAttributes,
 )
 
 
-class ImportersImportPhoneNumberListsRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[ImportersImportPhoneNumberListsRequestDataAttributes]
+class ImportGovernmentIdNumberListsRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[ImportGovernmentIdNumberListsRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_phone_number_lists_request_data_attributes_file import (
-    ImportersImportPhoneNumberListsRequestDataAttributesFile,
-)
+from .import_name_lists_request_data_attributes_file import ImportNameListsRequestDataAttributesFile
 
 
-class ImportersImportPhoneNumberListsRequestDataAttributes(pydantic.BaseModel):
+class ImportNameListsRequestDataAttributes(pydantic.BaseModel):
     list_id: typing.Optional[str] = pydantic.Field(alias="list-id")
-    file: typing.Optional[ImportersImportPhoneNumberListsRequestDataAttributesFile]
+    file: typing.Optional[ImportNameListsRequestDataAttributesFile]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_request_data_attributes_file.py` & `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .import_phone_number_lists_response_data import ImportPhoneNumberListsResponseData
 
 
-class ImportersImportPhoneNumberListsRequestDataAttributesFile(pydantic.BaseModel):
-    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
-    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
+class ImportPhoneNumberListsResponse(pydantic.BaseModel):
+    data: typing.Optional[ImportPhoneNumberListsResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_response.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_phone_number_lists_response_data import ImportersImportPhoneNumberListsResponseData
+from .retrieve_a_document_response_data_relationships_inquiry import RetrieveADocumentResponseDataRelationshipsInquiry
 
 
-class ImportersImportPhoneNumberListsResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersImportPhoneNumberListsResponseData]
+class RetrieveADocumentResponseDataRelationships(pydantic.BaseModel):
+    inquiry: typing.Optional[RetrieveADocumentResponseDataRelationshipsInquiry]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_response_data.py` & `fern_persona-0.0.2/src/persona/types/import_an_account_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_import_phone_number_lists_response_data_attributes import (
-    ImportersImportPhoneNumberListsResponseDataAttributes,
-)
+from .import_an_account_response_data_attributes import ImportAnAccountResponseDataAttributes
 
 
-class ImportersImportPhoneNumberListsResponseData(pydantic.BaseModel):
+class ImportAnAccountResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ImportersImportPhoneNumberListsResponseDataAttributes]
+    attributes: typing.Optional[ImportAnAccountResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_import_phone_number_lists_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersImportPhoneNumberListsResponseDataAttributes(pydantic.BaseModel):
+class ImportPhoneNumberListsResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_retrieve_response_data import ImportersRetrieveResponseData
 
 
-class ImportersRetrieveResponse(pydantic.BaseModel):
-    data: typing.Optional[ImportersRetrieveResponseData]
-
+class CreateAnIpAddressListResponse(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_retrieve_response_data.py` & `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .importers_retrieve_response_data_attributes import ImportersRetrieveResponseDataAttributes
 
 
-class ImportersRetrieveResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[ImportersRetrieveResponseDataAttributes]
+class ImportGovernmentIdNumberListsRequestDataAttributesFile(pydantic.BaseModel):
+    data: typing.Optional[str] = pydantic.Field(description=("Base64 encoded file\n"))
+    filename: typing.Optional[str] = pydantic.Field(description=("Name of file\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/importers_retrieve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/import_face_lists_response_data_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ImportersRetrieveResponseDataAttributes(pydantic.BaseModel):
+class ImportFaceListsResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     error_count: typing.Optional[int] = pydantic.Field(alias="error-count")
     successful_count: typing.Optional[int] = pydantic.Field(alias="successful-count")
     duplicate_count: typing.Optional[int] = pydantic.Field(alias="duplicate-count")
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_request_meta.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_post_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesApproveRequestMeta(pydantic.BaseModel):
-    comment: typing.Optional[str] = pydantic.Field(description=("Comments for auditing purposes\n"))
-
+class RetrieveAnApiLogResponseDataAttributesRequestPostParams(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response.py` & `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_approve_response_data import InquiriesApproveResponseData
+from .set_status_for_a_case_response_data_relationships_inquiries_data_item import (
+    SetStatusForACaseResponseDataRelationshipsInquiriesDataItem,
+)
 
 
-class InquiriesApproveResponse(pydantic.BaseModel):
-    data: typing.Optional[InquiriesApproveResponseData]
+class SetStatusForACaseResponseDataRelationshipsInquiries(pydantic.BaseModel):
+    data: typing.Optional[typing.List[SetStatusForACaseResponseDataRelationshipsInquiriesDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_approve_response_data_attributes import InquiriesApproveResponseDataAttributes
-from .inquiries_approve_response_data_relationships import InquiriesApproveResponseDataRelationships
+from .approve_an_inquiry_response_data_attributes import ApproveAnInquiryResponseDataAttributes
+from .approve_an_inquiry_response_data_relationships import ApproveAnInquiryResponseDataRelationships
 
 
-class InquiriesApproveResponseData(pydantic.BaseModel):
+class ApproveAnInquiryResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesApproveResponseDataAttributes]
-    relationships: typing.Optional[InquiriesApproveResponseDataRelationships]
+    attributes: typing.Optional[ApproveAnInquiryResponseDataAttributes]
+    relationships: typing.Optional[ApproveAnInquiryResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesApproveResponseDataAttributes(pydantic.BaseModel):
+class ReportActionReRunReportResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
-    subject: typing.Optional[typing.Any]
-    reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
-    expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
+    redacted_at: typing.Optional[typing.Any] = pydantic.Field(alias="redacted-at")
+    report_template_version_name: typing.Optional[str] = pydantic.Field(alias="report-template-version-name")
+    term: typing.Optional[str]
+    matched_lists: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_approve_response_data_relationships_account import InquiriesApproveResponseDataRelationshipsAccount
-from .inquiries_approve_response_data_relationships_reports import InquiriesApproveResponseDataRelationshipsReports
-from .inquiries_approve_response_data_relationships_template import InquiriesApproveResponseDataRelationshipsTemplate
-from .inquiries_approve_response_data_relationships_verifications import (
-    InquiriesApproveResponseDataRelationshipsVerifications,
+from .resume_an_inquiry_response_data_relationships_account import ResumeAnInquiryResponseDataRelationshipsAccount
+from .resume_an_inquiry_response_data_relationships_reports import ResumeAnInquiryResponseDataRelationshipsReports
+from .resume_an_inquiry_response_data_relationships_template import ResumeAnInquiryResponseDataRelationshipsTemplate
+from .resume_an_inquiry_response_data_relationships_verifications import (
+    ResumeAnInquiryResponseDataRelationshipsVerifications,
 )
 
 
-class InquiriesApproveResponseDataRelationships(pydantic.BaseModel):
-    account: typing.Optional[InquiriesApproveResponseDataRelationshipsAccount]
-    template: typing.Optional[InquiriesApproveResponseDataRelationshipsTemplate]
-    reports: typing.Optional[InquiriesApproveResponseDataRelationshipsReports]
-    verifications: typing.Optional[InquiriesApproveResponseDataRelationshipsVerifications]
+class ResumeAnInquiryResponseDataRelationships(pydantic.BaseModel):
+    account: typing.Optional[ResumeAnInquiryResponseDataRelationshipsAccount]
+    template: typing.Optional[ResumeAnInquiryResponseDataRelationshipsTemplate]
+    reports: typing.Optional[ResumeAnInquiryResponseDataRelationshipsReports]
+    verifications: typing.Optional[ResumeAnInquiryResponseDataRelationshipsVerifications]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_approve_response_data_relationships_account_data import (
-    InquiriesApproveResponseDataRelationshipsAccountData,
+from .report_action_resume_continuous_monitoring_response_data_relationships_report_template_data import (
+    ReportActionResumeContinuousMonitoringResponseDataRelationshipsReportTemplateData,
 )
 
 
-class InquiriesApproveResponseDataRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesApproveResponseDataRelationshipsAccountData]
+class ReportActionResumeContinuousMonitoringResponseDataRelationshipsReportTemplate(pydantic.BaseModel):
+    data: typing.Optional[ReportActionResumeContinuousMonitoringResponseDataRelationshipsReportTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesApproveResponseDataRelationshipsAccountData(pydantic.BaseModel):
+class CreateAnInquiryResponseDataRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesApproveResponseDataRelationshipsReports(pydantic.BaseModel):
+class CreateACaseResponseDataRelationshipsReports(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_approve_response_data_relationships_template_data import (
-    InquiriesApproveResponseDataRelationshipsTemplateData,
+from .create_an_inquiry_response_data_relationships_template_data import (
+    CreateAnInquiryResponseDataRelationshipsTemplateData,
 )
 
 
-class InquiriesApproveResponseDataRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesApproveResponseDataRelationshipsTemplateData]
+class CreateAnInquiryResponseDataRelationshipsTemplate(pydantic.BaseModel):
+    data: typing.Optional[CreateAnInquiryResponseDataRelationshipsTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesApproveResponseDataRelationshipsTemplateData(pydantic.BaseModel):
+class ListAllInquiriesResponseDataItemRelationshipsTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_approve_response_data_relationships_verifications_data_item import (
-    InquiriesApproveResponseDataRelationshipsVerificationsDataItem,
+from .create_an_inquiry_response_data_relationships_verifications_data_item import (
+    CreateAnInquiryResponseDataRelationshipsVerificationsDataItem,
 )
 
 
-class InquiriesApproveResponseDataRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesApproveResponseDataRelationshipsVerificationsDataItem]]
+class CreateAnInquiryResponseDataRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[CreateAnInquiryResponseDataRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_approve_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesApproveResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class ExpireAnInquiryResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_request_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_request_data_attributes import InquiriesCreateRequestDataAttributes
+from .create_a_face_list_request_data_attributes import CreateAFaceListRequestDataAttributes
 
 
-class InquiriesCreateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[InquiriesCreateRequestDataAttributes]
+class CreateAFaceListRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[CreateAFaceListRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_request_data_attributes_fields import InquiriesCreateRequestDataAttributesFields
+from .create_an_inquiry_request_data_attributes_fields import CreateAnInquiryRequestDataAttributesFields
 
 
-class InquiriesCreateRequestDataAttributes(pydantic.BaseModel):
+class CreateAnInquiryRequestDataAttributes(pydantic.BaseModel):
     template_id: typing.Optional[str] = pydantic.Field(
         alias="template-id",
         description=(
             "Template ID for flow requirements (use this field if your template ID starts with `tmpl_`). *You must pass in either template-id OR inquiry-template-id OR inquiry-template-version-id*\n"
         ),
     )
     inquiry_template_id: typing.Optional[str] = pydantic.Field(
@@ -38,15 +38,15 @@
     redirect_uri: typing.Optional[str] = pydantic.Field(
         alias="redirect-uri", description=("If using the Hosted flow, redirect to this URL after completion\n")
     )
     note: typing.Optional[str] = pydantic.Field(description=("Unstructured field for your custom use\n"))
     country_code: typing.Optional[str] = pydantic.Field(
         alias="country-code", description=("Country code of residence for verification, in ISO 3166 Alpha-2 format.\n")
     )
-    fields: typing.Optional[InquiriesCreateRequestDataAttributesFields] = pydantic.Field(
+    fields: typing.Optional[CreateAnInquiryRequestDataAttributesFields] = pydantic.Field(
         description=(
             "JSON key-value pairs of field name to field value. <br><br>Common fields include <ul><li>`name-first`</li><li>`name-last`</li><li>`birthdate`</li><li>`address-street-1`</li><li>`address-city`</li><li>`address-subdivision`</li><li>`address-postal-code`</li><li>`address-country-code`</li><li>`phone-number`</li><li>`email-address`</li></ul>\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_request_data_attributes_fields.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesCreateRequestDataAttributesFields(pydantic.BaseModel):
+class CreateAnInquiryRequestDataAttributesFields(pydantic.BaseModel):
     """
     JSON key-value pairs of field name to field value. <br><br>Common fields include <ul><li>`name-first`</li><li>`name-last`</li><li>`birthdate`</li><li>`address-street-1`</li><li>`address-city`</li><li>`address-subdivision`</li><li>`address-postal-code`</li><li>`address-country-code`</li><li>`phone-number`</li><li>`email-address`</li></ul>
     """
 
     name_first: typing.Optional[str] = pydantic.Field(alias="name-first", description=("optional\n"))
     name_last: typing.Optional[str] = pydantic.Field(alias="name-last", description=("optional\n"))
     birthdate: typing.Optional[str] = pydantic.Field(description=("optional\n"))
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response.py` & `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_response_data import InquiriesCreateResponseData
+from .submit_a_serpro_database_verification_response_data import SubmitASerproDatabaseVerificationResponseData
 
 
-class InquiriesCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[InquiriesCreateResponseData]
+class SubmitASerproDatabaseVerificationResponse(pydantic.BaseModel):
+    data: typing.Optional[SubmitASerproDatabaseVerificationResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_response_data_attributes import InquiriesCreateResponseDataAttributes
-from .inquiries_create_response_data_relationships import InquiriesCreateResponseDataRelationships
+from .list_all_inquiries_response_data_item_attributes import ListAllInquiriesResponseDataItemAttributes
+from .list_all_inquiries_response_data_item_relationships import ListAllInquiriesResponseDataItemRelationships
 
 
-class InquiriesCreateResponseData(pydantic.BaseModel):
+class ListAllInquiriesResponseDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesCreateResponseDataAttributes]
-    relationships: typing.Optional[InquiriesCreateResponseDataRelationships]
+    attributes: typing.Optional[ListAllInquiriesResponseDataItemAttributes]
+    relationships: typing.Optional[ListAllInquiriesResponseDataItemRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesCreateResponseDataAttributes(pydantic.BaseModel):
-    status: typing.Optional[str]
-    subject: typing.Optional[typing.Any]
+class RetrieveCaseResponseIncludedItemAttributes(pydantic.BaseModel):
     reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
-    expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
+    updated_at: typing.Optional[str] = pydantic.Field(alias="updated-at")
+    tags: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_response_data_relationships_account import InquiriesCreateResponseDataRelationshipsAccount
-from .inquiries_create_response_data_relationships_reports import InquiriesCreateResponseDataRelationshipsReports
-from .inquiries_create_response_data_relationships_template import InquiriesCreateResponseDataRelationshipsTemplate
-from .inquiries_create_response_data_relationships_verifications import (
-    InquiriesCreateResponseDataRelationshipsVerifications,
-)
-
-
-class InquiriesCreateResponseDataRelationships(pydantic.BaseModel):
-    account: typing.Optional[InquiriesCreateResponseDataRelationshipsAccount]
-    template: typing.Optional[InquiriesCreateResponseDataRelationshipsTemplate]
-    reports: typing.Optional[InquiriesCreateResponseDataRelationshipsReports]
-    verifications: typing.Optional[InquiriesCreateResponseDataRelationshipsVerifications]
+from .create_a_case_response_data_relationships_accounts import CreateACaseResponseDataRelationshipsAccounts
+from .create_a_case_response_data_relationships_case_comments import CreateACaseResponseDataRelationshipsCaseComments
+from .create_a_case_response_data_relationships_case_template import CreateACaseResponseDataRelationshipsCaseTemplate
+from .create_a_case_response_data_relationships_inquiries import CreateACaseResponseDataRelationshipsInquiries
+from .create_a_case_response_data_relationships_reports import CreateACaseResponseDataRelationshipsReports
+
+
+class CreateACaseResponseDataRelationships(pydantic.BaseModel):
+    case_template: typing.Optional[CreateACaseResponseDataRelationshipsCaseTemplate] = pydantic.Field(
+        alias="case-template"
+    )
+    case_comments: typing.Optional[CreateACaseResponseDataRelationshipsCaseComments] = pydantic.Field(
+        alias="case-comments"
+    )
+    accounts: typing.Optional[CreateACaseResponseDataRelationshipsAccounts]
+    inquiries: typing.Optional[CreateACaseResponseDataRelationshipsInquiries]
+    reports: typing.Optional[CreateACaseResponseDataRelationshipsReports]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_response_data_relationships_account_data import (
-    InquiriesCreateResponseDataRelationshipsAccountData,
+from .create_an_inquiry_response_data_relationships_account_data import (
+    CreateAnInquiryResponseDataRelationshipsAccountData,
 )
 
 
-class InquiriesCreateResponseDataRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesCreateResponseDataRelationshipsAccountData]
+class CreateAnInquiryResponseDataRelationshipsAccount(pydantic.BaseModel):
+    data: typing.Optional[CreateAnInquiryResponseDataRelationshipsAccountData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesCreateResponseDataRelationshipsAccountData(pydantic.BaseModel):
+class GenerateAOneTimeLinkResponseDataRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesCreateResponseDataRelationshipsReports(pydantic.BaseModel):
+class ListAllInquiriesResponseDataItemRelationshipsReports(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_response_data_relationships_template_data import (
-    InquiriesCreateResponseDataRelationshipsTemplateData,
+from .create_a_case_response_data_relationships_case_template_data import (
+    CreateACaseResponseDataRelationshipsCaseTemplateData,
 )
 
 
-class InquiriesCreateResponseDataRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesCreateResponseDataRelationshipsTemplateData]
+class CreateACaseResponseDataRelationshipsCaseTemplate(pydantic.BaseModel):
+    data: typing.Optional[CreateACaseResponseDataRelationshipsCaseTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesCreateResponseDataRelationshipsTemplateData(pydantic.BaseModel):
+class ListAllInquiriesResponseDataItemRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_create_response_data_relationships_verifications_data_item import (
-    InquiriesCreateResponseDataRelationshipsVerificationsDataItem,
+from .list_all_inquiries_response_data_item_relationships_verifications_data_item import (
+    ListAllInquiriesResponseDataItemRelationshipsVerificationsDataItem,
 )
 
 
-class InquiriesCreateResponseDataRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesCreateResponseDataRelationshipsVerificationsDataItem]]
+class ListAllInquiriesResponseDataItemRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ListAllInquiriesResponseDataItemRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_create_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesCreateResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class CreateAnInquiryResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_request_meta.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_request_meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesDeclineRequestMeta(pydantic.BaseModel):
-    comment: typing.Optional[str] = pydantic.Field(description=("Comments for auditing purposes\n"))
+class CreateACaseRequestMeta(pydantic.BaseModel):
+    object_ids: typing.Optional[typing.List[str]] = pydantic.Field(
+        alias="object-ids", description=("Array of Persona object IDs that should be related to this case\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response.py` & `fern_persona-0.0.2/src/persona/types/add_persona_objects_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_decline_response_data import InquiriesDeclineResponseData
+from .add_persona_objects_response_data import AddPersonaObjectsResponseData
 
 
-class InquiriesDeclineResponse(pydantic.BaseModel):
-    data: typing.Optional[InquiriesDeclineResponseData]
+class AddPersonaObjectsResponse(pydantic.BaseModel):
+    data: typing.Optional[AddPersonaObjectsResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_decline_response_data_attributes import InquiriesDeclineResponseDataAttributes
-from .inquiries_decline_response_data_relationships import InquiriesDeclineResponseDataRelationships
+from .create_a_case_response_data_attributes import CreateACaseResponseDataAttributes
+from .create_a_case_response_data_relationships import CreateACaseResponseDataRelationships
 
 
-class InquiriesDeclineResponseData(pydantic.BaseModel):
+class CreateACaseResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesDeclineResponseDataAttributes]
-    relationships: typing.Optional[InquiriesDeclineResponseDataRelationships]
+    attributes: typing.Optional[CreateACaseResponseDataAttributes]
+    relationships: typing.Optional[CreateACaseResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_attributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesDeclineResponseDataAttributes(pydantic.BaseModel):
+class CreateAnInquiryResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     subject: typing.Optional[typing.Any]
     reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
+    completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_decline_response_data_relationships_account import InquiriesDeclineResponseDataRelationshipsAccount
-from .inquiries_decline_response_data_relationships_reports import InquiriesDeclineResponseDataRelationshipsReports
-from .inquiries_decline_response_data_relationships_template import InquiriesDeclineResponseDataRelationshipsTemplate
-from .inquiries_decline_response_data_relationships_verifications import (
-    InquiriesDeclineResponseDataRelationshipsVerifications,
+from .create_an_inquiry_response_data_relationships_account import CreateAnInquiryResponseDataRelationshipsAccount
+from .create_an_inquiry_response_data_relationships_reports import CreateAnInquiryResponseDataRelationshipsReports
+from .create_an_inquiry_response_data_relationships_template import CreateAnInquiryResponseDataRelationshipsTemplate
+from .create_an_inquiry_response_data_relationships_verifications import (
+    CreateAnInquiryResponseDataRelationshipsVerifications,
 )
 
 
-class InquiriesDeclineResponseDataRelationships(pydantic.BaseModel):
-    account: typing.Optional[InquiriesDeclineResponseDataRelationshipsAccount]
-    template: typing.Optional[InquiriesDeclineResponseDataRelationshipsTemplate]
-    reports: typing.Optional[InquiriesDeclineResponseDataRelationshipsReports]
-    verifications: typing.Optional[InquiriesDeclineResponseDataRelationshipsVerifications]
+class CreateAnInquiryResponseDataRelationships(pydantic.BaseModel):
+    account: typing.Optional[CreateAnInquiryResponseDataRelationshipsAccount]
+    template: typing.Optional[CreateAnInquiryResponseDataRelationshipsTemplate]
+    reports: typing.Optional[CreateAnInquiryResponseDataRelationshipsReports]
+    verifications: typing.Optional[CreateAnInquiryResponseDataRelationshipsVerifications]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_decline_response_data_relationships_account_data import (
-    InquiriesDeclineResponseDataRelationshipsAccountData,
+from .create_a_document_response_data_relationships_inquiry_data import (
+    CreateADocumentResponseDataRelationshipsInquiryData,
 )
 
 
-class InquiriesDeclineResponseDataRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesDeclineResponseDataRelationshipsAccountData]
+class CreateADocumentResponseDataRelationshipsInquiry(pydantic.BaseModel):
+    data: typing.Optional[CreateADocumentResponseDataRelationshipsInquiryData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesDeclineResponseDataRelationshipsAccountData(pydantic.BaseModel):
+class DeclineAnInquiryResponseDataRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesDeclineResponseDataRelationshipsReports(pydantic.BaseModel):
+class CreateAnInquiryResponseDataRelationshipsReports(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_decline_response_data_relationships_template_data import (
-    InquiriesDeclineResponseDataRelationshipsTemplateData,
+from .update_a_case_response_data_relationships_inquiries_data_item import (
+    UpdateACaseResponseDataRelationshipsInquiriesDataItem,
 )
 
 
-class InquiriesDeclineResponseDataRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesDeclineResponseDataRelationshipsTemplateData]
+class UpdateACaseResponseDataRelationshipsInquiries(pydantic.BaseModel):
+    data: typing.Optional[typing.List[UpdateACaseResponseDataRelationshipsInquiriesDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesDeclineResponseDataRelationshipsTemplateData(pydantic.BaseModel):
+class DeclineAnInquiryResponseDataRelationshipsTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_decline_response_data_relationships_verifications_data_item import (
-    InquiriesDeclineResponseDataRelationshipsVerificationsDataItem,
+from .decline_an_inquiry_response_data_relationships_verifications_data_item import (
+    DeclineAnInquiryResponseDataRelationshipsVerificationsDataItem,
 )
 
 
-class InquiriesDeclineResponseDataRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesDeclineResponseDataRelationshipsVerificationsDataItem]]
+class DeclineAnInquiryResponseDataRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[DeclineAnInquiryResponseDataRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_decline_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesDeclineResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class ResumeAnInquiryResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item import InquiriesListAllResponseDataItem
-from .inquiries_list_all_response_links import InquiriesListAllResponseLinks
+from .list_all_inquiries_response_data_item import ListAllInquiriesResponseDataItem
+from .list_all_inquiries_response_links import ListAllInquiriesResponseLinks
 
 
-class InquiriesListAllResponse(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesListAllResponseDataItem]]
-    links: typing.Optional[InquiriesListAllResponseLinks]
+class ListAllInquiriesResponse(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ListAllInquiriesResponseDataItem]]
+    links: typing.Optional[ListAllInquiriesResponseLinks]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item_attributes import InquiriesListAllResponseDataItemAttributes
-from .inquiries_list_all_response_data_item_relationships import InquiriesListAllResponseDataItemRelationships
+from .create_a_case_response_data_relationships_inquiries_data_item import (
+    CreateACaseResponseDataRelationshipsInquiriesDataItem,
+)
 
 
-class InquiriesListAllResponseDataItem(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesListAllResponseDataItemAttributes]
-    relationships: typing.Optional[InquiriesListAllResponseDataItemRelationships]
+class CreateACaseResponseDataRelationshipsInquiries(pydantic.BaseModel):
+    data: typing.Optional[typing.List[CreateACaseResponseDataRelationshipsInquiriesDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_attributes.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_attributes.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseDataItemAttributes(pydantic.BaseModel):
+class ExpireAnInquiryResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     subject: typing.Optional[typing.Any]
     reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
-    completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
-    expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
+    completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
+    expired_at: typing.Optional[str] = pydantic.Field(alias="expired-at")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item_relationships_account import (
-    InquiriesListAllResponseDataItemRelationshipsAccount,
+from .list_all_inquiries_response_data_item_relationships_account import (
+    ListAllInquiriesResponseDataItemRelationshipsAccount,
 )
-from .inquiries_list_all_response_data_item_relationships_reports import (
-    InquiriesListAllResponseDataItemRelationshipsReports,
+from .list_all_inquiries_response_data_item_relationships_reports import (
+    ListAllInquiriesResponseDataItemRelationshipsReports,
 )
-from .inquiries_list_all_response_data_item_relationships_sessions import (
-    InquiriesListAllResponseDataItemRelationshipsSessions,
+from .list_all_inquiries_response_data_item_relationships_sessions import (
+    ListAllInquiriesResponseDataItemRelationshipsSessions,
 )
-from .inquiries_list_all_response_data_item_relationships_template import (
-    InquiriesListAllResponseDataItemRelationshipsTemplate,
+from .list_all_inquiries_response_data_item_relationships_template import (
+    ListAllInquiriesResponseDataItemRelationshipsTemplate,
 )
-from .inquiries_list_all_response_data_item_relationships_verifications import (
-    InquiriesListAllResponseDataItemRelationshipsVerifications,
+from .list_all_inquiries_response_data_item_relationships_verifications import (
+    ListAllInquiriesResponseDataItemRelationshipsVerifications,
 )
 
 
-class InquiriesListAllResponseDataItemRelationships(pydantic.BaseModel):
-    account: typing.Optional[InquiriesListAllResponseDataItemRelationshipsAccount]
-    template: typing.Optional[InquiriesListAllResponseDataItemRelationshipsTemplate]
-    reports: typing.Optional[InquiriesListAllResponseDataItemRelationshipsReports]
-    verifications: typing.Optional[InquiriesListAllResponseDataItemRelationshipsVerifications]
-    sessions: typing.Optional[InquiriesListAllResponseDataItemRelationshipsSessions]
+class ListAllInquiriesResponseDataItemRelationships(pydantic.BaseModel):
+    account: typing.Optional[ListAllInquiriesResponseDataItemRelationshipsAccount]
+    template: typing.Optional[ListAllInquiriesResponseDataItemRelationshipsTemplate]
+    reports: typing.Optional[ListAllInquiriesResponseDataItemRelationshipsReports]
+    verifications: typing.Optional[ListAllInquiriesResponseDataItemRelationshipsVerifications]
+    sessions: typing.Optional[ListAllInquiriesResponseDataItemRelationshipsSessions]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item_relationships_account_data import (
-    InquiriesListAllResponseDataItemRelationshipsAccountData,
+from .retrieve_an_inquiry_response_data_relationships_account_data import (
+    RetrieveAnInquiryResponseDataRelationshipsAccountData,
 )
 
 
-class InquiriesListAllResponseDataItemRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesListAllResponseDataItemRelationshipsAccountData]
+class RetrieveAnInquiryResponseDataRelationshipsAccount(pydantic.BaseModel):
+    data: typing.Optional[RetrieveAnInquiryResponseDataRelationshipsAccountData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseDataItemRelationshipsAccountData(pydantic.BaseModel):
+class ResumeAnInquiryResponseDataRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseDataItemRelationshipsReports(pydantic.BaseModel):
+class RetrieveAnInquiryResponseDataRelationshipsReports(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_sessions.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item_relationships_sessions_data_item import (
-    InquiriesListAllResponseDataItemRelationshipsSessionsDataItem,
+from .create_a_case_response_included_item_relationships_sessions_data_item import (
+    CreateACaseResponseIncludedItemRelationshipsSessionsDataItem,
 )
 
 
-class InquiriesListAllResponseDataItemRelationshipsSessions(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesListAllResponseDataItemRelationshipsSessionsDataItem]]
+class CreateACaseResponseIncludedItemRelationshipsSessions(pydantic.BaseModel):
+    data: typing.Optional[typing.List[CreateACaseResponseIncludedItemRelationshipsSessionsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_sessions_data_item.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_request_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseDataItemRelationshipsSessionsDataItem(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
+class ApproveAnInquiryRequestMeta(pydantic.BaseModel):
+    comment: typing.Optional[str] = pydantic.Field(description=("Comments for auditing purposes\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item_relationships_template_data import (
-    InquiriesListAllResponseDataItemRelationshipsTemplateData,
+from .list_all_inquiries_response_data_item_relationships_template_data import (
+    ListAllInquiriesResponseDataItemRelationshipsTemplateData,
 )
 
 
-class InquiriesListAllResponseDataItemRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesListAllResponseDataItemRelationshipsTemplateData]
+class ListAllInquiriesResponseDataItemRelationshipsTemplate(pydantic.BaseModel):
+    data: typing.Optional[ListAllInquiriesResponseDataItemRelationshipsTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseDataItemRelationshipsTemplateData(pydantic.BaseModel):
+class ResumeAnInquiryResponseDataRelationshipsTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_list_all_response_data_item_relationships_verifications_data_item import (
-    InquiriesListAllResponseDataItemRelationshipsVerificationsDataItem,
+from .resume_an_inquiry_response_data_relationships_verifications_data_item import (
+    ResumeAnInquiryResponseDataRelationshipsVerificationsDataItem,
 )
 
 
-class InquiriesListAllResponseDataItemRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesListAllResponseDataItemRelationshipsVerificationsDataItem]]
+class ResumeAnInquiryResponseDataRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ResumeAnInquiryResponseDataRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_data_item_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents_data_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseDataItemRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class CreateACaseResponseIncludedItemRelationshipsDocumentsDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_list_all_response_links.py` & `fern_persona-0.0.2/src/persona/types/list_all_accounts_response_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesListAllResponseLinks(pydantic.BaseModel):
+class ListAllAccountsResponseLinks(pydantic.BaseModel):
     prev: typing.Optional[typing.Any]
     next: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response.py` & `fern_persona-0.0.2/src/persona/types/send_an_sms_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_redact_response_data import InquiriesRedactResponseData
+from .send_an_sms_response_data_attributes import SendAnSmsResponseDataAttributes
 
 
-class InquiriesRedactResponse(pydantic.BaseModel):
-    data: typing.Optional[InquiriesRedactResponseData]
+class SendAnSmsResponseData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
+    attributes: typing.Optional[SendAnSmsResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data.py` & `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_redact_response_data_attributes import InquiriesRedactResponseDataAttributes
-from .inquiries_redact_response_data_relationships import InquiriesRedactResponseDataRelationships
+from .list_all_inquiries_response_data_item_relationships_sessions_data_item import (
+    ListAllInquiriesResponseDataItemRelationshipsSessionsDataItem,
+)
 
 
-class InquiriesRedactResponseData(pydantic.BaseModel):
-    type: typing.Optional[str]
-    id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesRedactResponseDataAttributes]
-    relationships: typing.Optional[InquiriesRedactResponseDataRelationships]
+class ListAllInquiriesResponseDataItemRelationshipsSessions(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ListAllInquiriesResponseDataItemRelationshipsSessionsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRedactResponseDataAttributes(pydantic.BaseModel):
+class ReportActionResumeContinuousMonitoringResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
-    subject: typing.Optional[typing.Any]
-    reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
-    expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
+    redacted_at: typing.Optional[typing.Any] = pydantic.Field(alias="redacted-at")
+    report_template_version_name: typing.Optional[str] = pydantic.Field(alias="report-template-version-name")
+    term: typing.Optional[str]
+    matched_lists: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_redact_response_data_relationships_account import InquiriesRedactResponseDataRelationshipsAccount
-from .inquiries_redact_response_data_relationships_reports import InquiriesRedactResponseDataRelationshipsReports
-from .inquiries_redact_response_data_relationships_template import InquiriesRedactResponseDataRelationshipsTemplate
-from .inquiries_redact_response_data_relationships_verifications import (
-    InquiriesRedactResponseDataRelationshipsVerifications,
+from .approve_an_inquiry_response_data_relationships_account import ApproveAnInquiryResponseDataRelationshipsAccount
+from .approve_an_inquiry_response_data_relationships_reports import ApproveAnInquiryResponseDataRelationshipsReports
+from .approve_an_inquiry_response_data_relationships_template import ApproveAnInquiryResponseDataRelationshipsTemplate
+from .approve_an_inquiry_response_data_relationships_verifications import (
+    ApproveAnInquiryResponseDataRelationshipsVerifications,
 )
 
 
-class InquiriesRedactResponseDataRelationships(pydantic.BaseModel):
-    account: typing.Optional[InquiriesRedactResponseDataRelationshipsAccount]
-    template: typing.Optional[InquiriesRedactResponseDataRelationshipsTemplate]
-    reports: typing.Optional[InquiriesRedactResponseDataRelationshipsReports]
-    verifications: typing.Optional[InquiriesRedactResponseDataRelationshipsVerifications]
+class ApproveAnInquiryResponseDataRelationships(pydantic.BaseModel):
+    account: typing.Optional[ApproveAnInquiryResponseDataRelationshipsAccount]
+    template: typing.Optional[ApproveAnInquiryResponseDataRelationshipsTemplate]
+    reports: typing.Optional[ApproveAnInquiryResponseDataRelationshipsReports]
+    verifications: typing.Optional[ApproveAnInquiryResponseDataRelationshipsVerifications]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships_inquiry.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_redact_response_data_relationships_account_data import (
-    InquiriesRedactResponseDataRelationshipsAccountData,
-)
 
 
-class InquiriesRedactResponseDataRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesRedactResponseDataRelationshipsAccountData]
+class RetrieveAPhoneCarrierDatabaseVerificationResponseDataRelationshipsInquiry(pydantic.BaseModel):
+    data: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRedactResponseDataRelationshipsAccountData(pydantic.BaseModel):
+class ReportsAddATagResponseDataRelationshipsReportTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRedactResponseDataRelationshipsReports(pydantic.BaseModel):
+class RedactAnInquiryResponseDataRelationshipsReports(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_redact_response_data_relationships_template_data import (
-    InquiriesRedactResponseDataRelationshipsTemplateData,
+from .add_persona_objects_response_data_relationships_case_template_data import (
+    AddPersonaObjectsResponseDataRelationshipsCaseTemplateData,
 )
 
 
-class InquiriesRedactResponseDataRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesRedactResponseDataRelationshipsTemplateData]
+class AddPersonaObjectsResponseDataRelationshipsCaseTemplate(pydantic.BaseModel):
+    data: typing.Optional[AddPersonaObjectsResponseDataRelationshipsCaseTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRedactResponseDataRelationshipsTemplateData(pydantic.BaseModel):
+class DismissMatchesResponseDataRelationshipsReportTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_redact_response_data_relationships_verifications_data_item import (
-    InquiriesRedactResponseDataRelationshipsVerificationsDataItem,
+from .approve_an_inquiry_response_data_relationships_verifications_data_item import (
+    ApproveAnInquiryResponseDataRelationshipsVerificationsDataItem,
 )
 
 
-class InquiriesRedactResponseDataRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesRedactResponseDataRelationshipsVerificationsDataItem]]
+class ApproveAnInquiryResponseDataRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ApproveAnInquiryResponseDataRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_redact_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRedactResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class ExpireAnInquiryResponseDataRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response.py` & `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_identification_number.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_resume_response_data import InquiriesResumeResponseData
-from .inquiries_resume_response_meta import InquiriesResumeResponseMeta
 
 
-class InquiriesResumeResponse(pydantic.BaseModel):
-    data: typing.Optional[InquiriesResumeResponseData]
-    meta: typing.Optional[InquiriesResumeResponseMeta]
+class GenerateAOneTimeLinkResponseDataAttributesFieldsIdentificationNumber(pydantic.BaseModel):
+    type: typing.Optional[str]
+    value: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data.py` & `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_resume_response_data_attributes import InquiriesResumeResponseDataAttributes
-from .inquiries_resume_response_data_relationships import InquiriesResumeResponseDataRelationships
+from .reports_add_a_tag_response_data_attributes import ReportsAddATagResponseDataAttributes
+from .reports_add_a_tag_response_data_relationships import ReportsAddATagResponseDataRelationships
 
 
-class InquiriesResumeResponseData(pydantic.BaseModel):
+class ReportsAddATagResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesResumeResponseDataAttributes]
-    relationships: typing.Optional[InquiriesResumeResponseDataRelationships]
+    attributes: typing.Optional[ReportsAddATagResponseDataAttributes]
+    relationships: typing.Optional[ReportsAddATagResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesResumeResponseDataAttributes(pydantic.BaseModel):
+class RedactAnInquiryResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     subject: typing.Optional[typing.Any]
     reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
     expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_resume_response_data_relationships_account import InquiriesResumeResponseDataRelationshipsAccount
-from .inquiries_resume_response_data_relationships_reports import InquiriesResumeResponseDataRelationshipsReports
-from .inquiries_resume_response_data_relationships_template import InquiriesResumeResponseDataRelationshipsTemplate
-from .inquiries_resume_response_data_relationships_verifications import (
-    InquiriesResumeResponseDataRelationshipsVerifications,
+from .expire_an_inquiry_response_data_relationships_account import ExpireAnInquiryResponseDataRelationshipsAccount
+from .expire_an_inquiry_response_data_relationships_reports import ExpireAnInquiryResponseDataRelationshipsReports
+from .expire_an_inquiry_response_data_relationships_template import ExpireAnInquiryResponseDataRelationshipsTemplate
+from .expire_an_inquiry_response_data_relationships_verifications import (
+    ExpireAnInquiryResponseDataRelationshipsVerifications,
 )
 
 
-class InquiriesResumeResponseDataRelationships(pydantic.BaseModel):
-    account: typing.Optional[InquiriesResumeResponseDataRelationshipsAccount]
-    template: typing.Optional[InquiriesResumeResponseDataRelationshipsTemplate]
-    reports: typing.Optional[InquiriesResumeResponseDataRelationshipsReports]
-    verifications: typing.Optional[InquiriesResumeResponseDataRelationshipsVerifications]
+class ExpireAnInquiryResponseDataRelationships(pydantic.BaseModel):
+    account: typing.Optional[ExpireAnInquiryResponseDataRelationshipsAccount]
+    template: typing.Optional[ExpireAnInquiryResponseDataRelationshipsTemplate]
+    reports: typing.Optional[ExpireAnInquiryResponseDataRelationshipsReports]
+    verifications: typing.Optional[ExpireAnInquiryResponseDataRelationshipsVerifications]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_resume_response_data_relationships_account_data import (
-    InquiriesResumeResponseDataRelationshipsAccountData,
+from .assign_a_case_response_data_relationships_case_template_data import (
+    AssignACaseResponseDataRelationshipsCaseTemplateData,
 )
 
 
-class InquiriesResumeResponseDataRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesResumeResponseDataRelationshipsAccountData]
+class AssignACaseResponseDataRelationshipsCaseTemplate(pydantic.BaseModel):
+    data: typing.Optional[AssignACaseResponseDataRelationshipsCaseTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesResumeResponseDataRelationshipsAccountData(pydantic.BaseModel):
+class RedactAnInquiryResponseDataRelationshipsTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_reports.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesResumeResponseDataRelationshipsReports(pydantic.BaseModel):
+class ApproveAnInquiryResponseDataRelationshipsReports(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_resume_response_data_relationships_template_data import (
-    InquiriesResumeResponseDataRelationshipsTemplateData,
+from .reports_set_all_tags_response_data_relationships_report_template_data import (
+    ReportsSetAllTagsResponseDataRelationshipsReportTemplateData,
 )
 
 
-class InquiriesResumeResponseDataRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesResumeResponseDataRelationshipsTemplateData]
+class ReportsSetAllTagsResponseDataRelationshipsReportTemplate(pydantic.BaseModel):
+    data: typing.Optional[ReportsSetAllTagsResponseDataRelationshipsReportTemplateData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesResumeResponseDataRelationshipsTemplateData(pydantic.BaseModel):
+class ExpireAnInquiryResponseDataRelationshipsTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_resume_response_data_relationships_verifications_data_item import (
-    InquiriesResumeResponseDataRelationshipsVerificationsDataItem,
+from .expire_an_inquiry_response_data_relationships_verifications_data_item import (
+    ExpireAnInquiryResponseDataRelationshipsVerificationsDataItem,
 )
 
 
-class InquiriesResumeResponseDataRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesResumeResponseDataRelationshipsVerificationsDataItem]]
+class ExpireAnInquiryResponseDataRelationshipsVerifications(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ExpireAnInquiryResponseDataRelationshipsVerificationsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesResumeResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class ReportActionResumeContinuousMonitoringResponseDataRelationshipsReportTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_resume_response_meta.py` & `fern_persona-0.0.2/src/persona/types/remove_a_tag_request_meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesResumeResponseMeta(pydantic.BaseModel):
-    session_token: typing.Optional[str] = pydantic.Field(alias="session-token")
+class RemoveATagRequestMeta(pydantic.BaseModel):
+    tag_name: typing.Optional[str] = pydantic.Field(alias="tag-name")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data import InquiriesRetrieveResponseData
-from .inquiries_retrieve_response_included_item import InquiriesRetrieveResponseIncludedItem
+from .retrieve_a_report_response_data_attributes import RetrieveAReportResponseDataAttributes
 
 
-class InquiriesRetrieveResponse(pydantic.BaseModel):
-    data: typing.Optional[InquiriesRetrieveResponseData]
-    included: typing.Optional[typing.List[InquiriesRetrieveResponseIncludedItem]]
+class RetrieveAReportResponseData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
+    attributes: typing.Optional[RetrieveAReportResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data.py` & `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_attributes import InquiriesRetrieveResponseDataAttributes
-from .inquiries_retrieve_response_data_relationships import InquiriesRetrieveResponseDataRelationships
+from .assign_a_case_response_data_attributes import AssignACaseResponseDataAttributes
+from .assign_a_case_response_data_relationships import AssignACaseResponseDataRelationships
 
 
-class InquiriesRetrieveResponseData(pydantic.BaseModel):
+class AssignACaseResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesRetrieveResponseDataAttributes]
-    relationships: typing.Optional[InquiriesRetrieveResponseDataRelationships]
+    attributes: typing.Optional[AssignACaseResponseDataAttributes]
+    relationships: typing.Optional[AssignACaseResponseDataRelationships]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_attributes_behaviours import InquiriesRetrieveResponseDataAttributesBehaviours
-from .inquiries_retrieve_response_data_attributes_fields import InquiriesRetrieveResponseDataAttributesFields
+from .retrieve_an_inquiry_response_data_attributes_behaviours import RetrieveAnInquiryResponseDataAttributesBehaviours
+from .retrieve_an_inquiry_response_data_attributes_fields import RetrieveAnInquiryResponseDataAttributesFields
 
 
-class InquiriesRetrieveResponseDataAttributes(pydantic.BaseModel):
+class RetrieveAnInquiryResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     reference_id: typing.Optional[typing.Any] = pydantic.Field(alias="reference-id")
-    behaviours: typing.Optional[InquiriesRetrieveResponseDataAttributesBehaviours]
+    behaviours: typing.Optional[RetrieveAnInquiryResponseDataAttributesBehaviours]
     tags: typing.Optional[typing.List[str]]
     creator: typing.Optional[str]
     reviewer_comment: typing.Optional[typing.Any] = pydantic.Field(alias="reviewer-comment")
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     started_at: typing.Optional[str] = pydantic.Field(alias="started-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
     failed_at: typing.Optional[typing.Any] = pydantic.Field(alias="failed-at")
     marked_for_review_at: typing.Optional[typing.Any] = pydantic.Field(alias="marked-for-review-at")
     decisioned_at: typing.Optional[typing.Any] = pydantic.Field(alias="decisioned-at")
     expired_at: typing.Optional[typing.Any] = pydantic.Field(alias="expired-at")
     redacted_at: typing.Optional[typing.Any] = pydantic.Field(alias="redacted-at")
     previous_step_name: typing.Optional[str] = pydantic.Field(alias="previous-step-name")
     next_step_name: typing.Optional[str] = pydantic.Field(alias="next-step-name")
-    fields: typing.Optional[InquiriesRetrieveResponseDataAttributesFields]
+    fields: typing.Optional[RetrieveAnInquiryResponseDataAttributesFields]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_behaviours.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_behaviours.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataAttributesBehaviours(pydantic.BaseModel):
+class RetrieveAnInquiryResponseDataAttributesBehaviours(pydantic.BaseModel):
     request_spoof_attempts: typing.Optional[int] = pydantic.Field(alias="request-spoof-attempts")
     user_agent_spoof_attempts: typing.Optional[int] = pydantic.Field(alias="user-agent-spoof-attempts")
     distraction_events: typing.Optional[int] = pydantic.Field(alias="distraction-events")
     hesitation_baseline: typing.Optional[int] = pydantic.Field(alias="hesitation-baseline")
     hesitation_count: typing.Optional[int] = pydantic.Field(alias="hesitation-count")
     hesitation_time: typing.Optional[int] = pydantic.Field(alias="hesitation-time")
     shortcut_copies: typing.Optional[int] = pydantic.Field(alias="shortcut-copies")
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_fields.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_attributes_fields_name_first import (
-    InquiriesRetrieveResponseDataAttributesFieldsNameFirst,
+from .retrieve_an_inquiry_response_data_attributes_fields_name_first import (
+    RetrieveAnInquiryResponseDataAttributesFieldsNameFirst,
 )
-from .inquiries_retrieve_response_data_attributes_fields_name_last import (
-    InquiriesRetrieveResponseDataAttributesFieldsNameLast,
+from .retrieve_an_inquiry_response_data_attributes_fields_name_last import (
+    RetrieveAnInquiryResponseDataAttributesFieldsNameLast,
 )
 
 
-class InquiriesRetrieveResponseDataAttributesFields(pydantic.BaseModel):
-    name_first: typing.Optional[InquiriesRetrieveResponseDataAttributesFieldsNameFirst] = pydantic.Field(
+class RetrieveAnInquiryResponseDataAttributesFields(pydantic.BaseModel):
+    name_first: typing.Optional[RetrieveAnInquiryResponseDataAttributesFieldsNameFirst] = pydantic.Field(
         alias="name-first"
     )
-    name_last: typing.Optional[InquiriesRetrieveResponseDataAttributesFieldsNameLast] = pydantic.Field(
+    name_last: typing.Optional[RetrieveAnInquiryResponseDataAttributesFieldsNameLast] = pydantic.Field(
         alias="name-last"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_fields_name_first.py` & `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_last.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataAttributesFieldsNameFirst(pydantic.BaseModel):
+class GenerateAOneTimeLinkResponseDataAttributesFieldsNameLast(pydantic.BaseModel):
     type: typing.Optional[str]
-    value: typing.Optional[str]
+    value: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_attributes_fields_name_last.py` & `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_postal_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataAttributesFieldsNameLast(pydantic.BaseModel):
+class GenerateAOneTimeLinkResponseDataAttributesFieldsAddressPostalCode(pydantic.BaseModel):
     type: typing.Optional[str]
-    value: typing.Optional[str]
+    value: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_account.py` & `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_relationships_account_data import (
-    InquiriesRetrieveResponseDataRelationshipsAccountData,
+from .create_a_name_list_item_response_data_relationships_creator import (
+    CreateANameListItemResponseDataRelationshipsCreator,
 )
 
 
-class InquiriesRetrieveResponseDataRelationshipsAccount(pydantic.BaseModel):
-    data: typing.Optional[InquiriesRetrieveResponseDataRelationshipsAccountData]
+class CreateANameListItemResponseDataRelationships(pydantic.BaseModel):
+    creator: typing.Optional[CreateANameListItemResponseDataRelationshipsCreator]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_account_data.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataRelationshipsAccountData(pydantic.BaseModel):
+class RetrieveAnInquiryResponseDataRelationshipsAccountData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_reports.py` & `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataRelationshipsReports(pydantic.BaseModel):
+class UpdateACaseResponseDataRelationshipsAccounts(pydantic.BaseModel):
     data: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_sessions.py` & `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_relationships_sessions_data_item import (
-    InquiriesRetrieveResponseDataRelationshipsSessionsDataItem,
+from .retrieve_case_response_data_relationships_case_comments_data_item import (
+    RetrieveCaseResponseDataRelationshipsCaseCommentsDataItem,
 )
 
 
-class InquiriesRetrieveResponseDataRelationshipsSessions(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesRetrieveResponseDataRelationshipsSessionsDataItem]]
+class RetrieveCaseResponseDataRelationshipsCaseComments(pydantic.BaseModel):
+    data: typing.Optional[typing.List[RetrieveCaseResponseDataRelationshipsCaseCommentsDataItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_sessions_data_item.py` & `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataRelationshipsSessionsDataItem(pydantic.BaseModel):
+class SubmitAGovernmentIdVerificationResponseDataRelationshipsDocumentData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_template.py` & `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_relationships_template_data import (
-    InquiriesRetrieveResponseDataRelationshipsTemplateData,
+from .approve_an_inquiry_response_data_relationships_account_data import (
+    ApproveAnInquiryResponseDataRelationshipsAccountData,
 )
 
 
-class InquiriesRetrieveResponseDataRelationshipsTemplate(pydantic.BaseModel):
-    data: typing.Optional[InquiriesRetrieveResponseDataRelationshipsTemplateData]
+class ApproveAnInquiryResponseDataRelationshipsAccount(pydantic.BaseModel):
+    data: typing.Optional[ApproveAnInquiryResponseDataRelationshipsAccountData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_template_data.py` & `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataRelationshipsTemplateData(pydantic.BaseModel):
+class ReportsRemoveATagResponseDataRelationshipsReportTemplateData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_verifications.py` & `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_data_relationships_verifications_data_item import (
-    InquiriesRetrieveResponseDataRelationshipsVerificationsDataItem,
+from .create_an_email_address_verification_response_data_attributes import (
+    CreateAnEmailAddressVerificationResponseDataAttributes,
 )
 
 
-class InquiriesRetrieveResponseDataRelationshipsVerifications(pydantic.BaseModel):
-    data: typing.Optional[typing.List[InquiriesRetrieveResponseDataRelationshipsVerificationsDataItem]]
+class CreateAnEmailAddressVerificationResponseData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
+    attributes: typing.Optional[CreateAnEmailAddressVerificationResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseDataRelationshipsVerificationsDataItem(pydantic.BaseModel):
+class SubmitAGovernmentIdDocumentResponseDataRelationshipsInquiryData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_included_item.py` & `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies_data_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_retrieve_response_included_item_attributes import InquiriesRetrieveResponseIncludedItemAttributes
 
 
-class InquiriesRetrieveResponseIncludedItem(pydantic.BaseModel):
+class CreateACaseResponseIncludedItemRelationshipsSelfiesDataItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[InquiriesRetrieveResponseIncludedItemAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_retrieve_response_included_item_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesRetrieveResponseIncludedItemAttributes(pydantic.BaseModel):
+class RetrieveAnInquiryResponseIncludedItemAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
     country_code: typing.Optional[str] = pydantic.Field(alias="country-code")
     name_first: typing.Optional[str] = pydantic.Field(alias="name-first")
     name_middle: typing.Optional[typing.Any] = pydantic.Field(alias="name-middle")
     name_last: typing.Optional[str] = pydantic.Field(alias="name-last")
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_update_request_data.py` & `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .inquiries_update_request_data_attributes import InquiriesUpdateRequestDataAttributes
+from .create_a_geolocation_list_item_response_data import CreateAGeolocationListItemResponseData
 
 
-class InquiriesUpdateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[InquiriesUpdateRequestDataAttributes]
+class CreateAGeolocationListItemResponse(pydantic.BaseModel):
+    data: typing.Optional[CreateAGeolocationListItemResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/inquiries_update_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InquiriesUpdateRequestDataAttributes(pydantic.BaseModel):
+class UpdateAnInquiryRequestDataAttributes(pydantic.BaseModel):
     identification_number: typing.Optional[str] = pydantic.Field(
         alias="identification-number", description=("Identification numbers, i.e. SSN\n")
     )
     locale: typing.Optional[str]
     selected_country_code: typing.Optional[str] = pydantic.Field(alias="selected-country-code")
     name_first: typing.Optional[str] = pydantic.Field(alias="name-first")
     name_middle: typing.Optional[str] = pydantic.Field(alias="name-middle")
```

### Comparing `fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_request_data.py` & `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .phone_number_verifications_create_request_data_attributes import (
-    PhoneNumberVerificationsCreateRequestDataAttributes,
+from .confirm_a_phone_number_verification_request_data_attributes import (
+    ConfirmAPhoneNumberVerificationRequestDataAttributes,
 )
 
 
-class PhoneNumberVerificationsCreateRequestData(pydantic.BaseModel):
-    attributes: typing.Optional[PhoneNumberVerificationsCreateRequestDataAttributes]
+class ConfirmAPhoneNumberVerificationRequestData(pydantic.BaseModel):
+    attributes: typing.Optional[ConfirmAPhoneNumberVerificationRequestDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_request_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data_attributes.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class PhoneNumberVerificationsCreateRequestDataAttributes(pydantic.BaseModel):
+class CreateAPhoneNumberVerificationRequestDataAttributes(pydantic.BaseModel):
     verification_template_id: str = pydantic.Field(
         alias="verification-template-id",
         description=(
             'ID of Verification Template. You can find your Verification Template IDs [here](https://app.withpersona.com/dashboard/verification-templates?filter=%7B%22type%22%3A%5B%22verification-template%2Fphone-number"%5D%7D)\n'
         ),
     )
     phone_number: str = pydantic.Field(
```

### Comparing `fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .phone_number_verifications_create_response_data import PhoneNumberVerificationsCreateResponseData
+from .retrieve_a_database_verification_response_data import RetrieveADatabaseVerificationResponseData
 
 
-class PhoneNumberVerificationsCreateResponse(pydantic.BaseModel):
-    data: typing.Optional[PhoneNumberVerificationsCreateResponseData]
+class RetrieveADatabaseVerificationResponse(pydantic.BaseModel):
+    data: typing.Optional[RetrieveADatabaseVerificationResponseData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response_data.py` & `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .phone_number_verifications_create_response_data_attributes import (
-    PhoneNumberVerificationsCreateResponseDataAttributes,
+from .confirm_a_phone_number_verification_1_response_data_attributes import (
+    ConfirmAPhoneNumberVerification1ResponseDataAttributes,
 )
 
 
-class PhoneNumberVerificationsCreateResponseData(pydantic.BaseModel):
+class ConfirmAPhoneNumberVerification1ResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[PhoneNumberVerificationsCreateResponseDataAttributes]
+    attributes: typing.Optional[ConfirmAPhoneNumberVerification1ResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .phone_number_verifications_create_response_data_attributes_metadata import (
-    PhoneNumberVerificationsCreateResponseDataAttributesMetadata,
+from .create_a_phone_number_verification_response_data_attributes_metadata import (
+    CreateAPhoneNumberVerificationResponseDataAttributesMetadata,
 )
 
 
-class PhoneNumberVerificationsCreateResponseDataAttributes(pydantic.BaseModel):
+class CreateAPhoneNumberVerificationResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     created_at_ts: typing.Optional[int] = pydantic.Field(alias="created-at-ts")
     submitted_at: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at")
     submitted_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="submitted-at-ts")
     completed_at: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at")
     completed_at_ts: typing.Optional[typing.Any] = pydantic.Field(alias="completed-at-ts")
     country_code: typing.Optional[str] = pydantic.Field(alias="country-code")
     confirmation_code: typing.Optional[str] = pydantic.Field(alias="confirmation-code")
     phone_number: typing.Optional[str] = pydantic.Field(alias="phone-number")
-    metadata: typing.Optional[PhoneNumberVerificationsCreateResponseDataAttributesMetadata]
+    metadata: typing.Optional[CreateAPhoneNumberVerificationResponseDataAttributesMetadata]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/phone_number_verifications_create_response_data_attributes_metadata.py` & `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class PhoneNumberVerificationsCreateResponseDataAttributesMetadata(pydantic.BaseModel):
+class ConfirmAPhoneNumberVerification1ResponseDataAttributesMetadata(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `fern_persona-0.0.1/src/persona/types/reports_redact_response.py` & `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .reports_redact_response_data import ReportsRedactResponseData
 
 
-class ReportsRedactResponse(pydantic.BaseModel):
-    data: typing.Optional[ReportsRedactResponseData]
+class ReportActionPauseContinuousMonitoringResponseDataRelationshipsReportTemplateData(pydantic.BaseModel):
+    type: typing.Optional[str]
+    id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/reports_redact_response_data.py` & `fern_persona-0.0.2/src/persona/types/create_an_account_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .reports_redact_response_data_attributes import ReportsRedactResponseDataAttributes
+from .create_an_account_response_data_attributes import CreateAnAccountResponseDataAttributes
 
 
-class ReportsRedactResponseData(pydantic.BaseModel):
+class CreateAnAccountResponseData(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ReportsRedactResponseDataAttributes]
+    attributes: typing.Optional[CreateAnAccountResponseDataAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/reports_redact_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ReportsRedactResponseDataAttributes(pydantic.BaseModel):
+class ReportActionPauseContinuousMonitoringResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
-    redacted_at: typing.Optional[str] = pydantic.Field(alias="redacted-at")
+    redacted_at: typing.Optional[typing.Any] = pydantic.Field(alias="redacted-at")
     report_template_version_name: typing.Optional[str] = pydantic.Field(alias="report-template-version-name")
-    result: typing.Optional[typing.List[typing.Any]]
+    term: typing.Optional[str]
+    matched_lists: typing.Optional[typing.List[typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/reports_retrieve_response.py` & `fern_persona-0.0.2/src/persona/types/add_a_tag_request_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .reports_retrieve_response_data import ReportsRetrieveResponseData
 
 
-class ReportsRetrieveResponse(pydantic.BaseModel):
-    data: typing.Optional[ReportsRetrieveResponseData]
+class AddATagRequestMeta(pydantic.BaseModel):
+    tag_name: typing.Optional[str] = pydantic.Field(alias="tag-name")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `fern_persona-0.0.1/src/persona/types/reports_retrieve_response_data.py` & `fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .reports_retrieve_response_data_attributes import ReportsRetrieveResponseDataAttributes
+from .retrieve_case_response_included_item_attributes import RetrieveCaseResponseIncludedItemAttributes
 
 
-class ReportsRetrieveResponseData(pydantic.BaseModel):
+class RetrieveCaseResponseIncludedItem(pydantic.BaseModel):
     type: typing.Optional[str]
     id: typing.Optional[str]
-    attributes: typing.Optional[ReportsRetrieveResponseDataAttributes]
+    attributes: typing.Optional[RetrieveCaseResponseIncludedItemAttributes]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_persona-0.0.1/src/persona/types/reports_retrieve_response_data_attributes.py` & `fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ReportsRetrieveResponseDataAttributes(pydantic.BaseModel):
+class RetrieveAReportResponseDataAttributes(pydantic.BaseModel):
     status: typing.Optional[str]
     created_at: typing.Optional[str] = pydantic.Field(alias="created-at")
     completed_at: typing.Optional[str] = pydantic.Field(alias="completed-at")
     name_first: typing.Optional[str] = pydantic.Field(alias="name-first")
     name_last: typing.Optional[str] = pydantic.Field(alias="name-last")
     birthdate: typing.Optional[str]
     address_street_1: typing.Optional[str] = pydantic.Field(alias="address-street-1")
```

### Comparing `fern_persona-0.0.1/src/persona/types/unprocessable_entity_error_body.py` & `fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.1/src/persona/types/unprocessable_entity_error_body_errors_item.py` & `fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body_errors_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.1/PKG-INFO` & `fern_persona-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-persona
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

