# Comparing `tmp/pybiolib-1.1.911.tar.gz` & `tmp/pybiolib-1.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiolib-1.1.911.tar", max compression
+gzip compressed data, was "pybiolib-1.1.94.tar", max compression
```

## Comparing `pybiolib-1.1.911.tar` & `pybiolib-1.1.94.tar`

### file list

```diff
@@ -1,110 +1,96 @@
--rw-r--r--   0        0        0     1067 2023-05-22 20:19:15.002725 pybiolib-1.1.911/LICENSE
--rw-r--r--   0        0        0      368 2023-05-22 20:19:15.002725 pybiolib-1.1.911/README.md
--rw-r--r--   0        0        0     3337 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/__init__.py
--rw-r--r--   0        0        0       95 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/api/__init__.py
--rw-r--r--   0        0        0     2969 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/api/client.py
--rw-r--r--   0        0        0       37 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/app/__init__.py
--rw-r--r--   0        0        0     7652 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/app/app.py
--rw-r--r--   0        0        0     1493 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/app/search_apps.py
--rw-r--r--   0        0        0     4405 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/app/utils.py
--rw-r--r--   0        0        0      182 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/__init__.py
--rw-r--r--   0        0        0     5574 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/api_client.py
--rw-r--r--   0        0        0     2397 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/app_types.py
--rw-r--r--   0        0        0     1668 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/auth.py
--rw-r--r--   0        0        0      580 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/biolib_account_api.py
--rw-r--r--   0        0        0     2859 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/biolib_app_api.py
--rw-r--r--   0        0        0     9865 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/biolib_job_api.py
--rw-r--r--   0        0        0     1777 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/biolib_large_file_system_api.py
--rw-r--r--   0        0        0      123 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/common_types.py
--rw-r--r--   0        0        0     1256 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/job_types.py
--rw-r--r--   0        0        0      227 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/lfs_types.py
--rw-r--r--   0        0        0      637 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_api_client/user_state.py
--rw-r--r--   0        0        0      303 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/__init__.py
--rw-r--r--   0        0        0      959 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/base_bbf_package.py
--rw-r--r--   0        0        0      154 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/common_types.py
--rw-r--r--   0        0        0     6450 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/encrypted_module_output.py
--rw-r--r--   0        0        0     2603 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/module_input.py
--rw-r--r--   0        0        0     2640 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/module_output.py
--rw-r--r--   0        0        0     2269 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
--rw-r--r--   0        0        0     1125 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/saved_job.py
--rw-r--r--   0        0        0     1023 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/stdout_and_stderr.py
--rw-r--r--   0        0        0      853 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/system_exception.py
--rw-r--r--   0        0        0     1191 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/system_status_update.py
--rw-r--r--   0        0        0     8514 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/unencrypted_module_output.py
--rw-r--r--   0        0        0     3938 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_binary_format/utils.py
--rw-r--r--   0        0        0     1481 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_docker_client/__init__.py
--rw-r--r--   0        0        0      532 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_errors.py
--rw-r--r--   0        0        0     2854 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_logging.py
--rw-r--r--   0        0        0    10225 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/biolib_push.py
--rw-r--r--   0        0        0      947 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/__init__.py
--rw-r--r--   0        0        0      820 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/init.py
--rw-r--r--   0        0        0     1966 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/lfs.py
--rw-r--r--   0        0        0      798 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/push.py
--rw-r--r--   0        0        0     1309 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/run.py
--rw-r--r--   0        0        0      361 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/runtime.py
--rw-r--r--   0        0        0     1284 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli/start.py
--rw-r--r--   0        0        0     8947 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/cli_utils.py
--rw-r--r--   0        0        0       45 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/.gitignore
--rw-r--r--   0        0        0        0 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/__init__.py
--rw-r--r--   0        0        0       67 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/cloud_utils/__init__.py
--rw-r--r--   0        0        0     6878 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/cloud_utils/cloud_utils.py
--rw-r--r--   0        0        0       71 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/__init__.py
--rw-r--r--   0        0        0     3670 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/cache_state.py
--rw-r--r--   0        0        0      891 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/cache_types.py
--rw-r--r--   0        0        0     7562 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/docker_image_cache.py
--rw-r--r--   0        0        0      221 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/__init__.py
--rw-r--r--   0        0        0      448 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/base_executor.py
--rw-r--r--   0        0        0    24367 2023-05-22 20:19:15.002725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/docker_executor.py
--rw-r--r--   0        0        0      122 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/docker_types.py
--rw-r--r--   0        0        0       91 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/remote/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/remote/remote_executor.py
--rw-r--r--   0        0        0        0 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/tars/__init__.py
--rw-r--r--   0        0        0     1564 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/executors/types.py
--rw-r--r--   0        0        0     1198 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
--rw-r--r--   0        0        0     1174 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
--rw-r--r--   0        0        0     4858 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/job_storage.py
--rw-r--r--   0        0        0    29919 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/job_worker.py
--rw-r--r--   0        0        0     9363 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/large_file_system.py
--rw-r--r--   0        0        0     2499 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/mappings.py
--rw-r--r--   0        0        0     1282 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/job_worker/utils.py
--rw-r--r--   0        0        0    12829 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/remote_host_proxy.py
--rw-r--r--   0        0        0     1601 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/socker_listener_thread.py
--rw-r--r--   0        0        0      971 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/socket_sender_thread.py
--rw-r--r--   0        0        0     4434 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/utils.py
--rw-r--r--   0        0        0        0 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/webserver/__init__.py
--rw-r--r--   0        0        0      914 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/webserver/gunicorn_flask_application.py
--rw-r--r--   0        0        0     7647 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/webserver/webserver.py
--rw-r--r--   0        0        0      420 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/webserver/webserver_types.py
--rw-r--r--   0        0        0     4234 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/webserver/webserver_utils.py
--rw-r--r--   0        0        0     9900 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/compute_node/webserver/worker_thread.py
--rw-r--r--   0        0        0        0 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/experiments/__init__.py
--rw-r--r--   0        0        0     5939 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/experiments/experiment.py
--rw-r--r--   0        0        0      171 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/experiments/types.py
--rw-r--r--   0        0        0       32 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/jobs/__init__.py
--rw-r--r--   0        0        0    14468 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/jobs/job.py
--rw-r--r--   0        0        0     5937 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/jobs/job_result.py
--rw-r--r--   0        0        0      905 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/jobs/types.py
--rw-r--r--   0        0        0      193 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/lfs/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/lfs/cache.py
--rw-r--r--   0        0        0     9832 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/lfs/utils.py
--rw-r--r--   0        0        0       44 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/runtime/__init__.py
--rw-r--r--   0        0        0      778 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/runtime/results.py
--rw-r--r--   0        0        0      210 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/start_cli.py
--rw-r--r--   0        0        0      872 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/tables.py
--rw-r--r--   0        0        0       36 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/templates/__init__.py
--rw-r--r--   0        0        0      715 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/templates/example_app.py
--rw-r--r--   0        0        0      263 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/typing_utils.py
--rw-r--r--   0        0        0       39 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/user/__init__.py
--rw-r--r--   0        0        0     2061 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/user/sign_in.py
--rw-r--r--   0        0        0     8190 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/utils/__init__.py
--rw-r--r--   0        0        0     2727 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/utils/cache_state.py
--rw-r--r--   0        0        0     9717 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/utils/multipart_uploader.py
--rw-r--r--   0        0        0     1345 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/utils/seq_util.py
--rw-r--r--   0        0        0    23500 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/utils/zip/remote_zip.py
--rw-r--r--   0        0        0     6916 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/validators/validate_app_version.py
--rw-r--r--   0        0        0     4300 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/validators/validate_argument.py
--rw-r--r--   0        0        0    13298 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/validators/validate_module.py
--rw-r--r--   0        0        0     1655 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/validators/validate_zip_file.py
--rw-r--r--   0        0        0     2135 2023-05-22 20:19:15.006725 pybiolib-1.1.911/biolib/validators/validator_utils.py
--rw-r--r--   0        0        0     1237 2023-05-22 20:20:07.799245 pybiolib-1.1.911/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.911/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-12 11:16:01.133705 pybiolib-1.1.94/LICENSE
+-rw-r--r--   0        0        0      369 2022-07-12 11:16:01.133705 pybiolib-1.1.94/README.md
+-rw-r--r--   0        0        0     1923 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/__init__.py
+-rw-r--r--   0        0        0       78 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/api/__init__.py
+-rw-r--r--   0        0        0     1643 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/api/client.py
+-rw-r--r--   0        0        0       37 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/app/__init__.py
+-rw-r--r--   0        0        0     4264 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/app/app.py
+-rw-r--r--   0        0        0     3162 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/app/app_result.py
+-rw-r--r--   0        0        0     4138 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/app/utils.py
+-rw-r--r--   0        0        0      182 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/__init__.py
+-rw-r--r--   0        0        0     5574 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/api_client.py
+-rw-r--r--   0        0        0     2355 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/app_types.py
+-rw-r--r--   0        0        0     1668 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/auth.py
+-rw-r--r--   0        0        0      580 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/biolib_account_api.py
+-rw-r--r--   0        0        0     2859 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/biolib_app_api.py
+-rw-r--r--   0        0        0     9165 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/biolib_job_api.py
+-rw-r--r--   0        0        0     2646 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/biolib_large_file_system_api.py
+-rw-r--r--   0        0        0      123 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/common_types.py
+-rw-r--r--   0        0        0     1205 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/job_types.py
+-rw-r--r--   0        0        0      493 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/lfs_types.py
+-rw-r--r--   0        0        0      635 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_api_client/user_state.py
+-rw-r--r--   0        0        0      303 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/__init__.py
+-rw-r--r--   0        0        0      959 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/base_bbf_package.py
+-rw-r--r--   0        0        0      154 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/common_types.py
+-rw-r--r--   0        0        0     6450 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/encrypted_module_output.py
+-rw-r--r--   0        0        0     2594 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/module_input.py
+-rw-r--r--   0        0        0     2452 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/module_output.py
+-rw-r--r--   0        0        0     2269 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
+-rw-r--r--   0        0        0     1125 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/saved_job.py
+-rw-r--r--   0        0        0     1023 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/stdout_and_stderr.py
+-rw-r--r--   0        0        0      853 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/system_exception.py
+-rw-r--r--   0        0        0     1191 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/system_status_update.py
+-rw-r--r--   0        0        0     6887 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/unencrypted_module_output.py
+-rw-r--r--   0        0        0     3595 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_binary_format/utils.py
+-rw-r--r--   0        0        0     1121 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_docker_client/__init__.py
+-rw-r--r--   0        0        0      381 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_errors.py
+-rw-r--r--   0        0        0     2854 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_logging.py
+-rw-r--r--   0        0        0    10219 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_push.py
+-rw-r--r--   0        0        0     1029 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/biolib_singularity_client/__init__.py
+-rw-r--r--   0        0        0    11204 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/cli.py
+-rw-r--r--   0        0        0     8859 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/cli_utils.py
+-rw-r--r--   0        0        0       45 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/.gitignore
+-rw-r--r--   0        0        0        0 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/__init__.py
+-rw-r--r--   0        0        0       67 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/cloud_utils/__init__.py
+-rw-r--r--   0        0        0     6976 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/cloud_utils/cloud_utils.py
+-rw-r--r--   0        0        0       71 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/__init__.py
+-rw-r--r--   0        0        0     3531 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/cache_state.py
+-rw-r--r--   0        0        0      922 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/cache_types.py
+-rw-r--r--   0        0        0     6517 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/docker_image_cache.py
+-rw-r--r--   0        0        0      315 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/__init__.py
+-rw-r--r--   0        0        0      448 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/base_executor.py
+-rw-r--r--   0        0        0    21198 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/docker_executor.py
+-rw-r--r--   0        0        0      122 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/docker_types.py
+-rw-r--r--   0        0        0       91 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/remote/__init__.py
+-rw-r--r--   0        0        0     1842 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/remote/remote_executor.py
+-rw-r--r--   0        0        0    13537 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/singularity_executor.py
+-rw-r--r--   0        0        0        0 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/tars/__init__.py
+-rw-r--r--   0        0        0     1493 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/executors/types.py
+-rw-r--r--   0        0        0      394 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/job_key_cache.py
+-rw-r--r--   0        0        0     1174 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
+-rw-r--r--   0        0        0     5332 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/job_storage.py
+-rw-r--r--   0        0        0    27753 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/job_worker.py
+-rw-r--r--   0        0        0    10277 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/large_file_system.py
+-rw-r--r--   0        0        0     2499 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/mappings.py
+-rw-r--r--   0        0        0     1282 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/job_worker/utils.py
+-rw-r--r--   0        0        0    10090 2022-07-12 11:16:01.133705 pybiolib-1.1.94/biolib/compute_node/remote_host_proxy.py
+-rw-r--r--   0        0        0     1601 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/socker_listener_thread.py
+-rw-r--r--   0        0        0      971 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/socket_sender_thread.py
+-rw-r--r--   0        0        0     4366 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/utils.py
+-rw-r--r--   0        0        0        0 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/webserver/__init__.py
+-rw-r--r--   0        0        0      914 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/webserver/gunicorn_flask_application.py
+-rw-r--r--   0        0        0     6570 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/webserver/webserver.py
+-rw-r--r--   0        0        0      490 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/webserver/webserver_types.py
+-rw-r--r--   0        0        0     4122 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/webserver/webserver_utils.py
+-rw-r--r--   0        0        0    10799 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/compute_node/webserver/worker_thread.py
+-rw-r--r--   0        0        0       32 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/jobs/__init__.py
+-rw-r--r--   0        0        0      453 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/jobs/job.py
+-rw-r--r--   0        0        0     3754 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/jobs/job_result.py
+-rw-r--r--   0        0        0     7412 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/lfs.py
+-rw-r--r--   0        0        0      210 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/start_cli.py
+-rw-r--r--   0        0        0       36 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/templates/__init__.py
+-rw-r--r--   0        0        0      715 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/templates/example_app.py
+-rw-r--r--   0        0        0      263 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/typing_utils.py
+-rw-r--r--   0        0        0       39 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/user/__init__.py
+-rw-r--r--   0        0        0     2061 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/user/sign_in.py
+-rw-r--r--   0        0        0     7554 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/utils/__init__.py
+-rw-r--r--   0        0        0     2635 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/utils/cache_state.py
+-rw-r--r--   0        0        0     7743 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/utils/multipart_uploader.py
+-rw-r--r--   0        0        0     6916 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/validators/validate_app_version.py
+-rw-r--r--   0        0        0     4300 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/validators/validate_argument.py
+-rw-r--r--   0        0        0    13298 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/validators/validate_module.py
+-rw-r--r--   0        0        0     1655 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/validators/validate_zip_file.py
+-rw-r--r--   0        0        0     2135 2022-07-12 11:16:01.137705 pybiolib-1.1.94/biolib/validators/validator_utils.py
+-rw-r--r--   0        0        0     1169 2022-07-12 11:17:14.966690 pybiolib-1.1.94/pyproject.toml
+-rw-r--r--   0        0        0     2043 2022-07-12 11:17:15.586946 pybiolib-1.1.94/setup.py
+-rw-r--r--   0        0        0     1546 2022-07-12 11:17:15.587411 pybiolib-1.1.94/PKG-INFO
```

### Comparing `pybiolib-1.1.911/LICENSE` & `pybiolib-1.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/api/client.py` & `pybiolib-1.1.94/biolib/api/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,51 @@
 from urllib.parse import urljoin
 
 import requests
-from requests import Response, HTTPError
+from requests import Response
 
-from biolib.typing_utils import Dict, Optional, Union
+from biolib.typing_utils import Dict
 from biolib.biolib_api_client import BiolibApiClient as DeprecatedApiClient
 
 
 class ApiClient:
 
-    def get(
-            self,
-            url: str,
-            params: Optional[Dict[str, Union[str, int]]] = None,
-            headers: Optional[Dict[str, str]] = None,
-            authenticate: bool = True,
-    ) -> Response:
+    def get(self, url: str, params: Dict[str, str]) -> Response:
         response = requests.get(
-            headers=self._get_headers(headers, authenticate),
+            headers=self._get_headers(),
             params=params,
             timeout=10,
             url=self._get_absolute_url(url),
         )
-        ApiClient.raise_for_status(response)
+        response.raise_for_status()
         return response
 
-    def post(self, path: str, data: Dict, headers: Optional[Dict[str, str]] = None) -> Response:
+    def post(self, path: str, data: Dict) -> Response:
         response = requests.post(
-            headers=self._get_headers(headers),
+            headers=self._get_headers(),
             json=data,
             timeout=10,
             url=self._get_absolute_url(path),
         )
-        ApiClient.raise_for_status(response)
+        response.raise_for_status()
         return response
 
-    def patch(self, path: str, data: Dict, headers: Optional[Dict[str, str]] = None) -> Response:
-        response = requests.patch(
-            headers=self._get_headers(headers),
-            json=data,
-            timeout=10,
-            url=self._get_absolute_url(path),
-        )
-        ApiClient.raise_for_status(response)
-        return response
-
-    @staticmethod
-    def raise_for_status(response):
-        # Logic taken from `requests.Response.raise_for_status()`
-        http_error_msg = ''
-        reason = response.text
-        if 400 <= response.status_code < 500:
-            http_error_msg = u'%s Client Error: %s for url: %s' % (response.status_code, reason, response.url)
-
-        elif 500 <= response.status_code < 600:
-            http_error_msg = u'%s Server Error: %s for url: %s' % (response.status_code, reason, response.url)
-
-        if http_error_msg:
-            raise HTTPError(http_error_msg, response=response)
-
     @staticmethod
