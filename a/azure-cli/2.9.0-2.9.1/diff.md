# Comparing `tmp/azure-cli-2.9.0.tar.gz` & `tmp/azure-cli-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vsts/work/1/a/azure-cli-2.9.0.tar", last modified: Fri Jul 10 07:14:00 2020, max compression
+gzip compressed data, was "/home/vsts/work/1/a/azure-cli-2.9.1.tar", last modified: Thu Jul 16 08:10:05 2020, max compression
```

## Comparing `azure-cli-2.9.0.tar` & `azure-cli-2.9.1.tar`

### file list

```diff
@@ -1,771 +1,771 @@
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/
--rw-r--r--   0 vsts      (1001) docker     (118)    88744 2020-07-10 07:13:51.000000 azure-cli-2.9.0/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     1109 2020-07-10 07:13:51.000000 azure-cli-2.9.0/LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (118)       87 2020-07-10 07:13:51.000000 azure-cli-2.9.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (118)   113303 2020-07-10 07:14:00.000000 azure-cli-2.9.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)     3200 2020-07-10 07:13:51.000000 azure-cli-2.9.0/README.rst
--rw-r--r--   0 vsts      (1001) docker     (118)      465 2020-07-10 07:13:51.000000 azure-cli-2.9.0/az
--rw-r--r--   0 vsts      (1001) docker     (118)      194 2020-07-10 07:13:51.000000 azure-cli-2.9.0/az.bat
--rw-r--r--   0 vsts      (1001) docker     (118)      168 2020-07-10 07:13:51.000000 azure-cli-2.9.0/az.completion.sh
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/
--rw-r--r--   0 vsts      (1001) docker     (118)      408 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/
--rw-r--r--   0 vsts      (1001) docker     (118)      613 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2219 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/
--rw-r--r--   0 vsts      (1001) docker     (118)     1156 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3953 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_agentpool_polling.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9202 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_archive_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1098 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_azure_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2159 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2768 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)    27477 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_docker_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4563 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_errors.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14484 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    53019 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    33700 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3787 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_run_polling.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8730 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_stream_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17876 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4325 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4771 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/agentpool.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6207 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/build.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12819 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/check_health.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14992 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1386 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/credential.py
--rw-r--r--   0 vsts      (1001) docker     (118)    25225 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14913 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/helm.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6878 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/import.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4130 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/network_rule.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1378 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/notary.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4267 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/pack.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3730 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/policy.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3837 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/private_endpoint_connection.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4163 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/replication.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17497 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/repository.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4239 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/run.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4853 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/scope_map.py
--rw-r--r--   0 vsts      (1001) docker     (118)    40546 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/task.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2396 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/taskrun.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10917 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/token.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5366 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acr/webhook.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/
--rw-r--r--   0 vsts      (1001) docker     (118)     1455 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4581 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3765 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)      461 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_consts.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6299 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    53356 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3881 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5536 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_loadbalancer.py
--rw-r--r--   0 vsts      (1001) docker     (118)    24350 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15266 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7234 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/acs_client.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7564 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   159622 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2637 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/proxy.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3185 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/acs/win_proxy.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/
--rw-r--r--   0 vsts      (1001) docker     (118)     1381 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      960 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2108 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3244 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1109 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1838 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5853 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/advisor/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/
--rw-r--r--   0 vsts      (1001) docker     (118)     1272 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2851 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2573 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)      718 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)      529 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19463 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    47379 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1717 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_sdk_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)      542 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_test_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4125 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4610 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15813 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/commands.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3815 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/account.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5433 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/account_filter.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2253 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/asset.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5432 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/asset_filter.py
--rw-r--r--   0 vsts      (1001) docker     (118)    25897 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/content_key_policy.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2588 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/job.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8332 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/live_event.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1913 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/live_output.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5711 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/mru.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14588 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/sp.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9878 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/streaming_endpoint.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3380 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/streaming_locator.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15081 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/streaming_policy.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6104 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/ams/operations/transform.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/
--rw-r--r--   0 vsts      (1001) docker     (118)     1459 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      719 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2436 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5089 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8839 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2305 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7941 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/apim/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/
--rw-r--r--   0 vsts      (1001) docker     (118)     1595 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/
--rw-r--r--   0 vsts      (1001) docker     (118)      411 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    24893 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/azconfig_client.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2055 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2811 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2916 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/execution_context.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2863 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/http_logger.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2392 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/keyvalue_iterable.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1242 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/mapper.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6120 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/models.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2880 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/request_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)      580 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/request_message.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5347 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1141 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      795 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10980 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_featuremodels.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5244 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    22382 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    39901 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_kv_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    22244 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4560 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8849 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5022 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10547 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)    39654 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/feature.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28203 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appconfig/keyvalue.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/
--rw-r--r--   0 vsts      (1001) docker     (118)     1460 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1179 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_appservice_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2421 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1004 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3617 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16576 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_create_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)    86023 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    71223 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8229 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7451 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/access_restrictions.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20458 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/appservice_environment.py
--rw-r--r--   0 vsts      (1001) docker     (118)    46724 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/azure_devops_build_interactive.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18624 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/azure_devops_build_provider.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23560 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   183730 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/resources/
--rw-r--r--   0 vsts      (1001) docker     (118)     9926 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/resources/LinuxFunctionsStacks.json
--rw-r--r--   0 vsts      (1001) docker     (118)     9774 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/resources/WindowsFunctionsStacks.json
--rw-r--r--   0 vsts      (1001) docker     (118)    13311 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/static_sites.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9509 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/tunnel.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2002 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3009 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/appservice/vsts_cd_provider.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/
--rw-r--r--   0 vsts      (1001) docker     (118)     1501 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2343 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_aad.py
--rw-r--r--   0 vsts      (1001) docker     (118)      637 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      967 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2770 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4829 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1960 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_rbac.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8369 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1505 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5544 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/aro/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/
--rw-r--r--   0 vsts      (1001) docker     (118)     1423 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4388 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4859 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23749 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23092 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      859 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7370 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    47334 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16482 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/custom_afs.py
--rw-r--r--   0 vsts      (1001) docker     (118)    24168 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/custom_base.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6103 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/custom_common.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14108 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/custom_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28648 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/backup/custom_wl.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/
--rw-r--r--   0 vsts      (1001) docker     (118)     1885 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3553 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    38293 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_command_type.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1475 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1198 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10807 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9966 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3578 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_parameter_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16118 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14395 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8737 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18746 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batch/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/
--rw-r--r--   0 vsts      (1001) docker     (118)     1435 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1169 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5809 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18748 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19546 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6084 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    55326 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/batchai/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/
--rw-r--r--   0 vsts      (1001) docker     (118)     1372 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      929 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      672 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)      859 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1137 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2108 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)      725 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/billing/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/
--rw-r--r--   0 vsts      (1001) docker     (118)     2238 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1020 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1308 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9375 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17339 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11859 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/bot_json_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6036 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/bot_publish_prep.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7193 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/bot_template_deployer.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9694 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/channel_operations.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3853 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)      416 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)    33844 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)      757 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/http_response_validator.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14580 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/kudu_client.py
--rw-r--r--   0 vsts      (1001) docker     (118)      708 2020-07-10 07:13:51.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/name_availability.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2532 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/typescript.web.config
--rw-r--r--   0 vsts      (1001) docker     (118)     2505 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/web.config
--rw-r--r--   0 vsts      (1001) docker     (118)     3667 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/web_app_operations.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6401 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/botservice/webappv4.template.json
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/
--rw-r--r--   0 vsts      (1001) docker     (118)     1501 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5181 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/_actions.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1185 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    26436 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14131 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1138 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9943 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    42484 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cdn/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/cloud/
--rw-r--r--   0 vsts      (1001) docker     (118)     4692 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cloud/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      864 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cloud/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1745 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cloud/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6665 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cloud/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/
--rw-r--r--   0 vsts      (1001) docker     (118)     1656 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      854 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11021 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6650 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2150 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9057 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/
--rw-r--r--   0 vsts      (1001) docker     (118)     1036 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2986 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/_consts.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2540 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2486 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      783 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1087 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1414 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12695 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/configure/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/
--rw-r--r--   0 vsts      (1001) docker     (118)     1415 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1308 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      680 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2965 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4694 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3630 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/_transformers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2037 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3867 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6259 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/consumption/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/container/
--rw-r--r--   0 vsts      (1001) docker     (118)     1446 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2371 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3142 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6452 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9657 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4156 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1723 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    36610 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/container/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/
--rw-r--r--   0 vsts      (1001) docker     (118)     2124 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3636 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3158 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_command_type.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3673 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1901 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    29383 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23809 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2616 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2621 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/actions.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15392 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    62399 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/
--rw-r--r--   0 vsts      (1001) docker     (118)     1557 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1226 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    13067 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12293 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4798 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12978 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/
--rw-r--r--   0 vsts      (1001) docker     (118)     1504 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4174 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    13053 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8397 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2782 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8282 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14630 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dla/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/
--rw-r--r--   0 vsts      (1001) docker     (118)     1480 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2112 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14673 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9334 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2644 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4671 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12482 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dls/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/
--rw-r--r--   0 vsts      (1001) docker     (118)     1552 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      934 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12392 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1610 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3632 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9506 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/dms/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/
--rw-r--r--   0 vsts      (1001) docker     (118)     1448 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1832 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    71339 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    29653 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5017 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/advanced_filter.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9873 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    64427 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5031 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/event_channel_filter.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1078 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventgrid/inbound_ip_rules.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/
--rw-r--r--   0 vsts      (1001) docker     (118)     1890 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      985 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1341 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19300 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16357 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      754 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3069 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_validator.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6203 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12590 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/eventhubs/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/extension/
--rw-r--r--   0 vsts      (1001) docker     (118)     4302 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/extension/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      842 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/extension/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2852 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/extension/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1619 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/extension/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/feedback/
--rw-r--r--   0 vsts      (1001) docker     (118)     1187 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/feedback/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      572 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/feedback/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    29075 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/feedback/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/find/
--rw-r--r--   0 vsts      (1001) docker     (118)     1798 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/find/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1151 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/find/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)      523 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/find/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      516 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/find/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4990 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/find/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/
--rw-r--r--   0 vsts      (1001) docker     (118)     1290 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3362 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3695 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7927 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16665 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5824 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5102 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    21234 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7074 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/hdinsight/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/interactive/
--rw-r--r--   0 vsts      (1001) docker     (118)     2155 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/interactive/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1810 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/interactive/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/
--rw-r--r--   0 vsts      (1001) docker     (118)     2281 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2123 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      656 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)    38741 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20745 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2549 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3574 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10474 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    66435 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/
--rw-r--r--   0 vsts      (1001) docker     (118)      887 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    24286 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/digital_twin_repository_provisioning_service.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/
--rw-r--r--   0 vsts      (1001) docker     (118)     1478 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2984 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/key_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1173 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1319 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request_properties.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1512 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1946 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata_properties.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1717 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_provision_response_base.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1207 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1265 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request_properties.py
--rw-r--r--   0 vsts      (1001) docker     (118)      695 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/version.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2251 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/sas_token_auth.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1888 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iot/shared.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/
--rw-r--r--   0 vsts      (1001) docker     (118)     1485 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      848 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2720 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1932 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1502 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3399 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/iotcentral/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/
--rw-r--r--   0 vsts      (1001) docker     (118)     2058 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2747 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8535 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_command_type.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2359 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18339 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28507 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1396 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_transformers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14725 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    13809 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    61625 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/keyvault/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/
--rw-r--r--   0 vsts      (1001) docker     (118)     1400 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1040 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4079 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1902 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      617 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2130 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6008 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/kusto/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/
--rw-r--r--   0 vsts      (1001) docker     (118)     1364 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2016 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2353 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    13079 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3527 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7252 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6000 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28337 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/lab/validators.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/
--rw-r--r--   0 vsts      (1001) docker     (118)     1440 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      844 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6658 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1527 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1743 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6197 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/managedservices/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/
--rw-r--r--   0 vsts      (1001) docker     (118)     1512 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      640 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2919 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2173 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1294 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3092 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/maps/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/
--rw-r--r--   0 vsts      (1001) docker     (118)     3138 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16751 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/_autoscale_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4209 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2802 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)    75912 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    33538 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19136 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/actions.py
--rw-r--r--   0 vsts      (1001) docker     (118)    27727 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5434 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/
--rw-r--r--   0 vsts      (1001) docker     (118)     9203 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionLexer.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4367 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionListener.py
--rw-r--r--   0 vsts      (1001) docker     (118)    38487 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionParser.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3715 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionValidator.py
--rw-r--r--   0 vsts      (1001) docker     (118)      654 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/
--rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3208 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/action_groups.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10499 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/activity_log_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1253 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/autoscale-parameters-template.json
--rw-r--r--   0 vsts      (1001) docker     (118)    16209 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/autoscale_settings.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1715 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/diagnostics_settings.py
--rw-r--r--   0 vsts      (1001) docker     (118)      789 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/general_operations.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2153 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_cluster.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2271 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_linked_storage_account.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8370 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_workspace.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1356 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_workspace_linked_service.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1059 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_profiles.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9763 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/metric_alert.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6147 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/monitor_clone_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6455 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/private_link_scope.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2435 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/subscription_diagnostic_settings.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3805 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/transformers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2654 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/util.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16460 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/monitor/validators.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/
--rw-r--r--   0 vsts      (1001) docker     (118)     1355 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      698 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2174 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1355 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1908 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1034 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2310 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/natgateway/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/
--rw-r--r--   0 vsts      (1001) docker     (118)     1617 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1108 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      742 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)    22466 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5227 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8166 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9547 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/netappfiles/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/network/
--rw-r--r--   0 vsts      (1001) docker     (118)     2294 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1495 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_actions.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8634 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3858 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10794 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)   244461 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)   153343 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15442 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_template_builder.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2924 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)    81755 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    73333 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   318797 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5123 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/
--rw-r--r--   0 vsts      (1001) docker     (118)    10814 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3373 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/batch_provider.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4380 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/keyvault_provider.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/
--rw-r--r--   0 vsts      (1001) docker     (118)     1651 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3960 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/make_zone_file.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17213 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/parse_zone_file.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4615 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/record_processors.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/
--rw-r--r--   0 vsts      (1001) docker     (118)     1513 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1259 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1627 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)      735 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15045 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7369 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1187 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2897 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17872 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/policyinsights/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/
--rw-r--r--   0 vsts      (1001) docker     (118)     1957 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1195 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3198 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    26418 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6644 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2022 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6557 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28221 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/privatedns/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/profile/
--rw-r--r--   0 vsts      (1001) docker     (118)     5371 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/profile/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      792 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/profile/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3888 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/profile/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1517 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/profile/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9867 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/profile/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/
--rw-r--r--   0 vsts      (1001) docker     (118)     1764 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7533 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    44241 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16425 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1658 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)    22110 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    25660 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4455 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/rdbms/validators.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/
--rw-r--r--   0 vsts      (1001) docker     (118)     1538 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1339 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3081 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4624 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1377 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2788 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6251 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/redis/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/
--rw-r--r--   0 vsts      (1001) docker     (118)     1373 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      848 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1271 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    15481 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9831 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      751 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)      435 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4784 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4737 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/relay/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/
--rw-r--r--   0 vsts      (1001) docker     (118)     1834 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      947 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      657 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6277 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5661 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2528 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4211 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/reservations/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/
--rw-r--r--   0 vsts      (1001) docker     (118)     1887 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4517 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2041 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_color.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1946 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)      729 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_exception_handler.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19292 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_formatters.py
--rw-r--r--   0 vsts      (1001) docker     (118)    79088 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    36582 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      679 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_symbol.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2280 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8901 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2439 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/_win_vt.py
--rw-r--r--   0 vsts      (1001) docker     (118)    26347 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   134313 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/resource/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/role/
--rw-r--r--   0 vsts      (1001) docker     (118)     1474 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1952 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      703 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    26017 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4155 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/_multi_api_adaptor.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16828 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4496 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10506 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    80774 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/role/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/search/
--rw-r--r--   0 vsts      (1001) docker     (118)     1461 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/search/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      819 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/search/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1001 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/search/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1453 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/search/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2060 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/search/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2674 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/search/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/security/
--rw-r--r--   0 vsts      (1001) docker     (118)     1215 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3822 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    26220 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14526 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1302 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18057 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    23555 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/security/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/
--rw-r--r--   0 vsts      (1001) docker     (118)     1896 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1269 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2220 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28140 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    25440 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      756 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6238 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7909 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    24186 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicebus/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/
--rw-r--r--   0 vsts      (1001) docker     (118)     1474 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2976 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_arm_deployment_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2691 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14934 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    18924 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5675 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4680 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   105103 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/operations/
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16825 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/operations/applications.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/linux/
--rw-r--r--   0 vsts      (1001) docker     (118)     1952 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/linux/parameter.json
--rw-r--r--   0 vsts      (1001) docker     (118)    34670 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/linux/template.json
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/service/
--rw-r--r--   0 vsts      (1001) docker     (118)      358 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/service/parameter.json
--rw-r--r--   0 vsts      (1001) docker     (118)     1916 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/service/template.json
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/windows/
--rw-r--r--   0 vsts      (1001) docker     (118)     1952 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/windows/parameter.json
--rw-r--r--   0 vsts      (1001) docker     (118)    32521 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/windows/template.json
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/
--rw-r--r--   0 vsts      (1001) docker     (118)     1108 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1277 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/_actions.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1014 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      515 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6042 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4971 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2744 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1653 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/cors.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2854 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)      806 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/key.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1288 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/network.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1156 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/signalr/upstream.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/
--rw-r--r--   0 vsts      (1001) docker     (118)     1376 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11258 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)    47943 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    77013 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6741 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5372 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    33780 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   114203 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sql/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/
--rw-r--r--   0 vsts      (1001) docker     (118)     1864 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    14035 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8140 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16589 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1286 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4612 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4676 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    24428 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/sqlvm/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/
--rw-r--r--   0 vsts      (1001) docker     (118)    19486 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11981 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11981 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_client_factory_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5199 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)   101791 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    87978 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    83426 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_params_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8899 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_transformers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8947 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_transformers_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)    58287 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    58287 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/_validators_azure_stack.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/azcopy/
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/azcopy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     8987 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/azcopy/util.py
--rw-r--r--   0 vsts      (1001) docker     (118)    45815 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)    39113 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/commands_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3545 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2443 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/oauth_token_util.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    30976 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/account.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4447 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/acl.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7514 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/azcopy.py
--rw-r--r--   0 vsts      (1001) docker     (118)    32366 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/blob.py
--rw-r--r--   0 vsts      (1001) docker     (118)    32366 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/blob_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)      799 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/cors.py
--rw-r--r--   0 vsts      (1001) docker     (118)      688 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/directory.py
--rw-r--r--   0 vsts      (1001) docker     (118)      688 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/directory_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16722 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/file.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16722 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/file_azure_stack.py
--rw-r--r--   0 vsts      (1001) docker     (118)      961 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1613 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/fs_directory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5807 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/fs_file.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1627 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/logging.py
--rw-r--r--   0 vsts      (1001) docker     (118)      687 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (118)      851 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/operations/table.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3304 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/sdkutil.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4408 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/services_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2719 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/storage_url_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1784 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/track2_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2058 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/url_quote_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9455 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/storage/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/util/
--rw-r--r--   0 vsts      (1001) docker     (118)     1194 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2445 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/util/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2602 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/util/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)      556 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/util/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1273 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/util/custom.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/
--rw-r--r--   0 vsts      (1001) docker     (118)     1554 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9845 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_actions.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2994 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_alias.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5181 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_client_factory.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1524 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_completers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6367 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_format.py
--rw-r--r--   0 vsts      (1001) docker     (118)   108073 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    31895 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_image_builder.py
--rw-r--r--   0 vsts      (1001) docker     (118)    83262 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_params.py
--rw-r--r--   0 vsts      (1001) docker     (118)    38674 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_template_builder.py
--rw-r--r--   0 vsts      (1001) docker     (118)    86784 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    49704 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_vm_diagnostics_templates.py
--rw-r--r--   0 vsts      (1001) docker     (118)    13788 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_vm_utils.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6273 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/_workspace_data_source_settings.py
--rw-r--r--   0 vsts      (1001) docker     (118)    29168 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)   172606 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/custom.py
--rw-r--r--   0 vsts      (1001) docker     (118)    27146 2020-07-10 07:13:52.000000 azure-cli-2.9.0/azure/cli/command_modules/vm/disk_encryption.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2358 2020-07-10 07:13:53.000000 azure-cli-2.9.0/azure_bdist_wheel.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure_cli.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (118)   113303 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure_cli.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)    34097 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure_cli.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure_cli.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-10 07:13:59.000000 azure-cli-2.9.0/azure_cli.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (118)     2400 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure_cli.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        6 2020-07-10 07:14:00.000000 azure-cli-2.9.0/azure_cli.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (118)       95 2020-07-10 07:14:00.000000 azure-cli-2.9.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (118)     6389 2020-07-10 07:13:53.000000 azure-cli-2.9.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/
+-rw-r--r--   0 vsts      (1001) docker     (118)    89114 2020-07-16 08:09:55.000000 azure-cli-2.9.1/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     1109 2020-07-16 08:09:55.000000 azure-cli-2.9.1/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)       87 2020-07-16 08:09:55.000000 azure-cli-2.9.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (118)   113825 2020-07-16 08:10:05.000000 azure-cli-2.9.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     3200 2020-07-16 08:09:55.000000 azure-cli-2.9.1/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)      465 2020-07-16 08:09:55.000000 azure-cli-2.9.1/az
+-rw-r--r--   0 vsts      (1001) docker     (118)      194 2020-07-16 08:09:55.000000 azure-cli-2.9.1/az.bat
+-rw-r--r--   0 vsts      (1001) docker     (118)      168 2020-07-16 08:09:55.000000 azure-cli-2.9.1/az.completion.sh
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/
+-rw-r--r--   0 vsts      (1001) docker     (118)      408 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/
+-rw-r--r--   0 vsts      (1001) docker     (118)      613 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2219 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1156 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3953 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_agentpool_polling.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9202 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_archive_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1098 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_azure_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2159 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2768 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    27477 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_docker_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4563 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_errors.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14484 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    53019 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    33700 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3787 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_run_polling.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8730 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_stream_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17876 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4325 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4771 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/agentpool.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6207 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/build.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12918 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/check_health.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14992 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1386 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/credential.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    25407 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14913 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/helm.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6878 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/import.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4130 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/network_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1378 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/notary.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4267 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/pack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3730 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/policy.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3837 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/private_endpoint_connection.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4163 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/replication.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17497 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/repository.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4239 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/run.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4853 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/scope_map.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    40546 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/task.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2396 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/taskrun.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10917 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/token.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5366 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acr/webhook.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1455 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4581 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3765 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      461 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_consts.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6299 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    53319 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3881 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5536 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_loadbalancer.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    24350 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15266 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7234 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/acs_client.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7564 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   159622 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2637 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/proxy.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3185 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/acs/win_proxy.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1381 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      960 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2108 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3244 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1109 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1838 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5853 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/advisor/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1272 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2851 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2573 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      718 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      529 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19463 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    47379 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1717 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_sdk_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      542 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_test_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4125 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4610 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15813 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/commands.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/
+-rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3815 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/account.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5433 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/account_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2253 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/asset.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5432 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/asset_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    25897 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/content_key_policy.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2588 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/job.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8332 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/live_event.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1913 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/live_output.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5711 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/mru.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14588 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/sp.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9878 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/streaming_endpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3380 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/streaming_locator.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15081 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/streaming_policy.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6104 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/ams/operations/transform.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1459 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      719 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2436 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5089 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8839 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2305 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7941 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/apim/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1595 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/
+-rw-r--r--   0 vsts      (1001) docker     (118)      411 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    24893 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/azconfig_client.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2055 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2811 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2916 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/execution_context.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2863 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/http_logger.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2392 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/keyvalue_iterable.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1242 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/mapper.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6120 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/models.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2880 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/request_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      580 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/request_message.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5347 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1141 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      795 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10980 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_featuremodels.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5244 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    22382 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    39901 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_kv_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    22244 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4560 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8849 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5022 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10547 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    39654 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/feature.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28203 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appconfig/keyvalue.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1460 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1179 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_appservice_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2421 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1004 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3617 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16576 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_create_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    86023 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    71223 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8229 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7451 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/access_restrictions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    20458 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/appservice_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    46724 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/azure_devops_build_interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18624 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/azure_devops_build_provider.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23560 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   183730 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/resources/
+-rw-r--r--   0 vsts      (1001) docker     (118)     9926 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/resources/LinuxFunctionsStacks.json
+-rw-r--r--   0 vsts      (1001) docker     (118)     9774 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/resources/WindowsFunctionsStacks.json
+-rw-r--r--   0 vsts      (1001) docker     (118)    13311 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/static_sites.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9509 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/tunnel.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2002 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3009 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/appservice/vsts_cd_provider.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1501 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2343 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_aad.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      637 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      967 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2770 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4829 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1960 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_rbac.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8369 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1505 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5544 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/aro/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1423 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4388 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4859 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23749 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23092 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      859 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7370 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    47334 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16482 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/custom_afs.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    24168 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/custom_base.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6103 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/custom_common.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14108 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/custom_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28648 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/backup/custom_wl.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1885 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3553 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    38293 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_command_type.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1475 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1198 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10807 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9966 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3578 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_parameter_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16118 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14395 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8737 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18746 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batch/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1435 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1169 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5809 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18748 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19546 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6084 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    55326 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/batchai/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1372 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      929 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      672 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      859 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1137 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2108 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      725 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/billing/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2238 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1020 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1308 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9375 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17339 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    11859 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/bot_json_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6036 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/bot_publish_prep.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7193 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/bot_template_deployer.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9694 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/channel_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3853 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      416 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    33844 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      757 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/http_response_validator.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14580 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/kudu_client.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      708 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/name_availability.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2532 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/typescript.web.config
+-rw-r--r--   0 vsts      (1001) docker     (118)     2505 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/web.config
+-rw-r--r--   0 vsts      (1001) docker     (118)     3667 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/web_app_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6401 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/botservice/webappv4.template.json
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1501 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5181 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/_actions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1185 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26436 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14131 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1138 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9943 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    42484 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cdn/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/cloud/
+-rw-r--r--   0 vsts      (1001) docker     (118)     4692 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cloud/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      864 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cloud/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1745 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cloud/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6665 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cloud/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1656 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      854 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    11021 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6650 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2150 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9057 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1036 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2986 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/_consts.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2540 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2486 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      783 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1087 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1414 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12695 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/configure/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1415 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1308 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      680 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2965 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4694 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3630 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/_transformers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2037 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3867 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6259 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/consumption/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/container/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1446 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2371 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3142 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6452 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9657 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4156 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1723 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    36610 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/container/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2124 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3636 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3158 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_command_type.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3673 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1901 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    29383 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23809 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2616 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2621 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15392 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    62399 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1557 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1226 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    13067 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12293 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4798 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12978 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1504 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4174 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    13053 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8397 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2782 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8282 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14630 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dla/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1480 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2112 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14673 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9334 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2644 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4671 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12482 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dls/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1552 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      934 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12392 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1610 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3632 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9506 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/dms/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1448 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1832 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    71339 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    29653 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5017 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/advanced_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9873 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    64427 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5031 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/event_channel_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1078 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventgrid/inbound_ip_rules.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1890 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      985 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1341 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19300 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16357 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      754 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3069 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_validator.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6203 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    12590 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/eventhubs/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/extension/
+-rw-r--r--   0 vsts      (1001) docker     (118)     4302 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/extension/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      842 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/extension/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2852 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/extension/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1619 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/extension/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/feedback/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1187 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/feedback/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      572 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/feedback/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    29075 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/feedback/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/find/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1798 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/find/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1151 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/find/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      523 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/find/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      516 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/find/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4990 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/find/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1290 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3362 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3695 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7927 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16665 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5824 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5102 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    21234 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7074 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/hdinsight/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/interactive/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2155 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/interactive/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1810 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/interactive/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2281 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1367 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      527 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    35523 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19595 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2168 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3574 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9541 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    62598 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/
+-rw-r--r--   0 vsts      (1001) docker     (118)      887 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    24286 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/digital_twin_repository_provisioning_service.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1478 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2984 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/key_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1173 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1319 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1512 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1946 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1717 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_provision_response_base.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1207 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1265 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      695 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/version.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2251 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/sas_token_auth.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1683 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iot/shared.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1485 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      848 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2720 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1932 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1502 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3399 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/iotcentral/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2058 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2747 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8535 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_command_type.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2359 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18339 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28507 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1396 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_transformers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14725 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    13809 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    61625 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/keyvault/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1400 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1040 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4079 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1902 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      617 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2130 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6008 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/kusto/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1364 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2016 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2353 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    13079 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3527 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7252 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6000 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28337 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/lab/validators.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1440 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      844 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6658 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1527 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1743 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6197 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/managedservices/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1512 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      640 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2919 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2173 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1294 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3092 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/maps/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/
+-rw-r--r--   0 vsts      (1001) docker     (118)     3138 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16751 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/_autoscale_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4209 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2802 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    75912 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    33538 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19136 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    27727 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5434 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/
+-rw-r--r--   0 vsts      (1001) docker     (118)     9202 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionLexer.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4366 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionListener.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    38646 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionParser.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3715 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionValidator.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      654 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3208 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/action_groups.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10499 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/activity_log_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1253 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/autoscale-parameters-template.json
+-rw-r--r--   0 vsts      (1001) docker     (118)    16209 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/autoscale_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1715 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/diagnostics_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      789 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/general_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2153 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_cluster.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2271 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_linked_storage_account.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8370 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_workspace.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1356 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_workspace_linked_service.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1059 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_profiles.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9763 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/metric_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6147 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/monitor_clone_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6455 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/private_link_scope.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2435 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/subscription_diagnostic_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3805 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/transformers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2654 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16460 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/monitor/validators.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1355 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      698 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2174 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1355 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1908 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1034 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2310 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/natgateway/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1617 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1108 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      742 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    22466 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5227 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8166 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9547 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/netappfiles/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/network/
+-rw-r--r--   0 vsts      (1001) docker     (118)     2294 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1495 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_actions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8634 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3858 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10794 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   244461 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   153343 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15442 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_template_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2924 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    81755 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    73333 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   319035 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/
+-rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5123 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/
+-rw-r--r--   0 vsts      (1001) docker     (118)    10814 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3373 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/batch_provider.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4380 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/keyvault_provider.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1651 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3960 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/make_zone_file.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17213 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/parse_zone_file.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4615 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/record_processors.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1513 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1259 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1627 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      735 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15045 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7369 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1187 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2897 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    17872 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/policyinsights/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1957 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1195 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3198 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26418 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6644 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2022 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6557 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28221 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/privatedns/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/profile/
+-rw-r--r--   0 vsts      (1001) docker     (118)     5371 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/profile/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      792 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/profile/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3888 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/profile/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1517 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/profile/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9867 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/profile/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1764 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7533 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    44241 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16425 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1658 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    22110 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    25660 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4455 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/rdbms/validators.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1538 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1339 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3081 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4624 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1377 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2788 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6251 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/redis/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1373 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      848 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1271 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    15481 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9831 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      751 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      435 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4784 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4737 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/relay/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1834 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      947 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      657 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6277 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5661 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2528 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4211 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/reservations/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1887 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4517 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2041 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_color.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1946 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      729 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_exception_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    19292 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_formatters.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    79088 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    36582 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      679 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_symbol.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2280 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8901 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2439 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/_win_vt.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26347 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   134313 2020-07-16 08:09:55.000000 azure-cli-2.9.1/azure/cli/command_modules/resource/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/role/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1474 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1952 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      703 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26017 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4155 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/_multi_api_adaptor.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16828 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4496 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    10506 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    80774 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/role/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/search/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1461 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/search/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      819 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/search/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1001 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/search/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1453 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/search/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2060 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/search/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2674 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/search/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/security/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1215 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3822 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26220 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14526 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1302 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18057 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    23555 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/security/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1896 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1269 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2220 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    28140 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    25440 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      756 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6238 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7909 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    24186 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicebus/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1474 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2976 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_arm_deployment_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2691 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14934 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18924 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5675 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4680 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   105103 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/operations/
+-rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16825 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/operations/applications.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/linux/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1952 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/linux/parameter.json
+-rw-r--r--   0 vsts      (1001) docker     (118)    34670 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/linux/template.json
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/service/
+-rw-r--r--   0 vsts      (1001) docker     (118)      358 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/service/parameter.json
+-rw-r--r--   0 vsts      (1001) docker     (118)     1916 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/service/template.json
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/windows/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1952 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/windows/parameter.json
+-rw-r--r--   0 vsts      (1001) docker     (118)    32521 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/windows/template.json
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1108 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1277 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/_actions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1014 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      515 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6042 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4971 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2744 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1653 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/cors.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2854 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      806 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/key.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1288 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/network.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1156 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/signalr/upstream.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1376 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    11258 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    47943 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    77013 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6741 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5372 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    33780 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   114203 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sql/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1864 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    14035 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8140 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16589 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1286 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4612 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4676 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    24428 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/sqlvm/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/
+-rw-r--r--   0 vsts      (1001) docker     (118)    19471 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    11981 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    11981 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_client_factory_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5199 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   102896 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    87873 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    83426 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_params_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8899 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_transformers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8947 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_transformers_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    58287 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    58287 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/_validators_azure_stack.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/azcopy/
+-rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/azcopy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     8987 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/azcopy/util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    45815 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    39113 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/commands_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3545 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2459 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/oauth_token_util.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/
+-rw-r--r--   0 vsts      (1001) docker     (118)      345 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    30976 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/account.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4447 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/acl.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7514 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/azcopy.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    32366 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/blob.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    32366 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/blob_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      799 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/cors.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      688 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/directory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      688 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/directory_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16722 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/file.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    16722 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/file_azure_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      961 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1613 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/fs_directory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5807 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/fs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1627 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      687 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      851 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/operations/table.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     3304 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/sdkutil.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     4408 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/services_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2719 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/storage_url_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1784 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/track2_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2058 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/url_quote_util.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9455 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/storage/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/util/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1194 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2445 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/util/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2602 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/util/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      556 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/util/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1273 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/util/custom.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/
+-rw-r--r--   0 vsts      (1001) docker     (118)     1554 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     9845 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_actions.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2994 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_alias.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     5181 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_client_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     1524 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_completers.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6367 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_format.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   108073 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_help.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    31895 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_image_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    83263 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_params.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    38674 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_template_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    86784 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_validators.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    49704 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_vm_diagnostics_templates.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    13788 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_vm_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     6273 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/_workspace_data_source_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    29168 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (118)   172606 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/custom.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    27146 2020-07-16 08:09:56.000000 azure-cli-2.9.1/azure/cli/command_modules/vm/disk_encryption.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     2358 2020-07-16 08:09:57.000000 azure-cli-2.9.1/azure_bdist_wheel.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-07-16 08:10:05.000000 azure-cli-2.9.1/azure_cli.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (118)   113825 2020-07-16 08:10:03.000000 azure-cli-2.9.1/azure_cli.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)    34097 2020-07-16 08:10:04.000000 azure-cli-2.9.1/azure_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-16 08:10:04.000000 azure-cli-2.9.1/azure_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-07-16 08:10:02.000000 azure-cli-2.9.1/azure_cli.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (118)     2400 2020-07-16 08:10:04.000000 azure-cli-2.9.1/azure_cli.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        6 2020-07-16 08:10:04.000000 azure-cli-2.9.1/azure_cli.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)       95 2020-07-16 08:10:05.000000 azure-cli-2.9.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (118)     6389 2020-07-16 08:09:57.000000 azure-cli-2.9.1/setup.py
```

### Comparing `azure-cli-2.9.0/HISTORY.rst` & `azure-cli-2.9.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 .. :changelog:
 
 Release History
 ===============
 
