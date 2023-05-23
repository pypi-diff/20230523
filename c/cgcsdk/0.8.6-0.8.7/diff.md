# Comparing `tmp/cgcsdk-0.8.6.tar.gz` & `tmp/cgcsdk-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.8.6.tar", last modified: Fri May 19 13:18:09 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.7.tar", last modified: Tue May 23 09:10:04 2023, max compression
```

## Comparing `cgcsdk-0.8.6.tar` & `cgcsdk-0.8.7.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.783755 cgcsdk-0.8.6/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.6/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-05-19 13:18:09.781681 cgcsdk-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.506079 cgcsdk-0.8.6/cgc/
--rw-rw-rw-   0        0        0      261 2023-05-19 13:13:56.000000 cgcsdk-0.8.6/cgc/.env
--rw-rw-rw-   0        0        0     3921 2023-05-19 13:08:19.000000 cgcsdk-0.8.6/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.8.6/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.528270 cgcsdk-0.8.6/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.547596 cgcsdk-0.8.6/cgc/commands/auth/
--rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.8.6/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.8.6/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.8.6/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.8.6/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.565073 cgcsdk-0.8.6/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     4006 2023-05-19 13:07:28.000000 cgcsdk-0.8.6/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.6/cgc/commands/cgc_cmd_responses.py
--rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.8.6/cgc/commands/cgc_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.588482 cgcsdk-0.8.6/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.596198 cgcsdk-0.8.6/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.6/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.603014 cgcsdk-0.8.6/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.6/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.609498 cgcsdk-0.8.6/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.631504 cgcsdk-0.8.6/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.6/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.6/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.652733 cgcsdk-0.8.6/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.6/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.6/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     2786 2023-05-18 09:34:33.000000 cgcsdk-0.8.6/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.661237 cgcsdk-0.8.6/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.8.6/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.670280 cgcsdk-0.8.6/cgc/tests/
--rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.6/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.706000 cgcsdk-0.8.6/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.739237 cgcsdk-0.8.6/cgc/utils/
--rw-rw-rw-   0        0        0     3405 2023-05-19 13:08:19.000000 cgcsdk-0.8.6/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.6/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2729 2023-05-19 13:09:02.000000 cgcsdk-0.8.6/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.747617 cgcsdk-0.8.6/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-18 13:48:23.000000 cgcsdk-0.8.6/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1112 2023-05-19 08:15:55.000000 cgcsdk-0.8.6/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.760738 cgcsdk-0.8.6/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.6/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.6/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.6/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-05-18 13:28:20.000000 cgcsdk-0.8.6/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.8.6/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.6/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.779093 cgcsdk-0.8.6/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 13:18:09.784922 cgcsdk-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.545846 cgcsdk-0.8.7/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-05-23 09:10:04.543832 cgcsdk-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.312039 cgcsdk-0.8.7/cgc/
+-rw-rw-rw-   0        0        0      234 2023-05-23 08:45:51.000000 cgcsdk-0.8.7/cgc/.env
+-rw-rw-rw-   0        0        0     4029 2023-05-23 08:47:20.000000 cgcsdk-0.8.7/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.8.7/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.331226 cgcsdk-0.8.7/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.342234 cgcsdk-0.8.7/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.8.7/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.8.7/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.8.7/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.8.7/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.355378 cgcsdk-0.8.7/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.8.7/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.7/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.8.7/cgc/commands/cgc_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.369838 cgcsdk-0.8.7/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.7/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.375831 cgcsdk-0.8.7/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.7/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.385200 cgcsdk-0.8.7/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.7/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.391057 cgcsdk-0.8.7/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.406715 cgcsdk-0.8.7/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.7/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.7/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.422923 cgcsdk-0.8.7/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.7/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.7/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     2786 2023-05-18 09:34:33.000000 cgcsdk-0.8.7/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.427935 cgcsdk-0.8.7/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.8.7/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.435402 cgcsdk-0.8.7/cgc/tests/
+-rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.7/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.464124 cgcsdk-0.8.7/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.7/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.7/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.495781 cgcsdk-0.8.7/cgc/utils/
+-rw-rw-rw-   0        0        0     3405 2023-05-19 13:08:19.000000 cgcsdk-0.8.7/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.7/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.8.7/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.506088 cgcsdk-0.8.7/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-18 13:48:23.000000 cgcsdk-0.8.7/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1218 2023-05-23 08:55:27.000000 cgcsdk-0.8.7/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.519133 cgcsdk-0.8.7/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.7/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.7/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.8.7/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.8.7/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-05-18 13:28:20.000000 cgcsdk-0.8.7/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.8.7/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.7/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.7/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:10:04.540599 cgcsdk-0.8.7/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-05-23 09:10:04.000000 cgcsdk-0.8.7/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-05-23 09:10:04.000000 cgcsdk-0.8.7/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:10:04.000000 cgcsdk-0.8.7/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-23 09:10:04.000000 cgcsdk-0.8.7/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-05-23 09:10:04.000000 cgcsdk-0.8.7/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 09:10:04.000000 cgcsdk-0.8.7/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:10:04.546767 cgcsdk-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.7/setup.py
```

### Comparing `cgcsdk-0.8.6/PKG-INFO` & `cgcsdk-0.8.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.6
+Version: 0.8.7
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.6/cgc/CHANGELOG.md` & `cgcsdk-0.8.7/cgc/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## 0.8.7
+
+Release on May 23, 2023.
+
+* hotfix: development changed .env file making it broken for new users
+
 ## 0.8.6
 
 Release on May 19, 2023.
 
 * added get_redis_client_async() for RedisConnector
 * get_redis_access() - async_client: bool, new parameter
 * new command: cgc context switch [number]