-    def _get_headers(opt_headers: Optional[Dict[str, str]] = None, authenticate: bool = True) -> Dict[str, str]:
-        headers: Dict[str, str] = opt_headers or {}
+    def _get_headers() -> Dict[str, str]:
+        headers: Dict[str, str] = {}
 
         deprecated_api_client = DeprecatedApiClient.get()
 
         if deprecated_api_client.is_signed_in:
             deprecated_api_client.refresh_access_token()
 
         # Adding access_token outside is_signed_in check as job_worker.py currently sets access_token
         # without setting refresh_token
         access_token = deprecated_api_client.access_token
-        if access_token and authenticate:
+        if access_token:
             headers['Authorization'] = f'Bearer {access_token}'
 
         return headers
 
     @staticmethod
     def _get_absolute_url(path: str) -> str:
         deprecated_api_client = DeprecatedApiClient.get()
```

### Comparing `pybiolib-1.1.911/biolib/app/utils.py` & `pybiolib-1.1.94/biolib/app/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,52 +2,49 @@
 import os
 import sys
 import random
 import subprocess
 import threading
 import time
 import pathlib
-from io import BytesIO
-from typing import BinaryIO
 
 import requests.exceptions
 
 from biolib import utils
 from biolib.biolib_api_client import BiolibApiClient
 from biolib.biolib_api_client.biolib_job_api import BiolibJobApi
-from biolib.biolib_binary_format import UnencryptedModuleOutput, InMemoryIndexableBuffer
+from biolib.biolib_binary_format import ModuleOutput
+from biolib.biolib_docker_client import BiolibDockerClient
 from biolib.biolib_errors import BioLibError
 from biolib.biolib_logging import logger
+from biolib.biolib_singularity_client import BiolibSingularityClient
 from biolib.compute_node.job_worker.executors import RemoteExecutor, RemoteExecuteOptions
 from biolib.utils import stream_process_output
 from biolib.typing_utils import Optional
 
 
-def run_job(
-        job,
-        module_input_serialized: bytes,
-        force_local: bool = False,
-        result_name_prefix: Optional[str] = None,
-) -> UnencryptedModuleOutput:
+# TODO: type return value as ModuleOutput class
+def run_job(job, module_input_serialized: bytes):
     job_id = job['public_id']
+    modules = job['app_version'].get('modules')
     logger.info(f'Job "{job_id}" is starting...')
 
