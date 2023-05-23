# Comparing `tmp/regula.documentreader.webclient-6.7.2.tar.gz` & `tmp/regula.documentreader.webclient-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regula.documentreader.webclient-6.7.2.tar", last modified: Thu Mar 23 13:31:12 2023, max compression
+gzip compressed data, was "regula.documentreader.webclient-6.8.0.tar", last modified: Tue May 23 14:36:30 2023, max compression
```

## Comparing `regula.documentreader.webclient-6.7.2.tar` & `regula.documentreader.webclient-6.8.0.tar`

### file list

```diff
@@ -1,175 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.971040 regula.documentreader.webclient-6.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-23 13:31:12.971040 regula.documentreader.webclient-6.7.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.931040 regula.documentreader.webclient-6.7.2/regula/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.935040 regula.documentreader.webclient-6.7.2/regula/documentreader/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.935040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/
--rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.935040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.935040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2104 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/api/document_reader_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.935040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.939040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/fiber.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/ident.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/image_ident.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/ocr_security_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/security_feature.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/images.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/raw_result_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/recognition_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2771 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/recognition_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/text_field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.939040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12156 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.939040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5872 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api/process_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26739 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16380 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4944 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.971040 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11346 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/area_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/area_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_check_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/bc_pdf417_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/bc_roidetect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/check_diagnose.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/chosen_document_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7627 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/chosen_document_type_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3719 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/container_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/critical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5477 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/data_module.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/details_optical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7940 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/details_rfid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_bar_code_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10823 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7661 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_image_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4049 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_image_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_position_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_position_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18666 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2847 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_type_recognition_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7743 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/fdsid_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/fiber_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/fiber_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9575 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphic_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphic_field_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3670 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphic_fields_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphics_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3582 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphics_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ident_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ident_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_check_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4648 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_available_source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5524 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9852 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_field_value.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9548 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/lcid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7915 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/lexical_analysis_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/license_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/license_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/light.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3484 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/list_verified_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/measure_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/mrz_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ocr_security_text_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/one_candidate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5388 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/original_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/p_array_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/per_document_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/photo_ident_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/point_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/points_container.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54631 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_params.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7804 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4983 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_request_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10150 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4385 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_system_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/processing_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/raw_image_container_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5908 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/rectangle_coordinates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7501 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/result_item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/rfid_location.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5960 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/rfid_origin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/security_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/security_feature_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2816 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/source_validity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8033 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/status_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/status_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3987 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/string_recognition_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5455 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/symbol_candidate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5176 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/symbol_recognition_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7450 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5543 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_available_source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_data_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3740 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_data_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12342 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36546 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_field_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10245 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_field_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_post_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7066 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3394 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_result_all_of.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10687 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/tfdsid_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/transaction_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2905 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/verification_result.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10406 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/verified_field_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/visibility.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12496 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:31:12.935040 regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-23 13:31:12.000000 regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-03-23 13:31:12.000000 regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 13:31:12.000000 regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-23 13:31:12.000000 regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 13:31:12.000000 regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 13:31:12.971040 regula.documentreader.webclient-6.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-23 13:30:32.000000 regula.documentreader.webclient-6.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.233732 regula.documentreader.webclient-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 14:36:30.233732 regula.documentreader.webclient-6.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula/documentreader/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2215 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/api/document_reader_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.209730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/fiber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/ident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/image_ident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/ocr_security_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/security_feature.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/raw_result_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/recognition_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/recognition_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/text_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.209730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12356 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.209730 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5872 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api/process_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26739 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16380 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4944 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.233732 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11546 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/area_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/area_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_check_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/bc_pdf417_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/bc_roidetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/check_diagnose.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/chosen_document_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7627 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/chosen_document_type_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3719 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/container_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/critical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5477 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/data_module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9543 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/details_optical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7940 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/details_rfid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_bar_code_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10823 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7661 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_image_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4049 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_image_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_position_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_position_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18666 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2847 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_type_recognition_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4349 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7743 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3691 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/fdsid_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/fiber_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/fiber_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9575 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphic_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphic_field_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3670 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphic_fields_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphics_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3582 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphics_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ident_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ident_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_check_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4648 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_available_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5524 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10847 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_field_value.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9548 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/lcid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7915 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/lexical_analysis_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3704 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/license_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/license_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/light.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3484 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/list_verified_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/measure_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/mrz_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ocr_security_text_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11554 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/one_candidate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5388 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/original_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/p_array_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/parsing_notification_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/per_document_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/photo_ident_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/point_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/points_container.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55259 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_params_rfid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7804 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4983 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_request_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10150 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4385 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_system_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/processing_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/raw_image_container_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5908 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/rectangle_coordinates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3572 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7501 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/result_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/rfid_location.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5960 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/rfid_origin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/security_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/security_feature_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2816 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/source_validity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8033 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/status_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/status_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3987 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/string_recognition_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5455 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/symbol_candidate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5176 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/symbol_recognition_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7450 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5543 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_available_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7599 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_data_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3740 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_data_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12342 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37465 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_field_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10245 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_post_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7066 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3394 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_result_all_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10687 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/tfdsid_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5624 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/transaction_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2905 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/verification_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10406 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/verified_field_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/visibility.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12496 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:36:30.205730 regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-23 14:36:30.000000 regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-23 14:36:30.000000 regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:36:30.000000 regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 14:36:30.000000 regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 14:36:30.000000 regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:36:30.233732 regula.documentreader.webclient-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 14:35:53.000000 regula.documentreader.webclient-6.8.0/setup.py
```

### Comparing `regula.documentreader.webclient-6.7.2/PKG-INFO` & `regula.documentreader.webclient-6.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.documentreader.webclient
-Version: 6.7.2
+Version: 6.8.0
 Summary: Regula's Document Reader python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: document-reader-client,document reader,document recognition,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.documentreader.webclient-6.7.2/README.md` & `regula.documentreader.webclient-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/__init__.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/api/document_reader_api.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/api/document_reader_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.api_client.close()
 
+    def set_configuration(self, configuration) -> None:
+        self.api_client.configuration = configuration
+
     @property
     def license(self) -> Base64String:
         return self.__license
 
     @license.setter
     def license(self, value: Union[Base64String, bytes]):
         if isinstance(value, bytes):
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/__init__.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/__init__.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/authenticity/authenticity_check_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/images.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/images.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/raw_authenticity_result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/raw_result_item.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/raw_result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/recognition_request.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/recognition_request.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/recognition_response.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/recognition_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, List
-from regula.documentreader.webclient import ImageQualityCheckList
+from regula.documentreader.webclient import ImageQualityCheckList, OneCandidate
 from regula.documentreader.webclient.ext.models.authenticity.authenticity_check_list import AuthenticityCheckList
 from regula.documentreader.webclient.ext.models.images import Images
 from regula.documentreader.webclient.ext.models.text import Text
 from regula.documentreader.webclient.gen import ResultItem
 from regula.documentreader.webclient.gen.models.process_response import ProcessResponse
 from regula.documentreader.webclient.gen.models.result import Result
 from regula.documentreader.webclient.gen.models.status import Status
@@ -41,14 +41,18 @@
             return result.authenticity_check_list
         return None
 
     def image_quality_checks(self, page_idx=0) -> Optional[ImageQualityCheckList]:
         result = self.pageable_result_by_type(Result.IMAGE_QUALITY, page_idx)
         return result.image_quality_check_list if result is not None else None
 
+    def document_type(self, page_idx=0) -> Optional[OneCandidate]:
+        result = self.pageable_result_by_type(Result.DOCUMENT_TYPE, page_idx)
+        return result.one_candidate if result else None
+
     def pageable_result_by_type(self, result_type: int, page_idx: int) -> Optional[ResultItem]:
         container_list = self.low_lvl_response.container_list.list
         for response in container_list:
             if response.result_type == result_type and response.page_idx == page_idx:
                 return response
         return None
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/text.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/text.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/ext/models/text_field.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/ext/models/text_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/__init__.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,21 +99,23 @@
 from regula.documentreader.webclient.gen.models.mrz_format import MRZFormat
 from regula.documentreader.webclient.gen.models.measure_system import MeasureSystem
 from regula.documentreader.webclient.gen.models.ocr_security_text_result import OCRSecurityTextResult
 from regula.documentreader.webclient.gen.models.ocr_security_text_result_all_of import OCRSecurityTextResultAllOf
 from regula.documentreader.webclient.gen.models.one_candidate import OneCandidate
 from regula.documentreader.webclient.gen.models.original_symbol import OriginalSymbol
 from regula.documentreader.webclient.gen.models.p_array_field import PArrayField
+from regula.documentreader.webclient.gen.models.parsing_notification_codes import ParsingNotificationCodes
 from regula.documentreader.webclient.gen.models.per_document_config import PerDocumentConfig
 from regula.documentreader.webclient.gen.models.photo_ident_result import PhotoIdentResult
 from regula.documentreader.webclient.gen.models.photo_ident_result_all_of import PhotoIdentResultAllOf
 from regula.documentreader.webclient.gen.models.point import Point
 from regula.documentreader.webclient.gen.models.point_array import PointArray
 from regula.documentreader.webclient.gen.models.points_container import PointsContainer
 from regula.documentreader.webclient.gen.models.process_params import ProcessParams
+from regula.documentreader.webclient.gen.models.process_params_rfid import ProcessParamsRfid
 from regula.documentreader.webclient.gen.models.process_request import ProcessRequest
 from regula.documentreader.webclient.gen.models.process_request_image import ProcessRequestImage
 from regula.documentreader.webclient.gen.models.process_response import ProcessResponse
 from regula.documentreader.webclient.gen.models.process_system_info import ProcessSystemInfo
 from regula.documentreader.webclient.gen.models.processing_status import ProcessingStatus
 from regula.documentreader.webclient.gen.models.raw_image_container_list import RawImageContainerList
 from regula.documentreader.webclient.gen.models.rectangle_coordinates import RectangleCoordinates
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api/default_api.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api/default_api.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api/process_api.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api/process_api.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/api_client.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/api_client.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/configuration.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.7.0\n"\
+               "Version of the API: 6.8.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/exceptions.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/exceptions.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/__init__.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,23 @@
 from regula.documentreader.webclient.gen.models.mrz_format import MRZFormat
 from regula.documentreader.webclient.gen.models.measure_system import MeasureSystem
 from regula.documentreader.webclient.gen.models.ocr_security_text_result import OCRSecurityTextResult
 from regula.documentreader.webclient.gen.models.ocr_security_text_result_all_of import OCRSecurityTextResultAllOf
 from regula.documentreader.webclient.gen.models.one_candidate import OneCandidate
 from regula.documentreader.webclient.gen.models.original_symbol import OriginalSymbol
 from regula.documentreader.webclient.gen.models.p_array_field import PArrayField
+from regula.documentreader.webclient.gen.models.parsing_notification_codes import ParsingNotificationCodes
 from regula.documentreader.webclient.gen.models.per_document_config import PerDocumentConfig
 from regula.documentreader.webclient.gen.models.photo_ident_result import PhotoIdentResult
 from regula.documentreader.webclient.gen.models.photo_ident_result_all_of import PhotoIdentResultAllOf
 from regula.documentreader.webclient.gen.models.point import Point
 from regula.documentreader.webclient.gen.models.point_array import PointArray
 from regula.documentreader.webclient.gen.models.points_container import PointsContainer
 from regula.documentreader.webclient.gen.models.process_params import ProcessParams
+from regula.documentreader.webclient.gen.models.process_params_rfid import ProcessParamsRfid
 from regula.documentreader.webclient.gen.models.process_request import ProcessRequest
 from regula.documentreader.webclient.gen.models.process_request_image import ProcessRequestImage
 from regula.documentreader.webclient.gen.models.process_response import ProcessResponse
 from regula.documentreader.webclient.gen.models.process_system_info import ProcessSystemInfo
 from regula.documentreader.webclient.gen.models.processing_status import ProcessingStatus
 from regula.documentreader.webclient.gen.models.raw_image_container_list import RawImageContainerList
 from regula.documentreader.webclient.gen.models.rectangle_coordinates import RectangleCoordinates
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/area_array.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/area_array.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/area_container.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/area_container.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_check_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_check_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_check_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_check_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_check_result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/authenticity_result_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/authenticity_result_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 
     OCR_SECURITY_TEXT = int("64")
 
     IPI = int("128")
 
     PHOTO_EMBED_TYPE = int("512")
 
-    HOLOGRAMS = int("4096")
+    HOLOGRAMS = int("1024")
+
+    OVI = int("4096")
 
     PHOTO_AREA = int("8192")
 
     PORTRAIT_COMPARISON = int("32768")
 
     BARCODE_FORMAT_CHECK = int("65536")
 
@@ -58,17 +60,17 @@
 
     FINGERPRINT_COMPARISON = int("1048576")
 
     LIVENESS = int("2097152")
 
     EXTENDED_OCR_CHECK = int("4194304")
 
-    MRZ = int("8388608")
+    EXTENDED_MRZ_CHECK = int("8388608")
 
-    allowable_values = [UV_LUMINESCENCE, IR_B900, IMAGE_PATTERN, AXIAL_PROTECTION, UV_FIBERS, IR_VISIBILITY, OCR_SECURITY_TEXT, IPI, PHOTO_EMBED_TYPE, HOLOGRAMS, PHOTO_AREA, PORTRAIT_COMPARISON, BARCODE_FORMAT_CHECK, KINEGRAM, LETTER_SCREEN, HOLOGRAM_DETECTION, FINGERPRINT_COMPARISON, LIVENESS, EXTENDED_OCR_CHECK, MRZ]  # noqa: E501
+    allowable_values = [UV_LUMINESCENCE, IR_B900, IMAGE_PATTERN, AXIAL_PROTECTION, UV_FIBERS, IR_VISIBILITY, OCR_SECURITY_TEXT, IPI, PHOTO_EMBED_TYPE, HOLOGRAMS, OVI, PHOTO_AREA, PORTRAIT_COMPARISON, BARCODE_FORMAT_CHECK, KINEGRAM, LETTER_SCREEN, HOLOGRAM_DETECTION, FINGERPRINT_COMPARISON, LIVENESS, EXTENDED_OCR_CHECK, EXTENDED_MRZ_CHECK]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/bc_pdf417_info.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/bc_pdf417_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/bc_roidetect.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/bc_roidetect.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/check_diagnose.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/check_diagnose.py`

 * *Files 15% similar despite different names*

```diff
@@ -102,14 +102,24 @@
 
     BAD_AREA_IN_AXIAL = int("60")
 
     FALSE_IP_PARAMETERS = int("65")
 
     FIELD_POS_CORRECTOR_HIGHLIGHT_IR = int("80")
 
+    FIELD_POS_CORRECTOR_GLARES_IN_PHOTO_AREA = int("81")
+
+    FIELD_POS_CORRECTOR_PHOTO_REPLACED = int("82")
+
+    FIELD_POS_CORRECTOR_LANDMARKS_CHECK_ERROR = int("83")
+
+    FIELD_POS_CORRECTOR_FACE_PRESENCE_CHECK_ERROR = int("84")
+
+    FIELD_POS_CORRECTOR_FACE_ABSENCE_CHECK_ERROR = int("85")
+
     OVI_IR_INVISIBLE = int("90")
 
     OVI_INSUFFICIENT_AREA = int("91")
 
     OVI_COLOR_INVARIABLE = int("92")
 
     OVI_BAD_COLOR_FRONT = int("93")