+2.9.1
+++++++
+
+**AKS**
+
+* Remove explicit setting of VMSS in Windows example command since it is now default (#14324)
+
+**IoT**
+
+* [BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI (#14117)
+
+**REST**
+
+* Fix #14152: `az rest`: Accept ARM URLs without subscription ID (#14370)
+
+**Storage**
+
+* Fix #14138: Make some permissions optional (#14385)
+
 2.9.0
 ++++++
 
 **ACR**
 
 * Handle log artifact link from Registry to stream logs (#14038)
 * Deprecate helm2 commands (#14143)
```

### Comparing `azure-cli-2.9.0/LICENSE.txt` & `azure-cli-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/PKG-INFO` & `azure-cli-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-cli
-Version: 2.9.0
+Version: 2.9.1
 Summary: Microsoft Azure Command-Line Tools
 Home-page: https://github.com/Azure/azure-cli
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Description: Microsoft Azure CLI
         ===================
@@ -114,14 +114,33 @@
         
         
         .. :changelog:
         
         Release History
         ===============
         
+        2.9.1
+        ++++++
+        
+        **AKS**
+        
+        * Remove explicit setting of VMSS in Windows example command since it is now default (#14324)
+        
+        **IoT**
+        
+        * [BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI (#14117)
+        
+        **REST**
+        
+        * Fix #14152: `az rest`: Accept ARM URLs without subscription ID (#14370)
+        
+        **Storage**
+        
+        * Fix #14138: Make some permissions optional (#14385)
+        
         2.9.0
         ++++++
         
         **ACR**
         
         * Handle log artifact link from Registry to stream logs (#14038)
         * Deprecate helm2 commands (#14143)
```

### Comparing `azure-cli-2.9.0/README.rst` & `azure-cli-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/__init__.py` & `azure-cli-2.9.1/azure/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 This tools provides a command-line interface to Azure's management and storage
 APIs.
 '''
 import pkg_resources
 pkg_resources.declare_namespace(__name__)
 
 __author__ = "Microsoft Corporation <python@microsoft.com>"
-__version__ = "2.9.0"
+__version__ = "2.9.1"
```

### Comparing `azure-cli-2.9.0/azure/cli/__main__.py` & `azure-cli-2.9.1/azure/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_agentpool_polling.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_agentpool_polling.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_archive_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_archive_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_azure_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_azure_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_constants.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_docker_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_docker_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_errors.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_errors.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_run_polling.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_run_polling.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_stream_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_stream_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/agentpool.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/agentpool.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/build.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/build.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/check_health.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/check_health.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,16 @@
 def _get_registry_status(login_server, registry_name, ignore_errors):
     import socket
 
     registry_ip = None
 
     try:
         registry_ip = socket.gethostbyname(login_server)
-    except socket.gaierror:
+    except (socket.gaierror, UnicodeError):
+        # capture UnicodeError for https://github.com/Azure/azure-cli/issues/12936
         pass
 
     if not registry_ip:
         from ._errors import CONNECTIVITY_DNS_ERROR
         _handle_error(CONNECTIVITY_DNS_ERROR.format_error_message(login_server), ignore_errors)
         return False
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/credential.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/credential.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,16 @@
 
 def show_encryption(cmd, client, registry_name, resource_group_name=None):
     return acr_show(cmd, client, registry_name, resource_group_name).encryption
 
 
 def rotate_key(cmd, client, registry_name, identity=None, key_encryption_key=None, resource_group_name=None):
     registry, resource_group_name = get_registry_by_name(cmd.cli_ctx, registry_name, resource_group_name)
+    if not registry.encryption or not registry.encryption.key_vault_properties:
+        raise CLIError('usage error: key rotation is only applicable to registries with CMK enabled')
     if key_encryption_key:
         registry.encryption.key_vault_properties.key_identifier = key_encryption_key
     if identity:
         try:
             import uuid
             uuid.UUID(identity)
             client_id = identity
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/helm.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/helm.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/import.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/import.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/network_rule.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/network_rule.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/notary.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/notary.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/pack.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/pack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/policy.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/policy.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/private_endpoint_connection.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/private_endpoint_connection.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/replication.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/replication.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/repository.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/repository.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/run.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/run.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/scope_map.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/scope_map.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/task.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/task.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/taskrun.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/taskrun.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/token.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/token.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acr/webhook.py` & `azure-cli-2.9.1/azure/cli/command_modules/acr/webhook.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
   - name: Create a kubernetes cluster with authorized apiserver IP ranges.
     text: az aks create -g MyResourceGroup -n MyManagedCluster --api-server-authorized-ip-ranges 193.168.1.0/24,194.168.1.0/24,195.168.1.0
   - name: Create a kubernetes cluster which enables managed identity.
     text: az aks create -g MyResourceGroup -n MyManagedCluster --enable-managed-identity
   - name: Create a kubernetes cluster with userDefinedRouting, standard load balancer SKU and a custom subnet preconfigured with a route table
     text: az aks create -g MyResourceGroup -n MyManagedCluster --outbound-type userDefinedRouting --load-balancer-sku standard --vnet-subnet-id customUserSubnetVnetID
   - name: Create a kubernetes cluster with supporting Windows agent pools.
-    text: az aks create -g MyResourceGroup -n MyManagedCluster --load-balancer-sku Standard --vm-set-type VirtualMachineScaleSet --network-plugin azure --windows-admin-username azure --windows-admin-password 'replacePassword1234$'
+    text: az aks create -g MyResourceGroup -n MyManagedCluster --load-balancer-sku Standard --network-plugin azure --windows-admin-username azure --windows-admin-password 'replacePassword1234$'
   - name: Create a kubernetes cluster with managed AAD enabled.
     text: az aks create -g MyResourceGroup -n MyManagedCluster --enable-aad --aad-admin-group-object-ids <id-1,id-2> --aad-tenant-id <id>
 """
 
 helps['aks update'] = """
 type: command
 short-summary: Update a managed Kubernetes cluster.
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_helpers.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_helpers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_loadbalancer.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/acs_client.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/acs_client.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/proxy.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/proxy.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/acs/win_proxy.py` & `azure-cli-2.9.1/azure/cli/command_modules/acs/win_proxy.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/advisor/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/advisor/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_sdk_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_sdk_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_test_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_test_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/account.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/account.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/account_filter.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/account_filter.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/asset.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/asset.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/asset_filter.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/asset_filter.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/content_key_policy.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/content_key_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/job.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/job.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/live_event.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/live_event.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/live_output.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/live_output.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/mru.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/mru.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/sp.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/sp.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/streaming_endpoint.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/streaming_endpoint.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/streaming_locator.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/streaming_locator.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/streaming_policy.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/streaming_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/ams/operations/transform.py` & `azure-cli-2.9.1/azure/cli/command_modules/ams/operations/transform.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/apim/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/apim/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/azconfig_client.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/azconfig_client.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/constants.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/constants.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/exceptions.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/execution_context.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/execution_context.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/http_logger.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/http_logger.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/keyvalue_iterable.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/keyvalue_iterable.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/mapper.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/mapper.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/models.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/models.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/request_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/request_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/request_message.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/request_message.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_azconfig/utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_azconfig/utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_constants.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_featuremodels.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_featuremodels.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_kv_helpers.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_kv_helpers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/feature.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/feature.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appconfig/keyvalue.py` & `azure-cli-2.9.1/azure/cli/command_modules/appconfig/keyvalue.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_appservice_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_appservice_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_constants.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_create_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_create_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/access_restrictions.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/access_restrictions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/appservice_environment.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/appservice_environment.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/azure_devops_build_interactive.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/azure_devops_build_interactive.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/azure_devops_build_provider.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/azure_devops_build_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/resources/LinuxFunctionsStacks.json` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/resources/LinuxFunctionsStacks.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/resources/WindowsFunctionsStacks.json` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/resources/WindowsFunctionsStacks.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/static_sites.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/static_sites.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/tunnel.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/tunnel.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/appservice/vsts_cd_provider.py` & `azure-cli-2.9.1/azure/cli/command_modules/appservice/vsts_cd_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_aad.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_aad.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_rbac.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_rbac.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/aro/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/aro/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/custom_afs.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/custom_afs.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/custom_base.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/custom_base.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/custom_common.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/custom_common.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/custom_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/custom_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/backup/custom_wl.py` & `azure-cli-2.9.1/azure/cli/command_modules/backup/custom_wl.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_command_type.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_command_type.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_parameter_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_parameter_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batch/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/batch/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/batchai/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/batchai/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/billing/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/billing/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/bot_json_formatter.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/bot_json_formatter.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/bot_publish_prep.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/bot_publish_prep.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/bot_template_deployer.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/bot_template_deployer.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/channel_operations.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/channel_operations.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/http_response_validator.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/http_response_validator.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/kudu_client.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/kudu_client.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/name_availability.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/name_availability.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/typescript.web.config` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/typescript.web.config`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/web.config` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/web.config`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/web_app_operations.py` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/web_app_operations.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/botservice/webappv4.template.json` & `azure-cli-2.9.1/azure/cli/command_modules/botservice/webappv4.template.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/_actions.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/_actions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cdn/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/cdn/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cloud/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cloud/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/cloud/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cloud/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/cloud/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cloud/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/cloud/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cognitiveservices/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/cognitiveservices/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/_consts.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/_consts.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/configure/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/configure/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/_transformers.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/_transformers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/consumption/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/consumption/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/container/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/container/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_command_type.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_command_type.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/actions.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/actions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/cosmosdb/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/cosmosdb/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/deploymentmanager/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/deploymentmanager/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dla/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/dla/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dls/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/dls/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dms/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/dms/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dms/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/dms/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dms/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/dms/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dms/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/dms/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dms/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/dms/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/dms/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/dms/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/advanced_filter.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/advanced_filter.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/event_channel_filter.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/event_channel_filter.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventgrid/inbound_ip_rules.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventgrid/inbound_ip_rules.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/_validator.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/_validator.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/eventhubs/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/eventhubs/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/extension/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/extension/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/extension/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/extension/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/extension/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/extension/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/extension/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/feedback/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/feedback/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/feedback/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/feedback/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/feedback/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/feedback/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/find/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/find/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/find/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/find/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/find/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/find/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/find/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/find/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/find/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/find/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/hdinsight/util.py` & `azure-cli-2.9.1/azure/cli/command_modules/hdinsight/util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/interactive/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/interactive/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/interactive/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/_help.py`

 * *Files 8% similar despite different names*

```diff
@@ -762,128 +762,14 @@
         az iot hub update --name MyIotHub --add properties.ipFilterRules filter_name=test-rule action=Accept ip_mask=127.0.0.0/31
   - name: Update metadata for an IoT hub. (autogenerated)
     text: |
         az iot hub update --name MyIotHub --set properties.allocationPolicy="GeoLatency"
     crafted: true
 """
 
-helps['iot pnp'] = """
-type: group
-short-summary: Manage IoT Plug and Play repositories and repository access keys.
-"""
-
-helps['iot pnp key'] = """
-type: group
-short-summary: Manage access keys to an IoT Plug and Play repository.
-"""
-
-helps['iot pnp key create'] = """
-type: command
-short-summary: Create a key for the given repository.
-examples:
-  - name: Create a key for the given repository.
-    text: >
-        az iot pnp key create -r aaaabbbb11112222aaaabbbb1111222 --role Reader
-"""
-
-helps['iot pnp key delete'] = """
-type: command
-short-summary: Delete a key from the given repository.
-examples:
-  - name: Delete a key from the given repository.
-    text: >
-        az iot pnp key delete -r aaaabbbb11112222aaaabbbb1111222 -k 12345
-"""
-
-helps['iot pnp key list'] = """
-type: command
-short-summary: List repository's keys.
-examples:
-  - name: List repository's keys.
-    text: >
-        az iot pnp key list -r aaaabbbb11112222aaaabbbb1111222
-"""
-
-helps['iot pnp key show'] = """
-type: command
-short-summary: Get the details of a repository key.
-examples:
-  - name: Get the details of a repository key.
-    text: >
-        az iot pnp key show -r aaaabbbb11112222aaaabbbb1111222 -k 12345
-"""
-
-helps['iot pnp key update'] = """
-type: command
-short-summary: Update the key for the given repository.
-examples:
-  - name: Update the key for the given repository.
-    text: >
-        az iot pnp key update -r aaaabbbb11112222aaaabbbb1111222 -k 12345 --role admin
-"""
-
-helps['iot pnp repository'] = """
-type: group
-short-summary: Manage IoT Plug and Play repositories.
-"""
-
-helps['iot pnp repository create'] = """
-type: command
-short-summary: Create an IoT Plug and Play repository.
-examples:
-  - name: Create a new IoT Plug and Play repository "myrepo"
-    text: >
-        az iot pnp repository create -n myrepo
-"""
-
-helps['iot pnp repository delete'] = """
-type: command
-short-summary: Delete an IoT Plug and Play repository.
-examples:
-  - name: Delete an IoT Plug and Play repository.
-    text: >
-        az iot pnp repository delete -r aaaabbbb11112222aaaabbbb1111222
-"""
-
-helps['iot pnp repository get-provision-status'] = """
-type: command
-short-summary: Returns the IoT Plug and Play repository provisioning status.
-examples:
-  - name: Returns the IoT Plug and Play repository provisioning status.
-    text: >
-        az iot pnp repository get-provision-status -r aaaabbbb11112222aaaabbbb1111222 -s aaaabbbb11112222aaaabbbb1111333
-"""
-
-helps['iot pnp repository list'] = """
-type: command
-short-summary: List IoT Plug and Play repositories.
-examples:
-  - name: List IoT Plug and Play repositories.
-    text: >
-        az iot pnp repository list
-"""
-
-helps['iot pnp repository show'] = """
-type: command
-short-summary: Gets the details for an IoT Plug and Play repository.
-examples:
-  - name: Gets the details for an IoT Plug and Play repository.
-    text: >
-        az iot pnp repository show -r aaaabbbb11112222aaaabbbb1111222
-"""
-
-helps['iot pnp repository update'] = """
-type: command
-short-summary: Update an IoT Plug and Play repository.
-examples:
-  - name: Update an IoT Plug and Play repository.
-    text: >
-        az iot pnp repository update -r aaaabbbb11112222aaaabbbb1111222 -n updatedreponame
-"""
-
 helps['iot central'] = """
 type: group
 short-summary: Manage IoT Central assets.
 """
 
 helps['iot central app'] = """
 type: group
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 from azure.mgmt.iothubprovisioningservices.models import (IotDpsSku,
                                                           AllocationPolicy,
                                                           AccessRightsDescription)
 from azure.cli.command_modules.iot.shared import (EndpointType,
                                                   RouteSourceType,
                                                   EncodingFormat,
                                                   RenewKeyType,
-                                                  AuthenticationType,
-                                                  UserRole)
+                                                  AuthenticationType)
 from .custom import KeyType, SimpleAccessRights
 from ._validators import (validate_policy_permissions,
                           validate_retention_days,
                           validate_fileupload_notification_max_delivery_count,
                           validate_fileupload_notification_ttl,
                           validate_fileupload_sas_ttl,
                           validate_feedback_ttl,
@@ -269,32 +268,14 @@
     # Arguments for Message Enrichments
     with self.argument_context('iot hub message-enrichment') as c:
         c.argument('key', options_list=['--key', '-k'], help='The enrichment\'s key.')
         c.argument('value', options_list=['--value', '-v'], help='The enrichment\'s value.')
         c.argument('endpoints', options_list=['--endpoints', '-e'], nargs='*',
                    help='Endpoint(s) to apply enrichments to. Use a space-separated list for multiple endpoints.')
 
-    # Arguments for IoT Digital Twin
-    with self.argument_context('iot pnp') as c:
-        c.argument('repo_endpoint', options_list=['--endpoint', '-e'], help='IoT Plug and Play endpoint.')
-        c.argument('repo_id', options_list=['--repo-id', '-r'], help='IoT Plug and Play repository Id.')
-
-    with self.argument_context('iot pnp repository') as c:
-        c.argument('repo_name', options_list=['--name', '-n'], help='IoT Plug and Play repository Name.')
-
-    with self.argument_context('iot pnp repository get-provision-status') as c:
-        c.argument('track_id', options_list=['--provisioning-State', '-s'],
-                   help='Provisioning state of an IoT Plug and Play repository.')
-
-    with self.argument_context('iot pnp key') as c:
-        c.argument('key_id', options_list=['--key-id', '-k'],
-                   help='Access key for the given IoT Plug and Play repository.')
-        c.argument('user_role', options_list=['--role'], arg_type=get_enum_type(UserRole),
-                   help='User role of the access key for the given IoT Plug and Play repository.')
-
     with self.argument_context('iot central app') as c:
         c.argument('app_name', app_name_type, options_list=['--name', '-n'])
 
     with self.argument_context('iot central app create') as c:
         c.argument('app_name', completer=None)
         c.argument('location', get_location_type(self.cli_ctx),
                    help='Location of your IoT Central application. Default is the location of target resource group.')
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 from azure.cli.core.commands import LongRunningOperation, CliCommandType
 from ._client_factory import iot_hub_service_factory
 from ._client_factory import iot_service_provisioning_factory
-from ._client_factory import iot_pnp_service_factory
 from ._client_factory import iot_central_service_factory
 
 JOB_DEPRECATION_INFO = 'IoT Extension (azure-cli-iot-ext) Job commands'
 
 
 class PolicyUpdateResultTransform(LongRunningOperation):  # pylint: disable=too-few-public-methods
     def __call__(self, poller):
@@ -152,30 +151,14 @@
         g.custom_command('test', 'iot_hub_route_test')
 
     # iot hub device stream commands
     with self.command_group('iot hub devicestream', client_factory=iot_hub_service_factory,
                             min_api="2019-07-01-preview") as g:
         g.custom_command('show', 'iot_hub_devicestream_show')
 
-    # iot pnp commands
-    with self.command_group('iot pnp repository', client_factory=iot_pnp_service_factory, is_preview=True) as g:
-        g.custom_command('list', 'pnp_list_repository')
-        g.custom_show_command('show', 'pnp_get_repository')
-        g.custom_command('create', 'pnp_create_repository')
-        g.custom_command('delete', 'pnp_delete_repository')
-        g.custom_command('update', 'pnp_update_repository')
-        g.custom_command('get-provision-status', 'pnp_track_provision_status')
-
-    with self.command_group('iot pnp key', client_factory=iot_pnp_service_factory, is_preview=True) as g:
-        g.custom_command('list', 'pnp_list_key')
-        g.custom_show_command('show', 'pnp_get_key')
-        g.custom_command('create', 'pnp_create_key')
-        g.custom_command('delete', 'pnp_delete_key')
-        g.custom_command('update', 'pnp_update_key')
-
     with self.command_group('iot central app', iot_central_sdk, client_factory=iot_central_service_factory,
                             is_preview=True) as g:
         g.custom_command('create', 'iot_central_app_create')
         g.custom_command('list', 'iot_central_app_list')
         g.custom_show_command('show', 'iot_central_app_get')
         g.generic_update_command('update', getter_name='iot_central_app_get',
                                  setter_name='iot_central_app_update', command_type=update_custom_util)
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,16 @@
                                                           SharedAccessSignatureAuthorizationRuleAccessRightsDescription)
 
 
 from azure.mgmt.iotcentral.models import (AppSkuInfo,
                                           App)
 
 from azure.cli.command_modules.iot.shared import EndpointType, EncodingFormat, RenewKeyType, AuthenticationType
-from ._constants import PNP_ENDPOINT
-from ._client_factory import resource_service_factory, get_pnp_client
-from ._utils import open_certificate, get_auth_header, generateKey
+from ._client_factory import resource_service_factory
+from ._utils import open_certificate, generateKey
 
 
 logger = get_logger(__name__)
 
 
 # CUSTOM TYPE
 class KeyType(Enum):
@@ -934,84 +933,14 @@
     failover_region = next(x.location for x in hub.properties.locations if x.role.lower() == 'secondary')
     if no_wait:
         return client.iot_hub.manual_failover(hub_name, resource_group_name, failover_region)
     LongRunningOperation(cmd.cli_ctx)(client.iot_hub.manual_failover(hub_name, resource_group_name, failover_region))
     return iot_hub_get(cmd, client, hub_name, resource_group_name)
 
 
-def pnp_create_repository(cmd, client, repo_name, repo_endpoint=PNP_ENDPOINT):
-    return _pnp_create_update_repository(cmd, client, repo_endpoint, repo_name)
-
-
-def pnp_update_repository(cmd, client, repo_id, repo_name, repo_endpoint=PNP_ENDPOINT):
-    return _pnp_create_update_repository(cmd, client, repo_endpoint, repo_name, repo_id)
-
-
-def pnp_list_repository(cmd, client, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).get_repositories_async(api_version=client.api_version, custom_headers=headers)
-
-
-def pnp_get_repository(cmd, client, repo_id, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).get_repository_async(repo_id, api_version=client.api_version, custom_headers=headers)
-
-
-def pnp_delete_repository(cmd, client, repo_id, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).delete_repository_async(repo_id, api_version=client.api_version, custom_headers=headers)
-
-
-def pnp_track_provision_status(cmd, client, repo_id, track_id, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).get_provision_status(repo_id, track_id, api_version=client.api_version, custom_headers=headers)
-
-
-def pnp_create_key(cmd, client, repo_id, user_role, repo_endpoint=PNP_ENDPOINT):
-    return _pnp_create_update_authkeys(cmd, client, repo_endpoint, repo_id, user_role)
-
-
-def pnp_update_key(cmd, client, repo_id, key_id, user_role, repo_endpoint=PNP_ENDPOINT):
-    return _pnp_create_update_authkeys(cmd, client, repo_endpoint, repo_id, user_role, key_id)
-
-
-def pnp_list_key(cmd, client, repo_id, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).get_keys_async(repository_id=repo_id, api_version=client.api_version, custom_headers=headers)
-
-
-def pnp_get_key(cmd, client, repo_id, key_id, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).get_key_async(repo_id, key_id, api_version=client.api_version, custom_headers=headers)
-
-
-def pnp_delete_key(cmd, client, repo_id, key_id, repo_endpoint=PNP_ENDPOINT):
-    headers = get_auth_header(cmd)
-    return get_pnp_client(repo_endpoint).delete_key_async(key_id, repo_id, api_version=client.api_version, custom_headers=headers)
-
-
-def _pnp_create_update_repository(cmd, client, repo_endpoint, repo_name, repo_id=None):
-    from .digitaltwinrepositoryprovisioningservice.models import RepositoryUpsertRequestProperties
-    headers = get_auth_header(cmd)
-    repositoryUpsertRequestProperties = RepositoryUpsertRequestProperties(id=repo_id, name=repo_name)
-    return get_pnp_client(repo_endpoint).create_or_update_repository_async(api_version=client.api_version,
-                                                                           properties=repositoryUpsertRequestProperties,
-                                                                           custom_headers=headers)
-
-
-def _pnp_create_update_authkeys(cmd, client, repo_endpoint, repo_id, user_role, key_id=None):
-    from .digitaltwinrepositoryprovisioningservice.models import RepositoryKeyRequestProperties
-    headers = get_auth_header(cmd)
-    repositoryKeyRequestProperties = RepositoryKeyRequestProperties(id=key_id, user_role=user_role)
-    return get_pnp_client(repo_endpoint).create_or_update_key_async(repository_id=repo_id,
-                                                                    api_version=client.api_version,
-                                                                    properties=repositoryKeyRequestProperties,
-                                                                    custom_headers=headers)
-
-
 def _get_iot_hub_by_name(client, hub_name):
     all_hubs = iot_hub_list(client)
     if all_hubs is None:
         raise CLIError("No IoT Hub found in current subscription.")
     try:
         target_hub = next(x for x in all_hubs if hub_name.lower() == x.name.lower())
     except StopIteration:
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/digital_twin_repository_provisioning_service.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/digital_twin_repository_provisioning_service.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/key_metadata.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/key_metadata.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request_properties.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_key_request_properties.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata_properties.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_metadata_properties.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_provision_response_base.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_provision_response_base.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request_properties.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/models/repository_upsert_request_properties.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/version.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/digitaltwinrepositoryprovisioningservice/version.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/sas_token_auth.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/sas_token_auth.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iot/shared.py` & `azure-cli-2.9.1/azure/cli/command_modules/iot/shared.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,24 +41,14 @@
     Type of the encoding format for the container.
     """
     JSON = 'json'
     AVRO = 'avro'
 
 
 # pylint: disable=too-few-public-methods
-class UserRole(Enum):
-    """
-    Type of the user role for the repository key.
-    """
-    Admin = 'admin'
-    Reader = 'reader'
-    Contributer = 'contributer'
-
-
-# pylint: disable=too-few-public-methods
 class RenewKeyType(Enum):
     """
     Type of the RegenerateKey for the authorization policy.
     """
     Primary = 'primary'
     Secondary = 'secondary'
     Swap = 'swap'
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iotcentral/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/iotcentral/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iotcentral/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/iotcentral/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iotcentral/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/iotcentral/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iotcentral/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/iotcentral/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iotcentral/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/iotcentral/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/iotcentral/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/iotcentral/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_command_type.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_command_type.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_transformers.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_transformers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/keyvault/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/keyvault/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/kusto/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/kusto/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/lab/validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/lab/validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/managedservices/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/managedservices/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/managedservices/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/managedservices/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/managedservices/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/managedservices/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/managedservices/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/managedservices/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/managedservices/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/managedservices/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/managedservices/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/managedservices/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/maps/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/maps/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/maps/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/maps/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/maps/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/maps/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/maps/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/maps/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/maps/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/maps/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/maps/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/_autoscale_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/_autoscale_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/actions.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/actions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionLexer.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionLexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
+# Generated from MetricAlertCondition.g4 by ANTLR 4.7.2
 # encoding: utf-8
-
 # pylint: disable=all
-# Generated from MetricAlertCondition.g4 by ANTLR 4.7.2
 from __future__ import print_function
 from antlr4 import *
 from io import StringIO
 import sys
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionListener.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
+# Generated from MetricAlertCondition.g4 by ANTLR 4.7.2
 # encoding: utf-8
-
 # pylint: disable=all
-# Generated from MetricAlertCondition.g4 by ANTLR 4.7.2
 from antlr4 import *
 
 # This class defines a complete listener for a parse tree produced by MetricAlertConditionParser.
 class MetricAlertConditionListener(ParseTreeListener):
 
     # Enter a parse tree produced by MetricAlertConditionParser#expression.
     def enterExpression(self, ctx):
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionParser.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
+# Generated from MetricAlertCondition.g4 by ANTLR 4.7.2
 # encoding: utf-8
-
 # pylint: disable=all
-# Generated from MetricAlertCondition.g4 by ANTLR 4.7.2
 from __future__ import print_function
 from antlr4 import *
 from io import StringIO
 import sys
 
 
 def serializedATN():
@@ -24,40 +23,40 @@
         buf.write(u"\5\6\5J\n\5\r\5\16\5K\3\6\3\6\3\6\3\7\3\7\3\b\3\b\3\b")
         buf.write(u"\3\t\3\t\3\t\3\t\3\t\7\t[\n\t\f\t\16\t^\13\t\3\n\3\n")
         buf.write(u"\3\n\3\n\3\13\3\13\3\13\3\f\3\f\3\f\3\r\3\r\3\r\3\16")
         buf.write(u"\3\16\3\16\3\17\3\17\3\17\3\17\7\17t\n\17\f\17\16\17")
         buf.write(u"w\13\17\3\20\6\20z\n\20\r\20\16\20{\3\20\2\2\21\2\4\6")
         buf.write(u"\b\n\f\16\20\22\24\26\30\32\34\36\2\b\4\2\3\4\30\30\5")
         buf.write(u"\2\3\13\26\26\30\30\4\2\n\n\17\17\3\2\20\21\4\2\n\n\22")
-        buf.write(u"\22\t\2\3\3\7\7\t\t\f\r\24\24\26\26\30\30\2w\2 \3\2\2")
-        buf.write(u"\2\4@\3\2\2\2\6D\3\2\2\2\bI\3\2\2\2\nM\3\2\2\2\fP\3\2")
-        buf.write(u"\2\2\16R\3\2\2\2\20U\3\2\2\2\22_\3\2\2\2\24c\3\2\2\2")
-        buf.write(u"\26f\3\2\2\2\30i\3\2\2\2\32l\3\2\2\2\34o\3\2\2\2\36y")
-        buf.write(u"\3\2\2\2 &\5\4\3\2!\"\5\6\4\2\"#\7\3\2\2#%\3\2\2\2$!")
-        buf.write(u"\3\2\2\2%(\3\2\2\2&$\3\2\2\2&\'\3\2\2\2\'/\3\2\2\2(&")
-        buf.write(u"\3\2\2\2)*\7\25\2\2*+\5\b\5\2+,\7\25\2\2,-\7\26\2\2-")
-        buf.write(u"\60\3\2\2\2.\60\5\b\5\2/)\3\2\2\2/.\3\2\2\2\60\61\3\2")
-        buf.write(u"\2\2\61\62\5\n\6\2\62\67\5\f\7\2\63\64\7\26\2\2\64\66")
-        buf.write(u"\5\20\t\2\65\63\3\2\2\2\669\3\2\2\2\67\65\3\2\2\2\67")
-        buf.write(u"8\3\2\2\28=\3\2\2\29\67\3\2\2\2:<\7\27\2\2;:\3\2\2\2")
-        buf.write(u"<?\3\2\2\2=;\3\2\2\2=>\3\2\2\2>\3\3\2\2\2?=\3\2\2\2@")
-        buf.write(u"A\7\30\2\2AB\7\26\2\2B\5\3\2\2\2CE\t\2\2\2DC\3\2\2\2")
-        buf.write(u"EF\3\2\2\2FD\3\2\2\2FG\3\2\2\2G\7\3\2\2\2HJ\t\3\2\2I")
-        buf.write(u"H\3\2\2\2JK\3\2\2\2KI\3\2\2\2KL\3\2\2\2L\t\3\2\2\2MN")
-        buf.write(u"\7\23\2\2NO\7\26\2\2O\13\3\2\2\2PQ\7\24\2\2Q\r\3\2\2")
-        buf.write(u"\2RS\7\16\2\2ST\7\26\2\2T\17\3\2\2\2UV\5\16\b\2V\\\5")
-        buf.write(u"\22\n\2WX\5\24\13\2XY\5\22\n\2Y[\3\2\2\2ZW\3\2\2\2[^")
-        buf.write(u"\3\2\2\2\\Z\3\2\2\2\\]\3\2\2\2]\21\3\2\2\2^\\\3\2\2\2")
-        buf.write(u"_`\5\32\16\2`a\5\26\f\2ab\5\34\17\2b\23\3\2\2\2cd\t\4")
-        buf.write(u"\2\2de\7\26\2\2e\25\3\2\2\2fg\t\5\2\2gh\7\26\2\2h\27")
-        buf.write(u"\3\2\2\2ij\t\6\2\2jk\7\26\2\2k\31\3\2\2\2lm\7\30\2\2")
-        buf.write(u"mn\7\26\2\2n\33\3\2\2\2ou\5\36\20\2pq\5\30\r\2qr\5\36")
-        buf.write(u"\20\2rt\3\2\2\2sp\3\2\2\2tw\3\2\2\2us\3\2\2\2uv\3\2\2")
-        buf.write(u"\2v\35\3\2\2\2wu\3\2\2\2xz\t\7\2\2yx\3\2\2\2z{\3\2\2")
-        buf.write(u"\2{y\3\2\2\2{|\3\2\2\2|\37\3\2\2\2\13&/\67=FK\\u{")
+        buf.write(u"\22\b\2\3\3\5\5\7\r\24\24\26\26\30\30\2w\2 \3\2\2\2\4")
+        buf.write(u"@\3\2\2\2\6D\3\2\2\2\bI\3\2\2\2\nM\3\2\2\2\fP\3\2\2\2")
+        buf.write(u"\16R\3\2\2\2\20U\3\2\2\2\22_\3\2\2\2\24c\3\2\2\2\26f")
+        buf.write(u"\3\2\2\2\30i\3\2\2\2\32l\3\2\2\2\34o\3\2\2\2\36y\3\2")
+        buf.write(u"\2\2 &\5\4\3\2!\"\5\6\4\2\"#\7\3\2\2#%\3\2\2\2$!\3\2")
+        buf.write(u"\2\2%(\3\2\2\2&$\3\2\2\2&\'\3\2\2\2\'/\3\2\2\2(&\3\2")
+        buf.write(u"\2\2)*\7\25\2\2*+\5\b\5\2+,\7\25\2\2,-\7\26\2\2-\60\3")
+        buf.write(u"\2\2\2.\60\5\b\5\2/)\3\2\2\2/.\3\2\2\2\60\61\3\2\2\2")
+        buf.write(u"\61\62\5\n\6\2\62\67\5\f\7\2\63\64\7\26\2\2\64\66\5\20")
+        buf.write(u"\t\2\65\63\3\2\2\2\669\3\2\2\2\67\65\3\2\2\2\678\3\2")
+        buf.write(u"\2\28=\3\2\2\29\67\3\2\2\2:<\7\27\2\2;:\3\2\2\2<?\3\2")
+        buf.write(u"\2\2=;\3\2\2\2=>\3\2\2\2>\3\3\2\2\2?=\3\2\2\2@A\7\30")
+        buf.write(u"\2\2AB\7\26\2\2B\5\3\2\2\2CE\t\2\2\2DC\3\2\2\2EF\3\2")
+        buf.write(u"\2\2FD\3\2\2\2FG\3\2\2\2G\7\3\2\2\2HJ\t\3\2\2IH\3\2\2")
+        buf.write(u"\2JK\3\2\2\2KI\3\2\2\2KL\3\2\2\2L\t\3\2\2\2MN\7\23\2")
+        buf.write(u"\2NO\7\26\2\2O\13\3\2\2\2PQ\7\24\2\2Q\r\3\2\2\2RS\7\16")
+        buf.write(u"\2\2ST\7\26\2\2T\17\3\2\2\2UV\5\16\b\2V\\\5\22\n\2WX")
+        buf.write(u"\5\24\13\2XY\5\22\n\2Y[\3\2\2\2ZW\3\2\2\2[^\3\2\2\2\\")
+        buf.write(u"Z\3\2\2\2\\]\3\2\2\2]\21\3\2\2\2^\\\3\2\2\2_`\5\32\16")
+        buf.write(u"\2`a\5\26\f\2ab\5\34\17\2b\23\3\2\2\2cd\t\4\2\2de\7\26")
+        buf.write(u"\2\2e\25\3\2\2\2fg\t\5\2\2gh\7\26\2\2h\27\3\2\2\2ij\t")
+        buf.write(u"\6\2\2jk\7\26\2\2k\31\3\2\2\2lm\7\30\2\2mn\7\26\2\2n")
+        buf.write(u"\33\3\2\2\2ou\5\36\20\2pq\5\30\r\2qr\5\36\20\2rt\3\2")
+        buf.write(u"\2\2sp\3\2\2\2tw\3\2\2\2us\3\2\2\2uv\3\2\2\2v\35\3\2")
+        buf.write(u"\2\2wu\3\2\2\2xz\t\7\2\2yx\3\2\2\2z{\3\2\2\2{y\3\2\2")
+        buf.write(u"\2{|\3\2\2\2|\37\3\2\2\2\13&/\67=FK\\u{")
         return buf.getvalue()
 
 
 class MetricAlertConditionParser ( Parser ):
 
     grammarFileName = "MetricAlertCondition.g4"
 
@@ -1013,15 +1012,15 @@
             self.state = 119 
             self._errHandler.sync(self)
             _alt = 1
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
                     self.state = 118
                     _la = self._input.LA(1)
-                    if not((((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << MetricAlertConditionParser.T__0) | (1 << MetricAlertConditionParser.T__4) | (1 << MetricAlertConditionParser.T__6) | (1 << MetricAlertConditionParser.T__9) | (1 << MetricAlertConditionParser.T__10) | (1 << MetricAlertConditionParser.NUMBER) | (1 << MetricAlertConditionParser.WHITESPACE) | (1 << MetricAlertConditionParser.WORD))) != 0)):
+                    if not((((_la) & ~0x3f) == 0 and ((1 << _la) & ((1 << MetricAlertConditionParser.T__0) | (1 << MetricAlertConditionParser.T__2) | (1 << MetricAlertConditionParser.T__4) | (1 << MetricAlertConditionParser.T__5) | (1 << MetricAlertConditionParser.T__6) | (1 << MetricAlertConditionParser.T__7) | (1 << MetricAlertConditionParser.T__8) | (1 << MetricAlertConditionParser.T__9) | (1 << MetricAlertConditionParser.T__10) | (1 << MetricAlertConditionParser.NUMBER) | (1 << MetricAlertConditionParser.WHITESPACE) | (1 << MetricAlertConditionParser.WORD))) != 0)):
                         self._errHandler.recoverInline(self)
                     else:
                         self._errHandler.reportMatch(self)
                         self.consume()
 
                 else:
                     raise NoViableAltException(self)
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/MetricAlertConditionValidator.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/MetricAlertConditionValidator.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/grammar/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/action_groups.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/action_groups.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/activity_log_alerts.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/activity_log_alerts.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/autoscale-parameters-template.json` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/autoscale-parameters-template.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/autoscale_settings.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/autoscale_settings.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/diagnostics_settings.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/diagnostics_settings.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/general_operations.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/general_operations.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_cluster.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_cluster.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_linked_storage_account.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_linked_storage_account.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_workspace.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_analytics_workspace_linked_service.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_analytics_workspace_linked_service.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/log_profiles.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/log_profiles.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/metric_alert.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/metric_alert.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/monitor_clone_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/monitor_clone_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/private_link_scope.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/private_link_scope.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/operations/subscription_diagnostic_settings.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/operations/subscription_diagnostic_settings.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/transformers.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/transformers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/util.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/monitor/validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/monitor/validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/natgateway/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/natgateway/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/netappfiles/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/netappfiles/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_actions.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_actions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_template_builder.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_template_builder.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -3300,22 +3300,26 @@
     address_pool = client.get(resource_group_name, load_balancer_name, backend_address_pool_name)
     (LoadBalancerBackendAddress,
      VirtualNetwork) = cmd.get_models('LoadBalancerBackendAddress',
                                       'VirtualNetwork')
     new_address = LoadBalancerBackendAddress(name=address_name,
                                              virtual_network=VirtualNetwork(id=vnet) if vnet else None,
                                              ip_address=ip_address if ip_address else None)
+    if address_pool.load_balancer_backend_addresses is None:
+        address_pool.load_balancer_backend_addresses = []
     address_pool.load_balancer_backend_addresses.append(new_address)
     return client.create_or_update(resource_group_name, load_balancer_name, backend_address_pool_name, address_pool)
 
 
 def remove_lb_backend_address_pool_address(cmd, resource_group_name, load_balancer_name,
                                            backend_address_pool_name, address_name):
     client = network_client_factory(cmd.cli_ctx).load_balancer_backend_address_pools
     address_pool = client.get(resource_group_name, load_balancer_name, backend_address_pool_name)
+    if address_pool.load_balancer_backend_addresses is None:
+        address_pool.load_balancer_backend_addresses = []
     lb_addresses = [addr for addr in address_pool.load_balancer_backend_addresses if addr.name != address_name]
     address_pool.load_balancer_backend_addresses = lb_addresses
     return client.create_or_update(resource_group_name, load_balancer_name, backend_address_pool_name, address_pool)
 
 
 def list_lb_backend_address_pool_address(cmd, resource_group_name, load_balancer_name,
                                          backend_address_pool_name):
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/batch_provider.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/batch_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/keyvault_provider.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/private_link_resource_and_endpoint_connections/resource_providers/keyvault_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/make_zone_file.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/make_zone_file.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/parse_zone_file.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/parse_zone_file.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/network/zone_file/record_processors.py` & `azure-cli-2.9.1/azure/cli/command_modules/network/zone_file/record_processors.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/policyinsights/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/policyinsights/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/privatedns/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/privatedns/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/profile/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/profile/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/profile/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/profile/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/profile/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/profile/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/profile/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/profile/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/profile/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/rdbms/validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/rdbms/validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/redis/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/redis/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/relay/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/relay/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/reservations/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/reservations/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_color.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_color.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_exception_handler.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_formatters.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_formatters.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_symbol.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_symbol.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/_win_vt.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/_win_vt.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/resource/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/resource/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/_multi_api_adaptor.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/_multi_api_adaptor.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/role/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/role/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/search/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/search/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/search/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/search/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/search/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/search/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/search/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/search/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/search/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/search/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/search/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/search/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/security/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/security/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicebus/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicebus/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_arm_deployment_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_arm_deployment_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/operations/applications.py` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/operations/applications.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/linux/parameter.json` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/linux/parameter.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/linux/template.json` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/linux/template.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/service/template.json` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/service/template.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/windows/parameter.json` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/windows/parameter.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/servicefabric/template/windows/template.json` & `azure-cli-2.9.1/azure/cli/command_modules/servicefabric/template/windows/template.json`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/_actions.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/_actions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/_constants.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/cors.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/cors.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/key.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/key.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/network.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/network.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/signalr/upstream.py` & `azure-cli-2.9.1/azure/cli/command_modules/signalr/upstream.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sql/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/sql/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/sqlvm/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/sqlvm/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 class StorageArgumentContext(AzArgumentContext):
     def register_sas_arguments(self):
         from azure.cli.command_modules.storage._validators import ipv4_range_type, get_datetime_type
         self.argument('ip', type=ipv4_range_type,
                       help='Specifies the IP address or range of IP addresses from which to accept requests. Supports '
                            'only IPv4 style addresses.')
-        self.argument('expiry', type=get_datetime_type(True), required=True,
+        self.argument('expiry', type=get_datetime_type(True),
                       help='Specifies the UTC datetime (Y-m-d\'T\'H:M\'Z\') at which the SAS becomes invalid. Do not '
                            'use if a stored access policy is referenced with --id that specifies this value.')
         self.argument('start', type=get_datetime_type(True),
                       help='Specifies the UTC datetime (Y-m-d\'T\'H:M\'Z\') at which the SAS becomes valid. Do not use '
                            'if a stored access policy is referenced with --id that specifies this value. Defaults to '
                            'the time of the request.')
         self.argument('protocol', options_list=('--https-only',), action='store_const', const='https',
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_client_factory_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_client_factory_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,14 +471,27 @@
 type: group
 short-summary: Manage blob copy operations. Use `az storage blob show` to check the status of the blobs.
 """
 
 helps['storage blob copy start'] = """
 type: command
 short-summary: Copies a blob asynchronously. Use `az storage blob show` to check the status of the blobs.
+parameters:
+  - name: --source-uri -u
+    type: string
+    short-summary: >
+        A URL of up to 2 KB in length that specifies an Azure file or blob.
+        The value should be URL-encoded as it would appear in a request URI.
+        If the source is in another account, the source must either be public
+        or must be authenticated via a shared access signature. If the source
+        is public, no authentication is required.
+        Examples:
+        `https://myaccount.blob.core.windows.net/mycontainer/myblob`,
+        `https://myaccount.blob.core.windows.net/mycontainer/myblob?snapshot=<DateTime>`,
+        `https://otheraccount.blob.core.windows.net/mycontainer/myblob?sastoken`
 examples:
   - name: Copies a blob asynchronously. Use `az storage blob show` to check the status of the blobs. (autogenerated)
     text: |
         az storage blob copy start --account-key 00000000 --account-name MyAccount --destination-blob MyDestinationBlob --destination-container MyDestinationContainer --source-uri https://storage.blob.core.windows.net/photos
     crafted: true
   - name: Copies a blob asynchronously. Use `az storage blob show` to check the status of the blobs (autogenerated)
     text: |
@@ -643,14 +656,22 @@
 short-summary: Manage blob incremental copy operations.
 """
 
 helps['storage blob incremental-copy start'] = """
 type: command
 short-summary: Copies an incremental copy of a blob asynchronously.
 long-summary: This operation returns a copy operation properties object, including a copy ID you can use to check or abort the copy operation. The Blob service copies blobs on a best-effort basis. The source blob for an incremental copy operation must be a page blob. Call get_blob_properties on the destination blob to check the status of the copy operation. The final blob will be committed when the copy completes.
+parameters:
+  - name: --source-uri -u
+    short-summary: >
+        A URL of up to 2 KB in length that specifies an Azure page blob.
+        The value should be URL-encoded as it would appear in a request URI.
+        The copy source must be a snapshot and include a valid SAS token or be public.
+        Example:
+        `https://myaccount.blob.core.windows.net/mycontainer/myblob?snapshot=<DateTime>&sastoken`
 examples:
   - name: Upload all files that end with .py unless blob exists and has been modified since given date.
     text: az storage blob incremental-copy start --source-container MySourceContainer --source-blob MyBlob --source-account-name MySourceAccount --source-account-key MySourceKey --source-snapshot MySnapshot --destination-container MyDestinationContainer --destination-blob MyDestinationBlob
   - name: Copies an incremental copy of a blob asynchronously. (autogenerated)
     text: |
         az storage blob incremental-copy start --account-key 00000000 --account-name MyAccount --destination-blob MyDestinationBlob --destination-container MyDestinationContainer --source-account-key MySourceKey --source-account-name MySourceAccount --source-blob MyBlob --source-container MySourceContainer --source-snapshot MySnapshot
     crafted: true
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
         t_account_permissions = self.get_sdk('common.models#AccountPermissions')
         c.register_sas_arguments()
         c.argument('services', type=services_type(self))
         c.argument('resource_types', type=resource_type_type(self))
         c.argument('expiry', type=get_datetime_type(True))
         c.argument('start', type=get_datetime_type(True))
         c.argument('account_name', acct_name_type, options_list=['--account-name'])
-        c.argument('permission', options_list=('--permissions',), required=True,
+        c.argument('permission', options_list=('--permissions',),
                    help='The permissions the SAS grants. Allowed values: {}. Can be combined.'.format(
                        get_permission_help_string(t_account_permissions)),
                    validator=get_permission_validator(t_account_permissions))
         c.ignore('sas_token')
 
     for item in ['show', 'off']:
         with self.argument_context('storage logging {}'.format(item)) as c:
@@ -480,15 +480,15 @@
                    validator=as_user_validator,
                    help="Indicates that this command return the SAS signed with the user delegation key. "
                         "The expiry parameter and '--auth-mode login' are required if this argument is specified. ")
         c.argument('id', options_list='--policy-name',
                    help='The name of a stored access policy within the container\'s ACL.',
                    completer=get_storage_acl_name_completion_list(t_base_blob_service, 'container_name',
                                                                   'get_container_acl'))
-        c.argument('permission', options_list='--permissions', required=True,
+        c.argument('permission', options_list='--permissions',
                    help=sas_help.format(get_permission_help_string(t_blob_permissions)),
                    validator=get_permission_validator(t_blob_permissions))
         c.ignore('sas_token')
 
     with self.argument_context('storage blob restore', resource_type=ResourceType.MGMT_STORAGE) as c:
         from ._validators import BlobRangeAddAction
         c.argument('blob_ranges', options_list=['--blob-range', '-r'], action=BlobRangeAddAction, nargs='+',
@@ -806,15 +806,15 @@
         from .completers import get_storage_acl_name_completion_list
         t_container_permissions = self.get_sdk('blob.models#ContainerPermissions')
         c.register_sas_arguments()
         c.argument('id', options_list='--policy-name',
                    help='The name of a stored access policy within the container\'s ACL.',
                    completer=get_storage_acl_name_completion_list(t_container_permissions, 'container_name',
                                                                   'get_container_acl'))
-        c.argument('permission', options_list='--permissions', required=True,
+        c.argument('permission', options_list='--permissions',
                    help=sas_help.format(get_permission_help_string(t_container_permissions)),
                    validator=get_permission_validator(t_container_permissions))
         c.argument('cache_control', help='Response header value for Cache-Control when resource is accessed'
                                          'using this shared access signature.')
         c.argument('content_disposition', help='Response header value for Content-Disposition when resource is accessed'
                                                'using this shared access signature.')
         c.argument('content_encoding', help='Response header value for Content-Encoding when resource is accessed'
@@ -899,15 +899,15 @@
         from .completers import get_storage_acl_name_completion_list
 
         t_share_permissions = self.get_sdk('file.models#SharePermissions')
         c.register_sas_arguments()
         c.argument('id', options_list='--policy-name',
                    help='The name of a stored access policy within the share\'s ACL.',
                    completer=get_storage_acl_name_completion_list(t_share_permissions, 'share_name', 'get_share_acl'))
-        c.argument('permission', options_list='--permissions', required=True,
+        c.argument('permission', options_list='--permissions',
                    help=sas_help.format(get_permission_help_string(t_share_permissions)),
                    validator=get_permission_validator(t_share_permissions))
         c.ignore('sas_token')
 
     with self.argument_context('storage directory') as c:
         c.argument('directory_name', directory_type, options_list=('--name', '-n'))
 
@@ -950,15 +950,15 @@
         c.register_sas_arguments()
 
         t_file_svc = self.get_sdk('file.fileservice#FileService')
         t_file_permissions = self.get_sdk('file.models#FilePermissions')
         c.argument('id', options_list='--policy-name',
                    help='The name of a stored access policy within the container\'s ACL.',
                    completer=get_storage_acl_name_completion_list(t_file_svc, 'container_name', 'get_container_acl'))
-        c.argument('permission', options_list='--permissions', required=True,
+        c.argument('permission', options_list='--permissions',
                    help=sas_help.format(get_permission_help_string(t_file_permissions)),
                    validator=get_permission_validator(t_file_permissions))
         c.ignore('sas_token')
 
     with self.argument_context('storage file list') as c:
         from .completers import dir_path_completer
         c.argument('directory_name', options_list=('--path', '-p'), help='The directory path within the file share.',
@@ -1060,15 +1060,15 @@
         t_queue_permissions = self.get_sdk('queue.models#QueuePermissions')
 
         c.register_sas_arguments()
 
         c.argument('id', options_list='--policy-name',
                    help='The name of a stored access policy within the share\'s ACL.',
                    completer=get_storage_acl_name_completion_list(t_queue_permissions, 'queue_name', 'get_queue_acl'))
-        c.argument('permission', options_list='--permissions', required=True,
+        c.argument('permission', options_list='--permissions',
                    help=sas_help.format(get_permission_help_string(t_queue_permissions)),
                    validator=get_permission_validator(t_queue_permissions))
         c.ignore('sas_token')
         c.ignore('auth_mode')
 
     with self.argument_context('storage queue') as c:
         c.argument('queue_name', queue_name_type, options_list=('--name', '-n'))
@@ -1141,15 +1141,15 @@
     with self.argument_context('storage table generate-sas') as c:
         from .completers import get_storage_acl_name_completion_list
 
         c.register_sas_arguments()
         c.argument('id', options_list='--policy-name',
                    help='The name of a stored access policy within the table\'s ACL.',
                    completer=get_storage_acl_name_completion_list(t_table_service, 'table_name', 'get_table_acl'))
-        c.argument('permission', options_list='--permissions', required=True,
+        c.argument('permission', options_list='--permissions',
                    help=sas_help.format('(r)ead/query (a)dd (u)pdate (d)elete'),
                    validator=table_permission_validator)
         c.ignore('sas_token')
 
     with self.argument_context('storage entity') as c:
         c.ignore('property_resolver')
         c.argument('entity', options_list=('--entity', '-e'), validator=validate_entity, nargs='+')
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_params_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_params_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_transformers.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_transformers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_transformers_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_transformers_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/_validators_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/_validators_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/azcopy/util.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/azcopy/util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/commands_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/commands_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/oauth_token_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/oauth_token_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,19 +29,19 @@
         from datetime import datetime
         # should give back token that is valid for at least 5 mins
         token = Profile(cli_ctx=self.cli_ctx).get_raw_token(
             resource="https://storage.azure.com", subscription=self.cli_ctx.data['subscription_id'])[0][2]
         try:
             self.token_credential.token = token['accessToken']
             expire = token['expiresOn']
-            seconds_left = (datetime.strptime(expire, "%Y-%m-%d %H:%M:%S.%f") - datetime.now()).seconds
+            seconds_left = (datetime.strptime(expire, "%Y-%m-%d %H:%M:%S.%f") - datetime.now()).total_seconds()
         except KeyError:  # needed to deal with differing unserialized MSI token payload
             self.token_credential.token = token['access_token']
             expire = datetime.fromtimestamp(int(token['expires_on']))
-            seconds_left = (expire - datetime.now()).seconds
+            seconds_left = (expire - datetime.now()).total_seconds()
 
         if seconds_left < 180:
             logger.warning("Acquired token will expire on %s. Current time is %s.", expire, datetime.now())
 
         with self.lock:
             self.timer = threading.Timer(seconds_left - 180, self.timer_callback)
             self.timer.daemon = True
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/account.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/account.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/acl.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/acl.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/azcopy.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/azcopy.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/blob.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/blob.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/blob_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/blob_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/cors.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/cors.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/directory.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/directory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/directory_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/directory_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/file.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/file.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/file_azure_stack.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/file_azure_stack.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/filesystem.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/filesystem.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/fs_directory.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/fs_directory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/fs_file.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/fs_file.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/logging.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/logging.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/metrics.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/metrics.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/operations/table.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/operations/table.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/sdkutil.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/sdkutil.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/services_wrapper.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/services_wrapper.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/storage_url_helpers.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/storage_url_helpers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/track2_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/track2_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/url_quote_util.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/url_quote_util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/storage/util.py` & `azure-cli-2.9.1/azure/cli/command_modules/storage/util.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/util/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/util/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/util/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/util/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/util/_params.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/util/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/util/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/util/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/util/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/__init__.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_actions.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_actions.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_alias.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_alias.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_client_factory.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_client_factory.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_completers.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_completers.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_format.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_format.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_help.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_help.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_image_builder.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_image_builder.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_params.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
                 c.argument(dest, vmss_name_type, id_part=None)  # due to instance-ids parameter
 
     with self.argument_context('vmss create') as c:
         VirtualMachineEvictionPolicyTypes = self.get_models('VirtualMachineEvictionPolicyTypes', resource_type=ResourceType.MGMT_COMPUTE)
         c.argument('name', name_arg_type)
         c.argument('nat_backend_port', default=None, help='Backend port to open with NAT rules. Defaults to 22 on Linux and 3389 on Windows.')
         c.argument('single_placement_group', arg_type=get_three_state_flag(), help="Limit the scale set to a single placement group."
-                   " See https://docs.microsoft.com/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-placement-groups for details")
+                   " See https://docs.microsoft.com/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-placement-groups for details.")
         c.argument('platform_fault_domain_count', type=int, help='Fault Domain count for each placement group in the availability zone', min_api='2017-12-01')
         c.argument('vmss_name', name_arg_type, id_part=None, help='Name of the virtual machine scale set.')
         c.argument('instance_count', help='Number of VMs in the scale set.', type=int)
         c.argument('disable_overprovision', help='Overprovision option (see https://azure.microsoft.com/documentation/articles/virtual-machine-scale-sets-overview/ for details).', action='store_true')
         c.argument('upgrade_policy_mode', help=None, arg_type=get_enum_type(UpgradeMode))
         c.argument('health_probe', help='Probe name from the existing load balancer, mainly used for rolling upgrade or automatic repairs')
         c.argument('vm_sku', help='Size of VMs in the scale set. Default to "Standard_DS1_v2". See https://azure.microsoft.com/pricing/details/virtual-machines/ for size info.')
```

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_template_builder.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_template_builder.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_validators.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_validators.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_vm_diagnostics_templates.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_vm_diagnostics_templates.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_vm_utils.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_vm_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/_workspace_data_source_settings.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/_workspace_data_source_settings.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/commands.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/commands.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/custom.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/custom.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure/cli/command_modules/vm/disk_encryption.py` & `azure-cli-2.9.1/azure/cli/command_modules/vm/disk_encryption.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure_bdist_wheel.py` & `azure-cli-2.9.1/azure_bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure_cli.egg-info/PKG-INFO` & `azure-cli-2.9.1/azure_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-cli
-Version: 2.9.0
+Version: 2.9.1
 Summary: Microsoft Azure Command-Line Tools
 Home-page: https://github.com/Azure/azure-cli
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Description: Microsoft Azure CLI
         ===================
@@ -114,14 +114,33 @@
         
         
         .. :changelog:
         
         Release History
         ===============
         
+        2.9.1
+        ++++++
+        
+        **AKS**
+        
+        * Remove explicit setting of VMSS in Windows example command since it is now default (#14324)
+        
+        **IoT**
+        
+        * [BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI (#14117)
+        
+        **REST**
+        
+        * Fix #14152: `az rest`: Accept ARM URLs without subscription ID (#14370)
+        
+        **Storage**
+        
+        * Fix #14138: Make some permissions optional (#14385)
+        
         2.9.0
         ++++++
         
         **ACR**
         
         * Handle log artifact link from Registry to stream logs (#14038)
         * Deprecate helm2 commands (#14143)
```

### Comparing `azure-cli-2.9.0/azure_cli.egg-info/SOURCES.txt` & `azure-cli-2.9.1/azure_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-2.9.0/azure_cli.egg-info/requires.txt` & `azure-cli-2.9.1/azure_cli.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 antlr4-python3-runtime~=4.7.2
 azure-batch~=9.0
 azure-cli-command_modules-nspkg~=2.0
-azure-cli-core==2.9.0.*
+azure-cli-core==2.9.1.*
 azure-cli-nspkg>=3.0.3,~=3.0
 azure-cosmos>=3.0.2,~=3.0
 azure-datalake-store~=0.0.48
 azure-functions-devops-build~=0.0.22
 azure-graphrbac~=0.60.0
 azure-keyvault~=1.1
 azure-mgmt-advisor<3.0.0,>=2.0.1
```

### Comparing `azure-cli-2.9.0/setup.py` & `azure-cli-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from azure_bdist_wheel import cmdclass
 except ImportError:
     from distutils import log as logger
 
     logger.warn("Wheel is not available, disabling bdist_wheel hook")
     cmdclass = {}
 
-VERSION = "2.9.0"
+VERSION = "2.9.1"
 # If we have source, validate that our version numbers match
 # This should prevent uploading releases with mismatched versions.
 try:
     with open('azure/cli/__init__.py', 'r', encoding='utf-8') as f:
         content = f.read()
 except OSError:
     pass
```