-    if not force_local:
-        return RemoteExecutor.execute_job(
+    # Run in remote (in cloud)
+    if modules is None or utils.BIOLIB_FORCE_REMOTE_COMPUTE or not utils.BASE_URL_IS_PUBLIC_BIOLIB or (
+            not BiolibDockerClient.is_docker_running() and not BiolibSingularityClient.is_singularity_running()
+    ):
+        result = RemoteExecutor.execute_job(
             RemoteExecuteOptions(
                 biolib_base_url=utils.BIOLIB_BASE_URL,
                 job=job,
-                result_name_prefix=result_name_prefix,
                 root_job_id=job_id,
             ),
             module_input_serialized,
         )
-
-    if not job['app_version'].get('modules'):
-        BioLibError('Unable to run the application locally')
+        return ModuleOutput(result).deserialize()
 
     # Run locally
     host = '127.0.0.1'
     port = str(random.choice(range(5000, 65000)))
     node_url = f'http://{host}:{port}'
     logger.debug(f'Starting local compute node at {node_url}')
     start_cli_path = pathlib.Path(__file__).parent.parent.resolve() / 'start_cli.py'
@@ -91,29 +88,22 @@
                 break
 
             except requests.exceptions.ConnectionError:
                 if retry == 19:
                     raise BioLibError('Could not connect to local compute node') from None
                 logger.debug('Could not connect to local compute node retrying...')
 
-        BiolibJobApi.start_local_job(job_id, module_input_serialized, node_url)
-        BiolibJobApi.await_local_compute_node_status(
+        BiolibJobApi.start_cloud_job(job_id, module_input_serialized, node_url)
+        BiolibJobApi.await_compute_node_status(
             retry_interval_seconds=1.5,
             retry_limit_minutes=43800,  # Let users run an app locally for a month (43800 minutes)
             status_to_await='Result Ready',
             compute_type='Compute Node',
             node_url=node_url,
             job=job,
         )
 
         result = BiolibJobApi.get_cloud_result(job_id, node_url)
-        unencrypted_module_output: BinaryIO = BytesIO()
-        legacy_module_output: BinaryIO = BytesIO(result)
-        UnencryptedModuleOutput.write_to_file_from_legacy_module_output_file(
-            input_file=legacy_module_output,
-            output_file=unencrypted_module_output
-        )
-        unencrypted_module_output.seek(0)
-        return UnencryptedModuleOutput(InMemoryIndexableBuffer(unencrypted_module_output.read()))
+        return ModuleOutput(result).deserialize()
 
     finally:
         compute_node_process.terminate()
```

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/api_client.py` & `pybiolib-1.1.94/biolib/biolib_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/app_types.py` & `pybiolib-1.1.94/biolib/biolib_api_client/app_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     active_version: str
     allow_client_side_execution: bool
     created_at: str
     is_license_required: bool
     name: str
     public_id: str
     state: str
-    resource_uri: str
 
 
 class AppGetResponse(TypedDict):
     app: App
     app_uri: str
     app_version: AppVersion
 
@@ -81,15 +80,14 @@
 
 # type optional keys with total=False
 class Module(_Module, total=False):
     secrets: Dict[str, str]
 
 
 class _AppVersionOnJob(TypedDict):
-    created_at: str
     client_side_executable_zip: Optional[str]
     consumes_stdin: bool
     is_runnable_by_user: bool
     public_id: str
     remote_hosts: List[RemoteHost]
     settings: List[Dict]
     stdout_render_type: Literal['text', 'markdown']
```

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/auth.py` & `pybiolib-1.1.94/biolib/biolib_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/biolib_account_api.py` & `pybiolib-1.1.94/biolib/biolib_api_client/biolib_account_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/biolib_app_api.py` & `pybiolib-1.1.94/biolib/biolib_api_client/biolib_app_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/biolib_job_api.py` & `pybiolib-1.1.94/biolib/biolib_api_client/biolib_job_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import base64
 import os
-import sys
 import time
-from urllib.parse import urlparse
-
+import sys
 import requests
 
 import biolib.api
 
 from biolib import utils
 from biolib.biolib_api_client.auth import BearerAuth
-from biolib.biolib_api_client import BiolibApiClient, CreatedJobDict, CloudJob
+from biolib.biolib_api_client import BiolibApiClient, Job
 from biolib.biolib_binary_format.stdout_and_stderr import StdoutAndStderr
-from biolib.biolib_errors import BioLibError, RetryLimitException, StorageDownloadFailed
+from biolib.biolib_errors import BioLibError
 from biolib.compute_node.utils import SystemExceptionCodeMap
 from biolib.biolib_logging import logger
-from biolib.utils import BIOLIB_PACKAGE_VERSION, IS_RUNNING_IN_NOTEBOOK
-from biolib.typing_utils import List, TypedDict, Optional, Literal
+from biolib.utils import BIOLIB_PACKAGE_VERSION
+from biolib.typing_utils import List, TypedDict, Optional
+
+
+class RetryException(Exception):
+    pass
 
 
 class PresignedS3UploadLinkResponse(TypedDict):
     presigned_upload_url: str
 
 
 class PresignedS3DownloadLinkResponse(TypedDict):
@@ -40,21 +42,15 @@
 
     return None
 
 
 class BiolibJobApi:
 
     @staticmethod
-    def create(
-            app_version_id,
-            override_command=False,
-            caller_job=None,
-            machine='',
-            experiment_uuid: Optional[str] = None
-    ):
+    def create(app_version_id, override_command=False, caller_job=None):
         data = {
             'app_version_id': app_version_id,
             'client_type': 'biolib-python',
             'client_version': BIOLIB_PACKAGE_VERSION,
             'client_opt_user_info': _get_user_info(),
         }
 
@@ -62,22 +58,14 @@
             data.update({
                 'arguments_override_command': override_command
             })
 
         if caller_job:
             data['caller_job'] = caller_job
 
-        if machine:
-            data.update({
-                'requested_machine': machine
-            })
-
-        if experiment_uuid:
-            data['experiment_uuid'] = experiment_uuid
-
         response = biolib.api._client.post(path='/jobs/', data=data)  # pylint: disable=protected-access
 
         return response.json()
 
     @staticmethod
     def update_state(job_id, state):
         response = requests.patch(
@@ -89,94 +77,101 @@
         # TODO: Error handling with response object
         if not response.ok:
             raise BioLibError(response.content)
 
         return response.json()
 
     @staticmethod
-    def create_cloud_job(job_id: str, result_name_prefix: Optional[str]) -> CloudJob:
+    def create_cloud_job(module_name, job_id):
         response = None
-        data = {'job_id': job_id}
-        if result_name_prefix:
-            data['result_name_prefix'] = result_name_prefix
-
         for retry in range(4):
             try:
                 response = requests.post(
                     f'{BiolibApiClient.get().base_url}/api/jobs/cloud/',
-                    json=data,
+                    json={'module_name': module_name, 'job_id': job_id},
                     auth=BearerAuth(BiolibApiClient.get().access_token)
                 )
 
                 if response.status_code == 503:
-                    raise RetryLimitException(response.content)
+                    raise RetryException(response.content)
                 # Handle possible validation errors from backend
                 elif not response.ok:
                     raise BioLibError(response.text)
 
                 break
 
-            except RetryLimitException as retry_exception:  # pylint: disable=broad-except
+            except RetryException as retry_exception:  # pylint: disable=broad-except
                 if retry > 3:
                     raise BioLibError('Reached retry limit for cloud job creation') from retry_exception
                 time.sleep(1)
 
         if not response:
             raise BioLibError('Could not create new cloud job')
 
-        cloud_job: CloudJob = response.json()
-        return cloud_job
+        cloud_job = response.json()
+        if cloud_job.get('is_compute_node_ready', False):
+            return cloud_job
+
+        max_retry_attempts = 100
+        retry_interval_seconds = 10
+
+        for _ in range(max_retry_attempts):
+            response = requests.get(
+                f'{BiolibApiClient.get().base_url}/api/jobs/cloud/{cloud_job["public_id"]}/status/',
+                auth=BearerAuth(BiolibApiClient.get().access_token)
+            )
+            cloud_job = response.json()
+            if cloud_job.get('is_compute_node_ready', False):
+                return cloud_job
+
+            logger.info('Cloud: Server capacity is being allocated. Please wait...')
+            time.sleep(retry_interval_seconds)
+
+        raise BioLibError('Cloud: The reserved compute node was not ready in time')
 
     @staticmethod
     def save_compute_node_job(job, module_name, access_token, node_url):
         response = requests.post(
             f'{node_url}/v1/job/',
             json={'module_name': module_name, 'job': job, 'access_token': access_token}
         )
 
         if not response.ok:
             raise BioLibError(response.content)
 
         return response.json
 
     @staticmethod
-    def start_local_job(job_id, module_input_serialized, node_url):
+    def start_cloud_job(job_id, module_input_serialized, node_url, aes_key_string_b64=None):
+        headers = {}
+        if aes_key_string_b64:
+            headers['AES-Key-String'] = aes_key_string_b64
+
         response = requests.post(
             f'{node_url}/v1/job/{job_id}/start/',
             data=module_input_serialized,
+            headers=headers
         )
 
         if not response.ok:
             raise BioLibError(response.content)
 
-    # TODO: Deprecate this
     @staticmethod
-    def await_local_compute_node_status(
+    def await_compute_node_status(
             retry_interval_seconds: float,
             retry_limit_minutes: float,
             status_to_await: str,
             compute_type: str,
             node_url: str,
-            job: CreatedJobDict,
+            job: Job,
     ):
         status_max_retry_attempts = int(retry_limit_minutes * 60 / retry_interval_seconds)
         status_is_reached = False
         final_status_messages: List[str] = []
 
-        def print_logs_packages(stdout_and_stderr_packages_b64):
-            for stdout_and_stderr_package_b64 in stdout_and_stderr_packages_b64:
-                stdout_and_stderr_package = base64.b64decode(stdout_and_stderr_package_b64)
-                stdout_and_stderr = StdoutAndStderr(stdout_and_stderr_package).deserialize()
-
-                sys.stdout.write(stdout_and_stderr.decode())
-                if not IS_RUNNING_IN_NOTEBOOK:  # for some reason flushing in jupyter notebooks breaks \r handling
-                    sys.stdout.flush()
-            # flush after having processed all packages
-            sys.stdout.flush()
-
         for _ in range(status_max_retry_attempts):
             response = requests.get(f'{node_url}/v1/job/{job["public_id"]}/status/')
             if not response.ok:
                 raise Exception(response.content)
 
             status_json = response.json()
 
@@ -190,15 +185,20 @@
                 else:
                     # Print the status before writing stdout and stderr
                     logger.info(f'{compute_type}: {status_update["log_message"]}')
 
             app_version = job['app_version']
             if 'stdout_and_stderr_packages_b64' in status_json and utils.STREAM_STDOUT and \
                     (app_version.get('main_output_file') or app_version.get('stdout_render_type') == 'text'):
-                print_logs_packages(status_json['stdout_and_stderr_packages_b64'])
+                for stdout_and_stderr_package_b64 in status_json['stdout_and_stderr_packages_b64']:
+                    stdout_and_stderr_package = base64.b64decode(stdout_and_stderr_package_b64)
+                    stdout_and_stderr = StdoutAndStderr(stdout_and_stderr_package).deserialize()
+
+                    sys.stdout.write(stdout_and_stderr.decode())
+                    sys.stdout.flush()
 
             if 'error_code' in status_json:
                 error_code = status_json['error_code']
                 error_message = SystemExceptionCodeMap.get(error_code, f'Unknown error code {error_code}')
 
                 raise BioLibError(f'{compute_type}: {error_message}')
 
@@ -236,36 +236,21 @@
     def get_enclave_json(biolib_base_url):
         response = requests.get(
             f'{biolib_base_url}/info-files/biolib-enclave.json',
         )
         return response.json()
 
     @staticmethod
-    def get_job_storage_download_url(
-            job_uuid: str,
-            job_auth_token: str,
-            storage_type: Literal['input', 'results'],
-    ) -> str:
+    def get_job_storage_result_download_url(job_auth_token) -> str:
         response = requests.get(
-            f'{BiolibApiClient.get().base_url}/api/jobs/{job_uuid}/storage/{storage_type}/download/',
+            f'{BiolibApiClient.get().base_url}/api/jobs/storage/results/download/',
             auth=BearerAuth(BiolibApiClient.get().access_token),
             headers={
                 'Job-Auth-Token': job_auth_token
             }
         )
 
         if not response.ok:
-            if response.status_code == 404:
-                raise StorageDownloadFailed(response.content)
-            else:
-                raise BioLibError(response.content)
+            raise BioLibError(response.content)
 
         presigned_s3_download_link_response: PresignedS3DownloadLinkResponse = response.json()
-        presigned_download_url = presigned_s3_download_link_response['presigned_download_url']
-
-        app_caller_proxy_job_storage_base_url = os.getenv('BIOLIB_CLOUD_JOB_STORAGE_BASE_URL', '')
-        if app_caller_proxy_job_storage_base_url:
-            # Done to hit App Caller Proxy when downloading result from inside an app
-            parsed_url = urlparse(presigned_download_url)
-            presigned_download_url = f'{app_caller_proxy_job_storage_base_url}{parsed_url.path}?{parsed_url.query}'
-
-        return presigned_download_url
+        return presigned_s3_download_link_response['presigned_download_url']
```

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/job_types.py` & `pybiolib-1.1.94/biolib/biolib_api_client/job_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,38 +12,36 @@
     COMPLETED = 'completed'
     FAILED = 'failed'
     IN_PROGRESS = 'in_progress'
 
 
 class _Job(TypedDict):
     app_version: AppVersionOnJob
-    arguments_override_command: bool
     auth_token: str
     caller_job: Optional[str]
     created_at: str
     federated_job_uuid: Optional[str]
     public_id: str
-    uuid: str
     remote_hosts_with_warning: List[RemoteHost]
-    state: str
     user_id: Optional[str]
+    arguments_override_command: bool
 
 
 # type optional keys with total=False
-class CreatedJobDict(_Job, total=False):
+class Job(_Job, total=False):
     custom_compute_node_url: str
 
 
 class CloudJob(TypedDict):
     public_id: str
     reserved_cpu_in_nano_shares: int
     reserved_memory_in_bytes: int
     max_runtime_in_seconds: int
 
 
 class JobWrapper(TypedDict):
     access_token: str
     BASE_URL: str  # TODO: refactor this to lower case
     compute_node_info: Optional[ComputeNodeInfo]
-    job: CreatedJobDict
+    job: Job
     cloud_job: Optional[CloudJob]
     job_temporary_dir: Optional[str]
```

### Comparing `pybiolib-1.1.911/biolib/biolib_api_client/user_state.py` & `pybiolib-1.1.94/biolib/biolib_api_client/user_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     # jobs: Dict[UuidStr, JobStateType]
 
 
 class UserState(CacheState[UserStateType]):
 
     @property
     def _state_path(self) -> str:
-        return f'{self._user_cache_dir}/user-state.json'
+        return f'{super()._cache_dir}/user-state.json'
 
     def _get_default_state(self) -> UserStateType:
         return UserStateType(refresh_token=None)
```

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/base_bbf_package.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/base_bbf_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/encrypted_module_output.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/encrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/module_input.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/module_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class ModuleInput(BioLibBinaryFormatBasePackage):
     def __init__(self, bbf=None):
         super().__init__(bbf)
         self.package_type = 1
 
-    def serialize(self, stdin, arguments, files) -> bytes:
+    def serialize(self, stdin, arguments, files):
         bbf_data = bytearray()
         bbf_data.extend(self.version.to_bytes(1, 'big'))
         bbf_data.extend(self.package_type.to_bytes(1, 'big'))
 
         bbf_data.extend(len(stdin).to_bytes(8, 'big'))
 
         argument_len = sum([len(arg.encode()) for arg in arguments]) + (2 * len(arguments))
```

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/module_output.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/module_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 import gc
 
 from biolib.biolib_binary_format.base_bbf_package import BioLibBinaryFormatBasePackage
-from biolib.typing_utils import TypedDict, Dict
-
-
-class ModuleOutputDict(TypedDict):
-    stdout: bytes
-    stderr: bytes
-    exit_code: int
-    files: Dict[str, bytes]
 
 
 class ModuleOutput(BioLibBinaryFormatBasePackage):
     def __init__(self, bbf=None):
         super().__init__(bbf)
         self.package_type = 2
 
@@ -44,15 +36,15 @@
 
             # Remove data from files and garbage collect
             files[path] = None
             gc.collect(1)
 
         return bbf_data
 
-    def deserialize(self) -> ModuleOutputDict:
+    def deserialize(self):
         version = self.get_data(1, output_type='int')
         package_type = self.get_data(1, output_type='int')
         self.check_version_and_type(version=version, package_type=package_type, expected_package_type=self.package_type)
 
         stdout_len = self.get_data(8, output_type='int')
         stderr_len = self.get_data(8, output_type='int')
         files_data_len = self.get_data(8, output_type='int')
```

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/rsa_encrypted_aes_package.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/rsa_encrypted_aes_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/saved_job.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/saved_job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/stdout_and_stderr.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/stdout_and_stderr.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/system_exception.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/system_exception.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/system_status_update.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/system_status_update.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_binary_format/utils.py` & `pybiolib-1.1.94/biolib/biolib_binary_format/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from abc import ABC, abstractmethod
 
-import io
 import requests
 
 from biolib.typing_utils import Iterable
-from biolib.utils.multipart_uploader import get_chunk_iterator_from_bytes
 
 
 class IndexableBuffer(ABC):
 
     def __init__(self):
         self.pointer = 0
 
@@ -91,36 +89,30 @@
         self._length_bytes = len(data)
 
     def get_data(self, start: int, length: int) -> bytes:
         end = start + length
         return self._buffer[start:end]
 
     def get_data_as_iterable(self, start: int, length: int, chunk_size: int) -> Iterable[bytes]:
-        return get_chunk_iterator_from_bytes(self._buffer[start:start + length], chunk_size)
+        raise NotImplementedError
 
     def __len__(self):
         return self._length_bytes
 
 
 class LazyLoadedFile:
 
     def __init__(self, path: str, buffer: IndexableBuffer, start: int, length: int):
         self._path = path
         self._buffer = buffer
         self._start = start
         self._length = length
 
-    def __repr__(self) -> str:
-        return f'File "{self._path}" with size of {self._length} bytes'
-
     @property
     def path(self) -> str:
         return self._path
 
-    def get_file_handle(self) -> io.BufferedIOBase:
-        return io.BytesIO(self.get_data())
-
     def get_data(self) -> bytes:
         return self._buffer.get_data(start=self._start, length=self._length)
 
     def get_data_as_iterable(self) -> Iterable[bytes]:
         return self._buffer.get_data_as_iterable(start=self._start, length=self._length, chunk_size=1_000_000)
```

### Comparing `pybiolib-1.1.911/biolib/biolib_logging.py` & `pybiolib-1.1.94/biolib/biolib_logging.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/biolib_push.py` & `pybiolib-1.1.94/biolib/biolib_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 from pathlib import Path
 import yaml
 import rich.progress
 
-from biolib.lfs.utils import get_iterable_zip_stream, get_files_and_size_of_directory
+from biolib.lfs import get_iterable_zip_stream, get_files_and_size_of_directory
 from biolib.typing_utils import Optional, Set, TypedDict, Iterable
 from biolib.biolib_api_client import BiolibApiClient
 from biolib.biolib_docker_client import BiolibDockerClient
 from biolib.biolib_api_client.biolib_app_api import BiolibAppApi
 from biolib.biolib_errors import BioLibError
 from biolib.biolib_logging import logger
 from biolib.utils import get_absolute_container_image_uri
```

### Comparing `pybiolib-1.1.911/biolib/cli_utils.py` & `pybiolib-1.1.94/biolib/cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,14 @@
     for file_command in file_commands:
         # TODO: figure out if splitting on space is good enough
         _, from_path, to_path = file_command.split(' ')
         files_mappings.append(FilesMapping(from_path=from_path, to_path=to_path))
     return files_mappings
 
 
-# Only used in run_dev which is deprecated and set to be removed
 def get_mocked_app_version_from_yaml(yaml_data: Dict, source_files_zip_path: str):
     modules: List[Module] = []
     for module_name in yaml_data['modules']:
         yaml_module = yaml_data['modules'][module_name]
 
         image_hostname, image_uri = yaml_module['image'].split('://')
         if image_hostname != 'local-docker':
@@ -234,16 +233,15 @@
         consumes_stdin=True,
         is_runnable_by_user=True,
         modules=modules,
         public_id='app-version-mock-id',
         remote_hosts=[],
         settings=[],
         stdout_render_type='text',
-        main_output_file=None,
-        created_at=''
+        main_output_file=None
     )
 
 
 def create_temporary_directory_with_source_files_zip(app_path: str) -> Tuple[tempfile.TemporaryDirectory, str]:
     original_working_directory = os.getcwd()
     temporary_directory = tempfile.TemporaryDirectory()
     os.chdir(app_path)
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/cloud_utils/cloud_utils.py` & `pybiolib-1.1.94/biolib/compute_node/cloud_utils/cloud_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,24 +25,28 @@
     @staticmethod
     def get_webserver_config() -> WebserverConfig:
         if CloudUtils._webserver_config:
             return CloudUtils._webserver_config
 
         CloudUtils._webserver_config = WebserverConfig(
             compute_node_info=ComputeNodeInfo(
-                auth_token=CloudUtils._get_environment_variable_or_fail('BIOLIB_COMPUTE_NODE_AUTH_TOKEN'),
-                ip_address=os.environ.get('BIOLIB_COMPUTE_NODE_CUSTOM_IP', default=gethostbyname(gethostname())),
-                public_id=CloudUtils._get_environment_variable_or_fail('BIOLIB_COMPUTE_NODE_PUBLIC_ID'),
-                pybiolib_version=utils.BIOLIB_PACKAGE_VERSION,
+                auth_token=CloudUtils._get_environment_variable('BIOLIB_COMPUTE_NODE_AUTH_TOKEN'),
+                public_id=CloudUtils._get_environment_variable('BIOLIB_COMPUTE_NODE_PUBLIC_ID'),
+                ip_address=gethostbyname(gethostname())
             ),
-            base_url=CloudUtils._get_environment_variable_or_fail('BIOLIB_BASE_URL'),
-            s3_general_storage_bucket_name=CloudUtils._get_environment_variable_or_fail(
-                'BIOLIB_S3_GENERAL_STORAGE_BUCKET_NAME',
+            base_url=CloudUtils._get_environment_variable('BIOLIB_BASE_URL'),
+            ecr_region_name=CloudUtils._get_environment_variable('BIOLIB_ECR_REGION_NAME'),
+            s3_general_storage_bucket_name=CloudUtils._get_environment_variable(
+                'BIOLIB_S3_GENERAL_STORAGE_BUCKET_NAME'
             ),
-            is_dev=os.environ.get('BIOLIB_DEV') == 'TRUE',
+            s3_lfs_bucket_name=CloudUtils._get_environment_variable('BIOLIB_S3_LFS_BUCKET_NAME'),
+            max_docker_image_cache_size_bytes=CloudUtils._get_environment_variable_as_int(
+                'BIOLIB_MAX_DOCKER_IMAGE_CACHE_SIZE_BYTES'
+            ),
+            is_dev=CloudUtils._get_environment_variable('BIOLIB_DEV').upper() == 'TRUE',
             shutdown_times=ShutdownTimes(
                 auto_shutdown_time_in_seconds=CloudUtils._get_environment_variable_as_int(
                     'BIOLIB_CLOUD_AUTO_SHUTDOWN_TIME_IN_SECONDS'
                 ),
             )
         )
 
@@ -98,17 +102,16 @@
                     'auth_token': config["compute_node_info"]["auth_token"],
                     'cloud_job_id': cloud_job_id,
                     'system_exception_code': system_exception_code,
                 },
                 timeout=5,
             )
 
-            opt_error_string = f' with error code {system_exception_code}' if system_exception_code else ''
             logger_no_user_data.debug(
-                f'Cloud Job "{cloud_job_id}" was reported as finished' + opt_error_string
+                f'Cloud Job "{cloud_job_id}" was reported as finished with error code {system_exception_code}'
             )
 
         except Exception as error:  # pylint: disable=broad-except
             logger_no_user_data.error(f'Could not finish cloud job with id: {cloud_job_id} got error: {error}')
 
     @staticmethod
     def _report_availability() -> None:
@@ -120,18 +123,16 @@
                 f'Registering with {compute_node_info} to host {api_client.base_url} at {datetime.now()}'
             )
 
             response: Optional[requests.Response] = None
             max_retries = 5
             for retry_count in range(max_retries):
                 try:
-                    response = requests.post(
-                        url=f'{api_client.base_url}/api/jobs/report_available/',
-                        json=compute_node_info,
-                    )
+                    response = requests.post(f'{api_client.base_url}/api/jobs/report_available/',
+                                             json=compute_node_info)
                     break
                 except Exception as error:  # pylint: disable=broad-except
                     logger_no_user_data.error(f'Self-registering failed with error: {error}')
                     if retry_count < max_retries - 1:
                         seconds_to_sleep = 1
                         logger_no_user_data.info(f'Retrying self-registering in {seconds_to_sleep} seconds')
                         time.sleep(seconds_to_sleep)
@@ -144,18 +145,18 @@
 
         except Exception as exception:  # pylint: disable=broad-except
             logger_no_user_data.error(f'Shutting down as self register failed due to: {exception}')
             if not utils.IS_DEV:
                 CloudUtils.deregister_and_shutdown()
 
     @staticmethod
-    def _get_environment_variable_or_fail(key: str) -> str:
+    def _get_environment_variable(key: str) -> str:
         value = os.environ.get(key)
         # Purposely loose falsy check (instead of `is not None`) as empty string should fail
         if not value:
             raise Exception(f'CloudUtils: Missing environment variable "{key}"')
 
         return value
 
     @staticmethod
     def _get_environment_variable_as_int(key: str) -> int:
-        return int(CloudUtils._get_environment_variable_or_fail(key))
+        return int(CloudUtils._get_environment_variable(key))
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/cache_state.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/cache_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,15 @@
 
     @property
     def main_lfs_storage_path(self) -> str:
         return self._storage_paths[0]
 
     @property
     def _state_path(self) -> str:
-        state_path = os.environ.get('BIOLIB_LFS_STATE_PATH')
-        if not state_path:
-            raise CacheStateError('Environment variable "BIOLIB_LFS_STATE_PATH" not set')
-
-        return state_path
+        return f'{self.main_lfs_storage_path}/lfs-cache-state.json'
 
     def _get_default_state(self) -> LfsCacheStateDict:
         return LfsCacheStateDict(
             large_file_systems={},
             storage_partitions=self._get_storage_partitions_from_env(),
         )
 
@@ -92,11 +88,11 @@
 
         return storage_states
 
 
 class DockerImageCacheState(CacheState):
     @property
     def _state_path(self) -> str:
-        return f'{self._user_cache_dir}/docker-cache-state.json'
+        return f'{super()._cache_dir}/docker-cache-state.json'
 
     def _get_default_state(self) -> DockerImageCacheStateDict:
         return {}
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/cache_types.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/cache_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 UuidStr = str
 DiskPath = str
 DockerImageUri = str
 
 
 class LargeFileSystemCache(TypedDict):
+    active_jobs: List[UuidStr]
     last_used_at: str
     size_bytes: int
     state: Literal['downloading', 'ready']
     storage_partition_uuid: UuidStr
     uuid: UuidStr
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/docker_image_cache.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/docker_image_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,64 @@
 import logging
 import subprocess
 
 from docker.errors import ImageNotFound, APIError  # type: ignore
 
 from biolib import utils
-from biolib.typing_utils import TypedDict
 from biolib.biolib_docker_client import BiolibDockerClient
 from biolib.biolib_errors import BioLibError
 from biolib.biolib_logging import logger_no_user_data
+from biolib.compute_node.cloud_utils import CloudUtils
 from biolib.compute_node.job_worker.cache_state import DockerImageCacheState, DockerCacheStateError
 from biolib.compute_node.job_worker.cache_types import DockerImageInfo, DockerImageCacheStateDict, DockerAuthConfig, \
     UuidStr
 
 
-class DiskUsage(TypedDict):
-    image_storage_available_in_bytes: int
-    max_image_capacity_in_bytes: int
-    used_in_bytes: int
-
-
 class DockerImageCache:
     def __init__(self):
         if not utils.IS_RUNNING_IN_CLOUD:
-            raise BioLibError('Using DockerImageCache outside Cloud is not supported')
+            raise BioLibError("Using DockerImageCache from outside of Cloud is not allowed.")
 
+        config = CloudUtils.get_webserver_config()
+        self._max_cache_size = config['max_docker_image_cache_size_bytes']  # pylint: disable=unsubscriptable-object
         self._docker_client = BiolibDockerClient().get_docker_client()
         self._docker_data_dir = self._docker_client.info()['DockerRootDir']
 
-    def _get_current_disk_usage_stats(self) -> DiskUsage:
-        disk_usage_command = ['df', '--block-size=1', self._docker_data_dir]
-        logger_no_user_data.debug(f'Running {disk_usage_command}...')
-        df_output = subprocess.run(
+    @property
+    def _current_cache_size_on_disk(self):
+        disk_usage_command = ['sudo', '/bin/bash', '-c', f'du -sb {self._docker_data_dir} | cut -f1']
+        du_output = subprocess.run(
             disk_usage_command,
             capture_output=True,
-            check=True,
-            timeout=3,
-        ).stdout.decode()
-        logger_no_user_data.debug(df_output)
-        df_output_lines = [s.split() for s in df_output.splitlines()]
-
-        # Expect the filesystem to be row 1
-        disk = df_output_lines[1]
-        # Expect column 1 to be total disk size and column 2 to be disk space used
-        total_size_in_bytes = int(disk[1])
-        used_in_bytes = int(disk[2])
-
-        # Allow 80% to be used for images
-        max_image_capacity_in_bytes = total_size_in_bytes * 80 // 100
-        available_for_images_in_bytes = max(0, max_image_capacity_in_bytes - used_in_bytes)
-
-        disk_usage = DiskUsage(
-            image_storage_available_in_bytes=available_for_images_in_bytes,
-            max_image_capacity_in_bytes=max_image_capacity_in_bytes,
-            used_in_bytes=used_in_bytes,
-        )
-        logger_no_user_data.debug(f'Disk usage for Docker: {disk_usage}')
-        return disk_usage
+            check=True
+        ).stdout
+        return int(du_output.decode().strip())
 
     def _clear_space_for_image(self, estimated_image_size_bytes: int, cache_state: DockerImageCacheStateDict):
         for _ in range(100):
             if not self._has_space_to_pull_image(estimated_image_size_bytes, cache_state):
                 self._remove_least_recently_used_image(cache_state)
             else:
                 return
 
         raise DockerCacheStateError('Failed to free space for Docker image')
 
-    def get(
-            self,
-            image_uri: str,
-            estimated_image_size_bytes: int,
-            pull_auth_config: DockerAuthConfig,
-            job_id: str,
-    ) -> None:
+    def get(self, image_uri: str, estimated_image_size_bytes: int,
+            pull_auth_config: DockerAuthConfig, job_id: str) -> None:
         try:
             with DockerImageCacheState() as cache_state:
                 if image_uri not in cache_state:
                     raise ImageNotFound('Image not found in cache')
 
                 self._docker_client.images.get(image_uri)
                 cache_state[image_uri]['last_used_at'] = DockerImageCacheState.get_timestamp_now()
                 cache_state[image_uri]['active_jobs'].append(job_id)
 
         except ImageNotFound:
-            disk_stats = self._get_current_disk_usage_stats()
-            if estimated_image_size_bytes > disk_stats['max_image_capacity_in_bytes']:
+            if estimated_image_size_bytes > self._max_cache_size:
                 logger_no_user_data.error(
                     f'Image {image_uri} with size: {estimated_image_size_bytes} is bigger than the max cache size'
                 )
                 raise DockerCacheStateError(  # pylint: disable=raise-missing-from
                     'Image is bigger than the max cache size'
                 )
 
@@ -153,21 +123,16 @@
                 )
                 continue  # Image is in use or cannot be removed at this time
 
             cache_state.pop(image['uri'])
             break
 
     def _has_space_to_pull_image(self, estimated_image_size_bytes: int, cache_state: DockerImageCacheStateDict) -> bool:
-        logger_no_user_data.debug('Calculating cache metrics...')
-        size_of_images_being_pulled = sum(
-            [image['estimated_image_size_bytes'] for image in cache_state.values() if image['state'] == 'pulling']
-        )
-        disk_stats = self._get_current_disk_usage_stats()
-        cache_space_remaining = disk_stats['image_storage_available_in_bytes'] - size_of_images_being_pulled
-
-        logger_no_user_data.debug(
-            f'Needed current image: {estimated_image_size_bytes}. '
-            f'Cache remaining: {cache_space_remaining}. '
-            f'Total pulling: {size_of_images_being_pulled}. '
-        )
+        size_of_images_being_pulled = sum([image['estimated_image_size_bytes'] for image in cache_state.values()
+                                           if image['state'] == 'pulling'])
+        current_cache_size = self._current_cache_size_on_disk + size_of_images_being_pulled
+
+        cache_space_remaining = self._max_cache_size - current_cache_size
+        logger_no_user_data.debug(f'Cache remaining: {cache_space_remaining}. Needed: {estimated_image_size_bytes}.')
+        logger_no_user_data.debug(f'Stored: {self._current_cache_size_on_disk}. Pulling: {size_of_images_being_pulled}')
 
         return bool(cache_space_remaining > estimated_image_size_bytes)
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/executors/docker_executor.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/executors/docker_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-import json
 import tempfile
 import time
 import tarfile
 import zipfile
 import os
 import io
-import re
 import shlex
-from datetime import datetime
 
 import docker  # type: ignore
-import docker.types  # type: ignore
-
 from docker.errors import ImageNotFound, APIError  # type: ignore
 from docker.models.containers import Container  # type: ignore
 
 from biolib import utils
 from biolib.biolib_binary_format import ModuleOutput, ModuleInput
 from biolib.biolib_docker_client import BiolibDockerClient
-from biolib.biolib_errors import DockerContainerNotFoundDuringExecutionException, BioLibError
+from biolib.biolib_errors import DockerContainerNotFoundDuringExecutionException
 from biolib.biolib_logging import logger, logger_no_user_data
 from biolib.compute_node import utils as compute_node_utils
 from biolib.compute_node.job_worker.docker_image_cache import DockerImageCache
 from biolib.compute_node.job_worker.executors.base_executor import BaseExecutor
 from biolib.compute_node.job_worker.executors.types import StatusUpdate, LocalExecutorOptions
 from biolib.compute_node.job_worker.mappings import Mappings, path_without_first_folder
 from biolib.compute_node.job_worker.utils import ComputeProcessException
@@ -78,63 +73,41 @@
         user_data_tar_dir = f'{self._compute_process_dir}/tars'
         os.makedirs(user_data_tar_dir, exist_ok=True)
 
         self._docker_container: Optional[Container] = None
         self._runtime_tar_path = f'{user_data_tar_dir}/runtime_{self._random_docker_id}.tar'
         self._input_tar_path = f'{user_data_tar_dir}/input_{self._random_docker_id}.tar'
 
-        if utils.IS_RUNNING_IN_CLOUD and not utils.BIOLIB_SECRETS_TMPFS_PATH:
-            error_message = 'Running in cloud but no TMPFS path has been set for secrets'
-            logger_no_user_data.error(error_message)
-            raise BioLibError(error_message)
-
-        # If BIOLIB_SECRETS_TMPFS_PATH is set create the temporary directory there
-        self._tmp_secrets_dir = tempfile.TemporaryDirectory(dir=utils.BIOLIB_SECRETS_TMPFS_PATH or None)
-        os.chmod(self._tmp_secrets_dir.name, 0o755)
-
     def execute_module(self, module_input_serialized: bytes) -> bytes:
-        try:
-            job_uuid = self._options['job']['public_id']
-            send_status_update = self._options['send_status_update']
-            send_system_exception = self._options['send_system_exception']
+        send_status_update = self._options['send_status_update']
+        send_system_exception = self._options['send_system_exception']
 
-            module_input = ModuleInput(module_input_serialized).deserialize()
+        module_input = ModuleInput(module_input_serialized).deserialize()
 
-            # TODO: fix these status updates such that they also make sense for run-dev
-            send_status_update(StatusUpdate(progress=55, log_message='Pulling images...'))
+        # TODO: fix these status updates such that they also make sense for run-dev
+        send_status_update(StatusUpdate(progress=55, log_message='Pulling images...'))
 
-            self._pull()
+        self._pull()
 
-            send_status_update(StatusUpdate(progress=70, log_message='Computing...'))
-            start_time = time.time()
+        send_status_update(StatusUpdate(progress=70, log_message='Computing...'))
+        start_time = time.time()
 
-            logger_no_user_data.debug(f'Starting execution of {job_uuid}.')
-            try:
-                stdout, stderr, exit_code, mapped_output_files = self._execute_helper(module_input)
-            except docker.errors.NotFound as docker_error:
-                raise DockerContainerNotFoundDuringExecutionException from docker_error
-            except Exception as exception:
-                raise ComputeProcessException(
-                    exception,
-                    SystemExceptionCodes.FAILED_TO_RUN_COMPUTE_CONTAINER.value,
-                    self._send_system_exception
-                ) from exception
-            logger_no_user_data.debug(f'Completed execution of {job_uuid}.')
+        stdout, stderr, exit_code, mapped_output_files = self._execute_helper(module_input)
 
-            try:
-                module_output_serialized = ModuleOutput().serialize(stdout, stderr, exit_code, mapped_output_files)
-                logger.debug(f'Compute time: {time.time() - start_time}')
-                return module_output_serialized
+        try:
+            module_output_serialized: bytes = ModuleOutput().serialize(stdout, stderr, exit_code, mapped_output_files)
+            logger.debug(f'Compute time: {time.time() - start_time}')
+            return module_output_serialized
 
-            except Exception as exception:
-                raise ComputeProcessException(
-                    exception,
-                    SystemExceptionCodes.FAILED_TO_SERIALIZE_AND_SEND_MODULE_OUTPUT.value,
-                    send_system_exception
-                ) from exception
+        except Exception as exception:
+            raise ComputeProcessException(
+                exception,
+                SystemExceptionCodes.FAILED_TO_SERIALIZE_AND_SEND_MODULE_OUTPUT.value,
+                send_system_exception
+            ) from exception
         finally:
             try:
                 self.cleanup()
             except Exception:  # pylint: disable=broad-except
                 logger.error('DockerExecutor failed to clean up container')
 
     def _pull(self):
@@ -160,60 +133,67 @@
                 exception,
                 SystemExceptionCodes.FAILED_TO_PULL_DOCKER_IMAGE.value,
                 self._send_system_exception,
                 may_contain_user_data=False
             ) from exception
 
     def _execute_helper(self, module_input):
-        job_uuid = self._options['job']['public_id']
-        logger_no_user_data.debug(f'Initializing container for {job_uuid}.')
         self._initialize_docker_container(module_input)
 
         if self._options['runtime_zip_bytes']:
             self._map_and_copy_runtime_files_to_container(self._options['runtime_zip_bytes'], module_input['arguments'])
 
-        logger_no_user_data.debug(f'_map_and_copy_input_files_to_container for {job_uuid}.')
         self._map_and_copy_input_files_to_container(module_input['files'], module_input['arguments'])
 
-        docker_api_client = BiolibDockerClient.get_docker_client().api
-        logger_no_user_data.debug(f'Starting Docker container for {job_uuid}')
+        try:
+            docker_api_client = BiolibDockerClient.get_docker_client().api
+            logger.debug('Starting Docker container')
 