@@ -122,14 +132,18 @@
 
     HOLOGRAM_ELEMENT_ABSENT = int("100")
 
     HOLOGRAM_SIDE_TOP_IMAGES_ABSENT = int("101")
 
     HOLOGRAM_ELEMENT_PRESENT = int("102")
 
+    HOLOGRAM_FRAMES_IS_ABSENT = int("103")
+
+    HOLOGRAM_HOLO_FIELD_IS_ABSENT = int("104")
+
     PHOTO_PATTERN_INTERRUPTED = int("110")
 
     PHOTO_PATTERN_SHIFTED = int("111")
 
     PHOTO_PATTERN_DIFFERENT_COLORS = int("112")
 
     PHOTO_PATTERN_IR_VISIBLE = int("113")
@@ -146,14 +160,16 @@
 
     PHOTO_PATTERN_DIFFERENT_LINES_THICKNESS = int("119")
 
     PHOTO_IS_NOT_RECTANGLE = int("120")
 
     PHOTO_CORNERS_IS_WRONG = int("121")
 
+    DOCUMENT_IS_CANCELLING = int("122")
+
     TEXT_COLOR_SHOULD_BE_BLUE = int("130")
 
     TEXT_COLOR_SHOULD_BE_GREEN = int("131")
 
     TEXT_COLOR_SHOULD_BE_RED = int("132")
 
     TEXT_SHOULD_BE_BLACK = int("133")
@@ -176,50 +192,14 @@
 
     PORTRAIT_COMPARISON_NO_LIVE_PHOTO = int("154")
 
     PORTRAIT_COMPARISON_NO_SERVICE_LICENSE = int("155")
 
     PORTRAIT_COMPARISON_NO_PORTRAIT_DETECTED = int("156")
 
-    FIELD_POS_CORRECTOR_PHOTO_REPLACED = int("82")
-
-    SCREEN_CAPTURE_DETECTED = int("191")
-
-    ELECTRONIC_DEVICE_DETECTED = int("192")
-
-    FIELD_POS_CORRECTOR_LANDMARKS_CHECK_ERROR = int("83")
-
-    FIELD_POS_CORRECTOR_FACE_PRESENCE_CHECK_ERROR = int("84")
-
-    FIELD_POS_CORRECTOR_FACE_ABSENCE_CHECK_ERROR = int("85")
-
-    WRONG_SYMBOL_BACKGROUND = int("200")
-
-    WRONG_BACKGROUND = int("201")
-
-    WRONG_MRZ_WIDTH = int("202")
-
-    WRONG_MRZ_HEIGHT = int("203")
-
-    WRONG_LINE_POSITION = int("204")
-
-    TEXT_POSITION = int("220")
-
-    INVALID_FONT = int("221")
-
-    INVALID_BACKGROUND = int("222")
-
-    FIELD_POS_CORRECTOR_GLARES_IN_PHOTO_AREA = int("81")
-
-    HOLOGRAM_FRAMES_IS_ABSENT = int("103")
-
-    HOLOGRAM_HOLO_FIELD_IS_ABSENT = int("104")
-
-    DOCUMENT_IS_CANCELLING = int("122")
-
     MOBILE_IMAGES_UNSUITABLE_LIGHT_CONDITIONS = int("160")
 
     MOBILE_IMAGES_WHITE_UV_NO_DIFFERENCE = int("161")
 
     FINGERPRINTS_COMPARISON_MISMATCH = int("170")
 
     HOLO_PHOTO_FACE_NOT_DETECTED = int("180")
@@ -236,19 +216,39 @@
 
     HOLO_PHOTO_FINISHED_BY_TIMEOUT = int("186")
 
     HOLO_PHOTO_DOCUMENT_OUTSIDE_FRAME = int("187")
 
     LIVENESS_DEPTH_CHECK_FAILED = int("190")
 
-    LAS_INK_INVALID_LINES_FREQUENCY = int("230")
+    MRZ_QUALITY_WRONG_SYMBOL_POSITION = int("200")
+
+    MRZ_QUALITY_WRONG_BACKGROUND = int("201")
+
+    MRZ_QUALITY_WRONG_MRZ_WIDTH = int("202")
+
+    MRZ_QUALITY_WRONG_MRZ_HEIGHT = int("203")
+
+    MRZ_QUALITY_WRONG_LINE_POSITION = int("204")
+
+    MRZ_QUALITY_WRONG_FONT_TYPE = int("205")
+
+    OCR_QUALITY_TEXT_POSITION = int("220")
+
+    OCR_QUALITY_INVALID_FONT = int("221")
+
+    OCR_QUALITY_INVALID_BACKGROUND = int("222")
+
+    LASINK_INVALID_LINES_FREQUENCY = int("230")
+
+    DOC_LIVENESS_ELECTRONIC_DEVICE_DETECTED = int("240")
 
-    LAST_DIAGNOSE_VALUE = int("240")
+    LAST_DIAGNOSE_VALUE = int("250")
 
