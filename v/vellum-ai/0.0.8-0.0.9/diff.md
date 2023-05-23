# Comparing `tmp/vellum_ai-0.0.8.tar.gz` & `tmp/vellum_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.0.8.tar", max compression
+gzip compressed data, was "vellum_ai-0.0.9.tar", max compression
```

## Comparing `vellum_ai-0.0.8.tar` & `vellum_ai-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     2980 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/README.md
--rw-r--r--   0        0        0      433 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3041 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/__init__.py
--rw-r--r--   0        0        0     9151 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/client.py
--rw-r--r--   0        0        0      348 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      498 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/environment.py
--rw-r--r--   0        0        0        0 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/py.typed
--rw-r--r--   0        0        0      172 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0     5769 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/model_versions/__init__.py
--rw-r--r--   0        0        0     2282 2023-05-09 22:09:52.146612 vellum_ai-0.0.8/src/vellum/resources/model_versions/client.py
--rw-r--r--   0        0        0       65 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/resources/sandboxes/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/resources/sandboxes/client.py
--rw-r--r--   0        0        0     4425 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/__init__.py
--rw-r--r--   0        0        0      687 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/block_type_enum.py
--rw-r--r--   0        0        0      818 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/chat_message.py
--rw-r--r--   0        0        0      825 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      645 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0     1117 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/document.py
--rw-r--r--   0        0        0     1268 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1745 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      639 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      831 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0      929 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1514 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1246 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1326 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0      992 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      840 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0     1012 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      435 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0      483 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_type_enum.py
--rw-r--r--   0        0        0     1241 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_build_config.py
--rw-r--r--   0        0        0     1021 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     1469 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_read.py
--rw-r--r--   0        0        0     2056 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_read.py
--rw-r--r--   0        0        0      895 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_read_status_enum.py
--rw-r--r--   0        0        0     1052 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0      890 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0      891 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      939 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0      835 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0      946 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/prompt_template_block.py
--rw-r--r--   0        0        0      860 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/prompt_template_block_data.py
--rw-r--r--   0        0        0      950 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/prompt_template_block_properties.py
--rw-r--r--   0        0        0     1039 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/provider_enum.py
--rw-r--r--   0        0        0      943 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/sandbox_input.py
--rw-r--r--   0        0        0      972 2023-05-09 22:09:52.150612 vellum_ai-0.0.8/src/vellum/types/sandbox_input_request.py
--rw-r--r--   0        0        0      802 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/sandbox_metric_input_params.py
--rw-r--r--   0        0        0      809 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/sandbox_metric_input_params_request.py
--rw-r--r--   0        0        0     1096 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/sandbox_scenario.py
--rw-r--r--   0        0        0      829 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0      881 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0     1486 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0      952 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1157 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_result.py
--rw-r--r--   0        0        0      834 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0      961 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     2009 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0      351 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/slim_document_status_enum.py
--rw-r--r--   0        0        0     1778 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      772 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0      468 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/type_enum.py
--rw-r--r--   0        0        0      763 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      837 2023-05-09 22:09:52.154612 vellum_ai-0.0.8/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 vellum_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2980 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/README.md
+-rw-r--r--   0        0        0      433 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3041 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/__init__.py
+-rw-r--r--   0        0        0    10132 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/client.py
+-rw-r--r--   0        0        0      348 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      498 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/environment.py
+-rw-r--r--   0        0        0        0 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/py.typed
+-rw-r--r--   0        0        0      172 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/model_versions/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/model_versions/client.py
+-rw-r--r--   0        0        0       65 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0     3912 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0     4425 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/block_type_enum.py
+-rw-r--r--   0        0        0      818 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0      825 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      645 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0     1117 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/document.py
+-rw-r--r--   0        0        0     1268 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1745 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      639 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      831 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0      929 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1514 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1246 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1326 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0      992 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      840 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0     1012 2023-05-12 00:21:24.135332 vellum_ai-0.0.9/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      435 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0      483 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_type_enum.py
+-rw-r--r--   0        0        0     1241 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_version_build_config.py
+-rw-r--r--   0        0        0     1021 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_version_exec_config_parameters.py
+-rw-r--r--   0        0        0     1469 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_version_exec_config_read.py
+-rw-r--r--   0        0        0     2056 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_version_read.py
+-rw-r--r--   0        0        0      895 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_version_read_status_enum.py
+-rw-r--r--   0        0        0     1052 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/model_version_sandbox_snapshot.py
+-rw-r--r--   0        0        0      890 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0      891 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      939 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0      835 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0      946 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/prompt_template_block.py
+-rw-r--r--   0        0        0      860 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/prompt_template_block_data.py
+-rw-r--r--   0        0        0      950 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/prompt_template_block_properties.py
+-rw-r--r--   0        0        0     1039 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/provider_enum.py
+-rw-r--r--   0        0        0      943 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/sandbox_input.py
+-rw-r--r--   0        0        0      972 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/sandbox_input_request.py
+-rw-r--r--   0        0        0      802 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/sandbox_metric_input_params.py
+-rw-r--r--   0        0        0      809 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/sandbox_metric_input_params_request.py
+-rw-r--r--   0        0        0     1096 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0      829 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0      881 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0     1486 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0      952 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1157 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0      834 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     2009 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0      351 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/slim_document_status_enum.py
+-rw-r--r--   0        0        0     1778 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      772 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0      468 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/type_enum.py
+-rw-r--r--   0        0        0      763 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      837 2023-05-12 00:21:24.139332 vellum_ai-0.0.9/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 vellum_ai-0.0.9/PKG-INFO
```

### Comparing `vellum_ai-0.0.8/README.md` & `vellum_ai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/__init__.py` & `vellum_ai-0.0.9/src/vellum/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/client.py` & `vellum_ai-0.0.9/src/vellum/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,86 +18,99 @@
 from .types.generate_options_request import GenerateOptionsRequest
 from .types.generate_request import GenerateRequest
 from .types.generate_response import GenerateResponse
 from .types.search_request_options_request import SearchRequestOptionsRequest
 from .types.search_response import SearchResponse
 from .types.submit_completion_actual_request import SubmitCompletionActualRequest
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
+
 
 class Vellum:
     def __init__(self, *, environment: VellumEnvironment = VellumEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     def generate(
         self,
         *,
-        deployment_id: typing.Optional[str] = None,
-        deployment_name: typing.Optional[str] = None,
+        deployment_id: typing.Optional[str] = OMIT,
+        deployment_name: typing.Optional[str] = OMIT,
         requests: typing.List[GenerateRequest],
-        options: typing.Optional[GenerateOptionsRequest] = None,
+        options: typing.Optional[GenerateOptionsRequest] = OMIT,
     ) -> GenerateResponse:
+        _request: typing.Dict[str, typing.Any] = {"requests": requests}
+        if deployment_id is not OMIT:
+            _request["deployment_id"] = deployment_id
+        if deployment_name is not OMIT:
+            _request["deployment_name"] = deployment_name
+        if options is not OMIT:
+            _request["options"] = options
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.predict}/", "v1/generate"),
-            json=jsonable_encoder(
-                {
-                    "deployment_id": deployment_id,
-                    "deployment_name": deployment_name,
-                    "requests": requests,
-                    "options": options,
-                }
-            ),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def search(
         self,
         *,
-        index_id: typing.Optional[str] = None,
-        index_name: typing.Optional[str] = None,
+        index_id: typing.Optional[str] = OMIT,
+        index_name: typing.Optional[str] = OMIT,
         query: str,
-        options: typing.Optional[SearchRequestOptionsRequest] = None,
+        options: typing.Optional[SearchRequestOptionsRequest] = OMIT,
     ) -> SearchResponse:
+        _request: typing.Dict[str, typing.Any] = {"query": query}
+        if index_id is not OMIT:
+            _request["index_id"] = index_id
+        if index_name is not OMIT:
+            _request["index_name"] = index_name
+        if options is not OMIT:
+            _request["options"] = options
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.predict}/", "v1/search"),
-            json=jsonable_encoder({"index_id": index_id, "index_name": index_name, "query": query, "options": options}),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SearchResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def submit_completion_actuals(
         self,
         *,
-        deployment_id: typing.Optional[str] = None,
-        deployment_name: typing.Optional[str] = None,
+        deployment_id: typing.Optional[str] = OMIT,
+        deployment_name: typing.Optional[str] = OMIT,
         actuals: typing.List[SubmitCompletionActualRequest],
     ) -> None:
+        _request: typing.Dict[str, typing.Any] = {"actuals": actuals}
+        if deployment_id is not OMIT:
+            _request["deployment_id"] = deployment_id
+        if deployment_name is not OMIT:
+            _request["deployment_name"] = deployment_name
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.predict}/", "v1/submit-completion-actuals"),
-            json=jsonable_encoder(
-                {"deployment_id": deployment_id, "deployment_name": deployment_name, "actuals": actuals}
-            ),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
@@ -122,82 +135,90 @@
     def __init__(self, *, environment: VellumEnvironment = VellumEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     async def generate(
         self,
         *,
-        deployment_id: typing.Optional[str] = None,
-        deployment_name: typing.Optional[str] = None,
+        deployment_id: typing.Optional[str] = OMIT,
+        deployment_name: typing.Optional[str] = OMIT,
         requests: typing.List[GenerateRequest],
-        options: typing.Optional[GenerateOptionsRequest] = None,
+        options: typing.Optional[GenerateOptionsRequest] = OMIT,
     ) -> GenerateResponse:
+        _request: typing.Dict[str, typing.Any] = {"requests": requests}
+        if deployment_id is not OMIT:
+            _request["deployment_id"] = deployment_id
+        if deployment_name is not OMIT:
+            _request["deployment_name"] = deployment_name
+        if options is not OMIT:
+            _request["options"] = options
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.predict}/", "v1/generate"),
-                json=jsonable_encoder(
-                    {
-                        "deployment_id": deployment_id,
-                        "deployment_name": deployment_name,
-                        "requests": requests,
-                        "options": options,
-                    }
-                ),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
                 timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def search(
         self,
         *,
-        index_id: typing.Optional[str] = None,
-        index_name: typing.Optional[str] = None,
+        index_id: typing.Optional[str] = OMIT,
+        index_name: typing.Optional[str] = OMIT,
         query: str,
-        options: typing.Optional[SearchRequestOptionsRequest] = None,
+        options: typing.Optional[SearchRequestOptionsRequest] = OMIT,
     ) -> SearchResponse:
+        _request: typing.Dict[str, typing.Any] = {"query": query}
+        if index_id is not OMIT:
+            _request["index_id"] = index_id
+        if index_name is not OMIT:
+            _request["index_name"] = index_name
+        if options is not OMIT:
+            _request["options"] = options
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.predict}/", "v1/search"),
-                json=jsonable_encoder(
-                    {"index_id": index_id, "index_name": index_name, "query": query, "options": options}
-                ),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
                 timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SearchResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def submit_completion_actuals(
         self,
         *,
-        deployment_id: typing.Optional[str] = None,
-        deployment_name: typing.Optional[str] = None,
+        deployment_id: typing.Optional[str] = OMIT,
+        deployment_name: typing.Optional[str] = OMIT,
         actuals: typing.List[SubmitCompletionActualRequest],
     ) -> None:
+        _request: typing.Dict[str, typing.Any] = {"actuals": actuals}
+        if deployment_id is not OMIT:
+            _request["deployment_id"] = deployment_id
+        if deployment_name is not OMIT:
+            _request["deployment_name"] = deployment_name
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.predict}/", "v1/submit-completion-actuals"),
-                json=jsonable_encoder(
-                    {"deployment_id": deployment_id, "deployment_name": deployment_name, "actuals": actuals}
-                ),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
                 timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
```

### Comparing `vellum_ai-0.0.8/src/vellum/core/datetime_utils.py` & `vellum_ai-0.0.9/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.0.9/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/resources/documents/client.py` & `vellum_ai-0.0.9/src/vellum/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/resources/model_versions/client.py` & `vellum_ai-0.0.9/src/vellum/resources/model_versions/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/resources/sandboxes/client.py` & `vellum_ai-0.0.9/src/vellum/resources/sandboxes/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,40 +11,43 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import VellumEnvironment
 from ...types.sandbox_input_request import SandboxInputRequest
 from ...types.sandbox_metric_input_params_request import SandboxMetricInputParamsRequest
 from ...types.sandbox_scenario import SandboxScenario
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
+
 
 class SandboxesClient:
     def __init__(self, *, environment: VellumEnvironment = VellumEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     def upsert_sandbox_scenario(
         self,
         id: str,
         *,
-        label: typing.Optional[str] = None,
+        label: typing.Optional[str] = OMIT,
         inputs: typing.List[SandboxInputRequest],
-        scenario_id: typing.Optional[str] = None,
-        metric_input_params: typing.Optional[SandboxMetricInputParamsRequest] = None,
+        scenario_id: typing.Optional[str] = OMIT,
+        metric_input_params: typing.Optional[SandboxMetricInputParamsRequest] = OMIT,
     ) -> SandboxScenario:
+        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
+        if label is not OMIT:
+            _request["label"] = label
+        if scenario_id is not OMIT:
+            _request["scenario_id"] = scenario_id
+        if metric_input_params is not OMIT:
+            _request["metric_input_params"] = metric_input_params
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.default}/", f"v1/sandboxes/{id}/scenarios"),
-            json=jsonable_encoder(
-                {
-                    "label": label,
-                    "inputs": inputs,
-                    "scenario_id": scenario_id,
-                    "metric_input_params": metric_input_params,
-                }
-            ),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SandboxScenario, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,31 +61,31 @@
         self._environment = environment
         self.api_key = api_key
 
     async def upsert_sandbox_scenario(
         self,
         id: str,
         *,
-        label: typing.Optional[str] = None,
+        label: typing.Optional[str] = OMIT,
         inputs: typing.List[SandboxInputRequest],
-        scenario_id: typing.Optional[str] = None,
-        metric_input_params: typing.Optional[SandboxMetricInputParamsRequest] = None,
+        scenario_id: typing.Optional[str] = OMIT,
+        metric_input_params: typing.Optional[SandboxMetricInputParamsRequest] = OMIT,
     ) -> SandboxScenario:
+        _request: typing.Dict[str, typing.Any] = {"inputs": inputs}
+        if label is not OMIT:
+            _request["label"] = label
+        if scenario_id is not OMIT:
+            _request["scenario_id"] = scenario_id
+        if metric_input_params is not OMIT:
+            _request["metric_input_params"] = metric_input_params
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.default}/", f"v1/sandboxes/{id}/scenarios"),
-                json=jsonable_encoder(
-                    {
-                        "label": label,
-                        "inputs": inputs,
-                        "scenario_id": scenario_id,
-                        "metric_input_params": metric_input_params,
-                    }
-                ),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers({"X_API_KEY": self.api_key}),
                 timeout=None,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SandboxScenario, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `vellum_ai-0.0.8/src/vellum/types/__init__.py` & `vellum_ai-0.0.9/src/vellum/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/block_type_enum.py` & `vellum_ai-0.0.9/src/vellum/types/block_type_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/chat_message.py` & `vellum_ai-0.0.9/src/vellum/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/chat_message_request.py` & `vellum_ai-0.0.9/src/vellum/types/chat_message_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/chat_message_role.py` & `vellum_ai-0.0.9/src/vellum/types/chat_message_role.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/document.py` & `vellum_ai-0.0.9/src/vellum/types/document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.0.9/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.0.9/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/finish_reason_enum.py` & `vellum_ai-0.0.9/src/vellum/types/finish_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_error_response.py` & `vellum_ai-0.0.9/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_options_request.py` & `vellum_ai-0.0.9/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_request.py` & `vellum_ai-0.0.9/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_response.py` & `vellum_ai-0.0.9/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_result.py` & `vellum_ai-0.0.9/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_result_data.py` & `vellum_ai-0.0.9/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/generate_result_error.py` & `vellum_ai-0.0.9/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/indexing_state_enum.py` & `vellum_ai-0.0.9/src/vellum/types/indexing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/model_version_build_config.py` & `vellum_ai-0.0.9/src/vellum/types/model_version_build_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_parameters.py` & `vellum_ai-0.0.9/src/vellum/types/model_version_exec_config_parameters.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/model_version_exec_config_read.py` & `vellum_ai-0.0.9/src/vellum/types/model_version_exec_config_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/model_version_read.py` & `vellum_ai-0.0.9/src/vellum/types/model_version_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/model_version_read_status_enum.py` & `vellum_ai-0.0.9/src/vellum/types/model_version_read_status_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/model_version_sandbox_snapshot.py` & `vellum_ai-0.0.9/src/vellum/types/model_version_sandbox_snapshot.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.0.9/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.0.9/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.0.9/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/processing_state_enum.py` & `vellum_ai-0.0.9/src/vellum/types/processing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/prompt_template_block.py` & `vellum_ai-0.0.9/src/vellum/types/prompt_template_block.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/prompt_template_block_data.py` & `vellum_ai-0.0.9/src/vellum/types/prompt_template_block_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/prompt_template_block_properties.py` & `vellum_ai-0.0.9/src/vellum/types/prompt_template_block_properties.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/provider_enum.py` & `vellum_ai-0.0.9/src/vellum/types/provider_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/sandbox_input.py` & `vellum_ai-0.0.9/src/vellum/types/sandbox_input.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/sandbox_input_request.py` & `vellum_ai-0.0.9/src/vellum/types/sandbox_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/sandbox_metric_input_params.py` & `vellum_ai-0.0.9/src/vellum/types/sandbox_metric_input_params.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/sandbox_metric_input_params_request.py` & `vellum_ai-0.0.9/src/vellum/types/sandbox_metric_input_params_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/sandbox_scenario.py` & `vellum_ai-0.0.9/src/vellum/types/sandbox_scenario.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_error_response.py` & `vellum_ai-0.0.9/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_filters_request.py` & `vellum_ai-0.0.9/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.0.9/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_response.py` & `vellum_ai-0.0.9/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_result.py` & `vellum_ai-0.0.9/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.0.9/src/vellum/types/search_result_merging_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/search_weights_request.py` & `vellum_ai-0.0.9/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/slim_document.py` & `vellum_ai-0.0.9/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.0.9/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.0.9/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.0.9/src/vellum/types/upload_document_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/src/vellum/types/upload_document_response.py` & `vellum_ai-0.0.9/src/vellum/types/upload_document_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.8/PKG-INFO` & `vellum_ai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