-        stdout_and_stderr_stream = docker_api_client.attach(
-            container=self._docker_container.id,
-            stderr=True,
-            stdout=True,
-            stream=True,
-        )
-
-        self._docker_container.start()
-
-        if self._options['job']['app_version'].get('stdout_render_type') != 'markdown':
-            for stdout_and_stderr in stdout_and_stderr_stream:
-                # Default messages to empty bytestring instead of None
-                stdout_and_stderr = stdout_and_stderr if stdout_and_stderr is not None else b''
-
-                self._send_stdout_and_stderr(stdout_and_stderr)
-
-        exit_code = docker_api_client.wait(self._docker_container.id)['StatusCode']
-        # 137 is the error code from linux OOM killer (Should catch 90% of OOM errors)
-        if exit_code == 137:
-            raise ComputeProcessException(
-                MemoryError(),
-                SystemExceptionCodes.OUT_OF_MEMORY.value,
-                self._send_system_exception
+            stdout_and_stderr_stream = docker_api_client.attach(
+                container=self._docker_container.id,
+                stderr=True,
+                stdout=True,
+                stream=True,
             )
 
-        logger_no_user_data.debug(f'Docker container exited with code {exit_code} for {job_uuid}')
+            self._docker_container.start()
+
+            if self._options['job']['app_version'].get('stdout_render_type') != 'markdown':
+                for stdout_and_stderr in stdout_and_stderr_stream:
+                    # Default messages to empty bytestring instead of None
+                    stdout_and_stderr = stdout_and_stderr if stdout_and_stderr is not None else b''
+
+                    self._send_stdout_and_stderr(stdout_and_stderr)
+
+            exit_code = docker_api_client.wait(self._docker_container.id)['StatusCode']
+            # 137 is the error code from linux OOM killer (Should catch 90% of OOM errors)
+            if exit_code == 137:
+                raise ComputeProcessException(
+                    MemoryError(),
+                    SystemExceptionCodes.OUT_OF_MEMORY.value,
+                    self._send_system_exception
+                )
+
+            logger.debug(f'Docker container exited with code {exit_code}')
 
-        full_stdout = docker_api_client.logs(self._docker_container.id, stdout=True, stderr=False)
-        full_stderr = docker_api_client.logs(self._docker_container.id, stdout=False, stderr=True)
+            full_stdout = docker_api_client.logs(self._docker_container.id, stdout=True, stderr=False)
+            full_stderr = docker_api_client.logs(self._docker_container.id, stdout=False, stderr=True)
 
-        mapped_output_files = self._get_output_files(arguments=module_input['arguments'])
-        return full_stdout, full_stderr, exit_code, mapped_output_files
+            mapped_output_files = self._get_output_files(arguments=module_input['arguments'])
+            return full_stdout, full_stderr, exit_code, mapped_output_files
 
+        except docker.errors.NotFound as docker_error:
+            raise DockerContainerNotFoundDuringExecutionException from docker_error
+
+        except Exception as exception:
+            raise ComputeProcessException(
+                exception,
+                SystemExceptionCodes.FAILED_TO_RUN_COMPUTE_CONTAINER.value,
+                self._send_system_exception
+            ) from exception
 
     def cleanup(self):
         # Don't clean up if already in the process of doing so, or done doing so
         if self._is_cleaning_up:
             return
         else:
             self._is_cleaning_up = True
@@ -231,68 +211,40 @@
         if utils.IS_RUNNING_IN_CLOUD:
             DockerImageCache().detach_job(
                 image_uri=self._image_uri,
                 job_id=self._options['job']['public_id']
             )
 
         logger.debug(f"Deleted compute container in: {time.time() - container_time}")
-        self._tmp_secrets_dir.cleanup()
 
     # TODO: type this method
     def _initialize_docker_container(self, module_input):
         try:
             module = self._options['module']
             logger.debug(f"Initializing docker container with command: {module['command']}")
 
             docker_volume_mounts = [lfs.docker_mount for lfs in self._options['large_file_systems'].values()]
 
             internal_network = self._options['internal_network']
             extra_hosts: Dict[str, str] = {}
             dns_list: List[str] = []
-
-            biolib_system_secret = {
-                'version': '1.0.0',
-                'job_uuid': self._options['job']['public_id'],
-                'job_auth_token': self._options['job']['auth_token'],
-            }
-            secrets: Dict[str, str] = dict(
-                **module.get('secrets', {}),
-                biolib_system_secret=json.dumps(biolib_system_secret, indent=4),
-            )
-            docker_volume_mounts.append(self._create_secrets_mount(secrets))
-
-            environment_vars = {}
-
-            # Include secrets and job info as env vars for app versions created before 20/11/2022
-            app_version_created_at = datetime.strptime(
-                self._options['job']['app_version']['created_at'],
-                '%Y-%m-%dT%H:%M:%S.%fZ',
-            )
-            if app_version_created_at < datetime(2022, 11, 30, 0, 0):
-                environment_vars = module.get('secrets', {})
-                environment_vars.update({
-                    'BIOLIB_JOB_UUID': self._options['job']['public_id'],
-                    'BIOLIB_JOB_AUTH_TOKEN': self._options['job']['auth_token']
-                })
-
-            if utils.IS_RUNNING_IN_CLOUD and self._options['cloud_job']:
-                environment_vars.update({
-                    'BIOLIB_JOB_MAX_RUNTIME_IN_SECONDS': self._options['cloud_job']['max_runtime_in_seconds'],
-                })
+            environment_vars = module.get('secrets', {})
+            environment_vars.update({
+                'BIOLIB_JOB_UUID': self._options['job']['public_id'],
+                'BIOLIB_JOB_AUTH_TOKEN': self._options['job']['auth_token']
+            })
 
             for proxy in self._options['remote_host_proxies']:
                 proxy_ip = proxy.get_ip_address_on_network(internal_network)
                 if proxy.is_app_caller_proxy:
                     logger_no_user_data.debug('Found app caller proxy, setting both base URLs in compute container')
                     environment_vars.update({
                         'BIOLIB_BASE_URL': f'http://{proxy_ip}',
                         'BIOLIB_CLOUD_BASE_URL': f'http://{proxy_ip}',
-                        # This should be removed eventually, but will break apps calling apps on older versions
                         'BIOLIB_CLOUD_RESULTS_BASE_URL': f'http://{proxy_ip}',
-                        'BIOLIB_CLOUD_JOB_STORAGE_BASE_URL': f'http://{proxy_ip}',
                         # Inform container if we are targeting public biolib as we change the BIOLIB_BASE_URL
                         'BIOLIB_ENVIRONMENT_IS_PUBLIC_BIOLIB': bool(utils.BASE_URL_IS_PUBLIC_BIOLIB)
                     })
                 else:
                     extra_hosts[proxy.hostname] = proxy_ip
 
             if self._options['dns_proxy']:
@@ -303,27 +255,27 @@
             create_container_args = {
                 'environment': environment_vars,
                 'extra_hosts': extra_hosts,
                 'image': self._image_uri,
                 'mounts': docker_volume_mounts,
                 'network': internal_network.name,
                 'working_dir': module['working_directory'],
-                'dns': dns_list,
+                'dns': dns_list
             }
 
             if self._options['job'].get('arguments_override_command'):
                 # In this case, arguments contains a user specified command to run in the app
                 create_container_args.update({
                     'command': module_input['arguments'],
                     'entrypoint': ''
                 })
 
             else:
                 create_container_args.update({
-                    'command': shlex.split(module['command']) + module_input['arguments']
+                   'command': shlex.split(module['command']) + module_input['arguments']
                 })
 
             app_version = self._options['job']['app_version']
             if app_version.get('main_output_file') or app_version.get('stdout_render_type') == 'text':
                 create_container_args['tty'] = True
 
             if utils.IS_RUNNING_IN_CLOUD:
@@ -510,24 +462,7 @@
             raise ComputeProcessException(
                 exception,
                 SystemExceptionCodes.FAILED_TO_RETRIEVE_AND_MAP_OUTPUT_FILES.value,
                 self._send_system_exception
             ) from exception
 
         return mapped_output_files
-
-    def _create_secrets_mount(self, secrets: Dict[str, str]) -> docker.types.Mount:
-        job_uuid = self._options['job']['public_id']
-
-        for key, value in secrets.items():
-            if re.match(r'^[a-zA-Z0-9-_]+$', key):
-                with open(f'{self._tmp_secrets_dir.name}/{key}', 'w') as secret_file:
-                    secret_file.write(value)
-            else:
-                logger_no_user_data.warning(f'Job {job_uuid} uses secret with a key not matching validation regex')
-
-        return docker.types.Mount(
-            read_only=True,
-            source=f'{self._tmp_secrets_dir.name}/',
-            target='/biolib/secrets/',
-            type='bind',
-        )
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/executors/remote/remote_executor.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/executors/remote/remote_executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,44 @@
+from urllib.parse import urlparse
+
 from biolib import utils
 from biolib.biolib_api_client import BiolibApiClient
 from biolib.biolib_api_client.biolib_job_api import BiolibJobApi
-from biolib.biolib_binary_format import UnencryptedModuleOutput
-from biolib.biolib_logging import logger
+from biolib.biolib_logging import logger, logger_no_user_data
 from biolib.compute_node.job_worker.executors.types import RemoteExecuteOptions
 
 from biolib.compute_node.job_worker.job_storage import JobStorage
-from biolib.jobs import Job
 
 
 class RemoteExecutor:
 
     @staticmethod
-    def execute_job(options: RemoteExecuteOptions, module_input_serialized: bytes) -> UnencryptedModuleOutput:
+    def execute_job(options: RemoteExecuteOptions, module_input_serialized: bytes) -> bytes:
         job_id = options['job']['public_id']
-        JobStorage.upload_module_input(
-            job=options['job'],
-            module_input_serialized=module_input_serialized
-        )
-        cloud_job = BiolibJobApi.create_cloud_job(job_id=job_id, result_name_prefix=options['result_name_prefix'])
+        cloud_job = BiolibJobApi.create_cloud_job(module_name='main', job_id=job_id)
         logger.debug(f"Cloud: Job created with id {cloud_job['public_id']}")
 
-        if utils.IS_RUNNING_IN_NOTEBOOK:
-            utils.STREAM_STDOUT = True
-
-        app_version = options['job']['app_version']
-        enable_print = bool(
-            utils.STREAM_STDOUT and
-            (app_version.get('main_output_file') or app_version.get('stdout_render_type') == 'text')
-        )
-        job = Job.create_from_uuid(
-            uuid=options['job']['public_id'],
-            auth_token=options['job']['auth_token']
+        node_url = cloud_job['compute_node_info']['url']
+        if utils.BIOLIB_CLOUD_BASE_URL:
+            logger_no_user_data.debug('Using cloud proxy URL from env var BIOLIB_CLOUD_BASE_URL')
+            node_url = utils.BIOLIB_CLOUD_BASE_URL + urlparse(node_url).path
+
+        logger_no_user_data.debug(f'Using compute node URL "{node_url}"')
+
+        if utils.BASE_URL_IS_PUBLIC_BIOLIB:
+            aes_key_string_b64 = JobStorage.generate_and_store_key_buffer_for_job(job_id)
+            BiolibJobApi.start_cloud_job(job_id, module_input_serialized, node_url, aes_key_string_b64)
+        else:
+            BiolibJobApi.start_cloud_job(job_id, module_input_serialized, node_url)
+
+        utils.STREAM_STDOUT = True
+        BiolibJobApi.await_compute_node_status(
+            compute_type='Cloud',
+            node_url=node_url,
+            retry_interval_seconds=1.5,
+            retry_limit_minutes=10080,  # 1 Week
+            status_to_await='Result Ready',
+            job=options['job'],
         )
-        job._stream_logs(enable_print)  # pylint: disable=protected-access
 
         BiolibApiClient.refresh_auth_token()
-        return JobStorage.get_module_output(job=options['job'])
+        return JobStorage.get_result(job=options['job'])
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/executors/types.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/executors/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 from docker.models.networks import Network  # type: ignore
 
 from biolib.compute_node.job_worker.large_file_system import LargeFileSystem
 from biolib.compute_node.webserver.webserver_types import ComputeNodeInfo
 from biolib.typing_utils import TypedDict, Callable, Optional, List, Dict
 from biolib.compute_node.remote_host_proxy import RemoteHostProxy
 from biolib.biolib_api_client.app_types import Module
-from biolib.biolib_api_client.job_types import CreatedJobDict, CloudJob
+from biolib.biolib_api_client.job_types import Job, CloudJob
 
 
 class StatusUpdate(TypedDict):
     progress: int
     log_message: str
 
 
 class RemoteExecuteOptions(TypedDict):
     biolib_base_url: str
-    job: CreatedJobDict
-    result_name_prefix: Optional[str]
+    job: Job
     root_job_id: str
 
 
 SendStatusUpdateType = Callable[[StatusUpdate], None]
 SendSystemExceptionType = Callable[[int], None]
 SendStdoutAndStderrType = Callable[[bytes], None]
 
 
 class LocalExecutorOptions(TypedDict):
     access_token: str
     biolib_base_url: str
     compute_node_info: Optional[ComputeNodeInfo]
     internal_network: Optional[Network]
-    job: CreatedJobDict
+    job: Job
     cloud_job: Optional[CloudJob]
     large_file_systems: Dict[str, LargeFileSystem]
     module: Module
     dns_proxy: Optional[Container]
     remote_host_proxies: List[RemoteHostProxy]
     root_job_id: str
     runtime_zip_bytes: Optional[bytes]  # TODO: replace this with a module_source_serialized
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/job_worker.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/job_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,35 @@
 
 import requests
 from docker.errors import ImageNotFound  # type: ignore
 from docker.models.networks import Network  # type: ignore
 from docker.models.containers import Container  # type: ignore
 
 from biolib.biolib_binary_format.stdout_and_stderr import StdoutAndStderr
-from biolib.compute_node.job_worker.job_legacy_input_wait_timeout_thread import JobLegacyInputWaitTimeout
-from biolib.compute_node.job_worker.job_storage import JobStorage
 from biolib.compute_node.job_worker.large_file_system import LargeFileSystem
-from biolib.biolib_errors import DockerContainerNotFoundDuringExecutionException, BioLibError, \
-    StorageDownloadFailed
+from biolib.biolib_errors import DockerContainerNotFoundDuringExecutionException
 from biolib.compute_node.job_worker.job_max_runtime_timer_thread import JobMaxRuntimeTimerThread
 from biolib.compute_node.remote_host_proxy import RemoteHostProxy
 from biolib.typing_utils import Optional, List, Dict
 from biolib import utils
-from biolib.biolib_api_client import ModuleEnvironment, CreatedJobDict, JobWrapper, Module, AppVersionOnJob, \
-    BiolibApiClient, RemoteHost
+from biolib.biolib_api_client import ModuleEnvironment, Job, JobWrapper, Module, AppVersionOnJob, BiolibApiClient, \
+    RemoteHost
 from biolib.biolib_api_client.biolib_job_api import BiolibJobApi
 from biolib.biolib_docker_client import BiolibDockerClient
+from biolib.biolib_singularity_client import BiolibSingularityClient
 from biolib.biolib_logging import logger, logger_no_user_data
-from biolib.compute_node.job_worker.executors import DockerExecutor
+from biolib.compute_node.job_worker.executors import DockerExecutor, SingularityExecutor
 from biolib.compute_node.job_worker.executors.base_executor import BaseExecutor
 from biolib.compute_node.job_worker.executors.types import LocalExecutorOptions, StatusUpdate
 from biolib.compute_node.socker_listener_thread import SocketListenerThread
 from biolib.compute_node.socket_sender_thread import SocketSenderThread
 from biolib.compute_node.job_worker.mappings import Mappings, path_without_first_folder
 from biolib.compute_node.job_worker.utils import ComputeProcessException, log_disk_and_memory_usage_info
 from biolib.compute_node.utils import get_package_type, SystemExceptionCodes, SystemExceptionCodeMap
-from biolib.biolib_binary_format import SavedJob, SystemStatusUpdate, ModuleInput, SystemException, \
-    UnencryptedModuleOutput
+from biolib.biolib_binary_format import SavedJob, SystemStatusUpdate, ModuleInput, SystemException
 
 _DNS_PROXY_IMAGE_URI = 'spx01/blocky@sha256:485ef739233341d3e14a64db646754aba7322c34645f804c3c0c00556d9a2cd1'
 DEFAULT_BUFFER_SIZE = 1024
 SOCKET_HOST = '127.0.0.1'
 
 
 class JobWorkerProcess(multiprocessing.Process):
@@ -71,18 +68,17 @@
             signal.signal(signal.SIGINT, self._handle_exit_gracefully)
             # handle termination signal from parent
             signal.signal(signal.SIGTERM, self._handle_exit_gracefully)
 
             self._socket_port = socket_port
             self._received_messages_queue: Queue = Queue()
             self._messages_to_send_queue: Queue = Queue()
-            self._legacy_input_wait_timeout_thread: Optional[JobLegacyInputWaitTimeout] = None
 
             self._app_version_id_to_runtime_zip: Dict[str, bytes] = {}
-            self._jobs: Dict[str, CreatedJobDict] = {}
+            self._jobs: Dict[str, Job] = {}
             self._root_job_wrapper: Optional[JobWrapper] = None
 
             self._dns_proxy: Optional[Container] = None
 
             self._remote_host_proxies: List[RemoteHostProxy] = []
             self._internal_network: Optional[Network] = None
             self._public_network: Optional[Network] = None
@@ -98,17 +94,16 @@
                 self.send_system_exception,
                 may_contain_user_data=False
             ) from exception
 
         self._connect_to_parent()
 
     def _handle_exit_gracefully(self, signum: int, frame: FrameType) -> None:  # pylint: disable=unused-argument
-        job_id = self._root_job_wrapper["job"]["public_id"] if self._root_job_wrapper else None
         logger_no_user_data.debug(
-            f'_JobWorker ({job_id}) got exit signal {signal.Signals(signum).name}'  # pylint: disable=no-member
+            f'_JobWorker got exit signal {signal.Signals(signum).name}'  # pylint: disable=no-member
         )
         self._received_messages_queue.put(self._STOP_HANDLE_MESSAGE_LOOP)
         self._cleanup()
 
     def run_handle_message_loop(self):
         logger_no_user_data.debug(f'Started JobWorkerProcess {os.getpid()}')
         while True:
@@ -117,79 +112,66 @@
                 if package == self._STOP_HANDLE_MESSAGE_LOOP:
                     break
 
                 package_type = get_package_type(package)
                 if package_type == 'SavedJob':
                     self._handle_save_job_wrapper(package)
                     if utils.IS_RUNNING_IN_CLOUD:
-                        job = self._root_job_wrapper['job']
-                        job_uuid = job['public_id']
+                        job_uuid = self._root_job_wrapper['job']['public_id']
                         max_runtime_in_seconds = self._root_job_wrapper['cloud_job']['max_runtime_in_seconds']
                         logger_no_user_data.debug(
                             f'Job "{job_uuid}" will have max run time set to {max_runtime_in_seconds} seconds'
                         )
                         JobMaxRuntimeTimerThread(
                             job_worker=self,
                             max_runtime_in_seconds=max_runtime_in_seconds,
                         ).start()
 
-                        try:
-                            module_input_serialized = JobStorage.get_module_input(job=job)
-                        except StorageDownloadFailed:
-                            # Expect module input to be handled in a separate ModuleInput package
-                            self._legacy_input_wait_timeout_thread = JobLegacyInputWaitTimeout(
-                                input_max_wait_in_seconds=120,
-                                job_uuid=job_uuid,
-                                send_system_exception=self.send_system_exception,
-                            )
-                            self._legacy_input_wait_timeout_thread.start()
-                            continue
-                        except Exception as error:
-                            raise error
-
-                        try:
-                            self._run_root_job(module_input_serialized)
-
-                        # This error occurs when trying to access the container after the job worker has cleaned it up.
-                        # In that case stop the computation.
-                        except DockerContainerNotFoundDuringExecutionException as err:
-                            if self.is_cleaning_up:
-                                break
-                            else:
-                                raise err
-
                 elif package_type == 'ModuleInput':
                     if not self._root_job_wrapper:
                         raise Exception('No job saved yet')
 
-                    if self._legacy_input_wait_timeout_thread:
-                        self._legacy_input_wait_timeout_thread.stop()
-
                     try:
-                        self._run_root_job(package)
+                        module_output_serialized = self._run_job(
+                            job=self._root_job_wrapper['job'],
+                            module_input_serialized=package,
+                        )
 
                     # This error occurs when trying to access the container after the job worker has cleaned it up.
                     # In that case stop the computation.
                     except DockerContainerNotFoundDuringExecutionException as err:
                         if self.is_cleaning_up:
                             break
                         else:
                             raise err
 
+                    module_output_size = len(module_output_serialized)
+                    job_uuid = self._root_job_wrapper['job']['public_id']
+                    logger_no_user_data.debug(
+                        f'Job "{job_uuid}" finished computation with module output size '
+                        f'of {module_output_size} bytes'
+                    )
+
+                    module_output_file_path = os.path.join(self.job_temporary_dir, "module_output.bbf")
+                    with open(module_output_file_path, 'wb') as module_output_file:
+                        module_output_file.write(module_output_serialized)
+
+                    self._send_status_update(StatusUpdate(progress=94, log_message='Computation finished'))
+
                 else:
                     logger_no_user_data.error('Package type from parent was not recognized')
 
                 self._received_messages_queue.task_done()
             except ComputeProcessException:
                 continue
 
             except Exception as exception:
                 raise ComputeProcessException(
                     exception,
-                    SystemExceptionCodes.UNKNOWN_COMPUTE_PROCESS_ERROR.value,
+                    SystemExceptionCodes.UNKOWN_COMPUTE_PROCESS_ERROR.value,
                     self.send_system_exception
                 ) from exception
 
     def _cleanup(self) -> None:
         self.is_cleaning_up = True
 
         for executor in self._executors:
@@ -252,24 +234,27 @@
         self._jobs[job['public_id']] = job
 
         if job['app_version'].get('modules') is not None and BiolibDockerClient.is_docker_running():
             self._start_network_and_remote_host_proxies(job)
 
         # TODO: start downloading runtime zip already at this point
 
-    def _start_network_and_remote_host_proxies(self, job: CreatedJobDict) -> None:
+    def _start_network_and_remote_host_proxies(self, job: Job) -> None:
         app_version = job['app_version']
         job_id = job['public_id']
         remote_hosts = app_version['remote_hosts']
-        if utils.IS_RUNNING_IN_CLOUD:
-            remote_hosts.append(
-                {
-                    'hostname': 'AppCallerProxy',
-                },
-            )
+
+        for module in app_version['modules']:
+            if module['environment'] == 'biolib-app' and module['name'] != 'main':
+                remote_hosts.append(
+                    {
+                        'hostname': 'AppCallerProxy',
+                    },
+                )
+                break
 
         docker_client = BiolibDockerClient.get_docker_client()
         try:
             self._internal_network = docker_client.networks.create(
                 name=f'biolib-sandboxed-network-{job_id}',
                 internal=True,
                 driver='bridge',
@@ -399,25 +384,20 @@
 
         if not proxy_is_ready:
             self._dns_proxy.remove(force=True)
             raise Exception('DNS Proxy did not start properly')
 
         self._dns_proxy.reload()
 
-    def _run_app_version(
-        self,
-        app_version_id: str,
-        module_input_serialized: bytes,
-        caller_job: CreatedJobDict
-    ) -> bytes:
-        job: CreatedJobDict = BiolibJobApi.create(app_version_id, caller_job=caller_job['public_id'])
+    def _run_app_version(self, app_version_id: str, module_input_serialized: bytes, caller_job: Job) -> bytes:
+        job: Job = BiolibJobApi.create(app_version_id, caller_job=caller_job['public_id'])
         self._jobs[job['public_id']] = job
         return self._run_job(job, module_input_serialized)
 
-    def _run_job(self, job: CreatedJobDict, module_input_serialized: bytes) -> bytes:
+    def _run_job(self, job: Job, module_input_serialized: bytes) -> bytes:
         job_uuid = job['public_id']
         logger_no_user_data.info(f'Job "{job_uuid}" running...')
         if self._root_job_wrapper is None:
             raise Exception('root_job_wrapper was None')
 
         root_job = job
         while root_job['caller_job'] is not None and self._jobs.get(root_job['caller_job']) is not None:
@@ -446,14 +426,15 @@
         for module in modules:
             if len(module['source_files_mappings']) > 0:
                 source_files_are_mapped = True
 
             for lfs_mapping in module['large_file_systems']:
                 logger_no_user_data.debug(f'Job "{job_uuid}" creating LFS for module "{module["name"]}"...')
                 lfs = LargeFileSystem(
+                    is_job_federated=job['federated_job_uuid'] is not None,
                     job_id=job['public_id'],
                     lfs_mapping=lfs_mapping,
                     send_status_update=self._send_status_update,
                 )
                 logger_no_user_data.debug(f'Job "{job_uuid}" created object for LFS "{lfs.uuid}"')
 
                 lfs.initialize()
@@ -480,14 +461,17 @@
                 send_status_update=self._send_status_update,
                 send_system_exception=self.send_system_exception,
                 send_stdout_and_stderr=self.send_stdout_and_stderr,
             ),
             module_input_serialized,
         )
 
+        for lfs in lfs_dict.values():
+            lfs.detach()
+
         if utils.IS_RUNNING_IN_CLOUD:
             # Log memory and disk after pulling and executing module
             log_disk_and_memory_usage_info()
 
         return module_output_serialized
 
     def _run_module(self, options: LocalExecutorOptions, module_input_serialized: bytes) -> bytes:
@@ -503,14 +487,18 @@
                 files=module_input_with_runtime_zip['files'],
             )
             return self._run_app_version(module['image_uri'], module_input_with_runtime_zip_serialized, options['job'])
 
         elif module['environment'] == ModuleEnvironment.BIOLIB_ECR.value and BiolibDockerClient.is_docker_running():
             executor_instance = DockerExecutor(options)
 
+        elif module['environment'] == ModuleEnvironment.BIOLIB_ECR.value and \
+                BiolibSingularityClient.is_singularity_running():
+            executor_instance = SingularityExecutor(options)
+
         else:
             raise Exception(f"Unsupported module environment {module['environment']}")
 
         self._executors.append(executor_instance)
 
         if utils.IS_RUNNING_IN_CLOUD:
             # Log memory and disk before pulling and executing module
@@ -640,40 +628,7 @@
         except Exception as exception:
             raise ComputeProcessException(
                 exception,
                 SystemExceptionCodes.FAILED_TO_SEND_STATUS_UPDATE.value,
                 self.send_system_exception,
                 may_contain_user_data=False
             ) from exception