-    allowable_values = [UNKNOWN, PASS, INVALID_INPUT_DATA, INTERNAL_ERROR, EXCEPTION_IN_MODULE, UNCERTAIN_VERIFICATION, NECESSARY_IMAGE_NOT_FOUND, PHOTO_SIDES_NOT_FOUND, INVALID_CHECKSUM, SYNTAX_ERROR, LOGIC_ERROR, SOURCES_COMPARISON_ERROR, FIELDS_COMPARISON_LOGIC_ERROR, INVALID_FIELD_FORMAT, TRUE_LUMINESCENCE_ERROR, FALSE_LUMINESCENCE_ERROR, FIXED_PATTERN_ERROR, LOW_CONTRAST_IN_IR_LIGHT, INCORRECT_BACKGROUND_LIGHT, BACKGROUND_COMPARISON_ERROR, INCORRECT_TEXT_COLOR, PHOTO_FALSE_LUMINESCENCE, TOO_MUCH_SHIFT, FIBERS_NOT_FOUND, TOO_MANY_OBJECTS, SPECKS_IN_UV, TOO_LOW_RESOLUTION, INVISIBLE_ELEMENT_PRESENT, VISIBLE_ELEMENT_ABSENT, ELEMENT_SHOULD_BE_COLORED, ELEMENT_SHOULD_BE_GRAYSCALE, PHOTO_WHITE_IR_DONT_MATCH, UV_DULL_PAPER_MRZ, FALSE_LUMINESCENCE_IN_MRZ, UV_DULL_PAPER_PHOTO, UV_DULL_PAPER_BLANK, UV_DULL_PAPER_ERROR, FALSE_LUMINESCENCE_IN_BLANK, BAD_AREA_IN_AXIAL, FALSE_IP_PARAMETERS, FIELD_POS_CORRECTOR_HIGHLIGHT_IR, OVI_IR_INVISIBLE, OVI_INSUFFICIENT_AREA, OVI_COLOR_INVARIABLE, OVI_BAD_COLOR_FRONT, OVI_BAD_COLOR_SIDE, OVI_WIDE_COLOR_SPREAD, OVI_BAD_COLOR_PERCENT, HOLOGRAM_ELEMENT_ABSENT, HOLOGRAM_SIDE_TOP_IMAGES_ABSENT, HOLOGRAM_ELEMENT_PRESENT, PHOTO_PATTERN_INTERRUPTED, PHOTO_PATTERN_SHIFTED, PHOTO_PATTERN_DIFFERENT_COLORS, PHOTO_PATTERN_IR_VISIBLE, PHOTO_PATTERN_NOT_INTERSECT, PHOTO_SIZE_IS_WRONG, PHOTO_PATTERN_INVALID_COLOR, PHOTO_PATTERN_SHIFTED_VERT, PHOTO_PATTERN_PATTERN_NOT_FOUND, PHOTO_PATTERN_DIFFERENT_LINES_THICKNESS, PHOTO_IS_NOT_RECTANGLE, PHOTO_CORNERS_IS_WRONG, TEXT_COLOR_SHOULD_BE_BLUE, TEXT_COLOR_SHOULD_BE_GREEN, TEXT_COLOR_SHOULD_BE_RED, TEXT_SHOULD_BE_BLACK, BARCODE_WAS_READ_WITH_ERRORS, BARCODE_DATA_FORMAT_ERROR, BARCODE_SIZE_PARAMS_ERROR, NOT_ALL_BARCODES_READ, PORTRAIT_COMPARISON_PORTRAITS_DIFFER, PORTRAIT_COMPARISON_NO_SERVICE_REPLY, PORTRAIT_COMPARISON_SERVICE_ERROR, PORTRAIT_COMPARISON_NOT_ENOUGH_IMAGES, PORTRAIT_COMPARISON_NO_LIVE_PHOTO, PORTRAIT_COMPARISON_NO_SERVICE_LICENSE, PORTRAIT_COMPARISON_NO_PORTRAIT_DETECTED, FIELD_POS_CORRECTOR_PHOTO_REPLACED, SCREEN_CAPTURE_DETECTED, ELECTRONIC_DEVICE_DETECTED, FIELD_POS_CORRECTOR_LANDMARKS_CHECK_ERROR, FIELD_POS_CORRECTOR_FACE_PRESENCE_CHECK_ERROR, FIELD_POS_CORRECTOR_FACE_ABSENCE_CHECK_ERROR, WRONG_SYMBOL_BACKGROUND, WRONG_BACKGROUND, WRONG_MRZ_WIDTH, WRONG_MRZ_HEIGHT, WRONG_LINE_POSITION, TEXT_POSITION, INVALID_FONT, INVALID_BACKGROUND, FIELD_POS_CORRECTOR_GLARES_IN_PHOTO_AREA, HOLOGRAM_FRAMES_IS_ABSENT, HOLOGRAM_HOLO_FIELD_IS_ABSENT, DOCUMENT_IS_CANCELLING, MOBILE_IMAGES_UNSUITABLE_LIGHT_CONDITIONS, MOBILE_IMAGES_WHITE_UV_NO_DIFFERENCE, FINGERPRINTS_COMPARISON_MISMATCH, HOLO_PHOTO_FACE_NOT_DETECTED, HOLO_PHOTO_FACE_COMPARISON_FAILED, HOLO_PHOTO_GLARE_IN_CENTER_ABSENT, HOLO_PHOTO_HOLO_ELEMENT_SHAPE_ERROR, HOLO_PHOTO_ALGORITHMS_STEPS_ERROR, HOLO_PHOTO_HOLO_AREAS_NOT_LOADED, HOLO_PHOTO_FINISHED_BY_TIMEOUT, HOLO_PHOTO_DOCUMENT_OUTSIDE_FRAME, LIVENESS_DEPTH_CHECK_FAILED, LAS_INK_INVALID_LINES_FREQUENCY, LAST_DIAGNOSE_VALUE]  # noqa: E501
+    allowable_values = [UNKNOWN, PASS, INVALID_INPUT_DATA, INTERNAL_ERROR, EXCEPTION_IN_MODULE, UNCERTAIN_VERIFICATION, NECESSARY_IMAGE_NOT_FOUND, PHOTO_SIDES_NOT_FOUND, INVALID_CHECKSUM, SYNTAX_ERROR, LOGIC_ERROR, SOURCES_COMPARISON_ERROR, FIELDS_COMPARISON_LOGIC_ERROR, INVALID_FIELD_FORMAT, TRUE_LUMINESCENCE_ERROR, FALSE_LUMINESCENCE_ERROR, FIXED_PATTERN_ERROR, LOW_CONTRAST_IN_IR_LIGHT, INCORRECT_BACKGROUND_LIGHT, BACKGROUND_COMPARISON_ERROR, INCORRECT_TEXT_COLOR, PHOTO_FALSE_LUMINESCENCE, TOO_MUCH_SHIFT, FIBERS_NOT_FOUND, TOO_MANY_OBJECTS, SPECKS_IN_UV, TOO_LOW_RESOLUTION, INVISIBLE_ELEMENT_PRESENT, VISIBLE_ELEMENT_ABSENT, ELEMENT_SHOULD_BE_COLORED, ELEMENT_SHOULD_BE_GRAYSCALE, PHOTO_WHITE_IR_DONT_MATCH, UV_DULL_PAPER_MRZ, FALSE_LUMINESCENCE_IN_MRZ, UV_DULL_PAPER_PHOTO, UV_DULL_PAPER_BLANK, UV_DULL_PAPER_ERROR, FALSE_LUMINESCENCE_IN_BLANK, BAD_AREA_IN_AXIAL, FALSE_IP_PARAMETERS, FIELD_POS_CORRECTOR_HIGHLIGHT_IR, FIELD_POS_CORRECTOR_GLARES_IN_PHOTO_AREA, FIELD_POS_CORRECTOR_PHOTO_REPLACED, FIELD_POS_CORRECTOR_LANDMARKS_CHECK_ERROR, FIELD_POS_CORRECTOR_FACE_PRESENCE_CHECK_ERROR, FIELD_POS_CORRECTOR_FACE_ABSENCE_CHECK_ERROR, OVI_IR_INVISIBLE, OVI_INSUFFICIENT_AREA, OVI_COLOR_INVARIABLE, OVI_BAD_COLOR_FRONT, OVI_BAD_COLOR_SIDE, OVI_WIDE_COLOR_SPREAD, OVI_BAD_COLOR_PERCENT, HOLOGRAM_ELEMENT_ABSENT, HOLOGRAM_SIDE_TOP_IMAGES_ABSENT, HOLOGRAM_ELEMENT_PRESENT, HOLOGRAM_FRAMES_IS_ABSENT, HOLOGRAM_HOLO_FIELD_IS_ABSENT, PHOTO_PATTERN_INTERRUPTED, PHOTO_PATTERN_SHIFTED, PHOTO_PATTERN_DIFFERENT_COLORS, PHOTO_PATTERN_IR_VISIBLE, PHOTO_PATTERN_NOT_INTERSECT, PHOTO_SIZE_IS_WRONG, PHOTO_PATTERN_INVALID_COLOR, PHOTO_PATTERN_SHIFTED_VERT, PHOTO_PATTERN_PATTERN_NOT_FOUND, PHOTO_PATTERN_DIFFERENT_LINES_THICKNESS, PHOTO_IS_NOT_RECTANGLE, PHOTO_CORNERS_IS_WRONG, DOCUMENT_IS_CANCELLING, TEXT_COLOR_SHOULD_BE_BLUE, TEXT_COLOR_SHOULD_BE_GREEN, TEXT_COLOR_SHOULD_BE_RED, TEXT_SHOULD_BE_BLACK, BARCODE_WAS_READ_WITH_ERRORS, BARCODE_DATA_FORMAT_ERROR, BARCODE_SIZE_PARAMS_ERROR, NOT_ALL_BARCODES_READ, PORTRAIT_COMPARISON_PORTRAITS_DIFFER, PORTRAIT_COMPARISON_NO_SERVICE_REPLY, PORTRAIT_COMPARISON_SERVICE_ERROR, PORTRAIT_COMPARISON_NOT_ENOUGH_IMAGES, PORTRAIT_COMPARISON_NO_LIVE_PHOTO, PORTRAIT_COMPARISON_NO_SERVICE_LICENSE, PORTRAIT_COMPARISON_NO_PORTRAIT_DETECTED, MOBILE_IMAGES_UNSUITABLE_LIGHT_CONDITIONS, MOBILE_IMAGES_WHITE_UV_NO_DIFFERENCE, FINGERPRINTS_COMPARISON_MISMATCH, HOLO_PHOTO_FACE_NOT_DETECTED, HOLO_PHOTO_FACE_COMPARISON_FAILED, HOLO_PHOTO_GLARE_IN_CENTER_ABSENT, HOLO_PHOTO_HOLO_ELEMENT_SHAPE_ERROR, HOLO_PHOTO_ALGORITHMS_STEPS_ERROR, HOLO_PHOTO_HOLO_AREAS_NOT_LOADED, HOLO_PHOTO_FINISHED_BY_TIMEOUT, HOLO_PHOTO_DOCUMENT_OUTSIDE_FRAME, LIVENESS_DEPTH_CHECK_FAILED, MRZ_QUALITY_WRONG_SYMBOL_POSITION, MRZ_QUALITY_WRONG_BACKGROUND, MRZ_QUALITY_WRONG_MRZ_WIDTH, MRZ_QUALITY_WRONG_MRZ_HEIGHT, MRZ_QUALITY_WRONG_LINE_POSITION, MRZ_QUALITY_WRONG_FONT_TYPE, OCR_QUALITY_TEXT_POSITION, OCR_QUALITY_INVALID_FONT, OCR_QUALITY_INVALID_BACKGROUND, LASINK_INVALID_LINES_FREQUENCY, DOC_LIVENESS_ELECTRONIC_DEVICE_DETECTED, LAST_DIAGNOSE_VALUE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/check_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/check_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/chosen_document_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/chosen_document_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/chosen_document_type_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/chosen_document_type_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/chosen_document_type_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/container_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/container_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/critical.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/critical.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/cross_source_value_comparison.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/data_module.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/data_module.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/details_optical.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/details_optical.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/details_rfid.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/details_rfid.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/device_info.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/device_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_bar_code_info.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_bar_code_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_bar_code_info_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_visual_extended_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/doc_visual_extended_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_format.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_format.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_image.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_image.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_image_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_image_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_image_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_image_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_position.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_position.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_position_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_position_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_position_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_position_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,20 +36,14 @@
 
     SEAMANS_IDENTITY_DOCUMENT = int("15")
 
     IDENTITY_CARD_FOR_RESIDENCE = int("16")
 
     TRAVEL_DOCUMENT = int("17")
 
-    OTHER = int("99")
-
-    VISA_ID2 = int("29")
-
-    VISA_ID3 = int("30")
-
     NATIONAL_IDENTITY_CARD = int("20")
 
     SOCIAL_IDENTITY_CARD = int("21")
 
     ALIENS_IDENTITY_CARD = int("22")
 
     PRIVILEGED_IDENTITY_CARD = int("23")
@@ -60,14 +54,18 @@
 
     EMERGENCY_PASSPORT = int("26")
 
     ALIENS_PASSPORT = int("27")
 
     ALTERNATIVE_IDENTITY_CARD = int("28")
 
+    VISA_ID2 = int("29")
+
+    VISA_ID3 = int("30")
+
     AUTHORIZATION_CARD = int("32")
 
     BEGINNER_PERMIT = int("33")
 
     BORDER_CROSSING_CARD = int("34")
 
     CHAUFFEUR_LICENSE = int("35")
@@ -194,14 +192,16 @@
 
     IDENTITY_CARD_TEMPORARY_VISITOR_UNDER_21 = int("96")
 
     IDENTITY_CARD_UNDER_18 = int("97")
 
     IDENTITY_CARD_UNDER_21 = int("98")
 
+    OTHER = int("99")
+
     IGNITION_INTERLOCK_PERMIT = int("100")
 
     IMMIGRANT_VISA = int("101")
 
     INSTRUCTION_PERMIT = int("102")
 
     INSTRUCTION_PERMIT_UNDER_18 = int("103")
@@ -476,15 +476,15 @@
 
     CERTIFICATE_OF_PROFICIENCY = int("238")
 
     TRADE_LICENSE = int("239")
 
     PASSPORT_PAGE = int("240")
 
-    allowable_values = [NOT_DEFINED, PASSPORT, IDENTITY_CARD, DIPLOMATIC_PASSPORT, SERVICE_PASSPORT, SEAMANS_IDENTITY_DOCUMENT, IDENTITY_CARD_FOR_RESIDENCE, TRAVEL_DOCUMENT, OTHER, VISA_ID2, VISA_ID3, NATIONAL_IDENTITY_CARD, SOCIAL_IDENTITY_CARD, ALIENS_IDENTITY_CARD, PRIVILEGED_IDENTITY_CARD, RESIDENCE_PERMIT_IDENTITY_CARD, ORIGIN_CARD, EMERGENCY_PASSPORT, ALIENS_PASSPORT, ALTERNATIVE_IDENTITY_CARD, AUTHORIZATION_CARD, BEGINNER_PERMIT, BORDER_CROSSING_CARD, CHAUFFEUR_LICENSE, CHAUFFEUR_LICENSE_UNDER_18, CHAUFFEUR_LICENSE_UNDER_21, COMMERCIAL_DRIVING_LICENSE, COMMERCIAL_DRIVING_LICENSE_INSTRUCTIONAL_PERMIT, COMMERCIAL_DRIVING_LICENSE_UNDER_18, COMMERCIAL_DRIVING_LICENSE_UNDER_21, COMMERCIAL_INSTRUCTION_PERMIT, COMMERCIAL_NEW_PERMIT, CONCEALED_CARRY_LICENSE, CONCEALED_FIREARM_PERMIT, CONDITIONAL_DRIVING_LICENSE, DEPARTMENT_OF_VETERANS_AFFAIRS_IDENTITY_CARD, DIPLOMATIC_DRIVING_LICENSE, DRIVING_LICENSE, DRIVING_LICENSE_INSTRUCTIONAL_PERMIT, DRIVING_LICENSE_INSTRUCTIONAL_PERMIT_UNDER_18, DRIVING_LICENSE_INSTRUCTIONAL_PERMIT_UNDER_21, DRIVING_LICENSE_LEARNERS_PERMIT, DRIVING_LICENSE_LEARNERS_PERMIT_UNDER_18, DRIVING_LICENSE_LEARNERS_PERMIT_UNDER_21, DRIVING_LICENSE_NOVICE, DRIVING_LICENSE_NOVICE_UNDER_18, DRIVING_LICENSE_NOVICE_UNDER_21, DRIVING_LICENSE_REGISTERED_OFFENDER, DRIVING_LICENSE_RESTRICTED_UNDER_18, DRIVING_LICENSE_RESTRICTED_UNDER_21, DRIVING_LICENSE_TEMPORARY_VISITOR, DRIVING_LICENSE_TEMPORARY_VISITOR_UNDER_18, DRIVING_LICENSE_TEMPORARY_VISITOR_UNDER_21, DRIVING_LICENSE_UNDER_18, DRIVING_LICENSE_UNDER_21, EMPLOYMENT_DRIVING_PERMIT, ENHANCED_CHAUFFEUR_LICENSE, ENHANCED_CHAUFFEUR_LICENSE_UNDER_18, ENHANCED_CHAUFFEUR_LICENSE_UNDER_21, ENHANCED_COMMERCIAL_DRIVING_LICENSE, ENHANCED_DRIVING_LICENSE, ENHANCED_DRIVING_LICENSE_UNDER_18, ENHANCED_DRIVING_LICENSE_UNDER_21, ENHANCED_IDENTITY_CARD, ENHANCED_IDENTITY_CARD_UNDER_18, ENHANCED_IDENTITY_CARD_UNDER_21, ENHANCED_OPERATORS_LICENSE, FIREARMS_PERMIT, FULL_PROVISIONAL_LICENSE, FULL_PROVISIONAL_LICENSE_UNDER_18, FULL_PROVISIONAL_LICENSE_UNDER_21, GENEVA_CONVENTIONS_IDENTITY_CARD, GRADUATED_DRIVING_LICENSE_UNDER_18, GRADUATED_DRIVING_LICENSE_UNDER_21, GRADUATED_INSTRUCTION_PERMIT_UNDER_18, GRADUATED_INSTRUCTION_PERMIT_UNDER_21, GRADUATED_LICENSE_UNDER_18, GRADUATED_LICENSE_UNDER_21, HANDGUN_CARRY_PERMIT, IDENTITY_AND_PRIVILEGE_CARD, IDENTITY_CARD_MOBILITY_IMPAIRED, IDENTITY_CARD_REGISTERED_OFFENDER, IDENTITY_CARD_TEMPORARY_VISITOR, IDENTITY_CARD_TEMPORARY_VISITOR_UNDER_18, IDENTITY_CARD_TEMPORARY_VISITOR_UNDER_21, IDENTITY_CARD_UNDER_18, IDENTITY_CARD_UNDER_21, IGNITION_INTERLOCK_PERMIT, IMMIGRANT_VISA, INSTRUCTION_PERMIT, INSTRUCTION_PERMIT_UNDER_18, INSTRUCTION_PERMIT_UNDER_21, INTERIM_DRIVING_LICENSE, INTERIM_IDENTITY_CARD, INTERMEDIATE_DRIVING_LICENSE, INTERMEDIATE_DRIVING_LICENSE_UNDER_18, INTERMEDIATE_DRIVING_LICENSE_UNDER_21, JUNIOR_DRIVING_LICENSE, LEARNER_INSTRUCTIONAL_PERMIT, LEARNER_LICENSE, LEARNER_LICENSE_UNDER_18, LEARNER_LICENSE_UNDER_21, LEARNER_PERMIT, LEARNER_PERMIT_UNDER_18, LEARNER_PERMIT_UNDER_21, LIMITED_LICENSE, LIMITED_PERMIT, LIMITED_TERM_DRIVING_LICENSE, LIMITED_TERM_IDENTITY_CARD, LIQUOR_IDENTITY_CARD, NEW_PERMIT, NEW_PERMIT_UNDER_18, NEW_PERMIT_UNDER_21, NON_US_CITIZEN_DRIVING_LICENSE, OCCUPATIONAL_DRIVING_LICENSE, ONEIDA_TRIBE_OF_INDIANS_IDENTITY_CARD, OPERATOR_LICENSE, OPERATOR_LICENSE_UNDER_18, OPERATOR_LICENSE_UNDER_21, PERMANENT_DRIVING_LICENSE, PERMIT_TO_REENTER, PROBATIONARY_AUTO_LICENSE, PROBATIONARY_DRIVING_LICENSE_UNDER_18, PROBATIONARY_DRIVING_LICENSE_UNDER_21, PROBATIONARY_VEHICLE_SALES_PERSON_LICENSE, PROVISIONAL_DRIVING_LICENSE, PROVISIONAL_DRIVING_LICENSE_UNDER_18, PROVISIONAL_DRIVING_LICENSE_UNDER_21, PROVISIONAL_LICENSE, PROVISIONAL_LICENSE_UNDER_18, PROVISIONAL_LICENSE_UNDER_21, PUBLIC_PASSENGER_CHAUFFEUR_LICENSE, RACING_AND_GAMING_COMISSION_CARD, REFUGEE_TRAVEL_DOCUMENT, RENEWAL_PERMIT, RESTRICTED_COMMERCIAL_DRIVER_LICENSE, RESTRICTED_DRIVER_LICENSE, RESTRICTED_PERMIT, SEASONAL_PERMIT, SEASONAL_RESIDENT_IDENTITY_CARD, SEASONAL_CITIZEN_IDENTITY_CARD, SEX_OFFENDER, SOCIAL_SECURITY_CARD, TEMPORARY_DRIVING_LICENSE, TEMPORARY_DRIVING_LICENSE_UNDER_18, TEMPORARY_DRIVING_LICENSE_UNDER_21, TEMPORARY_IDENTITY_CARD, TEMPORARY_INSTRUCTION_PERMIT_IDENTITY_CARD, TEMPORARY_INSTRUCTION_PERMIT_IDENTITY_CARD_UNDER_18, TEMPORARY_INSTRUCTION_PERMIT_IDENTITY_CARD_UNDER_21, TEMPORARY_VISITOR_DRIVING_LICENSE, TEMPORARY_VISITOR_DRIVING_LICENSE_UNDER_18, TEMPORARY_VISITOR_DRIVING_LICENSE_UNDER_21, UNIFORMED_SERVICES_IDENTITY_CARD, VEHICLE_SALES_PERSON_LICENSE, WORKER_IDENTIFICATION_CREDENTIAL, COMMERCIAL_DRIVING_LICENSE_NOVICE, COMMERCIAL_DRIVING_LICENSE_NOVICE_UNDER_18, COMMERCIAL_DRIVING_LICENSE_NOVICE_UNDER_21, PASSPORT_CARD, PASSPORT_RESIDENT_CARD, PERSONAL_IDENTIFICATION_VERIFICATION, TEMPORARY_OPERATOR_LICENSE, DRIVING_LICENSE_UNDER_19, IDENTITY_CARD_UNDER_19, VISA, TEMPORARY_PASSPORT, VOTING_CARD, HEALTH_CARD, CERTIFICATE_OF_CITIZENSHIP, ADDRESS_CARD, AIRPORT_IMMIGRATION_CARD, ALIEN_REGISTRATION_CARD, APEH_CARD, COUPON_TO_DRIVING_LICENSE, CREW_MEMBER_CERTIFICATE, DOCUMENT_FOR_RETURN, E_CARD, EMPLOYMENT_CARD, HKSAR_IMMIGRATION_FORM, IMMIGRANT_CARD, LABOUR_CARD, LAISSEZ_PASSER, LAWYER_IDENTITY_CERTIFICATE, LICENSE_CARD, PASSPORT_STATELESS, PASSPORT_CHILD, PASSPORT_CONSULAR, PASSPORT_DIPLOMATIC_SERVICE, PASSPORT_OFFICIAL, PASSPORT_PROVISIONAL, PASSPORT_SPECIAL, PERMISSION_TO_THE_LOCAL_BORDER_TRAFFIC, REGISTRATION_CERTIFICATE, SEDESOL_CARD, SOCIAL_CARD, TB_CARD, VEHICLE_PASSPORT, W_DOCUMENT, DIPLOMATIC_IDENTITY_CARD, CONSULAR_IDENTITY_CARD, INCOME_TAX_CARD, RESIDENCE_PERMIT, DOCUMENT_OF_IDENTITY, BORDER_CROSSING_PERMIT, PASSPORT_LIMITED_VALIDITY, SIM_CARD, TAX_CARD, COMPANY_CARD, DOMESTIC_PASSPORT, IDENTITY_CERTIFICATE, RESIDENT_ID_CARD, ARMED_FORCES_IDENTITY_CARD, PROFESSIONAL_CARD, REGISTRATION_STAMP, DRIVER_CARD, DRIVER_TRAINING_CERTIFICATE, QUALIFICATION_DRIVING_LICENSE, MEMBERSHIP_CARD, PUBLIC_VEHICLE_DRIVER_AUTHORITY_CARD, MARINE_LICENSE, TEMPORARY_LEARNER_LICENSE, TEMPORARY_COMMERCIAL_DRIVING_LICENSE, INTERIM_INSTRUCTIONAL_PERMIT, CERTIFICATE_OF_COMPETENCY, CERTIFICATE_OF_PROFICIENCY, TRADE_LICENSE, PASSPORT_PAGE]  # noqa: E501
+    allowable_values = [NOT_DEFINED, PASSPORT, IDENTITY_CARD, DIPLOMATIC_PASSPORT, SERVICE_PASSPORT, SEAMANS_IDENTITY_DOCUMENT, IDENTITY_CARD_FOR_RESIDENCE, TRAVEL_DOCUMENT, NATIONAL_IDENTITY_CARD, SOCIAL_IDENTITY_CARD, ALIENS_IDENTITY_CARD, PRIVILEGED_IDENTITY_CARD, RESIDENCE_PERMIT_IDENTITY_CARD, ORIGIN_CARD, EMERGENCY_PASSPORT, ALIENS_PASSPORT, ALTERNATIVE_IDENTITY_CARD, VISA_ID2, VISA_ID3, AUTHORIZATION_CARD, BEGINNER_PERMIT, BORDER_CROSSING_CARD, CHAUFFEUR_LICENSE, CHAUFFEUR_LICENSE_UNDER_18, CHAUFFEUR_LICENSE_UNDER_21, COMMERCIAL_DRIVING_LICENSE, COMMERCIAL_DRIVING_LICENSE_INSTRUCTIONAL_PERMIT, COMMERCIAL_DRIVING_LICENSE_UNDER_18, COMMERCIAL_DRIVING_LICENSE_UNDER_21, COMMERCIAL_INSTRUCTION_PERMIT, COMMERCIAL_NEW_PERMIT, CONCEALED_CARRY_LICENSE, CONCEALED_FIREARM_PERMIT, CONDITIONAL_DRIVING_LICENSE, DEPARTMENT_OF_VETERANS_AFFAIRS_IDENTITY_CARD, DIPLOMATIC_DRIVING_LICENSE, DRIVING_LICENSE, DRIVING_LICENSE_INSTRUCTIONAL_PERMIT, DRIVING_LICENSE_INSTRUCTIONAL_PERMIT_UNDER_18, DRIVING_LICENSE_INSTRUCTIONAL_PERMIT_UNDER_21, DRIVING_LICENSE_LEARNERS_PERMIT, DRIVING_LICENSE_LEARNERS_PERMIT_UNDER_18, DRIVING_LICENSE_LEARNERS_PERMIT_UNDER_21, DRIVING_LICENSE_NOVICE, DRIVING_LICENSE_NOVICE_UNDER_18, DRIVING_LICENSE_NOVICE_UNDER_21, DRIVING_LICENSE_REGISTERED_OFFENDER, DRIVING_LICENSE_RESTRICTED_UNDER_18, DRIVING_LICENSE_RESTRICTED_UNDER_21, DRIVING_LICENSE_TEMPORARY_VISITOR, DRIVING_LICENSE_TEMPORARY_VISITOR_UNDER_18, DRIVING_LICENSE_TEMPORARY_VISITOR_UNDER_21, DRIVING_LICENSE_UNDER_18, DRIVING_LICENSE_UNDER_21, EMPLOYMENT_DRIVING_PERMIT, ENHANCED_CHAUFFEUR_LICENSE, ENHANCED_CHAUFFEUR_LICENSE_UNDER_18, ENHANCED_CHAUFFEUR_LICENSE_UNDER_21, ENHANCED_COMMERCIAL_DRIVING_LICENSE, ENHANCED_DRIVING_LICENSE, ENHANCED_DRIVING_LICENSE_UNDER_18, ENHANCED_DRIVING_LICENSE_UNDER_21, ENHANCED_IDENTITY_CARD, ENHANCED_IDENTITY_CARD_UNDER_18, ENHANCED_IDENTITY_CARD_UNDER_21, ENHANCED_OPERATORS_LICENSE, FIREARMS_PERMIT, FULL_PROVISIONAL_LICENSE, FULL_PROVISIONAL_LICENSE_UNDER_18, FULL_PROVISIONAL_LICENSE_UNDER_21, GENEVA_CONVENTIONS_IDENTITY_CARD, GRADUATED_DRIVING_LICENSE_UNDER_18, GRADUATED_DRIVING_LICENSE_UNDER_21, GRADUATED_INSTRUCTION_PERMIT_UNDER_18, GRADUATED_INSTRUCTION_PERMIT_UNDER_21, GRADUATED_LICENSE_UNDER_18, GRADUATED_LICENSE_UNDER_21, HANDGUN_CARRY_PERMIT, IDENTITY_AND_PRIVILEGE_CARD, IDENTITY_CARD_MOBILITY_IMPAIRED, IDENTITY_CARD_REGISTERED_OFFENDER, IDENTITY_CARD_TEMPORARY_VISITOR, IDENTITY_CARD_TEMPORARY_VISITOR_UNDER_18, IDENTITY_CARD_TEMPORARY_VISITOR_UNDER_21, IDENTITY_CARD_UNDER_18, IDENTITY_CARD_UNDER_21, OTHER, IGNITION_INTERLOCK_PERMIT, IMMIGRANT_VISA, INSTRUCTION_PERMIT, INSTRUCTION_PERMIT_UNDER_18, INSTRUCTION_PERMIT_UNDER_21, INTERIM_DRIVING_LICENSE, INTERIM_IDENTITY_CARD, INTERMEDIATE_DRIVING_LICENSE, INTERMEDIATE_DRIVING_LICENSE_UNDER_18, INTERMEDIATE_DRIVING_LICENSE_UNDER_21, JUNIOR_DRIVING_LICENSE, LEARNER_INSTRUCTIONAL_PERMIT, LEARNER_LICENSE, LEARNER_LICENSE_UNDER_18, LEARNER_LICENSE_UNDER_21, LEARNER_PERMIT, LEARNER_PERMIT_UNDER_18, LEARNER_PERMIT_UNDER_21, LIMITED_LICENSE, LIMITED_PERMIT, LIMITED_TERM_DRIVING_LICENSE, LIMITED_TERM_IDENTITY_CARD, LIQUOR_IDENTITY_CARD, NEW_PERMIT, NEW_PERMIT_UNDER_18, NEW_PERMIT_UNDER_21, NON_US_CITIZEN_DRIVING_LICENSE, OCCUPATIONAL_DRIVING_LICENSE, ONEIDA_TRIBE_OF_INDIANS_IDENTITY_CARD, OPERATOR_LICENSE, OPERATOR_LICENSE_UNDER_18, OPERATOR_LICENSE_UNDER_21, PERMANENT_DRIVING_LICENSE, PERMIT_TO_REENTER, PROBATIONARY_AUTO_LICENSE, PROBATIONARY_DRIVING_LICENSE_UNDER_18, PROBATIONARY_DRIVING_LICENSE_UNDER_21, PROBATIONARY_VEHICLE_SALES_PERSON_LICENSE, PROVISIONAL_DRIVING_LICENSE, PROVISIONAL_DRIVING_LICENSE_UNDER_18, PROVISIONAL_DRIVING_LICENSE_UNDER_21, PROVISIONAL_LICENSE, PROVISIONAL_LICENSE_UNDER_18, PROVISIONAL_LICENSE_UNDER_21, PUBLIC_PASSENGER_CHAUFFEUR_LICENSE, RACING_AND_GAMING_COMISSION_CARD, REFUGEE_TRAVEL_DOCUMENT, RENEWAL_PERMIT, RESTRICTED_COMMERCIAL_DRIVER_LICENSE, RESTRICTED_DRIVER_LICENSE, RESTRICTED_PERMIT, SEASONAL_PERMIT, SEASONAL_RESIDENT_IDENTITY_CARD, SEASONAL_CITIZEN_IDENTITY_CARD, SEX_OFFENDER, SOCIAL_SECURITY_CARD, TEMPORARY_DRIVING_LICENSE, TEMPORARY_DRIVING_LICENSE_UNDER_18, TEMPORARY_DRIVING_LICENSE_UNDER_21, TEMPORARY_IDENTITY_CARD, TEMPORARY_INSTRUCTION_PERMIT_IDENTITY_CARD, TEMPORARY_INSTRUCTION_PERMIT_IDENTITY_CARD_UNDER_18, TEMPORARY_INSTRUCTION_PERMIT_IDENTITY_CARD_UNDER_21, TEMPORARY_VISITOR_DRIVING_LICENSE, TEMPORARY_VISITOR_DRIVING_LICENSE_UNDER_18, TEMPORARY_VISITOR_DRIVING_LICENSE_UNDER_21, UNIFORMED_SERVICES_IDENTITY_CARD, VEHICLE_SALES_PERSON_LICENSE, WORKER_IDENTIFICATION_CREDENTIAL, COMMERCIAL_DRIVING_LICENSE_NOVICE, COMMERCIAL_DRIVING_LICENSE_NOVICE_UNDER_18, COMMERCIAL_DRIVING_LICENSE_NOVICE_UNDER_21, PASSPORT_CARD, PASSPORT_RESIDENT_CARD, PERSONAL_IDENTIFICATION_VERIFICATION, TEMPORARY_OPERATOR_LICENSE, DRIVING_LICENSE_UNDER_19, IDENTITY_CARD_UNDER_19, VISA, TEMPORARY_PASSPORT, VOTING_CARD, HEALTH_CARD, CERTIFICATE_OF_CITIZENSHIP, ADDRESS_CARD, AIRPORT_IMMIGRATION_CARD, ALIEN_REGISTRATION_CARD, APEH_CARD, COUPON_TO_DRIVING_LICENSE, CREW_MEMBER_CERTIFICATE, DOCUMENT_FOR_RETURN, E_CARD, EMPLOYMENT_CARD, HKSAR_IMMIGRATION_FORM, IMMIGRANT_CARD, LABOUR_CARD, LAISSEZ_PASSER, LAWYER_IDENTITY_CERTIFICATE, LICENSE_CARD, PASSPORT_STATELESS, PASSPORT_CHILD, PASSPORT_CONSULAR, PASSPORT_DIPLOMATIC_SERVICE, PASSPORT_OFFICIAL, PASSPORT_PROVISIONAL, PASSPORT_SPECIAL, PERMISSION_TO_THE_LOCAL_BORDER_TRAFFIC, REGISTRATION_CERTIFICATE, SEDESOL_CARD, SOCIAL_CARD, TB_CARD, VEHICLE_PASSPORT, W_DOCUMENT, DIPLOMATIC_IDENTITY_CARD, CONSULAR_IDENTITY_CARD, INCOME_TAX_CARD, RESIDENCE_PERMIT, DOCUMENT_OF_IDENTITY, BORDER_CROSSING_PERMIT, PASSPORT_LIMITED_VALIDITY, SIM_CARD, TAX_CARD, COMPANY_CARD, DOMESTIC_PASSPORT, IDENTITY_CERTIFICATE, RESIDENT_ID_CARD, ARMED_FORCES_IDENTITY_CARD, PROFESSIONAL_CARD, REGISTRATION_STAMP, DRIVER_CARD, DRIVER_TRAINING_CERTIFICATE, QUALIFICATION_DRIVING_LICENSE, MEMBERSHIP_CARD, PUBLIC_VEHICLE_DRIVER_AUTHORITY_CARD, MARINE_LICENSE, TEMPORARY_LEARNER_LICENSE, TEMPORARY_COMMERCIAL_DRIVING_LICENSE, INTERIM_INSTRUCTIONAL_PERMIT, CERTIFICATE_OF_COMPETENCY, CERTIFICATE_OF_PROFICIENCY, TRADE_LICENSE, PASSPORT_PAGE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_type_recognition_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_type_recognition_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/document_types_candidates_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/encrypted_rcl_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/encrypted_rcl_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/fdsid_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/fdsid_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/fiber_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/fiber_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/fiber_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/fiber_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphic_field.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphic_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphic_field_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphic_field_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphic_fields_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphic_fields_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphics_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphics_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/graphics_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/graphics_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ident_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ident_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ident_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ident_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_data.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_data.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_qa.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_qa.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_check.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_check.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_check_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_check_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_check_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_check_type.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/image_quality_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_available_source.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_available_source.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_field.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_field_value.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_field_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,52 +31,57 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'source': 'Source',
         'value': 'str',
         'original_value': 'str',
+        'original_page_index': 'int',
         'page_index': 'int',
         'light_index': 'Light',
         'container_type': 'int',
         'field_rect': 'RectangleCoordinates',
         'rfid_origin': 'RfidOrigin'
     }
 
     attribute_map = {
         'source': 'source',
         'value': 'value',
         'original_value': 'originalValue',
+        'original_page_index': 'originalPageIndex',
         'page_index': 'pageIndex',
         'light_index': 'lightIndex',
         'container_type': 'containerType',
         'field_rect': 'fieldRect',
         'rfid_origin': 'rfidOrigin'
     }
 
-    def __init__(self, source=None, value=None, original_value=None, page_index=None, light_index=None, container_type=0, field_rect=None, rfid_origin=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, source=None, value=None, original_value=None, original_page_index=None, page_index=None, light_index=None, container_type=0, field_rect=None, rfid_origin=None, local_vars_configuration=None):  # noqa: E501
         """ImagesFieldValue - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._source = None
         self._value = None
         self._original_value = None
+        self._original_page_index = None
         self._page_index = None
         self._light_index = None
         self._container_type = None
         self._field_rect = None
         self._rfid_origin = None
         self.discriminator = None
 
         self.source = source
         self.value = value
         if original_value is not None:
             self.original_value = original_value
+        if original_page_index is not None:
+            self.original_page_index = original_page_index
         self.page_index = page_index
         self.light_index = light_index
         self.container_type = container_type
         if field_rect is not None:
             self.field_rect = field_rect
         if rfid_origin is not None:
             self.rfid_origin = rfid_origin
@@ -149,14 +154,37 @@
         :param original_value: The original_value of this ImagesFieldValue.  # noqa: E501
         :type original_value: str
         """
 
         self._original_value = original_value
 
     @property
+    def original_page_index(self):
+        """Gets the original_page_index of this ImagesFieldValue.  # noqa: E501
+
+        Original page index  # noqa: E501
+
+        :return: The original_page_index of this ImagesFieldValue.  # noqa: E501
+        :rtype: int
+        """
+        return self._original_page_index
+
+    @original_page_index.setter
+    def original_page_index(self, original_page_index):
+        """Sets the original_page_index of this ImagesFieldValue.
+
+        Original page index  # noqa: E501
+
+        :param original_page_index: The original_page_index of this ImagesFieldValue.  # noqa: E501
+        :type original_page_index: int
+        """
+
+        self._original_page_index = original_page_index
+
+    @property
     def page_index(self):
         """Gets the page_index of this ImagesFieldValue.  # noqa: E501
 
         Page index of the image from input list  # noqa: E501
 
         :return: The page_index of this ImagesFieldValue.  # noqa: E501
         :rtype: int
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/images_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/images_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/lcid.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/lcid.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/lexical_analysis_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/lexical_analysis_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/lexical_analysis_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/license_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/license_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/license_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/license_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/light.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/light.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/list_verified_fields.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/list_verified_fields.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/log_level.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/log_level.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/measure_system.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/measure_system.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/mrz_format.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/mrz_format.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ocr_security_text_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ocr_security_text_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/one_candidate.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/one_candidate.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/original_symbol.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/original_symbol.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/p_array_field.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/p_array_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/per_document_config.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/per_document_config.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/photo_ident_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/photo_ident_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/point.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/point.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/point_array.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/point_array.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/points_container.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/points_container.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_params.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
         'disable_perforation_ocr': 'bool',
         'document_group_filter': 'list[DocumentType]',
         'process_auth': 'AuthenticityResultType[object]',
         'device_id': 'int',
         'device_type': 'int',
         'device_type_hex': 'str',
         'ignore_device_id_from_image': 'bool',
-        'document_id_list': 'list[int]'
+        'document_id_list': 'list[int]',
+        'rfid': 'ProcessParamsRfid'
     }
 
     attribute_map = {
         'image_output_max_height': 'imageOutputMaxHeight',
         'image_output_max_width': 'imageOutputMaxWidth',
         'scenario': 'scenario',
         'result_type_output': 'resultTypeOutput',
@@ -118,18 +119,19 @@
         'disable_perforation_ocr': 'disablePerforationOCR',
         'document_group_filter': 'documentGroupFilter',
         'process_auth': 'processAuth',
         'device_id': 'deviceId',
         'device_type': 'deviceType',
         'device_type_hex': 'deviceTypeHex',
         'ignore_device_id_from_image': 'ignoreDeviceIdFromImage',
-        'document_id_list': 'documentIdList'
+        'document_id_list': 'documentIdList',
+        'rfid': 'rfid'
     }
 
-    def __init__(self, image_output_max_height=None, image_output_max_width=None, scenario=None, result_type_output=None, double_page_spread=None, generate_double_page_spread_image=None, field_types_filter=None, date_format=None, measure_system=None, image_dpi_out_max=None, already_cropped=None, custom_params=None, config=None, log=None, log_level=None, force_doc_id=None, match_text_field_mask=None, fast_doc_detect=None, update_ocr_validity_by_glare=None, check_required_text_fields=None, return_cropped_barcode=None, image_qa=None, respect_image_quality=None, force_doc_format=None, no_graphics=None, document_area_min=None, depersonalize_log=None, multi_doc_on_image=None, shift_expiry_date=None, minimal_holder_age=None, return_uncropped_image=None, mrz_formats_filter=None, force_read_mrz_before_locate=None, parse_barcodes=None, convert_case=None, split_names=None, disable_perforation_ocr=None, document_group_filter=None, process_auth=None, device_id=None, device_type=None, device_type_hex=None, ignore_device_id_from_image=None, document_id_list=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, image_output_max_height=None, image_output_max_width=None, scenario=None, result_type_output=None, double_page_spread=None, generate_double_page_spread_image=None, field_types_filter=None, date_format=None, measure_system=None, image_dpi_out_max=None, already_cropped=None, custom_params=None, config=None, log=None, log_level=None, force_doc_id=None, match_text_field_mask=None, fast_doc_detect=None, update_ocr_validity_by_glare=None, check_required_text_fields=None, return_cropped_barcode=None, image_qa=None, respect_image_quality=None, force_doc_format=None, no_graphics=None, document_area_min=None, depersonalize_log=None, multi_doc_on_image=None, shift_expiry_date=None, minimal_holder_age=None, return_uncropped_image=None, mrz_formats_filter=None, force_read_mrz_before_locate=None, parse_barcodes=None, convert_case=None, split_names=None, disable_perforation_ocr=None, document_group_filter=None, process_auth=None, device_id=None, device_type=None, device_type_hex=None, ignore_device_id_from_image=None, document_id_list=None, rfid=None, local_vars_configuration=None):  # noqa: E501
         """ProcessParams - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._image_output_max_height = None
         self._image_output_max_width = None
@@ -171,14 +173,15 @@
         self._document_group_filter = None
         self._process_auth = None
         self._device_id = None
         self._device_type = None
         self._device_type_hex = None
         self._ignore_device_id_from_image = None
         self._document_id_list = None
+        self._rfid = None
         self.discriminator = None
 
         if image_output_max_height is not None:
             self.image_output_max_height = image_output_max_height
         if image_output_max_width is not None:
             self.image_output_max_width = image_output_max_width
         self.scenario = scenario
@@ -260,14 +263,16 @@
             self.device_type = device_type
         if device_type_hex is not None:
             self.device_type_hex = device_type_hex
         if ignore_device_id_from_image is not None:
             self.ignore_device_id_from_image = ignore_device_id_from_image
         if document_id_list is not None:
             self.document_id_list = document_id_list
+        if rfid is not None:
+            self.rfid = rfid
 
     @property
     def image_output_max_height(self):
         """Gets the image_output_max_height of this ProcessParams.  # noqa: E501
 
         This parameter allows setting maximum height in pixels of output images and thus reducing image size to desired. Does not change the aspect ratio. Changes disabled if equals to 0. Default 0.  # noqa: E501
 
@@ -1261,14 +1266,35 @@
 
         :param document_id_list: The document_id_list of this ProcessParams.  # noqa: E501
         :type document_id_list: list[int]
         """
 
         self._document_id_list = document_id_list
 
+    @property
+    def rfid(self):
+        """Gets the rfid of this ProcessParams.  # noqa: E501
+
+
+        :return: The rfid of this ProcessParams.  # noqa: E501
+        :rtype: ProcessParamsRfid
+        """
+        return self._rfid
+
+    @rfid.setter
+    def rfid(self, rfid):
+        """Sets the rfid of this ProcessParams.
+
+
+        :param rfid: The rfid of this ProcessParams.  # noqa: E501
+        :type rfid: ProcessParamsRfid
+        """
+
+        self._rfid = rfid
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_request.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_request.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_request_image.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_request_image.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_response.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_response.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/process_system_info.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/process_system_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/processing_status.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/processing_status.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/raw_image_container_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/raw_image_container_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/rectangle_coordinates.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/rectangle_coordinates.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/result_item.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/result_item.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/rfid_location.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/rfid_location.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/rfid_origin.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/rfid_origin.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/scenario.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/scenario.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/security_feature_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/security_feature_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/security_feature_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/security_feature_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/security_feature_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,19 @@
 
     LIVENESS_ELECTRONIC_DEVICE = int("40")
 
     LIVENESS_OVI = int("41")
 
     BARCODE_SIZE_CHECK = int("42")
 
-    allowable_values = [BLANK, FILL, PHOTO, MRZ, FALSE_LUMINESCENCE, HOLO_SIMPLE, HOLO_VERIFY_STATIC, HOLO_VERIFY_MULTI_STATIC, HOLO_VERIFY_DYNAMIC, PATTERN_NOT_INTERRUPTED, PATTERN_NOT_SHIFTED, PATTERN_SAME_COLORS, PATTERN_IR_INVISIBLE, PHOTO_SIZE_CHECK, PORTRAIT_COMPARISON_VS_GHOST, PORTRAIT_COMPARISON_VS_RFID, PORTRAIT_COMPARISON_VS_VISUAL, BARCODE, PATTERN_DIFFERENT_LINES_THICKNESS, PORTRAIT_COMPARISON_VS_CAMERA, PORTRAIT_COMPARISON_RFID_VS_CAMERA, GHOST_PHOTO, CLEAR_GHOST_PHOTO, INVISIBLE_OBJECT, LOW_CONTRAST_OBJECT, PHOTO_COLOR, PHOTO_SHAPE, PHOTO_CORNERS, OCR, PORTRAIT_COMPARISON_EXT_VS_VISUAL, PORTRAIT_COMPARISON_EXT_VS_RFID, PORTRAIT_COMPARISON_EXT_VS_CAMERA, LIVENESS_DEPTH, MICRO_TEXT, FLUORESCENT_OBJECT, LANDMARK_CHECK, FACE_PRESENCE, FACE_ABSENCE, LIVENESS_SCREEN_CAPTURE, LIVENESS_ELECTRONIC_DEVICE, LIVENESS_OVI, BARCODE_SIZE_CHECK]  # noqa: E501
+    LASINK = int("43")
+
+    LIVENESS_MLI = int("44")
+
+    allowable_values = [BLANK, FILL, PHOTO, MRZ, FALSE_LUMINESCENCE, HOLO_SIMPLE, HOLO_VERIFY_STATIC, HOLO_VERIFY_MULTI_STATIC, HOLO_VERIFY_DYNAMIC, PATTERN_NOT_INTERRUPTED, PATTERN_NOT_SHIFTED, PATTERN_SAME_COLORS, PATTERN_IR_INVISIBLE, PHOTO_SIZE_CHECK, PORTRAIT_COMPARISON_VS_GHOST, PORTRAIT_COMPARISON_VS_RFID, PORTRAIT_COMPARISON_VS_VISUAL, BARCODE, PATTERN_DIFFERENT_LINES_THICKNESS, PORTRAIT_COMPARISON_VS_CAMERA, PORTRAIT_COMPARISON_RFID_VS_CAMERA, GHOST_PHOTO, CLEAR_GHOST_PHOTO, INVISIBLE_OBJECT, LOW_CONTRAST_OBJECT, PHOTO_COLOR, PHOTO_SHAPE, PHOTO_CORNERS, OCR, PORTRAIT_COMPARISON_EXT_VS_VISUAL, PORTRAIT_COMPARISON_EXT_VS_RFID, PORTRAIT_COMPARISON_EXT_VS_CAMERA, LIVENESS_DEPTH, MICRO_TEXT, FLUORESCENT_OBJECT, LANDMARK_CHECK, FACE_PRESENCE, FACE_ABSENCE, LIVENESS_SCREEN_CAPTURE, LIVENESS_ELECTRONIC_DEVICE, LIVENESS_OVI, BARCODE_SIZE_CHECK, LASINK, LIVENESS_MLI]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/source.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/source.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/source_validity.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/source_validity.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/status.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/status.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/status_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/status_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/status_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/status_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/string_recognition_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/string_recognition_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/symbol_candidate.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/symbol_candidate.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/symbol_recognition_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/symbol_recognition_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_available_source.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_available_source.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_data_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_data_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_data_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_data_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_field.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_field.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_field_type.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_field_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1206,35 +1206,61 @@
 
     VACCINATION_CERTIFICATE_IDENTIFIER = int("644")
 
     FIRST_NAME = int("645")
 
     DATE_OF_ARRIVAL = int("646")
 
-    FT_SECOND_NAME = int("647")
+    SECOND_NAME = int("647")
 
-    FT_THIRD_NAME = int("648")
+    THIRD_NAME = int("648")
 
-    FT_FOURTH_NAME = int("649")
+    FOURTH_NAME = int("649")
 
-    FT_LAST_NAME = int("650")
+    LAST_NAME = int("650")
 
-    RM_FROM = int("651")
+    DL_CLASS_CODE_RM_FROM = int("651")
 
-    RM_NOTES = int("652")
+    DL_CLASS_CODE_RM_NOTES = int("652")
 
-    RM_TO = int("653")
+    DL_CLASS_CODE_RM_TO = int("653")
 
-    PW_FROM = int("654")
+    DL_CLASS_CODE_PW_FROM = int("654")
 
-    PW_NOTES = int("655")
+    DL_CLASS_CODE_PW_NOTES = int("655")
 
-    PW_TO = int("656")
+    DL_CLASS_CODE_PW_TO = int("656")
 
-    allowable_values = [DOCUMENT_CLASS_CODE, ISSUING_STATE_CODE, DOCUMENT_NUMBER, DATE_OF_EXPIRY, DATE_OF_ISSUE, DATE_OF_BIRTH, PLACE_OF_BIRTH, PERSONAL_NUMBER, SURNAME, GIVEN_NAME, MOTHERS_NAME, NATIONALITY, SEX, HEIGHT, WEIGHT, EYES_COLOR, HAIR_COLOR, ADDRESS, DONOR, SOCIAL_SECURITY_NUMBER, DL_CLASS, DL_ENDORSED, DL_RESTRICTION_CODE, DL_UNDER_21_DATE, AUTHORITY, SURNAME_AND_GIVEN_NAMES, NATIONALITY_CODE, PASSPORT_NUMBER, INVITATION_NUMBER, VISA_ID, VISA_CLASS, VISA_SUBCLASS, MRZ_TYPE, OPTIONAL_DATA, DOCUMENT_CLASS_NAME, ISSUING_STATE_NAME, PLACE_OF_ISSUE, DOCUMENT_NUMBER_CHECKSUM, DATE_OF_BIRTH_CHECKSUM, DATE_OF_EXPIRY_CHECKSUM, PERSONAL_NUMBER_CHECKSUM, FINAL_CHECKSUM, PASSPORT_NUMBER_CHECKSUM, INVITATION_NUMBER_CHECKSUM, VISA_ID_CHECKSUM, SURNAME_AND_GIVEN_NAME_CHECKSUM, VISA_VALID_UNTIL_CHECKSUM, OTHER, MRZ_STRINGS, NAME_SUFFIX, NAME_PREFIX, DATE_OF_ISSUE_CHECKSUM, DATE_OF_ISSUE_CHECK_DIGIT, DOCUMENT_SERIES, REG_CERT_REG_NUMBER, REG_CERT_CAR_MODEL, REG_CERT_CAR_COLOR, REG_CERT_BODY_NUMBER, REG_CERT_CAR_TYPE, REG_CERT_MAX_WEIGHT, REG_CERT_WEIGHT, ADDRESS_AREA, ADDRESS_STATE, ADDRESS_BUILDING, ADDRESS_HOUSE, ADDRESS_FLAT, PLACE_OF_REGISTRATION, DATE_OF_REGISTRATION, RESIDENT_FROM, RESIDENT_UNTIL, AUTHORITY_CODE, PLACE_OF_BIRTH_AREA, PLACE_OF_BIRTH_STATE_CODE, ADDRESS_STREET, ADDRESS_CITY, ADDRESS_JURISDICTION_CODE, ADDRESS_POSTAL_CODE, DOCUMENT_NUMBER_CHECK_DIGIT, DATE_OF_BIRTH_CHECK_DIGIT, DATE_OF_EXPIRY_CHECK_DIGIT, PERSONAL_NUMBER_CHECK_DIGIT, FINAL_CHECK_DIGIT, PASSPORT_NUMBER_CHECK_DIGIT, INVITATION_NUMBER_CHECK_DIGIT, VISA_ID_CHECK_DIGIT, SURNAME_AND_GIVEN_NAMES_CHECK_DIGIT, VISA_VALID_UNTIL_CHECK_DIGIT, PERMIT_DL_CLASS, PERMIT_DATE_OF_EXPIRY, PERMIT_IDENTIFIER, PERMIT_DATE_OF_ISSUE, PERMIT_RESTRICTION_CODE, PERMIT_ENDORSED, ISSUE_TIMESTAMP, NUMBER_OF_DUPLICATES, MEDICAL_INDICATOR_CODES, NON_RESIDENT_INDICATOR, VISA_TYPE, VISA_VALID_FROM, VISA_VALID_UNTIL, DURATION_OF_STAY, NUMBER_OF_ENTRIES, DAY, MONTH, YEAR, UNIQUE_CUSTOMER_IDENTIFIER, COMMERCIAL_VEHICLE_CODES, AKA_DATE_OF_BIRTH, AKA_SOCIAL_SECURITY_NUMBER, AKA_SURNAME, AKA_GIVEN_NAMES, AKA_NAME_SUFFIX, AKA_NAME_PREFIX, MAILING_ADDRESS_STREET, MAILING_ADDRESS_CITY, MAILING_ADDRESS_JURISDICTION_CODE, MAILING_ADDRESS_POSTAL_CODE, AUDIT_INFORMATION, INVENTORY_NUMBER, RACE_ETHNICITY, JURISDICTION_VEHICLE_CLASS, JURISDICTION_ENDORSEMENT_CODE, JURISDICTION_RESTRICTION_CODE, FAMILY_NAME, GIVEN_NAMES_RUS, VISA_ID_RUS, FATHERS_NAME, FATHERS_NAME_RUS, SURNAME_AND_GIVEN_NAME_RUS, PLACE_OF_BIRTH_RUS, AUTHORITY_RUS, ISSUING_STATE_CODE_NUMERIC, NATIONALITY_CODE_NUMERIC, ENGINE_POWER, ENGINE_VOLUME, CHASSIS_NUMBER, ENGINE_NUMBER, ENGINE_MODEL, VEHICLE_CATEGORY, IDENTITY_CARD_NUMBER, CONTROL_NUMBER, PARENTS_GIVEN_NAMES, SECOND_SURNAME, MIDDLE_NAME, REG_CERT_VIN, REG_CERT_VIN_CHECK_DIGIT, REG_CERT_VIN_CHECKSUM, LINE_1_CHECK_DIGIT, LINE_2_CHECK_DIGIT, LINE_3_CHECK_DIGIT, LINE_1_CHECKSUM, LINE_2_CHECKSUM, LINE_3_CHECKSUM, REG_CERT_REG_NUMBER_CHECK_DIGIT, REG_CERT_REG_NUMBER_CHECKSUM, REG_CERT_VEHICLE_ITS_CODE, CARD_ACCESS_NUMBER, MARITAL_STATUS, COMPANY_NAME, SPECIAL_NOTES, SURNAME_OF_SPOUSE, TRACKING_NUMBER, BOOKLET_NUMBER, CHILDREN, COPY_NUMBER, SERIAL_NUMBER, DOSSIER_NUMBER, AKA_SURNAME_AND_GIVEN_NAMES, TERRITORIAL_VALIDITY, MRZ_STRINGS_WITH_CORRECT_CHECK_SUMS, DL_CDL_RESTRICTION_CODE, DL_UNDER_18_DATE, DL_RECORD_CREATED, DL_DUPLICATE_DATE, DL_ISSUE_TYPE, MILITARY_BOOK_NUMBER, DESTINATION, BLOOD_GROUP, SEQUENCE_NUMBER, REG_CERT_BODY_TYPE, REG_CERT_CAR_MARK, TRANSACTION_NUMBER, AGE, FOLIO_NUMBER, VOTER_KEY, ADDRESS_MUNICIPALITY, ADDRESS_LOCATION, SECTION, OCR_NUMBER, FEDERAL_ELECTIONS, REFERENCE_NUMBER, OPTIONAL_DATA_CHECKSUM, OPTIONAL_DATA_CHECK_DIGIT, VISA_NUMBER, VISA_NUMBER_CHECKSUM, VISA_NUMBER_CHECK_DIGIT, VOTER, PREVIOUS_TYPE, FIELD_FROM_MRZ, CURRENT_DATE, STATUS_DATE_OF_EXPIRY, BANK_NOTE_NUMBER, CSC_CODE, ARTISTIC_NAME, ACADEMIC_TITLE, ADDRESS_COUNTRY, ADDRESS_ZIP_CODE, E_ID_RESIDENCE_PERMIT_1, E_ID_RESIDENCE_PERMIT_2, E_ID_PLACE_OF_BIRTH_STREET, E_ID_PLACE_OF_BIRTH_CITY, E_ID_PLACE_OF_BIRTH_STATE, E_ID_PLACE_OF_BIRTH_COUNTRY, E_ID_PLACE_OF_BIRTH_ZIP_CODE, CDL_CLASS, DL_UNDER_19_DATE, WEIGHT_POUNDS, LIMITED_DURATION_DOCUMENT_INDICATOR, ENDORSEMENT_EXPIRATION_DATE, REVISION_DATE, COMPLIANCE_TYPE, FAMILY_NAME_TRUNCATION, FIRST_NAME_TRUNCATION, MIDDLE_NAME_TRUNCATION, EXAM_DATE, ORGANIZATION, DEPARTMENT, PAY_GRADE, RANK, BENEFITS_NUMBER, SPONSOR_SERVICE, SPONSOR_STATUS, SPONSOR, RELATIONSHIP, USCIS, CATEGORY, CONDITIONS, IDENTIFIER, CONFIGURATION, DISCRETIONARY_DATA, LINE_1_OPTIONAL_DATA, LINE_2_OPTIONAL_DATA, LINE_3_OPTIONAL_DATA, EQV_CODE, ALT_CODE, BINARY_CODE, PSEUDO_CODE, FEE, STAMP_NUMBER, SBH_SECURITY_OPTIONS, SBH_INTEGRITY_OPTIONS, DATE_OF_CREATION, VALIDITY_PERIOD, PATRON_HEADER_VERSION, BDB_TYPE, BIOMETRIC_TYPE, BIOMETRIC_SUBTYPE, BIOMETRIC_PRODUCT_ID, BIOMETRIC_FORMAT_OWNER, BIOMETRIC_FORMAT_TYPE, PHONE, PROFESSION, TITLE, PERSONAL_SUMMARY, OTHER_VALID_ID, CUSTODY_INFO, OTHER_NAME, OBSERVATIONS, TAX, DATE_OF_PERSONALIZATION, PERSONALIZATION_SN, OTHER_PERSON_NAME, PERSON_TO_NOTIFY_DATE_OF_RECORD, PERSON_TO_NOTIFY_NAME, PERSON_TO_NOTIFY_PHONE, PERSON_TO_NOTIFY_ADDRESS, DS_CERTIFICATE_ISSUER, DS_CERTIFICATE_SUBJECT, DS_CERTIFICATE_VALID_FROM, DS_CERTIFICATE_VALID_TO, VRC_DATA_OBJECT_ENTRY, TYPE_APPROVAL_NUMBER, ADMINISTRATIVE_NUMBER, DOCUMENT_DISCRIMINATOR, DATA_DISCRIMINATOR, ISO_ISSUER_ID_NUMBER, GNIB_NUMBER, DEPT_NUMBER, TELEX_CODE, ALLERGIES, SP_CODE, COURT_CODE, CTY, SPONSOR_SSN, DOD_NUMBER, MC_NOVICE_DATE, DUF_NUMBER, AGY, PNR_CODE, FROM_AIRPORT_CODE, TO_AIRPORT_CODE, FLIGHT_NUMBER, DATE_OF_FLIGHT, SEAT_NUMBER, DATE_OF_ISSUE_BOARDING_PASS, CCW_UNTIL, REFERENCE_NUMBER_CHECKSUM, REFERENCE_NUMBER_CHECK_DIGIT, ROOM_NUMBER, RELIGION, REMAINDER_TERM, ELECTRONIC_TICKET_INDICATOR, COMPARTMENT_CODE, CHECK_IN_SEQUENCE_NUMBER, AIRLINE_DESIGNATOR_OF_BOARDING_PASS_ISSUER, AIRLINE_NUMERIC_CODE, TICKET_NUMBER, FREQUENT_FLYER_AIRLINE_DESIGNATOR, FREQUENT_FLYER_NUMBER, FREE_BAGGAGE_ALLOWANCE, PDF_417_CODEC, IDENTITY_CARD_NUMBER_CHECKSUM, IDENTITY_CARD_NUMBER_CHECK_DIGIT, VETERAN, DL_CLASS_CODE_A1_FROM, DL_CLASS_CODE_A1_TO, DL_CLASS_CODE_A1_NOTES, DL_CLASS_CODE_A_FROM, DL_CLASS_CODE_A_TO, DL_CLASS_CODE_A_NOTES, DL_CLASS_CODE_B_FROM, DL_CLASS_CODE_B_TO, DL_CLASS_CODE_B_NOTES, DL_CLASS_CODE_C1_FROM, DL_CLASS_CODE_C1_TO, DL_CLASS_CODE_C1_NOTES, DL_CLASS_CODE_C_FROM, DL_CLASS_CODE_C_TO, DL_CLASS_CODE_C_NOTES, DL_CLASS_CODE_D1_FROM, DL_CLASS_CODE_D1_TO, DL_CLASS_CODE_D1_NOTES, DL_CLASS_CODE_D_FROM, DL_CLASS_CODE_D_TO, DL_CLASS_CODE_D_NOTES, DL_CLASS_CODE_BE_FROM, DL_CLASS_CODE_BE_TO, DL_CLASS_CODE_BE_NOTES, DL_CLASS_CODE_C1E_FROM, DL_CLASS_CODE_C1E_TO, DL_CLASS_CODE_C1E_NOTES, DL_CLASS_CODE_CE_FROM, DL_CLASS_CODE_CE_TO, DL_CLASS_CODE_CE_NOTES, DL_CLASS_CODE_D1E_FROM, DL_CLASS_CODE_D1E_TO, DL_CLASS_CODE_D1E_NOTES, DL_CLASS_CODE_DE_FROM, DL_CLASS_CODE_DE_TO, DL_CLASS_CODE_DE_NOTES, DL_CLASS_CODE_M_FROM, DL_CLASS_CODE_M_TO, DL_CLASS_CODE_M_NOTES, DL_CLASS_CODE_L_FROM, DL_CLASS_CODE_L_TO, DL_CLASS_CODE_L_NOTES, DL_CLASS_CODE_T_FROM, DL_CLASS_CODE_T_TO, DL_CLASS_CODE_T_NOTES, DL_CLASS_CODE_AM_FROM, DL_CLASS_CODE_AM_TO, DL_CLASS_CODE_AM_NOTES, DL_CLASS_CODE_A2_FROM, DL_CLASS_CODE_A2_TO, DL_CLASS_CODE_A2_NOTES, DL_CLASS_CODE_B1_FROM, DL_CLASS_CODE_B1_TO, DL_CLASS_CODE_B1_NOTES, SURNAME_AT_BIRTH, CIVIL_STATUS, NUMBER_OF_SEATS, NUMBER_OF_STANDING_PLACES, MAX_SPEED, FUEL_TYPE, EC_ENVIRONMENTAL_TYPE, POWER_WEIGHT_RATIO, MAX_MASS_OF_TRAILER_BRAKED, MAX_MASS_OF_TRAILER_UNBRAKED, TRANSMISSION_TYPE, TRAILER_HITCH, ACCOMPANIED_BY, POLICE_DISTRICT, FIRST_ISSUE_DATE, PAYLOAD_CAPACITY, NUMBER_OF_AXLES, PERMISSIBLE_AXLE_LOAD, PRECINCT, INVITED_BY, PURPOSE_OF_ENTRY, SKIN_COLOR, COMPLEXION, AIRPORT_FROM, AIRPORT_TO, AIRLINE_NAME, AIRLINE_NAME_FREQUENT_FLYER, LICENSE_NUMBER, IN_TANKS, EXCEPT_IN_TANKS, FAST_TRACK, OWNER, MRZ_STRINGS_ICAO_RFID, NUMBER_OF_CARD_ISSUANCE, NUMBER_OF_CARD_ISSUANCE_CHECKSUM, NUMBER_OF_CARD_ISSUANCE_CHECK_DIGIT, CENTURY_DATE_OF_BIRTH, DL_CLASS_CODE_A3_FROM, DL_CLASS_CODE_A3_TO, DL_CLASS_CODE_A3_NOTES, DL_CLASS_CODE_C2_FROM, DL_CLASS_CODE_C2_TO, DL_CLASS_CODE_C2_NOTES, DL_CLASS_CODE_B2_FROM, DL_CLASS_CODE_B2_TO, DL_CLASS_CODE_B2_NOTES, DL_CLASS_CODE_D2_FROM, DL_CLASS_CODE_D2_TO, DL_CLASS_CODE_D2_NOTES, DL_CLASS_CODE_B2E_FROM, DL_CLASS_CODE_B2E_TO, DL_CLASS_CODE_B2E_NOTES, DL_CLASS_CODE_G_FROM, DL_CLASS_CODE_G_TO, DL_CLASS_CODE_G_NOTES, DL_CLASS_CODE_J_FROM, DL_CLASS_CODE_J_TO, DL_CLASS_CODE_J_NOTES, DL_CLASS_CODE_LC_FROM, DL_CLASS_CODE_LC_TO, DL_CLASS_CODE_LC_NOTES, BANK_CARD_NUMBER, BANK_CARD_VALID_THRU, TAX_NUMBER, HEALTH_NUMBER, GRANDFATHER_NAME, SELECTEE_INDICATOR, MOTHER_SURNAME, MOTHER_GIVEN_NAME, FATHER_SURNAME, FATHER_GIVEN_NAME, MOTHER_DATE_OF_BIRTH, FATHER_DATE_OF_BIRTH, MOTHER_PERSONAL_NUMBER, FATHER_PERSONAL_NUMBER, MOTHER_PLACE_OF_BIRTH, FATHER_PLACE_OF_BIRTH, MOTHER_COUNTRY_OF_BIRTH, FATHER_COUNTRY_OF_BIRTH, DATE_FIRST_RENEWAL, DATE_SECOND_RENEWAL, PLACE_OF_EXAMINATION, APPLICATION_NUMBER, VOUCHER_NUMBER, AUTHORIZATION_NUMBER, FACULTY, FORM_OF_EDUCATION, DNI_NUMBER, RETIREMENT_NUMBER, PROFESSIONAL_ID_NUMBER, AGE_AT_ISSUE, YEARS_SINCE_ISSUE, DL_CLASS_CODE_BTP_FROM, DL_CLASS_CODE_BTP_NOTES, DL_CLASS_CODE_BTP_TO, DL_CLASS_CODE_C3_FROM, DL_CLASS_CODE_C3_NOTES, DL_CLASS_CODE_C3_TO, DL_CLASS_CODE_E_FROM, DL_CLASS_CODE_E_NOTES, DL_CLASS_CODE_E_TO, DL_CLASS_CODE_F_FROM, DL_CLASS_CODE_F_NOTES, DL_CLASS_CODE_F_TO, DL_CLASS_CODE_FA_FROM, DL_CLASS_CODE_FA_NOTES, DL_CLASS_CODE_FA_TO, DL_CLASS_CODE_FA1_FROM, DL_CLASS_CODE_FA1_NOTES, DL_CLASS_CODE_FA1_TO, DL_CLASS_CODE_FB_FROM, DL_CLASS_CODE_FB_NOTES, DL_CLASS_CODE_FB_TO, DL_CLASS_CODE_G1_FROM, DL_CLASS_CODE_G1_NOTES, DL_CLASS_CODE_G1_TO, DL_CLASS_CODE_H_FROM, DL_CLASS_CODE_H_NOTES, DL_CLASS_CODE_H_TO, DL_CLASS_CODE_I_FROM, DL_CLASS_CODE_I_NOTES, DL_CLASS_CODE_I_TO, DL_CLASS_CODE_K_FROM, DL_CLASS_CODE_K_NOTES, DL_CLASS_CODE_K_TO, DL_CLASS_CODE_LK_FROM, DL_CLASS_CODE_LK_NOTES, DL_CLASS_CODE_LK_TO, DL_CLASS_CODE_N_FROM, DL_CLASS_CODE_N_NOTES, DL_CLASS_CODE_N_TO, DL_CLASS_CODE_S_FROM, DL_CLASS_CODE_S_NOTES, DL_CLASS_CODE_S_TO, DL_CLASS_CODE_TB_FROM, DL_CLASS_CODE_TB_NOTES, DL_CLASS_CODE_TB_TO, DL_CLASS_CODE_TM_FROM, DL_CLASS_CODE_TM_NOTES, DL_CLASS_CODE_TM_TO, DL_CLASS_CODE_TR_FROM, DL_CLASS_CODE_TR_NOTES, DL_CLASS_CODE_TR_TO, DL_CLASS_CODE_TV_FROM, DL_CLASS_CODE_TV_NOTES, DL_CLASS_CODE_TV_TO, DL_CLASS_CODE_V_FROM, DL_CLASS_CODE_V_NOTES, DL_CLASS_CODE_V_TO, DL_CLASS_CODE_W_FROM, DL_CLASS_CODE_W_NOTES, DL_CLASS_CODE_W_TO, URL, CALIBER, MODEL, MAKE, NUMBER_OF_CYLINDERS, SURNAME_OF_HUSBAND_AFTER_REGISTRATION, SURNAME_OF_WIFE_AFTER_REGISTRATION, DATE_OF_BIRTH_OF_WIFE, DATE_OF_BIRTH_OF_HUSBAND, CITIZENSHIP_OF_FIRST_PERSON, CITIZENSHIP_OF_SECOND_PERSON, CVV, DATE_OF_INSURANCE_EXPIRY, MORTGAGE_BY, OLD_DOCUMENT_NUMBER, OLD_DATE_OF_ISSUE, OLD_PLACE_OF_ISSUE, DL_CLASS_CODE_LR_FROM, DL_CLASS_CODE_LR_TO, DL_CLASS_CODE_LR_NOTES, DL_CLASS_CODE_MR_FROM, DL_CLASS_CODE_MR_TO, DL_CLASS_CODE_MR_NOTES, DL_CLASS_CODE_HR_FROM, DL_CLASS_CODE_HR_TO, DL_CLASS_CODE_HR_NOTES, DL_CLASS_CODE_HC_FROM, DL_CLASS_CODE_HC_TO, DL_CLASS_CODE_HC_NOTES, DL_CLASS_CODE_MC_FROM, DL_CLASS_CODE_MC_TO, DL_CLASS_CODE_MC_NOTES, DL_CLASS_CODE_RE_FROM, DL_CLASS_CODE_RE_TO, DL_CLASS_CODE_RE_NOTES, DL_CLASS_CODE_R_FROM, DL_CLASS_CODE_R_TO, DL_CLASS_CODE_R_NOTES, DL_CLASS_CODE_CA_FROM, DL_CLASS_CODE_CA_TO, DL_CLASS_CODE_CA_NOTES, CITIZENSHIP_STATUS, MILITARY_SERVICE_FROM, MILITARY_SERVICE_TO, DL_CLASS_CODE_NT_FROM, DL_CLASS_CODE_NT_TO, DL_CLASS_CODE_NT_NOTES, DL_CLASS_CODE_TN_FROM, DL_CLASS_CODE_TN_TO, DL_CLASS_CODE_TN_NOTES, DL_CLASS_CODE_D3_FROM, DL_CLASS_CODE_D3_TO, DL_CLASS_CODE_D3_NOTES, ALT_DATE_OF_EXPIRE, DL_CLASS_CODE_CD_FROM, DL_CLASS_CODE_CD_TO, DL_CLASS_CODE_CD_NOTES, ISSUER_IDENTIFICATION_NUMBER, PAYMENT_PERIOD_FROM, PAYMENT_PERIOD_TO, VACCINATION_CERTIFICATE_IDENTIFIER, FIRST_NAME, DATE_OF_ARRIVAL, FT_SECOND_NAME, FT_THIRD_NAME, FT_FOURTH_NAME, FT_LAST_NAME, RM_FROM, RM_NOTES, RM_TO, PW_FROM, PW_NOTES, PW_TO]  # noqa: E501
+    DL_CLASS_CODE_EB_FROM = int("657")
+
+    DL_CLASS_CODE_EB_NOTES = int("658")
+
+    DL_CLASS_CODE_EB_TO = int("659")
+
+    DL_CLASS_CODE_EC_FROM = int("660")
+
+    DL_CLASS_CODE_EC_NOTES = int("661")
+
+    DL_CLASS_CODE_EC_TO = int("662")
+
+    DL_CLASS_CODE_EC1_FROM = int("663")
+
+    DL_CLASS_CODE_EC1_NOTES = int("664")
+
+    DL_CLASS_CODE_EC1_TO = int("665")
+
+    PLACE_OF_BIRTH_CITY = int("666")
+
+    YEAR_OF_EXPIRY = int("667")
+
+    GRANDFATHER_NAME_MATERNAL = int("668")
+
+    _669 = int("669")
+
+    allowable_values = [DOCUMENT_CLASS_CODE, ISSUING_STATE_CODE, DOCUMENT_NUMBER, DATE_OF_EXPIRY, DATE_OF_ISSUE, DATE_OF_BIRTH, PLACE_OF_BIRTH, PERSONAL_NUMBER, SURNAME, GIVEN_NAME, MOTHERS_NAME, NATIONALITY, SEX, HEIGHT, WEIGHT, EYES_COLOR, HAIR_COLOR, ADDRESS, DONOR, SOCIAL_SECURITY_NUMBER, DL_CLASS, DL_ENDORSED, DL_RESTRICTION_CODE, DL_UNDER_21_DATE, AUTHORITY, SURNAME_AND_GIVEN_NAMES, NATIONALITY_CODE, PASSPORT_NUMBER, INVITATION_NUMBER, VISA_ID, VISA_CLASS, VISA_SUBCLASS, MRZ_TYPE, OPTIONAL_DATA, DOCUMENT_CLASS_NAME, ISSUING_STATE_NAME, PLACE_OF_ISSUE, DOCUMENT_NUMBER_CHECKSUM, DATE_OF_BIRTH_CHECKSUM, DATE_OF_EXPIRY_CHECKSUM, PERSONAL_NUMBER_CHECKSUM, FINAL_CHECKSUM, PASSPORT_NUMBER_CHECKSUM, INVITATION_NUMBER_CHECKSUM, VISA_ID_CHECKSUM, SURNAME_AND_GIVEN_NAME_CHECKSUM, VISA_VALID_UNTIL_CHECKSUM, OTHER, MRZ_STRINGS, NAME_SUFFIX, NAME_PREFIX, DATE_OF_ISSUE_CHECKSUM, DATE_OF_ISSUE_CHECK_DIGIT, DOCUMENT_SERIES, REG_CERT_REG_NUMBER, REG_CERT_CAR_MODEL, REG_CERT_CAR_COLOR, REG_CERT_BODY_NUMBER, REG_CERT_CAR_TYPE, REG_CERT_MAX_WEIGHT, REG_CERT_WEIGHT, ADDRESS_AREA, ADDRESS_STATE, ADDRESS_BUILDING, ADDRESS_HOUSE, ADDRESS_FLAT, PLACE_OF_REGISTRATION, DATE_OF_REGISTRATION, RESIDENT_FROM, RESIDENT_UNTIL, AUTHORITY_CODE, PLACE_OF_BIRTH_AREA, PLACE_OF_BIRTH_STATE_CODE, ADDRESS_STREET, ADDRESS_CITY, ADDRESS_JURISDICTION_CODE, ADDRESS_POSTAL_CODE, DOCUMENT_NUMBER_CHECK_DIGIT, DATE_OF_BIRTH_CHECK_DIGIT, DATE_OF_EXPIRY_CHECK_DIGIT, PERSONAL_NUMBER_CHECK_DIGIT, FINAL_CHECK_DIGIT, PASSPORT_NUMBER_CHECK_DIGIT, INVITATION_NUMBER_CHECK_DIGIT, VISA_ID_CHECK_DIGIT, SURNAME_AND_GIVEN_NAMES_CHECK_DIGIT, VISA_VALID_UNTIL_CHECK_DIGIT, PERMIT_DL_CLASS, PERMIT_DATE_OF_EXPIRY, PERMIT_IDENTIFIER, PERMIT_DATE_OF_ISSUE, PERMIT_RESTRICTION_CODE, PERMIT_ENDORSED, ISSUE_TIMESTAMP, NUMBER_OF_DUPLICATES, MEDICAL_INDICATOR_CODES, NON_RESIDENT_INDICATOR, VISA_TYPE, VISA_VALID_FROM, VISA_VALID_UNTIL, DURATION_OF_STAY, NUMBER_OF_ENTRIES, DAY, MONTH, YEAR, UNIQUE_CUSTOMER_IDENTIFIER, COMMERCIAL_VEHICLE_CODES, AKA_DATE_OF_BIRTH, AKA_SOCIAL_SECURITY_NUMBER, AKA_SURNAME, AKA_GIVEN_NAMES, AKA_NAME_SUFFIX, AKA_NAME_PREFIX, MAILING_ADDRESS_STREET, MAILING_ADDRESS_CITY, MAILING_ADDRESS_JURISDICTION_CODE, MAILING_ADDRESS_POSTAL_CODE, AUDIT_INFORMATION, INVENTORY_NUMBER, RACE_ETHNICITY, JURISDICTION_VEHICLE_CLASS, JURISDICTION_ENDORSEMENT_CODE, JURISDICTION_RESTRICTION_CODE, FAMILY_NAME, GIVEN_NAMES_RUS, VISA_ID_RUS, FATHERS_NAME, FATHERS_NAME_RUS, SURNAME_AND_GIVEN_NAME_RUS, PLACE_OF_BIRTH_RUS, AUTHORITY_RUS, ISSUING_STATE_CODE_NUMERIC, NATIONALITY_CODE_NUMERIC, ENGINE_POWER, ENGINE_VOLUME, CHASSIS_NUMBER, ENGINE_NUMBER, ENGINE_MODEL, VEHICLE_CATEGORY, IDENTITY_CARD_NUMBER, CONTROL_NUMBER, PARENTS_GIVEN_NAMES, SECOND_SURNAME, MIDDLE_NAME, REG_CERT_VIN, REG_CERT_VIN_CHECK_DIGIT, REG_CERT_VIN_CHECKSUM, LINE_1_CHECK_DIGIT, LINE_2_CHECK_DIGIT, LINE_3_CHECK_DIGIT, LINE_1_CHECKSUM, LINE_2_CHECKSUM, LINE_3_CHECKSUM, REG_CERT_REG_NUMBER_CHECK_DIGIT, REG_CERT_REG_NUMBER_CHECKSUM, REG_CERT_VEHICLE_ITS_CODE, CARD_ACCESS_NUMBER, MARITAL_STATUS, COMPANY_NAME, SPECIAL_NOTES, SURNAME_OF_SPOUSE, TRACKING_NUMBER, BOOKLET_NUMBER, CHILDREN, COPY_NUMBER, SERIAL_NUMBER, DOSSIER_NUMBER, AKA_SURNAME_AND_GIVEN_NAMES, TERRITORIAL_VALIDITY, MRZ_STRINGS_WITH_CORRECT_CHECK_SUMS, DL_CDL_RESTRICTION_CODE, DL_UNDER_18_DATE, DL_RECORD_CREATED, DL_DUPLICATE_DATE, DL_ISSUE_TYPE, MILITARY_BOOK_NUMBER, DESTINATION, BLOOD_GROUP, SEQUENCE_NUMBER, REG_CERT_BODY_TYPE, REG_CERT_CAR_MARK, TRANSACTION_NUMBER, AGE, FOLIO_NUMBER, VOTER_KEY, ADDRESS_MUNICIPALITY, ADDRESS_LOCATION, SECTION, OCR_NUMBER, FEDERAL_ELECTIONS, REFERENCE_NUMBER, OPTIONAL_DATA_CHECKSUM, OPTIONAL_DATA_CHECK_DIGIT, VISA_NUMBER, VISA_NUMBER_CHECKSUM, VISA_NUMBER_CHECK_DIGIT, VOTER, PREVIOUS_TYPE, FIELD_FROM_MRZ, CURRENT_DATE, STATUS_DATE_OF_EXPIRY, BANK_NOTE_NUMBER, CSC_CODE, ARTISTIC_NAME, ACADEMIC_TITLE, ADDRESS_COUNTRY, ADDRESS_ZIP_CODE, E_ID_RESIDENCE_PERMIT_1, E_ID_RESIDENCE_PERMIT_2, E_ID_PLACE_OF_BIRTH_STREET, E_ID_PLACE_OF_BIRTH_CITY, E_ID_PLACE_OF_BIRTH_STATE, E_ID_PLACE_OF_BIRTH_COUNTRY, E_ID_PLACE_OF_BIRTH_ZIP_CODE, CDL_CLASS, DL_UNDER_19_DATE, WEIGHT_POUNDS, LIMITED_DURATION_DOCUMENT_INDICATOR, ENDORSEMENT_EXPIRATION_DATE, REVISION_DATE, COMPLIANCE_TYPE, FAMILY_NAME_TRUNCATION, FIRST_NAME_TRUNCATION, MIDDLE_NAME_TRUNCATION, EXAM_DATE, ORGANIZATION, DEPARTMENT, PAY_GRADE, RANK, BENEFITS_NUMBER, SPONSOR_SERVICE, SPONSOR_STATUS, SPONSOR, RELATIONSHIP, USCIS, CATEGORY, CONDITIONS, IDENTIFIER, CONFIGURATION, DISCRETIONARY_DATA, LINE_1_OPTIONAL_DATA, LINE_2_OPTIONAL_DATA, LINE_3_OPTIONAL_DATA, EQV_CODE, ALT_CODE, BINARY_CODE, PSEUDO_CODE, FEE, STAMP_NUMBER, SBH_SECURITY_OPTIONS, SBH_INTEGRITY_OPTIONS, DATE_OF_CREATION, VALIDITY_PERIOD, PATRON_HEADER_VERSION, BDB_TYPE, BIOMETRIC_TYPE, BIOMETRIC_SUBTYPE, BIOMETRIC_PRODUCT_ID, BIOMETRIC_FORMAT_OWNER, BIOMETRIC_FORMAT_TYPE, PHONE, PROFESSION, TITLE, PERSONAL_SUMMARY, OTHER_VALID_ID, CUSTODY_INFO, OTHER_NAME, OBSERVATIONS, TAX, DATE_OF_PERSONALIZATION, PERSONALIZATION_SN, OTHER_PERSON_NAME, PERSON_TO_NOTIFY_DATE_OF_RECORD, PERSON_TO_NOTIFY_NAME, PERSON_TO_NOTIFY_PHONE, PERSON_TO_NOTIFY_ADDRESS, DS_CERTIFICATE_ISSUER, DS_CERTIFICATE_SUBJECT, DS_CERTIFICATE_VALID_FROM, DS_CERTIFICATE_VALID_TO, VRC_DATA_OBJECT_ENTRY, TYPE_APPROVAL_NUMBER, ADMINISTRATIVE_NUMBER, DOCUMENT_DISCRIMINATOR, DATA_DISCRIMINATOR, ISO_ISSUER_ID_NUMBER, GNIB_NUMBER, DEPT_NUMBER, TELEX_CODE, ALLERGIES, SP_CODE, COURT_CODE, CTY, SPONSOR_SSN, DOD_NUMBER, MC_NOVICE_DATE, DUF_NUMBER, AGY, PNR_CODE, FROM_AIRPORT_CODE, TO_AIRPORT_CODE, FLIGHT_NUMBER, DATE_OF_FLIGHT, SEAT_NUMBER, DATE_OF_ISSUE_BOARDING_PASS, CCW_UNTIL, REFERENCE_NUMBER_CHECKSUM, REFERENCE_NUMBER_CHECK_DIGIT, ROOM_NUMBER, RELIGION, REMAINDER_TERM, ELECTRONIC_TICKET_INDICATOR, COMPARTMENT_CODE, CHECK_IN_SEQUENCE_NUMBER, AIRLINE_DESIGNATOR_OF_BOARDING_PASS_ISSUER, AIRLINE_NUMERIC_CODE, TICKET_NUMBER, FREQUENT_FLYER_AIRLINE_DESIGNATOR, FREQUENT_FLYER_NUMBER, FREE_BAGGAGE_ALLOWANCE, PDF_417_CODEC, IDENTITY_CARD_NUMBER_CHECKSUM, IDENTITY_CARD_NUMBER_CHECK_DIGIT, VETERAN, DL_CLASS_CODE_A1_FROM, DL_CLASS_CODE_A1_TO, DL_CLASS_CODE_A1_NOTES, DL_CLASS_CODE_A_FROM, DL_CLASS_CODE_A_TO, DL_CLASS_CODE_A_NOTES, DL_CLASS_CODE_B_FROM, DL_CLASS_CODE_B_TO, DL_CLASS_CODE_B_NOTES, DL_CLASS_CODE_C1_FROM, DL_CLASS_CODE_C1_TO, DL_CLASS_CODE_C1_NOTES, DL_CLASS_CODE_C_FROM, DL_CLASS_CODE_C_TO, DL_CLASS_CODE_C_NOTES, DL_CLASS_CODE_D1_FROM, DL_CLASS_CODE_D1_TO, DL_CLASS_CODE_D1_NOTES, DL_CLASS_CODE_D_FROM, DL_CLASS_CODE_D_TO, DL_CLASS_CODE_D_NOTES, DL_CLASS_CODE_BE_FROM, DL_CLASS_CODE_BE_TO, DL_CLASS_CODE_BE_NOTES, DL_CLASS_CODE_C1E_FROM, DL_CLASS_CODE_C1E_TO, DL_CLASS_CODE_C1E_NOTES, DL_CLASS_CODE_CE_FROM, DL_CLASS_CODE_CE_TO, DL_CLASS_CODE_CE_NOTES, DL_CLASS_CODE_D1E_FROM, DL_CLASS_CODE_D1E_TO, DL_CLASS_CODE_D1E_NOTES, DL_CLASS_CODE_DE_FROM, DL_CLASS_CODE_DE_TO, DL_CLASS_CODE_DE_NOTES, DL_CLASS_CODE_M_FROM, DL_CLASS_CODE_M_TO, DL_CLASS_CODE_M_NOTES, DL_CLASS_CODE_L_FROM, DL_CLASS_CODE_L_TO, DL_CLASS_CODE_L_NOTES, DL_CLASS_CODE_T_FROM, DL_CLASS_CODE_T_TO, DL_CLASS_CODE_T_NOTES, DL_CLASS_CODE_AM_FROM, DL_CLASS_CODE_AM_TO, DL_CLASS_CODE_AM_NOTES, DL_CLASS_CODE_A2_FROM, DL_CLASS_CODE_A2_TO, DL_CLASS_CODE_A2_NOTES, DL_CLASS_CODE_B1_FROM, DL_CLASS_CODE_B1_TO, DL_CLASS_CODE_B1_NOTES, SURNAME_AT_BIRTH, CIVIL_STATUS, NUMBER_OF_SEATS, NUMBER_OF_STANDING_PLACES, MAX_SPEED, FUEL_TYPE, EC_ENVIRONMENTAL_TYPE, POWER_WEIGHT_RATIO, MAX_MASS_OF_TRAILER_BRAKED, MAX_MASS_OF_TRAILER_UNBRAKED, TRANSMISSION_TYPE, TRAILER_HITCH, ACCOMPANIED_BY, POLICE_DISTRICT, FIRST_ISSUE_DATE, PAYLOAD_CAPACITY, NUMBER_OF_AXLES, PERMISSIBLE_AXLE_LOAD, PRECINCT, INVITED_BY, PURPOSE_OF_ENTRY, SKIN_COLOR, COMPLEXION, AIRPORT_FROM, AIRPORT_TO, AIRLINE_NAME, AIRLINE_NAME_FREQUENT_FLYER, LICENSE_NUMBER, IN_TANKS, EXCEPT_IN_TANKS, FAST_TRACK, OWNER, MRZ_STRINGS_ICAO_RFID, NUMBER_OF_CARD_ISSUANCE, NUMBER_OF_CARD_ISSUANCE_CHECKSUM, NUMBER_OF_CARD_ISSUANCE_CHECK_DIGIT, CENTURY_DATE_OF_BIRTH, DL_CLASS_CODE_A3_FROM, DL_CLASS_CODE_A3_TO, DL_CLASS_CODE_A3_NOTES, DL_CLASS_CODE_C2_FROM, DL_CLASS_CODE_C2_TO, DL_CLASS_CODE_C2_NOTES, DL_CLASS_CODE_B2_FROM, DL_CLASS_CODE_B2_TO, DL_CLASS_CODE_B2_NOTES, DL_CLASS_CODE_D2_FROM, DL_CLASS_CODE_D2_TO, DL_CLASS_CODE_D2_NOTES, DL_CLASS_CODE_B2E_FROM, DL_CLASS_CODE_B2E_TO, DL_CLASS_CODE_B2E_NOTES, DL_CLASS_CODE_G_FROM, DL_CLASS_CODE_G_TO, DL_CLASS_CODE_G_NOTES, DL_CLASS_CODE_J_FROM, DL_CLASS_CODE_J_TO, DL_CLASS_CODE_J_NOTES, DL_CLASS_CODE_LC_FROM, DL_CLASS_CODE_LC_TO, DL_CLASS_CODE_LC_NOTES, BANK_CARD_NUMBER, BANK_CARD_VALID_THRU, TAX_NUMBER, HEALTH_NUMBER, GRANDFATHER_NAME, SELECTEE_INDICATOR, MOTHER_SURNAME, MOTHER_GIVEN_NAME, FATHER_SURNAME, FATHER_GIVEN_NAME, MOTHER_DATE_OF_BIRTH, FATHER_DATE_OF_BIRTH, MOTHER_PERSONAL_NUMBER, FATHER_PERSONAL_NUMBER, MOTHER_PLACE_OF_BIRTH, FATHER_PLACE_OF_BIRTH, MOTHER_COUNTRY_OF_BIRTH, FATHER_COUNTRY_OF_BIRTH, DATE_FIRST_RENEWAL, DATE_SECOND_RENEWAL, PLACE_OF_EXAMINATION, APPLICATION_NUMBER, VOUCHER_NUMBER, AUTHORIZATION_NUMBER, FACULTY, FORM_OF_EDUCATION, DNI_NUMBER, RETIREMENT_NUMBER, PROFESSIONAL_ID_NUMBER, AGE_AT_ISSUE, YEARS_SINCE_ISSUE, DL_CLASS_CODE_BTP_FROM, DL_CLASS_CODE_BTP_NOTES, DL_CLASS_CODE_BTP_TO, DL_CLASS_CODE_C3_FROM, DL_CLASS_CODE_C3_NOTES, DL_CLASS_CODE_C3_TO, DL_CLASS_CODE_E_FROM, DL_CLASS_CODE_E_NOTES, DL_CLASS_CODE_E_TO, DL_CLASS_CODE_F_FROM, DL_CLASS_CODE_F_NOTES, DL_CLASS_CODE_F_TO, DL_CLASS_CODE_FA_FROM, DL_CLASS_CODE_FA_NOTES, DL_CLASS_CODE_FA_TO, DL_CLASS_CODE_FA1_FROM, DL_CLASS_CODE_FA1_NOTES, DL_CLASS_CODE_FA1_TO, DL_CLASS_CODE_FB_FROM, DL_CLASS_CODE_FB_NOTES, DL_CLASS_CODE_FB_TO, DL_CLASS_CODE_G1_FROM, DL_CLASS_CODE_G1_NOTES, DL_CLASS_CODE_G1_TO, DL_CLASS_CODE_H_FROM, DL_CLASS_CODE_H_NOTES, DL_CLASS_CODE_H_TO, DL_CLASS_CODE_I_FROM, DL_CLASS_CODE_I_NOTES, DL_CLASS_CODE_I_TO, DL_CLASS_CODE_K_FROM, DL_CLASS_CODE_K_NOTES, DL_CLASS_CODE_K_TO, DL_CLASS_CODE_LK_FROM, DL_CLASS_CODE_LK_NOTES, DL_CLASS_CODE_LK_TO, DL_CLASS_CODE_N_FROM, DL_CLASS_CODE_N_NOTES, DL_CLASS_CODE_N_TO, DL_CLASS_CODE_S_FROM, DL_CLASS_CODE_S_NOTES, DL_CLASS_CODE_S_TO, DL_CLASS_CODE_TB_FROM, DL_CLASS_CODE_TB_NOTES, DL_CLASS_CODE_TB_TO, DL_CLASS_CODE_TM_FROM, DL_CLASS_CODE_TM_NOTES, DL_CLASS_CODE_TM_TO, DL_CLASS_CODE_TR_FROM, DL_CLASS_CODE_TR_NOTES, DL_CLASS_CODE_TR_TO, DL_CLASS_CODE_TV_FROM, DL_CLASS_CODE_TV_NOTES, DL_CLASS_CODE_TV_TO, DL_CLASS_CODE_V_FROM, DL_CLASS_CODE_V_NOTES, DL_CLASS_CODE_V_TO, DL_CLASS_CODE_W_FROM, DL_CLASS_CODE_W_NOTES, DL_CLASS_CODE_W_TO, URL, CALIBER, MODEL, MAKE, NUMBER_OF_CYLINDERS, SURNAME_OF_HUSBAND_AFTER_REGISTRATION, SURNAME_OF_WIFE_AFTER_REGISTRATION, DATE_OF_BIRTH_OF_WIFE, DATE_OF_BIRTH_OF_HUSBAND, CITIZENSHIP_OF_FIRST_PERSON, CITIZENSHIP_OF_SECOND_PERSON, CVV, DATE_OF_INSURANCE_EXPIRY, MORTGAGE_BY, OLD_DOCUMENT_NUMBER, OLD_DATE_OF_ISSUE, OLD_PLACE_OF_ISSUE, DL_CLASS_CODE_LR_FROM, DL_CLASS_CODE_LR_TO, DL_CLASS_CODE_LR_NOTES, DL_CLASS_CODE_MR_FROM, DL_CLASS_CODE_MR_TO, DL_CLASS_CODE_MR_NOTES, DL_CLASS_CODE_HR_FROM, DL_CLASS_CODE_HR_TO, DL_CLASS_CODE_HR_NOTES, DL_CLASS_CODE_HC_FROM, DL_CLASS_CODE_HC_TO, DL_CLASS_CODE_HC_NOTES, DL_CLASS_CODE_MC_FROM, DL_CLASS_CODE_MC_TO, DL_CLASS_CODE_MC_NOTES, DL_CLASS_CODE_RE_FROM, DL_CLASS_CODE_RE_TO, DL_CLASS_CODE_RE_NOTES, DL_CLASS_CODE_R_FROM, DL_CLASS_CODE_R_TO, DL_CLASS_CODE_R_NOTES, DL_CLASS_CODE_CA_FROM, DL_CLASS_CODE_CA_TO, DL_CLASS_CODE_CA_NOTES, CITIZENSHIP_STATUS, MILITARY_SERVICE_FROM, MILITARY_SERVICE_TO, DL_CLASS_CODE_NT_FROM, DL_CLASS_CODE_NT_TO, DL_CLASS_CODE_NT_NOTES, DL_CLASS_CODE_TN_FROM, DL_CLASS_CODE_TN_TO, DL_CLASS_CODE_TN_NOTES, DL_CLASS_CODE_D3_FROM, DL_CLASS_CODE_D3_TO, DL_CLASS_CODE_D3_NOTES, ALT_DATE_OF_EXPIRE, DL_CLASS_CODE_CD_FROM, DL_CLASS_CODE_CD_TO, DL_CLASS_CODE_CD_NOTES, ISSUER_IDENTIFICATION_NUMBER, PAYMENT_PERIOD_FROM, PAYMENT_PERIOD_TO, VACCINATION_CERTIFICATE_IDENTIFIER, FIRST_NAME, DATE_OF_ARRIVAL, SECOND_NAME, THIRD_NAME, FOURTH_NAME, LAST_NAME, DL_CLASS_CODE_RM_FROM, DL_CLASS_CODE_RM_NOTES, DL_CLASS_CODE_RM_TO, DL_CLASS_CODE_PW_FROM, DL_CLASS_CODE_PW_NOTES, DL_CLASS_CODE_PW_TO, DL_CLASS_CODE_EB_FROM, DL_CLASS_CODE_EB_NOTES, DL_CLASS_CODE_EB_TO, DL_CLASS_CODE_EC_FROM, DL_CLASS_CODE_EC_NOTES, DL_CLASS_CODE_EC_TO, DL_CLASS_CODE_EC1_FROM, DL_CLASS_CODE_EC1_NOTES, DL_CLASS_CODE_EC1_TO, PLACE_OF_BIRTH_CITY, YEAR_OF_EXPIRY, GRANDFATHER_NAME_MATERNAL, _669]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_field_value.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_field_value.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_post_processing.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_post_processing.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/text_result_all_of.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/text_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/tfdsid_list.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/tfdsid_list.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/transaction_info.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/transaction_info.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/verification_result.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/verification_result.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/verified_field_map.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/verified_field_map.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/models/visibility.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/models/visibility.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula/documentreader/webclient/gen/rest.py` & `regula.documentreader.webclient-6.8.0/regula/documentreader/webclient/gen/rest.py`

 * *Files identical despite different names*

### Comparing `regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/PKG-INFO` & `regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.documentreader.webclient
-Version: 6.7.2
+Version: 6.8.0
 Summary: Regula's Document Reader python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: document-reader-client,document reader,document recognition,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.documentreader.webclient-6.7.2/regula.documentreader.webclient.egg-info/SOURCES.txt` & `regula.documentreader.webclient-6.8.0/regula.documentreader.webclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,23 @@
 regula/documentreader/webclient/gen/models/measure_system.py
 regula/documentreader/webclient/gen/models/mrz_format.py
 regula/documentreader/webclient/gen/models/ocr_security_text_result.py
 regula/documentreader/webclient/gen/models/ocr_security_text_result_all_of.py
 regula/documentreader/webclient/gen/models/one_candidate.py
 regula/documentreader/webclient/gen/models/original_symbol.py
 regula/documentreader/webclient/gen/models/p_array_field.py
+regula/documentreader/webclient/gen/models/parsing_notification_codes.py
 regula/documentreader/webclient/gen/models/per_document_config.py
 regula/documentreader/webclient/gen/models/photo_ident_result.py
 regula/documentreader/webclient/gen/models/photo_ident_result_all_of.py
 regula/documentreader/webclient/gen/models/point.py
 regula/documentreader/webclient/gen/models/point_array.py
 regula/documentreader/webclient/gen/models/points_container.py
 regula/documentreader/webclient/gen/models/process_params.py
+regula/documentreader/webclient/gen/models/process_params_rfid.py
 regula/documentreader/webclient/gen/models/process_request.py
 regula/documentreader/webclient/gen/models/process_request_image.py
 regula/documentreader/webclient/gen/models/process_response.py
 regula/documentreader/webclient/gen/models/process_system_info.py
 regula/documentreader/webclient/gen/models/processing_status.py
 regula/documentreader/webclient/gen/models/raw_image_container_list.py
 regula/documentreader/webclient/gen/models/rectangle_coordinates.py
```

### Comparing `regula.documentreader.webclient-6.7.2/setup.py` & `regula.documentreader.webclient-6.8.0/setup.py`

 * *Files identical despite different names*