```

### Comparing `cgcsdk-0.8.6/cgc/cgc.py` & `cgcsdk-0.8.7/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.7/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.7/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.7/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.7/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.7/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.7/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.7/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.7/cgc/commands/cgc_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 @click.argument("number", type=click.INT)
 # @click.pass_context
 def switch_context(number: int):
     """Set which namespace config should be used. After switching context your next command will be run in given namespace that corresponds to user namespace"""
     file_name = f"{number}.json" if number > 1 else "cfg.json"
 
     if not check_if_config_exist(file_name):
+        click.echo("Selected context does not exist.")
         click.echo("To get all available contexts use:")
         click.echo("cgc context list")
         exit(0)
         # user_id = input("User ID: ")
         # access_key = input("Access key: ")
         # ctx.invoke(
         #     auth_register,
```

### Comparing `cgcsdk-0.8.6/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.7/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/cgc_helpers.py` & `cgcsdk-0.8.7/cgc/commands/cgc_helpers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.7/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.7/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.7/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.7/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/db/db_cmd.py` & `cgcsdk-0.8.7/cgc/commands/db/db_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/resource/resource_cmd.py` & `cgcsdk-0.8.7/cgc/commands/resource/resource_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.7/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.8.7/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.7/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.7/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/sdk/handlers.py` & `cgcsdk-0.8.7/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/sdk/mongodb.py` & `cgcsdk-0.8.7/cgc/sdk/mongodb.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/sdk/postgresql.py` & `cgcsdk-0.8.7/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/sdk/redis.py` & `cgcsdk-0.8.7/cgc/sdk/redis.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/server.crt` & `cgcsdk-0.8.7/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/telemetry/basic.py` & `cgcsdk-0.8.7/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/tests/__init__.py` & `cgcsdk-0.8.7/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.7/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.7/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.7/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.7/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/tests/responses_tests.py` & `cgcsdk-0.8.7/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/__init__.py` & `cgcsdk-0.8.7/cgc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/click_group.py` & `cgcsdk-0.8.7/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/config_utils.py` & `cgcsdk-0.8.7/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.7/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.7/cgc/utils/consts/message_consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+CONFIG_FILE_NOT_FOUND = (
+    "Config file not found. Please register with CGC or verify user context."
+)
 UNKNOWN_ERROR = "An unknown error occurred. Please try again or contact support at support@comtegra.pl."
 TIMEOUT_ERROR = (
     "Connection timed out. Try again or contact support at support@comtegra.pl"
 )
 CONNECTION_ERROR = "Error connecting to the server. Try again or contact support at support@comtegra.pl"
 CERTIFICATE_ERROR = " Could not find a suitable TLS CA certificate bundle, invalid path to server certificate."
```

### Comparing `cgcsdk-0.8.6/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.7/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.7/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.7/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.7/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/message_utils.py` & `cgcsdk-0.8.7/cgc/utils/message_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import click
+
 from colorama import Fore, Style
 from functools import wraps
 
 from cgc.commands.exceptions import ResponseException
 from cgc.telemetry.basic import increment_metric
-from cgc.utils.consts.message_consts import UNKNOWN_ERROR
+from cgc.utils.consts.message_consts import UNKNOWN_ERROR, CONFIG_FILE_NOT_FOUND
+from cgc.commands.auth import NoConfigFileFound
 
 
 def prepare_error_message(message: str) -> str:
     """Prepare error message for CLI.
 
     :param message: error message.
     :type message: str
@@ -42,14 +45,17 @@
     :rtype: _type_
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
+        except NoConfigFileFound as err:
+            click.echo(prepare_warning_message(CONFIG_FILE_NOT_FOUND))
+            exit(1)
         except (TypeError, KeyError, IndexError) as err:
             print(args, "\n", kwargs)
             increment_metric("client.parser", True)
             if "debug" in kwargs:
                 raise err
             return prepare_error_message(UNKNOWN_ERROR)
         except ResponseException as err:
```

### Comparing `cgcsdk-0.8.6/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.7/cgc/utils/prepare_headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from cgc.utils.config_utils import read_from_cfg
 from cgc.utils.consts.env_consts import API_URL, CGC_SECRET
 from cgc.commands.auth import auth_utils
+from cgc.utils.message_utils import key_error_decorator_for_helpers
 
 
 def load_user_api_keys():
     """Based on configuration getter creates pair of API keys
 
     :return: api_key and api_secret
     :rtype: list of strings
     """
     return read_from_cfg("api_key"), read_from_cfg("api_secret")
 
 
+@key_error_decorator_for_helpers
 def get_api_url_and_prepare_headers():
     """Loads API_URL and user api keys into single function. Ment to be used as single point of truth for all andpoints except register - due to different Content-Type header
 
     :return: API_URL and headers
     :rtype: string and dict
     """
     api_key, api_secret = load_user_api_keys()
@@ -49,14 +51,15 @@
     headers = {
         "accept": "application/json",
         "Content-Type": "application/x-www-form-urlencoded",
     }
     return url, headers
 
 
+@key_error_decorator_for_helpers
 def prepare_headers_api_key():
     """Prepares headers for create API key request.
 
     :return: headers in a for of dictionary
     :rtype: dict
     """
     headers = {
```

### Comparing `cgcsdk-0.8.6/cgc/utils/requests_helper.py` & `cgcsdk-0.8.7/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/response_utils.py` & `cgcsdk-0.8.7/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgc/utils/version_control.py` & `cgcsdk-0.8.7/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.7/cgcsdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.6
+Version: 0.8.7
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.6/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.7/cgcsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.6/setup.py` & `cgcsdk-0.8.7/setup.py`

 * *Files identical despite different names*