-
-    def _run_root_job(self, module_input_serialized: bytes) -> None:
-        # Make typechecker happy
-        if not self._root_job_wrapper or not self.job_temporary_dir:
-            raise BioLibError('Undefined job_wrapper or job_temporary_dir')
-
-        module_output_serialized = self._run_job(
-            job=self._root_job_wrapper['job'],
-            module_input_serialized=module_input_serialized,
-        )
-
-        module_output_size = len(module_output_serialized)
-        job_uuid = self._root_job_wrapper['job']['public_id']
-        logger_no_user_data.debug(
-            f'Job "{job_uuid}" finished computation with module output size '
-            f'of {module_output_size} bytes'
-        )
-
-        # TODO: Remove when webserver endpoint /v1/job/<job_id>/result/ is deprecated
-        legacy_module_output_file_path = os.path.join(self.job_temporary_dir, JobStorage.legacy_module_output_file_name)
-        with open(legacy_module_output_file_path, mode='wb') as file:
-            file.write(module_output_serialized)
-
-        module_output_file_path = os.path.join(self.job_temporary_dir, JobStorage.module_output_file_name)
-        with open(legacy_module_output_file_path, 'rb') as legacy_module_output, \
-                open(module_output_file_path, 'wb') as module_output:
-
-            UnencryptedModuleOutput.write_to_file_from_legacy_module_output_file(
-                input_file=legacy_module_output,
-                output_file=module_output,
-            )
-
-        self._send_status_update(StatusUpdate(progress=94, log_message='Computation finished'))
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/large_file_system.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/large_file_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,24 +36,26 @@
     pass
 
 
 class LargeFileSystem:
 
     def __init__(
             self,
+            is_job_federated: bool,
             job_id: str,
             lfs_mapping: LargeFileSystemMapping,
             send_status_update: Callable[[StatusUpdate], None],
     ):
         if not utils.IS_RUNNING_IN_CLOUD:
             raise LargeFileSystemError('Large File System is currently not supported in local compute environments')
 
         if lfs_mapping['size_bytes'] is None:
             raise LargeFileSystemError('Error: You attempted to attach an LFS without a known size.')
 
+        self._is_job_federated = is_job_federated
         self._job_id: str = job_id
         self._lfs_mapping: LargeFileSystemMapping = lfs_mapping
         self._path_on_disk: Optional[str] = None
         self._send_status_update: Callable[[StatusUpdate], None] = send_status_update
 
     @property
     def _is_initialized(self) -> bool:
@@ -79,17 +81,24 @@
         if self._is_initialized:
             logger_no_user_data.debug(f'LFS {self.uuid} is already initialized')
             return
 
         lfs_size_bytes = self._lfs_mapping['size_bytes']
         logger_no_user_data.debug(f'Initializing LFS {self.uuid} of size {lfs_size_bytes} bytes...')
 
+        lfs_path = f'{LfsCacheState().main_lfs_storage_path}/lfs/{self.uuid}/data'
+        if os.path.exists(lfs_path):
+            logger_no_user_data.debug(f'Job "{self._job_id}" LFS already exists at path: {lfs_path}')
+            self._path_on_disk = lfs_path
+            return
+
         lfs_is_already_downloading = False
+
         with LfsCacheState() as cache_state:
-            lfs_cache: Optional[LargeFileSystemCache] = cache_state['large_file_systems'].get(self.uuid)
+            lfs_cache = cache_state['large_file_systems'].get(self.uuid)
 
             if lfs_cache is None:
                 logger_no_user_data.debug(f'LFS {self.uuid} was not found in cache')
                 storage_partition_to_use: Optional[StoragePartition] = None
                 logger_no_user_data.debug(f"Storage partitions to check: {cache_state['storage_partitions'].values()}")
 
                 for storage_partition in cache_state['storage_partitions'].values():
@@ -100,27 +109,28 @@
 
                 if storage_partition_to_use is None:
                     raise LargeFileSystemError('No storage partition with space available')
                 else:
                     storage_partition_to_use['allocated_size_bytes'] += lfs_size_bytes
 
                 cache_state['large_file_systems'][self.uuid] = LargeFileSystemCache(
+                    active_jobs=[self._job_id],
                     last_used_at=LfsCacheState.get_timestamp_now(),
                     size_bytes=lfs_size_bytes,
                     state='downloading',
                     storage_partition_uuid=storage_partition_to_use['uuid'],
                     uuid=self.uuid,
                 )
 
                 self._path_on_disk = f"{storage_partition_to_use['path']}/lfs/{self.uuid}/data"
                 logger_no_user_data.debug(f'Using path {self._path_on_disk} for LFS')
 
             else:
                 logger_no_user_data.debug(f"LFS {self.uuid} found in cache with state {lfs_cache['state']}")
-                lfs_cache['last_used_at'] = LfsCacheState.get_timestamp_now()
+                lfs_cache['active_jobs'].append(self._job_id)
                 storage_partition = cache_state['storage_partitions'][lfs_cache['storage_partition_uuid']]
                 self._path_on_disk = f"{storage_partition['path']}/lfs/{self.uuid}/data"
 
                 if lfs_cache['state'] == 'ready':
                     return
                 else:
                     lfs_is_already_downloading = True
@@ -154,14 +164,28 @@
             ))
             with LfsCacheState() as cache_state:
                 cache_state['large_file_systems'][self.uuid]['state'] = 'ready'
                 logger_no_user_data.debug(f'LFS cache state: {cache_state}')
 
         logger_no_user_data.debug(f'LFS {self.uuid} is initialized')
 
+    def detach(self) -> None:
+        if not self._is_initialized:
+            return
+
+        logger_no_user_data.debug(f'Job "{self._job_id}" detaching from LFS {self.uuid}')
+
+        # TODO: Fix
+        # with LfsCacheState() as cache_state:
+        #     lfs_cache = cache_state['large_file_systems'][self.uuid]
+        #     lfs_cache['last_used_at'] = LfsCacheState.get_timestamp_now()
+        #     lfs_cache['active_jobs'] = [job_id for job_id in lfs_cache['active_jobs'] if job_id != self._job_id]
+
+        self._path_on_disk = None
+
     def _remove_from_state(self) -> None:
         with LfsCacheState() as cache_state:
             lfs = cache_state['large_file_systems'][self.uuid]
             storage_partition = cache_state['storage_partitions'][lfs['storage_partition_uuid']]
             storage_partition['allocated_size_bytes'] -= lfs['size_bytes']
 
             cache_state['large_file_systems'].pop(self.uuid)
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/mappings.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/mappings.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/compute_node/job_worker/utils.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/compute_node/remote_host_proxy.py` & `pybiolib-1.1.94/biolib/compute_node/remote_host_proxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -71,33 +71,20 @@
     def start(self) -> None:
         # TODO: Implement nice error handling in this method
 
         upstream_server_name = self._remote_host['hostname']
         upstream_server_ports = self._remote_host['ports']
 
         docker = BiolibDockerClient.get_docker_client()
-
-        for index in range(3):
-            logger_no_user_data.debug(f'Attempt {index} at creating RemoteHostProxy container "{self._name}"...')
-            try:
-                self._container = docker.containers.create(
-                    detach=True,
-                    image=self._get_nginx_docker_image(),
-                    name=self._name,
-                    network=self._public_network.name,
-                )
-                break
-            except Exception as error:  # pylint: disable=broad-except
-                logger_no_user_data.exception(f'Failed to create container "{self._name}" hit error: {error}')
-
-            logger_no_user_data.debug('Sleeping before re-trying container creation...')
-            time.sleep(3)
-
-        if not self._container:
-            raise BioLibError(f'Exceeded re-try limit for creating container {self._name}')
+        self._container = docker.containers.create(
+            detach=True,
+            image=self._get_nginx_docker_image(),
+            name=self._name,
+            network=self._public_network.name,
+        )
 
         self._write_nginx_config_to_container(
             upstream_server_name,
             upstream_server_ports,
         )
 
         if self._internal_network:
@@ -170,15 +157,14 @@
 
             nginx_config = f'''
 events {{
   worker_connections  1024;
 }}
 
 http {{
-    client_max_body_size 0; 
     map $request_method $bearer_token_on_post {{
         POST       "{bearer_token}";
         default    "";
     }}
 
     map $request_method $bearer_token_on_get {{
         GET        "{bearer_token}";
@@ -205,55 +191,25 @@
             # Note: Using $1 here as URI part from regex must be used for proxy_pass
             proxy_pass               {base_url}/api/jobs/cloud/$1;
             proxy_set_header         authorization $bearer_token_on_post;
             proxy_set_header         cookie "";
             proxy_ssl_server_name    on;
         }}
 
-        location ~* "^/api/jobs/(?<job_id>[a-z0-9-]{{36}})/storage/input/start_upload/$" {{
-            proxy_pass               {base_url}/api/jobs/$job_id/storage/input/start_upload/;
-            proxy_set_header         authorization "";
-            proxy_set_header         cookie "";
-            proxy_ssl_server_name    on;
-        }}
-
-        location ~* "^/api/jobs/(?<job_id>[a-z0-9-]{{36}})/storage/input/presigned_upload_url/$" {{
-            proxy_pass               {base_url}/api/jobs/$job_id/storage/input/presigned_upload_url/$is_args$args;
-            proxy_set_header         authorization "";
-            proxy_set_header         cookie "";
-            proxy_ssl_server_name    on;
-        }}
-
-        location ~* "^/api/jobs/(?<job_id>[a-z0-9-]{{36}})/storage/input/complete_upload/$" {{
-            proxy_pass               {base_url}/api/jobs/$job_id/storage/input/complete_upload/;
-            proxy_set_header         authorization "";
-            proxy_set_header         cookie "";
-            proxy_ssl_server_name    on;
-        }}
-        
-        location ~* "^/api/jobs/(?<job_id>[a-z0-9-]{{36}})/main_result/$" {{
-            proxy_pass                  {base_url}/api/jobs/$job_id/main_result/;
-            proxy_set_header            authorization "";
-            proxy_set_header            cookie "";
-            proxy_pass_request_headers  on;
-            proxy_ssl_server_name       on;
-        }}
-
         location ~* "^/api/jobs/(?<job_id>[a-z0-9-]{{36}})/$" {{
             proxy_pass               {base_url}/api/jobs/$job_id/;
             proxy_set_header         authorization $bearer_token_on_patch;
             proxy_set_header         cookie "";
             proxy_ssl_server_name    on;
         }}
 
         location ~* "^/api/jobs/$" {{
             # Note: Using $1 here as URI part from regex must be used for proxy_pass
             proxy_pass               {base_url}/api/jobs/$1;
             proxy_set_header         authorization $bearer_token_on_post;
-            proxy_set_header         caller-job-uuid "{self._job_uuid}";
             proxy_set_header         cookie "";
             proxy_ssl_server_name    on;
         }}
 
         location /api/ {{
             proxy_pass               {base_url}/api/;
             proxy_set_header         authorization "";
@@ -270,28 +226,14 @@
 
         location /job-storage/ {{
             proxy_pass               {s3_results_base_url}/job-storage/;
             proxy_set_header         authorization "";
             proxy_set_header         cookie "";
             proxy_ssl_server_name    on;
         }}
-
-        location /proxy/storage/job-storage/ {{
-            proxy_pass               {cloud_base_url}/proxy/storage/job-storage/;
-            proxy_set_header         authorization "";
-            proxy_set_header         cookie "";
-            proxy_ssl_server_name    on;
-        }}
-
-        location /proxy/cloud/ {{
-            proxy_pass               {cloud_base_url}/proxy/cloud/;
-            proxy_set_header         authorization "";
-            proxy_set_header         cookie "";
-            proxy_ssl_server_name    on;
-        }}
     }}
 }}
 '''
         else:
             nginx_config = '''
 events {}
 error_log /dev/stdout info;
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/socker_listener_thread.py` & `pybiolib-1.1.94/biolib/compute_node/socker_listener_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/compute_node/socket_sender_thread.py` & `pybiolib-1.1.94/biolib/compute_node/socket_sender_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/compute_node/utils.py` & `pybiolib-1.1.94/biolib/compute_node/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         return 'StdoutAndStderr'
 
     else:
         raise Exception(f"Unexpected package type {package_type}")
 
 
 class SystemExceptionCodes(Enum):
-    COMPLETED_SUCCESSFULLY = 0
     FAILED_TO_INIT_COMPUTE_PROCESS_VARIABLES = 1
     FAILED_TO_CONNECT_TO_WORKER_THREAD_SOCKET = 2
     FAILED_TO_START_SENDER_THREAD_OR_RECEIVER_THREAD = 3
     FAILED_TO_GET_ATTESTATION_DOCUMENT = 4
     FAILED_TO_CREATE_DOCKER_NETWORKS = 5
     FAILED_TO_START_REMOTE_HOST_PROXIES = 6
     FAILED_TO_REDIRECT_ENCLAVE_TRAFFIC_TO_PROXIES = 7
@@ -54,27 +53,27 @@
     FAILED_TO_START_COMPUTE_CONTAINER = 18
     FAILED_TO_COPY_INPUT_FILES_TO_COMPUTE_CONTAINER = 19
     FAILED_TO_COPY_RUNTIME_FILES_TO_COMPUTE_CONTAINER = 20
     FAILED_TO_RUN_COMPUTE_CONTAINER = 21
     FAILED_TO_RETRIEVE_AND_MAP_OUTPUT_FILES = 22
     FAILED_TO_SERIALIZE_AND_SEND_MODULE_OUTPUT = 23
     FAILED_TO_DESERIALIZE_SAVED_JOB = 24
-    UNKNOWN_COMPUTE_PROCESS_ERROR = 25
+    UNKOWN_COMPUTE_PROCESS_ERROR = 25
     FAILED_TO_INITIALIZE_WORKER_THREAD = 26
     FAILED_TO_HANDLE_PACKAGE_IN_WORKER_THREAD = 27
     EXCEEDED_MAX_JOB_RUNTIME = 28
     OUT_OF_MEMORY = 29
     CANCELLED_BY_USER = 30
     COMMAND_OVERRIDE_NOT_ALLOWED = 31
     FAILED_TO_ALLOCATE_JOB_TO_COMPUTE_NODE = 32
     NO_MODULES_FOUND_ON_JOB = 33
 
 
+
 SystemExceptionCodeMap = {
-    0: 'Job completed successfully',
     1: 'Failed to init compute process variables',
     2: 'Failed to connect to worker thread socket',
     3: 'Failed to start sender or receiver thread',
     4: 'Failed to get attestation document',
     5: 'Failed to create docker networks',
     6: 'Failed to start remote host proxies',
     7: 'Failed to redirect enclave traffic to proxies',
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/webserver/gunicorn_flask_application.py` & `pybiolib-1.1.94/biolib/compute_node/webserver/gunicorn_flask_application.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/compute_node/webserver/webserver.py` & `pybiolib-1.1.94/biolib/compute_node/webserver/webserver.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,38 +8,31 @@
 import logging
 from flask import Flask, request, Response, jsonify, after_this_request
 from flask_cors import CORS  # type: ignore
 
 from biolib import utils
 from biolib.biolib_api_client import BiolibApiClient
 from biolib.biolib_binary_format import SavedJob
-from biolib.compute_node.job_worker.job_storage import JobStorage
 from biolib.compute_node.webserver import webserver_utils
 from biolib.compute_node.cloud_utils.cloud_utils import CloudUtils
 from biolib.compute_node.webserver.gunicorn_flask_application import GunicornFlaskApplication
 from biolib.biolib_logging import logger, TRACE, logger_no_user_data
 from biolib.compute_node.webserver.webserver_utils import get_job_compute_state_or_404
-from biolib.typing_utils import Optional
 
 app = Flask(__name__)
 CORS(app)
 
 biolib_tmp_dir = tempfile.TemporaryDirectory()
 
 
 @app.route('/hello/')
 def hello():
     return 'Hello'
 
 
-@app.route('/health/')
-def health():
-    return 'biolib-compute-node is running', 200
-
-
 @app.route('/v1/job/', methods=['POST'])
 def save_job():
     saved_job = json.loads(request.data.decode())
 
     # TODO: figure out why this shallow validate method is used
     if not webserver_utils.validate_saved_job(saved_job):
         return jsonify({'job': 'Invalid job'}), 400
@@ -90,48 +83,36 @@
     compute_state['received_messages_queue'].put(b'CANCEL_JOB')
     return Response()
 
 
 @app.route('/v1/job/<job_id>/status/')
 def status(job_id):
     # TODO Implement auth token
-    return_full_logs = request.args.get('logs') == 'full'
 
     compute_state = get_job_compute_state_or_404(job_id)
     current_status = compute_state['status'].copy()
-    response_data = current_status
-    response_data['is_completed'] = compute_state['is_completed']
-
-    if current_status['stdout_and_stderr_packages_b64']:
-        compute_state['streamed_logs_packages_b64'] = compute_state['streamed_logs_packages_b64'] + \
-                                                      current_status['stdout_and_stderr_packages_b64']
-
-        compute_state['status']['stdout_and_stderr_packages_b64'] = []
+    response = jsonify(current_status)
 
     if current_status['status_updates']:
-        compute_state['previous_status_updates'].extend(
-            current_status['status_updates']
-        )
-        compute_state['status']['status_updates'] = []
-
-    if return_full_logs:
-        response_data['streamed_logs_packages_b64'] = compute_state['streamed_logs_packages_b64']
-        response_data['previous_status_updates'] = compute_state['previous_status_updates']
+        webserver_utils.JOB_ID_TO_COMPUTE_STATE_DICT[job_id]['status']['status_updates'] = []
+
+    if current_status['stdout_and_stderr_packages_b64']:
+        webserver_utils.JOB_ID_TO_COMPUTE_STATE_DICT[job_id]['status']['stdout_and_stderr_packages_b64'] = []
 
-    return jsonify(response_data)
+    return response
 
 
 @app.route('/v1/job/<job_id>/result/')
 def result(job_id):
     compute_state = webserver_utils.JOB_ID_TO_COMPUTE_STATE_DICT[job_id]
     result_is_ready = compute_state['progress'] == 95
     if result_is_ready:
         logger_no_user_data.debug(f'Job "{job_id}" result is being downloaded by the user...')
         job_temporary_dir = compute_state["job_temporary_dir"]
-        module_output_path = os.path.join(job_temporary_dir, JobStorage.legacy_module_output_file_name)
+        module_output_path = f'{job_temporary_dir}/module_output.bbf'
         # Set the progress to 99 to inform other cleanup code that result is being downloaded
         compute_state['progress'] = 99
 
         @after_this_request
         def remove_job_temporary_dir(response):  # pylint: disable=unused-variable
             if os.path.exists(job_temporary_dir):
                 logger_no_user_data.debug(f'Removing result dir after download from path: {job_temporary_dir}')
@@ -147,20 +128,15 @@
 
 def send_package_to_compute_process(job_id, package_bytes):
     compute_state = get_job_compute_state_or_404(job_id)
     message_queue = compute_state['messages_to_send_queue']
     message_queue.put(package_bytes)
 
 
-def start_webserver(
-        host: str,
-        port: int,
-        tls_pem_certificate_path: Optional[str] = None,
-        tls_pem_key_path: Optional[str] = None,
-) -> None:
+def start_webserver(port, host):
     def worker_exit(server, worker):  # pylint: disable=unused-argument
         active_compute_states = list(
             webserver_utils.JOB_ID_TO_COMPUTE_STATE_DICT.values()) + webserver_utils.UNASSIGNED_COMPUTE_PROCESSES
         logger.debug(f'Sending terminate signal to {len(active_compute_states)} compute processes')
         if active_compute_states:
             for compute_state in active_compute_states:
                 if compute_state['worker_thread']:
@@ -187,19 +163,16 @@
     elif logger.level == logging.INFO:
         gunicorn_log_level_name = 'WARNING'
     else:
         gunicorn_log_level_name = logging.getLevelName(logger.level)
 
     options = {
         'bind': f'{host}:{port}',
-        'certfile': tls_pem_certificate_path,
-        'graceful_timeout': 4,
-        'keyfile': tls_pem_key_path,
-        'loglevel': gunicorn_log_level_name,
+        'workers': 1,
         'post_fork': post_fork,
-        'ssl_version': 'TLSv1_2',
-        'timeout': '7200',  # Reduce to 300 when frontend no longer downloads from webserver
         'worker_exit': worker_exit,
-        'workers': 1,
+        'timeout': '7200',  # Reduce to 300 when frontend no longer downloads from webserver
+        'graceful_timeout': 4,
+        'loglevel': gunicorn_log_level_name,
     }
 
     GunicornFlaskApplication(app, options).run()
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/webserver/webserver_utils.py` & `pybiolib-1.1.94/biolib/compute_node/webserver/webserver_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 
 def start_compute_process(unassigned_compute_processes):
     compute_state = {
         'job_id': None,
         'job': None,
         'cloud_job_id': None,
         'cloud_job': None,
-        'streamed_logs_packages_b64': [],
-        'previous_status_updates': [],
-        'is_completed': False,
         'status': {
             'status_updates': [
                 {
                     'progress': 10,
                     'log_message': 'Initializing'
                 }
             ],
```

### Comparing `pybiolib-1.1.911/biolib/compute_node/webserver/worker_thread.py` & `pybiolib-1.1.94/biolib/compute_node/webserver/worker_thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,19 @@
 
     @property
     def _job_uuid(self):
         return self.compute_state['job_id']
 
     @property
     def _job_temporary_dir(self):
-        return self.compute_state['job_temporary_dir']
+        return self.compute_state["job_temporary_dir"]
+
+    @property
+    def _result_path(self):
+        return f'{self._job_temporary_dir}/module_output.bbf'
 
     def run(self):
         try:
             while True:
                 package = self.compute_state['received_messages_queue'].get()
                 if package == b'CANCEL_JOB':
                     logger_no_user_data.info(f'Job "{self._job_uuid}" got cancel signal')
@@ -73,21 +77,29 @@
                 elif package_type == 'SystemStatusUpdate':
                     progress, log_message = SystemStatusUpdate(package).deserialize()
                     self._set_status_update(progress, log_message)
 
                     # If 'Computation Finished'
                     if progress == 94:
                         if utils.IS_RUNNING_IN_CLOUD:
-                            JobStorage.upload_module_output(
-                                job_temporary_dir=self._job_temporary_dir,
-                                job_uuid=self._job_uuid,
-                            )
+                            aes_key_string_b64 = self.compute_state.get('aes_key_string_b64')
+                            if aes_key_string_b64 or utils.DISABLE_CLIENT_SIDE_ENCRYPTION:
+                                logger_no_user_data.debug(f'Job "{self._job_uuid}" uploading result...')
+                                with open(self._result_path, 'rb') as serialized_module_output_file:
+                                    serialized_module_output = serialized_module_output_file.read()
+                                    JobStorage.upload_module_output(
+                                        job_uuid=self._job_uuid,
+                                        module_output=serialized_module_output,
+                                        aes_key_string_b64=aes_key_string_b64
+                                    )
+                                    logger_no_user_data.debug(f'Job "{self._job_uuid}" result uploaded successfully')
+                            else:
+                                logger_no_user_data.debug("Assuming user will consume result from webserver")
 
                         self._set_status_update(progress=95, log_message='Result Ready')
-                        self.compute_state['is_completed'] = True
                         self.terminate()
 
                 elif package_type == 'SystemException':
                     error_code = SystemException(package).deserialize()
                     self.compute_state['status']['error_code'] = error_code
                     logger.debug("Hit error. Terminating Worker Thread and Compute Process")
                     self.compute_state['progress'] = 95
```

### Comparing `pybiolib-1.1.911/biolib/jobs/job_result.py` & `pybiolib-1.1.94/biolib/compute_node/job_worker/job_storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,120 @@
+import base64
 import os
-from pathlib import Path
-from fnmatch import fnmatch
-import time
 from urllib.parse import urlparse
 
 import requests
+from Crypto.Random import get_random_bytes
 
-from biolib import api
-from biolib.biolib_binary_format import UnencryptedModuleOutput
-from biolib.biolib_binary_format.utils import RemoteIndexableBuffer, LazyLoadedFile
+from biolib import utils
+from biolib.biolib_api_client import BiolibApiClient, Job
+from biolib.biolib_api_client.biolib_job_api import BiolibJobApi
+from biolib.biolib_binary_format.utils import InMemoryIndexableBuffer, RemoteIndexableBuffer
+from biolib.biolib_binary_format.encrypted_module_output import EncryptedModuleOutputWithKey
+from biolib.biolib_binary_format.unencrypted_module_output import UnencryptedModuleOutput
 from biolib.biolib_errors import BioLibError
+from biolib.compute_node.cloud_utils import CloudUtils
+from biolib.compute_node.job_worker.job_key_cache import JobKeyCacheState
 from biolib.biolib_logging import logger_no_user_data, logger
-from biolib.typing_utils import Optional, Dict, List, cast, Union, Callable
 
 
-class JobResultError(BioLibError):
-    pass
-
-
-class JobResultNotFound(JobResultError):
-    pass
-
-
-class JobResultPermissionError(JobResultError):
-    pass
-
-
-PathFilter = Union[str, Callable[[LazyLoadedFile], bool]]
-
-
-class JobResult:
-
-    def __init__(
-            self,
-            job_uuid: str,
-            job_auth_token: Optional[str],
-            module_output: Optional[UnencryptedModuleOutput] = None,
-    ):
-        self._job_uuid: str = job_uuid
-        self._job_auth_token: Optional[str] = job_auth_token
-
-        self._module_output: Optional[UnencryptedModuleOutput] = module_output
-
-    def get_stdout(self) -> bytes:
-        return self._get_module_output().get_stdout()
-
-    def get_stderr(self) -> bytes:
-        return self._get_module_output().get_stderr()
-
-    def get_exit_code(self) -> int:
-        return self._get_module_output().get_exit_code()
-
-    def save_files(self, output_dir: str, path_filter: Optional[PathFilter] = None) -> None:
-        module_output = self._get_module_output()
-        output_files = module_output.get_files()
-
-        if path_filter:
-            output_files = self._get_filtered_files(output_files, path_filter)
-
-        logger.info(f'Saving {len(output_files)} files to {output_dir}...')
-
-        for file in output_files:
-            # Remove leading slash of file_path
-            destination_file_path = Path(output_dir) / Path(file.path.lstrip('/'))
-            if destination_file_path.exists():
-                destination_file_path.rename(f'{destination_file_path}.biolib-renamed.{time.strftime("%Y%m%d%H%M%S")}')
-
-            dir_path = destination_file_path.parent
-            if dir_path:
-                dir_path.mkdir(parents=True, exist_ok=True)
-
-            with open(destination_file_path, mode='wb') as file_handler:
-                for chunk_number, chunk in enumerate(file.get_data_as_iterable()):
-                    logger_no_user_data.debug(f'Processing chunk {chunk_number}...')
-                    file_handler.write(chunk)
-
-            logger.info(f'  - {destination_file_path}')
-
-    def get_output_file(self, filename) -> LazyLoadedFile:
-        files = self._get_module_output().get_files()
-        filtered_files = self._get_filtered_files(files, path_filter=filename)
-        if not filtered_files:
-            raise BioLibError(f"File {filename} not found in results.")
-
-        if len(filtered_files) != 1:
-            raise BioLibError(f"Found multiple results for filename {filename}.")
-
-        return filtered_files[0]
-
-    def list_output_files(self, path_filter: Optional[PathFilter] = None) -> List[LazyLoadedFile]:
-        files = self._get_module_output().get_files()
-        if not path_filter:
-            return files
-
-        return self._get_filtered_files(files, path_filter)
+class JobStorage:
 
     @staticmethod
-    def _get_filtered_files(files: List[LazyLoadedFile], path_filter: PathFilter) -> List[LazyLoadedFile]:
-        if not (isinstance(path_filter, str) or callable(path_filter)):
-            raise Exception('Expected path_filter to be a string or a function')
-
-        if callable(path_filter):
-            return list(filter(path_filter, files))
-
-        glob_filter = cast(str, path_filter)
+    def upload_module_output(job_uuid: str, module_output: bytes, aes_key_string_b64: str) -> None:
+        try:
+            if utils.DISABLE_CLIENT_SIDE_ENCRYPTION:
+                storage_module_output = UnencryptedModuleOutput.create_from_serialized_module_output(module_output)
+                logger_no_user_data.debug(f'Job "{job_uuid}" uploading result to S3...')
 
-        # since all file paths start with /, make sure filter does too
-        if not glob_filter.startswith("/"):
-            glob_filter = "/" + glob_filter
+            else:
+                if not aes_key_string_b64:
+                    raise Exception('Missing AES key for module output upload as client side encryption is enabled')
+                storage_module_output = EncryptedModuleOutputWithKey(
+                    aes_key_string_b64=aes_key_string_b64
+                ).create_from_serialized_module_output(module_output)
+                logger_no_user_data.debug(f'Job "{job_uuid}" uploading encrypted result to S3...')
 
-        def _filter_function(file: LazyLoadedFile) -> bool:
-            return fnmatch(file.path, glob_filter)
+        except Exception as error:
+            logger_no_user_data.debug('Failed to get storage module output from serialized module output')
+            logger.debug(f'Failed to get storage module output from serialized module output due to {error}')
+            raise error
+
+        # Free up memory as quickly as possible
+        del module_output
+
+        base_url = BiolibApiClient.get().base_url
+        config = CloudUtils.get_webserver_config()
+        compute_node_auth_token = config['compute_node_info']['auth_token']  # pylint: disable=unsubscriptable-object
+        headers = {'Compute-Node-Auth-Token': compute_node_auth_token}
+
+        multipart_uploader = utils.MultiPartUploader(
+            start_multipart_upload_request=dict(
+                requires_biolib_auth=False,
+                url=f'{base_url}/api/jobs/{job_uuid}/storage/results/start_upload/',
+                headers=headers,
+            ),
+            get_presigned_upload_url_request=dict(
+                requires_biolib_auth=False,
+                url=f'{base_url}/api/jobs/{job_uuid}/storage/results/presigned_upload_url/',
+                headers=headers,
+            ),
+            complete_upload_request=dict(
+                requires_biolib_auth=False,
+                url=f'{base_url}/api/jobs/{job_uuid}/storage/results/complete_upload/',
+                headers=headers,
+            ),
+        )
+
+        multipart_uploader.upload(
+            payload_iterator=utils.get_chunk_iterator_from_bytes(storage_module_output),
+            payload_size_in_bytes=len(storage_module_output),
+        )
 
-        return list(filter(_filter_function, files))
+    @staticmethod
+    def get_result(job: Job) -> bytes:
+        presigned_download_url = BiolibJobApi.get_job_storage_result_download_url(job['auth_token'])
 
-    def _get_presigned_download_url(self) -> str:
-        try:
-            response_dict: Dict[str, str] = api.client.get(
-                url=f'/jobs/{self._job_uuid}/storage/results/download/',
-                headers={'Job-Auth-Token': self._job_auth_token} if self._job_auth_token else None,
-            ).json()
-            presigned_download_url = response_dict['presigned_download_url']
-
-            app_caller_proxy_job_storage_base_url = os.getenv('BIOLIB_CLOUD_JOB_STORAGE_BASE_URL', '')
-            if app_caller_proxy_job_storage_base_url:
-                # Done to hit App Caller Proxy when downloading result from inside an app
-                parsed_url = urlparse(presigned_download_url)
-                presigned_download_url = f'{app_caller_proxy_job_storage_base_url}{parsed_url.path}?{parsed_url.query}'
-
-            return presigned_download_url
-        except requests.exceptions.HTTPError as error:
-            status_code = error.response.status_code
-
-            if status_code == 401:
-                raise JobResultPermissionError('You must be signed in to get result of the job') from None
-            elif status_code == 403:
-                raise JobResultPermissionError(
-                    'Cannot get result of job. Maybe the job was created without being signed in?'
-                ) from None
-            elif status_code == 404:
-                raise JobResultNotFound('Job result not found') from None
-            else:
-                raise JobResultError('Failed to get result of job') from error
+        s3_results_base_url = os.getenv('BIOLIB_CLOUD_RESULTS_BASE_URL', '')
+        if s3_results_base_url:
+            # Done to hit App Caller Proxy when downloading result from inside an app
+            parsed_url = urlparse(presigned_download_url)
+            presigned_download_url = f'{s3_results_base_url}{parsed_url.path}?{parsed_url.query}'
+
+        if utils.BASE_URL_IS_PUBLIC_BIOLIB:
+            # TODO: Use RemoteIndexableBuffer for EncryptedModuleOutputWithKey
+            try:
+                result_response = requests.get(
+                    url=presigned_download_url,
+                    timeout=3600,  # timeout after 1 hour
+                )
+
+                if not result_response.ok:
+                    raise BioLibError(result_response.content)
+
+            except Exception as error:
+                logger.debug(f'Failed to get results from S3 due to {error}')
+                raise error
+
+            with JobKeyCacheState() as cache_state:
+                aes_key_string_b64 = cache_state[job['public_id']]
+
+            encrypted_module_output = EncryptedModuleOutputWithKey(
+                buffer=InMemoryIndexableBuffer(result_response.content),
+                aes_key_string_b64=aes_key_string_b64,
+            )
+            return encrypted_module_output.convert_to_serialized_module_output()
+
+        else:
+            buffer = RemoteIndexableBuffer(url=presigned_download_url)
+            unencrypted_module_output = UnencryptedModuleOutput(buffer)
+            return unencrypted_module_output.convert_to_serialized_module_output()
 
-        except Exception as error:
-            raise JobResultError('Failed to get result of job') from error
+    @staticmethod
+    def generate_and_store_key_buffer_for_job(job_id: str) -> str:
+        aes_key_buffer = get_random_bytes(32)
+        aes_key_string_b64 = base64.urlsafe_b64encode(aes_key_buffer).decode()
 
-    def _get_module_output(self) -> UnencryptedModuleOutput:
-        if self._module_output is None:
-            buffer = RemoteIndexableBuffer(url=self._get_presigned_download_url())
-            self._module_output = UnencryptedModuleOutput(buffer)
+        with JobKeyCacheState() as cache_state:
+            cache_state[job_id] = aes_key_string_b64
 
-        return self._module_output
+        return aes_key_string_b64
```

### Comparing `pybiolib-1.1.911/biolib/templates/example_app.py` & `pybiolib-1.1.94/biolib/templates/example_app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/user/sign_in.py` & `pybiolib-1.1.94/biolib/user/sign_in.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/utils/__init__.py` & `pybiolib-1.1.94/biolib/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,70 @@
 import io
 import collections.abc
 import multiprocessing
 import os
 import time
-import socket
 import sys
 from urllib.parse import urlparse
 
 import requests
 from importlib_metadata import version, PackageNotFoundError
 
-from biolib.utils.seq_util import SeqUtil, SeqUtilRecord
-
 # try fetching version, if it fails (usually when in dev), add default
 from biolib.biolib_errors import BioLibError
-from biolib.biolib_logging import logger_no_user_data, logger
+from biolib.biolib_logging import logger_no_user_data
 from biolib.typing_utils import Tuple, Iterator
 from .multipart_uploader import MultiPartUploader, get_chunk_iterator_from_bytes
 
 try:
     BIOLIB_PACKAGE_VERSION = version('pybiolib')
 except PackageNotFoundError:
     BIOLIB_PACKAGE_VERSION = '0.0.0'
 
 IS_DEV = os.getenv('BIOLIB_DEV', '').upper() == 'TRUE'
 
-def _get_base_url() -> str:
-    base_url = os.getenv('BIOLIB_BASE_URL')
-    if base_url:
-        return base_url.lower().rstrip('/')
-
-    try:
-        search_list = []
-        with open('/etc/resolv.conf') as file:
-            for line in file:
-                line_trimmed = line.strip()
-                if line_trimmed.startswith('search'):
-                    search_list = line_trimmed.split()[1:]
-                    logger.debug(f'Found search list: {search_list} when resolving base url.')
-                    break
-
-        for search_host in search_list:
-            host_to_try = f'biolib.{search_host}'
-            if len(socket.getaddrinfo(host_to_try, 443)) > 0:
-                return f'https://{host_to_try}'.lower()
-    except BaseException: # pylint: disable=broad-except
-        pass
-
-    return 'https://biolib.com'
-
-BIOLIB_BASE_URL = _get_base_url()
+BIOLIB_BASE_URL = os.getenv('BIOLIB_BASE_URL', default='https://biolib.com').lower()
 
 BIOLIB_CLOUD_BASE_URL = os.getenv('BIOLIB_CLOUD_BASE_URL', '').lower()
 
 BIOLIB_PACKAGE_ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 BIOLIB_CLOUD_ENVIRONMENT = os.getenv('BIOLIB_CLOUD_ENVIRONMENT', '').lower()
 
-BIOLIB_SECRETS_TMPFS_PATH = os.environ.get('BIOLIB_SECRETS_TMPFS_PATH')
-
 IS_RUNNING_IN_CLOUD = BIOLIB_CLOUD_ENVIRONMENT == 'non-enclave'
 
+DISABLE_CLIENT_SIDE_ENCRYPTION = os.getenv('BIOLIB_DISABLE_CLIENT_SIDE_ENCRYPTION', '').upper() == 'TRUE'
+
 BASE_URL_IS_PUBLIC_BIOLIB = BIOLIB_BASE_URL.endswith('biolib.com') or \
                             os.environ.get('BIOLIB_ENVIRONMENT_IS_PUBLIC_BIOLIB', '').upper() == 'TRUE'
 
+BIOLIB_ENABLE_SINGULARITY_CONTAINERS = os.getenv('BIOLIB_ENABLE_SINGULARITY_CONTAINERS', '').upper() == 'TRUE'
+
 # sys.stdout is an instance of OutStream in Jupyter and Colab which does not have .buffer
 if not hasattr(sys.stdout, 'buffer'):
     IS_RUNNING_IN_NOTEBOOK = True
 else:
     IS_RUNNING_IN_NOTEBOOK = False
 
 STREAM_STDOUT = False
 
 if BIOLIB_CLOUD_ENVIRONMENT and not IS_RUNNING_IN_CLOUD:
     logger_no_user_data.warning((
         'BIOLIB_CLOUD_ENVIRONMENT defined but does not specify the cloud environment correctly. ',
         'The compute node will not act as a cloud compute node'
     ))
 
+BIOLIB_CLOUD_SKIP_PCR_VERIFICATION = os.getenv('BIOLIB_CLOUD_SKIP_PCR_VERIFICATION', '').upper() == 'TRUE'
+
 BIOLIB_ENABLE_DNS_PROXY = os.getenv('BIOLIB_ENABLE_DNS_PROXY', '').upper() == 'TRUE'
 
 RUN_DEV_JOB_ID = 'run-dev-mocked-job-id'
 
+BIOLIB_FORCE_REMOTE_COMPUTE = os.getenv('BIOLIB_FORCE_REMOTE_COMPUTE', '').upper() == 'TRUE'
+
 
 def get_absolute_container_image_uri(base_url: str, relative_image_uri: str, job_is_federated: bool = False):
     if base_url == 'https://biolib.com' or job_is_federated:
         container_registry_hostname = 'containers.biolib.com'
     elif base_url in ('https://staging-elb.biolib.com', 'https://staging.biolib.com'):
         container_registry_hostname = 'containers.staging.biolib.com'
     else:
@@ -190,17 +169,15 @@
                 approx_progress_percent = min(bytes_written / file_size * 100, 100)
                 logger_no_user_data.debug(
                     f'Wrote part {index} of {file_size} to file, '
                     f'the approximate progress is {round(approx_progress_percent, 2)}%'
                 )
                 chunk_iterator.chunk_completed()
     finally:
-        logger_no_user_data.debug('Closing process poll...')
         process_pool.close()
-        logger_no_user_data.debug('Process poll closed.')
 
 
 def stream_process_output(proc) -> None:
     while proc.poll() is None:
         stdout = io.TextIOWrapper(proc.stdout, newline='')
         stderr = io.TextIOWrapper(proc.stderr, newline='')
         try:
```

### Comparing `pybiolib-1.1.911/biolib/utils/cache_state.py` & `pybiolib-1.1.94/biolib/utils/cache_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,26 @@
 
 
 class CacheStateError(BioLibError):
     pass
 
 
 class CacheState(abc.ABC, Generic[StateType]):
+    _cache_dir: str = appdirs.user_cache_dir(appname='pybiolib', appauthor='biolib')
+
     @property
     @abc.abstractmethod
     def _state_path(self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
     def _get_default_state(self) -> StateType:
         raise NotImplementedError
 
     @property
-    def _user_cache_dir(self) -> str:
-        user_cache_dir: str = appdirs.user_cache_dir(appname='pybiolib', appauthor='biolib')
-        os.makedirs(user_cache_dir, exist_ok=True)
-        return user_cache_dir
-
-    @property
     def _state_lock_path(self) -> str:
         return f'{self._state_path}.lock'
 
     def __init__(self):
         self._state: Optional[StateType] = None
 
     def __enter__(self) -> StateType:
@@ -70,19 +66,20 @@
 
         while os.path.exists(self._state_lock_path):
             time.sleep(seconds_to_sleep)
             timeout_seconds -= seconds_to_sleep
             if timeout_seconds < 0:
                 raise CacheStateError('Cache state timed out waiting for lock file')
 
+        os.makedirs(self._cache_dir, exist_ok=True)
         lock_file = open(self._state_lock_path, mode='x')
         lock_file.close()
 
     def _release_state_lock(self) -> None:
         if os.path.exists(self._state_lock_path):
             os.remove(self._state_lock_path)
         else:
             raise CacheStateError('Cache state was not locked.')
 
     @staticmethod
     def get_timestamp_now() -> str:
-        return datetime.utcnow().isoformat()
+        return datetime.now().isoformat()
```

### Comparing `pybiolib-1.1.911/biolib/utils/multipart_uploader.py` & `pybiolib-1.1.94/biolib/utils/multipart_uploader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 import math
 import multiprocessing
-import os
 import time
-from urllib.parse import urlparse
+from typing import Dict
 
 import requests
 
 from biolib.biolib_api_client import BiolibApiClient
 from biolib.biolib_api_client.auth import BearerAuth
 from biolib.biolib_errors import BioLibError
 from biolib.biolib_logging import logger, logger_no_user_data
-from biolib.typing_utils import TypedDict, List, Iterator, Tuple, Optional, Dict
+from biolib.typing_utils import TypedDict, List, Iterator, Tuple, Optional
 
 
 def get_chunk_iterator_from_bytes(byte_buffer: bytes, chunk_size_in_bytes: int = 50_000_000) -> Iterator[bytes]:
     chunk_count = math.ceil(len(byte_buffer) / chunk_size_in_bytes)
     for chunk_number in range(chunk_count):
         start = chunk_size_in_bytes * chunk_number
         stop = start + chunk_size_in_bytes
         yield byte_buffer[start:stop]
 
 
-def get_chunk_iterator_from_file_object(file_object, chunk_size_in_bytes: int = 50_000_000) -> Iterator[bytes]:
-    while True:
-        data = file_object.read(chunk_size_in_bytes)
-        if not data:
-            break
-        yield data
-
-
 class RequestOptions(TypedDict):
     headers: Optional[Dict[str, str]]
     requires_biolib_auth: bool
     url: str
 
 
 class _PartMetadata(TypedDict):
@@ -75,41 +66,34 @@
                 logger_no_user_data.debug('Multipart upload started')
             else:
                 logger_no_user_data.debug(
                     f'Failed to start multipart upload got response status: {start_multipart_upload.status_code}'
                 )
                 raise Exception('Failed to start multipart upload')
 
-        # if multiprocessing start method is spawn or we are running in a daemon process,
-        # multiprocessing.Pool may fail when called from script
-        if multiprocessing.get_start_method() == 'spawn' or multiprocessing.current_process().daemon:
-            logger_no_user_data.debug('Uploading multipart from main process...')
-            for chunk in iterator_with_index:
-                upload_chunk_response = self._upload_chunk(chunk)
-                self._update_progress_bar_and_parts(
-                    upload_chunk_response=upload_chunk_response,
-                    parts=parts,
-                    bytes_uploaded=bytes_uploaded,
-                    payload_size_in_bytes=payload_size_in_bytes
+        # use 16 cores, unless less is available
+        process_pool = multiprocessing.Pool(processes=min(16, multiprocessing.cpu_count() - 1))
+        try:
+            response: _UploadChunkReturnType
+            for response in process_pool.imap(self._upload_chunk, iterator_with_index):
+                part_metadata, chunk_byte_length = response
+                part_number = part_metadata['PartNumber']
+
+                parts.append(part_metadata)
+                bytes_uploaded += chunk_byte_length
+
+                approx_progress_percent = min(bytes_uploaded / (payload_size_in_bytes + 1) * 100, 100)
+                approx_rounded_progress = round(approx_progress_percent, 2)
+                logger_no_user_data.info(
+                    f'Uploaded part {part_number} of {chunk_byte_length} bytes, '
+                    f'the approximate progress is {approx_rounded_progress}%'
                 )
-        else:
-            # use 16 cores, unless less is available
-            process_pool = multiprocessing.Pool(processes=min(16, multiprocessing.cpu_count() - 1))
-            try:
-                response: _UploadChunkReturnType
-                for response in process_pool.imap(self._upload_chunk, iterator_with_index):
-                    self._update_progress_bar_and_parts(
-                        upload_chunk_response=response,
-                        parts=parts,
-                        bytes_uploaded=bytes_uploaded,
-                        payload_size_in_bytes=payload_size_in_bytes
-                    )
-            finally:
-                logger_no_user_data.debug('Multipart upload closing process pool...')
-                process_pool.close()
+        finally:
+            logger_no_user_data.debug('Multipart upload closing process pool...')
+            process_pool.close()
 
         requires_biolib_auth = self._complete_upload_request['requires_biolib_auth']
         if requires_biolib_auth:
             BiolibApiClient.refresh_auth_token()
 
         logger_no_user_data.debug(f'Uploaded {len(parts)} parts, now calling complete upload...')
         for index in range(3):
@@ -141,15 +125,15 @@
         part_number, chunk = _input
         requires_biolib_auth = self._get_presigned_upload_url_request['requires_biolib_auth']
 
         for index in range(20):  # will fail after approximately sum_i(i^2+2) = 41 min if range (20)
             if requires_biolib_auth:
                 BiolibApiClient.refresh_auth_token()
 
-            logger_no_user_data.debug(f'Uploading chunk {part_number} of length {len(chunk)}...')
+            logger_no_user_data.info(f'Uploading chunk {part_number} of length {len(chunk)}...')
             try:
                 logger_no_user_data.debug(f'Getting upload URL for chunk {part_number}...')
                 get_url_response = requests.get(
                     auth=BearerAuth(BiolibApiClient.get().access_token) if requires_biolib_auth else None,
                     headers=self._get_presigned_upload_url_request['headers'],
                     params={'part_number': part_number},
                     timeout=30,
@@ -158,22 +142,14 @@
                 if not get_url_response.ok:
                     raise Exception(
                         f'Failed to get upload URL for part {part_number} got response status code '
                         f'{get_url_response.status_code}'
                     )
 
                 presigned_upload_url = get_url_response.json()['presigned_upload_url']
-
-                app_caller_proxy_job_storage_base_url = os.getenv('BIOLIB_CLOUD_JOB_STORAGE_BASE_URL', '')
-                if app_caller_proxy_job_storage_base_url:
-                    # Done to hit App Caller Proxy when uploading result from inside an app
-                    parsed_url = urlparse(presigned_upload_url)
-                    presigned_upload_url = \
-                        f'{app_caller_proxy_job_storage_base_url}{parsed_url.path}?{parsed_url.query}'
-
                 put_chunk_response = requests.put(url=presigned_upload_url, data=chunk, timeout=300)
 
                 if put_chunk_response.ok:
                     return _PartMetadata(PartNumber=part_number, ETag=put_chunk_response.headers['ETag']), len(chunk)
                 else:
                     logger_no_user_data.warning(
                         f'Got response with status {put_chunk_response.status_code} when uploading part {part_number}. '
@@ -185,27 +161,7 @@
                 logger_no_user_data.warning(f'Encountered error when uploading part {part_number}. Retrying...')
                 logger.debug(f'Upload error: {error}')
 
             time.sleep(index * index + 2)
 
         logger_no_user_data.debug(f'Max retries hit, when uploading part {part_number}. Exiting...')
         raise BioLibError(f'Max retries hit, when uploading part {part_number}. Exiting...')
-
-    def _update_progress_bar_and_parts(
-        self,
-        upload_chunk_response: _UploadChunkReturnType,
-        parts: List[_PartMetadata],
-        bytes_uploaded: int,
-        payload_size_in_bytes: int,
-    ) -> None:
-        part_metadata, chunk_byte_length = upload_chunk_response
-        part_number = part_metadata['PartNumber']
-
-        parts.append(part_metadata)
-        bytes_uploaded += chunk_byte_length
-
-        approx_progress_percent = min(bytes_uploaded / (payload_size_in_bytes + 1) * 100, 100)
-        approx_rounded_progress = round(approx_progress_percent, 2)
-        logger_no_user_data.debug(
-            f'Uploaded part {part_number} of {chunk_byte_length} bytes, '
-            f'the approximate progress is {approx_rounded_progress}%'
-        )
```

### Comparing `pybiolib-1.1.911/biolib/validators/validate_app_version.py` & `pybiolib-1.1.94/biolib/validators/validate_app_version.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/validators/validate_argument.py` & `pybiolib-1.1.94/biolib/validators/validate_argument.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/validators/validate_module.py` & `pybiolib-1.1.94/biolib/validators/validate_module.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/validators/validate_zip_file.py` & `pybiolib-1.1.94/biolib/validators/validate_zip_file.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/biolib/validators/validator_utils.py` & `pybiolib-1.1.94/biolib/validators/validator_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.911/pyproject.toml` & `pybiolib-1.1.94/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybiolib"
-version = "1.1.911"
+version = "1.1.94"
 description = "BioLib Python Client"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/biolib"
 keywords = ["biolib"]
 authors = [
     "biolib <hello@biolib.com>",
@@ -22,35 +22,33 @@
 ]
 
 [tool.poetry.scripts]
 biolib = "biolib:call_cli"
 
 [tool.poetry.dependencies]
 appdirs = ">=1.4.3"
-click = ">= 8.0.0, < 8.1.0"
 docker = ">=5.0.3"
 flask = ">=2.0.1"
 flask-cors = ">=3.0.10"
 gunicorn = ">=20.1.0"
 importlib-metadata = ">=1.6.1"
 pycryptodome = ">=3.9.9"
 pyjwt = ">=2.3.0"
 python = "^3.6.3"
 pyyaml = ">=5.3.1"
-requests = ">=2.25.1, < 2.30.0"
-rich = "^12.4.4"
+requests = ">=2.25.1"
+spython = ">=0.1.18"
 typing_extensions = { version = ">=3.10.0", python = "<3.8" }
 typing_inspect = { version = "^0.5.0", python = "<3.8" }
+rich = "^12.4.4"
 
 [tool.poetry.dev-dependencies]
 mypy = "==0.910"
 pylint = "==2.7.4"
 pytest = "==6.2.4"
-pytest-timeout = "^2.1.0"
-types-click = "==7.1.8"
 types-Flask = "==1.1.1"
 types-PyYAML = "==5.4.3"
 types-requests = "==2.25.0"
 types-termcolor = "==0.1.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `pybiolib-1.1.911/PKG-INFO` & `pybiolib-1.1.94/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: pybiolib
-Version: 1.1.911
+Version: 1.1.94
 Summary: BioLib Python Client
 Home-page: https://github.com/biolib
 License: MIT
 Keywords: biolib
 Author: biolib
 Author-email: hello@biolib.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.3)
-Requires-Dist: click (>=8.0.0,<8.1.0)
 Requires-Dist: docker (>=5.0.3)
 Requires-Dist: flask (>=2.0.1)
 Requires-Dist: flask-cors (>=3.0.10)
 Requires-Dist: gunicorn (>=20.1.0)
 Requires-Dist: importlib-metadata (>=1.6.1)
 Requires-Dist: pycryptodome (>=3.9.9)
 Requires-Dist: pyjwt (>=2.3.0)
 Requires-Dist: pyyaml (>=5.3.1)
-Requires-Dist: requests (>=2.25.1,<2.30.0)
+Requires-Dist: requests (>=2.25.1)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
-Requires-Dist: typing_extensions (>=3.10.0) ; python_version < "3.8"
-Requires-Dist: typing_inspect (>=0.5.0,<0.6.0) ; python_version < "3.8"
+Requires-Dist: spython (>=0.1.18)
+Requires-Dist: typing_extensions (>=3.10.0); python_version < "3.8"
+Requires-Dist: typing_inspect (>=0.5.0,<0.6.0); python_version < "3.8"
 Description-Content-Type: text/markdown
 
 # PyBioLib
 
 PyBioLib is a Python package for running BioLib applications from Python scripts and the command line.
 
 ### Python Example
@@ -46,7 +45,8 @@
 
 ### Command Line Example
 ```bash
 pip3 install -U pybiolib
 biolib run samtools/samtools --help
 ```
 
+
```

