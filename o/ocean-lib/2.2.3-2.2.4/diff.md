# Comparing `tmp/ocean-lib-2.2.3.tar.gz` & `tmp/ocean-lib-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean-lib-2.2.3.tar", last modified: Mon Apr 17 08:56:24 2023, max compression
+gzip compressed data, was "ocean-lib-2.2.4.tar", last modified: Tue May 23 21:15:35 2023, max compression
```

## Comparing `ocean-lib-2.2.3.tar` & `ocean-lib-2.2.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.446375 ocean-lib-2.2.3/ocean_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/agreements/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/agreements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/agreements/consumable.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/agreements/service_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/aquarius/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/aquarius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/aquarius/aquarius.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/asset_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/ddo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/data_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/data_service_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/fileinfo_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/example_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/http_requests/requests_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/compute_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/data_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/data_nft_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/datatoken1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/datatoken2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/datatoken_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/models/df/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/df/df_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/df/df_strategy_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/dispenser.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/erc721_token_factory_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/factory_router.py
--rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/fixed_rate_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/models/ve/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/smart_wallet_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_allocate.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_delegation.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_delegation_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_fee_distributor.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_fee_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_ocean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/ocean/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/mint_fake_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/ocean_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/ocean_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/services/consumer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/structures/abi_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/structures/algorithm_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/structures/file_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/web3_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/contract_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/contract_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.090407 ocean-lib-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-23 21:15:35.090407 ocean-lib-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib/agreements/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/agreements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/agreements/consumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/agreements/service_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib/aquarius/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/aquarius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/aquarius/aquarius.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/assets/asset_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/assets/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/assets/ddo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/data_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/data_provider/data_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/data_provider/data_service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/data_provider/fileinfo_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/example_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/http_requests/requests_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.086407 ocean-lib-2.2.4/ocean_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/compute_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/data_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/data_nft_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/datatoken1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/datatoken2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/datatoken_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.086407 ocean-lib-2.2.4/ocean_lib/models/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/df/df_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/df/df_strategy_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/dispenser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/erc721_token_factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/factory_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/fixed_rate_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.086407 ocean-lib-2.2.4/ocean_lib/models/ve/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/smart_wallet_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/ve_allocate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/ve_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/ve_delegation_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/ve_fee_distributor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/ve_fee_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/models/ve/ve_ocean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.086407 ocean-lib-2.2.4/ocean_lib/ocean/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/mint_fake_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/ocean_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/ocean_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/ocean/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.086407 ocean-lib-2.2.4/ocean_lib/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/services/consumer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.086407 ocean-lib-2.2.4/ocean_lib/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/structures/abi_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/structures/algorithm_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/structures/file_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.090407 ocean-lib-2.2.4/ocean_lib/web3_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/web3_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/web3_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/web3_internal/contract_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/web3_internal/contract_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/ocean_lib/web3_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:15:35.082407 ocean-lib-2.2.4/ocean_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-23 21:15:35.000000 ocean-lib-2.2.4/ocean_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-23 21:15:35.000000 ocean-lib-2.2.4/ocean_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:15:35.000000 ocean-lib-2.2.4/ocean_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:15:35.000000 ocean-lib-2.2.4/ocean_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 21:15:35.000000 ocean-lib-2.2.4/ocean_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 21:15:35.000000 ocean-lib-2.2.4/ocean_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 21:15:35.090407 ocean-lib-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-23 21:15:25.000000 ocean-lib-2.2.4/setup.py
```

### Comparing `ocean-lib-2.2.3/LICENSE` & `ocean-lib-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/PKG-INFO` & `ocean-lib-2.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-lib
-Version: 2.2.3
+Version: 2.2.4
 Summary: 🐳 Ocean protocol library.
 Home-page: https://github.com/oceanprotocol/ocean.py
 Author: ocean-core-team
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Keywords: ocean-lib
 Classifier: Development Status :: 4 - Beta
@@ -74,27 +74,29 @@
 ### More types of data assets
 
 Each of the following shows how to publish & consume a particular type of data.
 - [C2D](READMEs/c2d-flow.md) - tokenize & monetize AI algorithms via Compute-to-Data
 - [REST API](READMEs/publish-flow-restapi.md) - Example on Binance ETH price feed
 - [GraphQL](READMEs/publish-flow-graphql.md) - Example on Ocean Data NFTs
 - [On-chain data](READMEs/publish-flow-onchain.md) - Example on Ocean swap fees
+- [Adding credentials](READMEs/publish-flow-credentials.md) - Example on publishing an asset with custom credentials
 
 ### Learn more
 - [Understand config parameters](READMEs/parameters.md) - envvars vs files
 - [Learn about off-chain services](READMEs/services.md) - Ocean Provider for data services, Aquarius metadata store
+- [Using hardware wallets with ocean.py](READMEs/using-clef.md) - Learn how to use hardware wallets with ocean.py via Brownie and Clef
 
 ## 🦑 Development
 
 - **[Developers flow](READMEs/developers.md)** - to further develop ocean.py
 - [Release process](READMEs/release-process.md) - to do a new release of ocean.py
 
 ## 🏛 License
 
-    Copyright ((C)) 2022 Ocean Protocol Foundation
+    Copyright ((C)) 2023 Ocean Protocol Foundation
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ocean-lib-2.2.3/README.md` & `ocean-lib-2.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,27 +55,29 @@
 ### More types of data assets
 
 Each of the following shows how to publish & consume a particular type of data.
 - [C2D](READMEs/c2d-flow.md) - tokenize & monetize AI algorithms via Compute-to-Data
 - [REST API](READMEs/publish-flow-restapi.md) - Example on Binance ETH price feed
 - [GraphQL](READMEs/publish-flow-graphql.md) - Example on Ocean Data NFTs
 - [On-chain data](READMEs/publish-flow-onchain.md) - Example on Ocean swap fees
+- [Adding credentials](READMEs/publish-flow-credentials.md) - Example on publishing an asset with custom credentials
 
 ### Learn more
 - [Understand config parameters](READMEs/parameters.md) - envvars vs files
 - [Learn about off-chain services](READMEs/services.md) - Ocean Provider for data services, Aquarius metadata store
+- [Using hardware wallets with ocean.py](READMEs/using-clef.md) - Learn how to use hardware wallets with ocean.py via Brownie and Clef
 
 ## 🦑 Development
 
 - **[Developers flow](READMEs/developers.md)** - to further develop ocean.py
 - [Release process](READMEs/release-process.md) - to do a new release of ocean.py
 
 ## 🏛 License
 
-    Copyright ((C)) 2022 Ocean Protocol Foundation
+    Copyright ((C)) 2023 Ocean Protocol Foundation
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ocean-lib-2.2.3/ocean_lib/agreements/consumable.py` & `ocean-lib-2.2.4/ocean_lib/agreements/consumable.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/aquarius/aquarius.py` & `ocean-lib-2.2.4/ocean_lib/aquarius/aquarius.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/assets/asset_downloader.py` & `ocean-lib-2.2.4/ocean_lib/assets/asset_downloader.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/assets/credentials.py` & `ocean-lib-2.2.4/ocean_lib/assets/credentials.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/assets/ddo.py` & `ocean-lib-2.2.4/ocean_lib/assets/ddo.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/data_provider/base.py` & `ocean-lib-2.2.4/ocean_lib/data_provider/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 
 """Provider module."""
 import logging
 import os
 import re
-from datetime import datetime
+from datetime import datetime, timezone
 from json import JSONDecodeError
 from typing import Dict, List, Optional, Tuple, Union
 from unittest.mock import Mock
-from requests.models import PreparedRequest
 
 import requests
+from brownie.network.account import ClefAccount
 from enforce_typing import enforce_types
 from requests.exceptions import InvalidURL
-from requests.models import Response
+from requests.models import PreparedRequest, Response
 from requests.sessions import Session
-from web3.main import Web3
 
 from ocean_lib.exceptions import DataProviderException
 from ocean_lib.http_requests.requests_session import get_requests_session
-from ocean_lib.web3_internal.utils import sign_with_key
+from ocean_lib.web3_internal.utils import sign_with_clef, sign_with_key
 
 logger = logging.getLogger(__name__)
 
 
 class DataServiceProviderBase:
     """DataServiceProviderBase class."""
 
@@ -44,42 +43,31 @@
     def set_http_client(http_client: Session) -> None:
         """Set the http client to something other than the default `requests`."""
         DataServiceProviderBase._http_client = http_client
 
     @staticmethod
     @enforce_types
     def sign_message(wallet, msg: str) -> Tuple[str, str]:
-        nonce = str(datetime.utcnow().timestamp())
+        nonce = str(datetime.now(timezone.utc).timestamp() * 1000)
         print(f"signing message with nonce {nonce}: {msg}, account={wallet.address}")
-        message_hash = Web3.solidityKeccak(
-            ["bytes"],
-            [Web3.toBytes(text=f"{msg}{nonce}")],
-        )
-        signed = sign_with_key(message_hash, wallet.private_key)
-
-        return nonce, str(signed)
 
-    @staticmethod
-    @enforce_types
-    def _remove_slash(path: str) -> str:
-        if path.endswith("/"):
-            path = path[:-1]
-        if path.startswith("/"):
-            path = path[1:]
-        return path
+        if isinstance(wallet, ClefAccount):
+            return nonce, str(sign_with_clef(f"{msg}{nonce}", wallet))
+
+        return nonce, str(sign_with_key(f"{msg}{nonce}", wallet.private_key))
 
     @staticmethod
     @enforce_types
     def get_url(config_dict: dict) -> str:
         """
         Return the DataProvider component url.
 
         :return: Url, str
         """
-        return DataServiceProviderBase._remove_slash(config_dict.get("PROVIDER_URL"))
+        return _remove_slash(config_dict.get("PROVIDER_URL"))
 
     @staticmethod
     @enforce_types
     def get_service_endpoints(provider_uri: str) -> Dict[str, List[str]]:
         """
         Return the service endpoints from the provider URL.
         """
@@ -92,20 +80,19 @@
     @staticmethod
     @enforce_types
     def get_c2d_environments(provider_uri: str, chain_id: int) -> Optional[str]:
         """
         Return the provider address
         """
         try:
-            _, envs_endpoint = DataServiceProviderBase.build_c2d_environments_endpoint(
-                provider_uri, chain_id
+            method, envs_endpoint = DataServiceProviderBase.build_endpoint(
+                "computeEnvironments", provider_uri, {"chainId": chain_id}
             )
             environments = DataServiceProviderBase._http_method(
-                "get",
-                envs_endpoint,
+                method, url=envs_endpoint
             ).json()
 
             if str(chain_id) not in environments:
                 logger.warning(
                     "You might be using an older provider. ocean.py can not verify the chain id."
                 )
                 return environments
@@ -152,34 +139,34 @@
 
         if len(parts) < 2:
             raise InvalidURL(f"InvalidURL {service_endpoint}.")
 
         if parts[-2] == "services":
             provider_uri = "/".join(parts[:-2])
 
-        result = DataServiceProviderBase._remove_slash(provider_uri)
+        result = _remove_slash(provider_uri)
 
         if not result:
             raise InvalidURL(f"InvalidURL {service_endpoint}.")
 
         try:
             root_result = "/".join(parts[0:3])
             response = requests.get(root_result).json()
         except (requests.exceptions.RequestException, JSONDecodeError):
             raise InvalidURL(f"InvalidURL {service_endpoint}.")
 
-        if "providerAddresses" not in response and "providerAddress" not in response:
-            raise InvalidURL(
-                f"Invalid Provider URL {service_endpoint}, no providerAddresses."
-            )
-
-        if "providerAddress" in response:
-            logger.warning(
-                "You might be using an older provider. ocean.py can not verify the chain id."
-            )
+        if "providerAddresses" not in response:
+            if "providerAddress" in response:
+                logger.warning(
+                    "You might be using an older provider. ocean.py can not verify the chain id."
+                )
+            else:
+                raise InvalidURL(
+                    f"Invalid Provider URL {service_endpoint}, no providerAddresses."
+                )
 
         return result
 
     @staticmethod
     @enforce_types
     def is_valid_provider(provider_uri: str) -> bool:
         try:
@@ -205,80 +192,34 @@
             req.prepare_url(url, params)
             url = req.url
 
         return method, url
 
     @staticmethod
     @enforce_types
-    def build_encrypt_endpoint(provider_uri: str, chain_id: int) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint(
-            "encrypt", provider_uri, {"chainId": chain_id}
-        )
-
-    @staticmethod
-    @enforce_types
-    def build_initialize_endpoint(provider_uri: str) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint("initialize", provider_uri)
-
-    @staticmethod
-    @enforce_types
-    def build_initialize_compute_endpoint(provider_uri: str) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint("initializeCompute", provider_uri)
-
-    @staticmethod
-    @enforce_types
-    def build_download_endpoint(provider_uri: str) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint("download", provider_uri)
-
-    @staticmethod
-    @enforce_types
-    def build_compute_endpoint(provider_uri: str) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint("computeStatus", provider_uri)
-
-    @staticmethod
-    @enforce_types
-    def build_compute_result_file_endpoint(provider_uri: str) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint("computeResult", provider_uri)
-
-    @staticmethod
-    @enforce_types
-    def build_fileinfo(provider_uri: str) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint("fileinfo", provider_uri)
-
-    @staticmethod
-    @enforce_types
-    def build_c2d_environments_endpoint(
-        provider_uri: str, chain_id: int
-    ) -> Tuple[str, str]:
-        return DataServiceProviderBase.build_endpoint(
-            "computeEnvironments", provider_uri, {"chainId": chain_id}
-        )
-
-    @staticmethod
-    @enforce_types
     def write_file(
         response: Response,
         destination_folder: Union[str, bytes, os.PathLike],
         index: int,
     ) -> None:
         """
         Write the response content in a file in the destination folder.
         :param response: Response
         :param destination_folder: Destination folder, string
         :param index: file index
         :return: None
         """
-
-        if response.status_code == 200:
-            with open(os.path.join(destination_folder, f"file{index}"), "wb") as f:
-                for chunk in response.iter_content(chunk_size=4096):
-                    f.write(chunk)
-            logger.info(f"Saved downloaded file in {f.name}")
-        else:
+        if response.status_code != 200:
             logger.warning(f"consume failed: {response.reason}")
+            return
+
+        with open(os.path.join(destination_folder, f"file{index}"), "wb") as f:
+            for chunk in response.iter_content(chunk_size=4096):
+                f.write(chunk)
+        logger.info(f"Saved downloaded file in {f.name}")
 
     @staticmethod
     @enforce_types
     def _validate_content_disposition(header: str) -> bool:
         pattern = re.compile(r"\\|\.\.|/")
         return not bool(pattern.findall(header))
 
@@ -289,27 +230,28 @@
             if not DataServiceProviderBase._validate_content_disposition(
                 response.headers.get("content-disposition")
             ):
                 logger.error(
                     "Invalid content disposition format. It was not possible to get the file name."
                 )
                 return None
+
             return re.match(
                 r"attachment;filename=(.+)",
                 response.headers.get("content-disposition"),
             )[1]
         except Exception as e:
             logger.warning(f"It was not possible to get the file name. {e}")
             return None
 
     @staticmethod
     @enforce_types
     def _http_method(method: str, *args, **kwargs) -> Optional[Union[Mock, Response]]:
         try:
-            return getattr(DataServiceProviderBase._http_client, method)(
+            return getattr(DataServiceProviderBase._http_client, method.lower())(
                 *args, **kwargs
             )
         except Exception:
             logger.error(
                 f"Error invoking http method {method}: args={str(args)}, kwargs={str(kwargs)}"
             )
             raise
@@ -322,25 +264,22 @@
         endpoint: str,
         payload: Union[Dict, bytes],
         success_codes: Optional[List] = None,
         exception_type=DataProviderException,
     ):
         if not response or not hasattr(response, "status_code"):
             if isinstance(response, Response) and response.status_code == 400:
-                error = response.json().get("error", None)
-                if error is None:
-                    error = response.json().get("errors", "unknown error")
+                error = response.json().get(
+                    "error", response.json().get("errors", "unknown error")
+                )
 
                 raise DataProviderException(f"{endpoint_name} failed: {error}")
 
-            response_content = (
-                getattr(response, "content")
-                if hasattr(response, "content")
-                else "<none>"
-            )
+            response_content = getattr(response, "content", "<none>")
+
             raise DataProviderException(
                 f"Failed to get a response for request: {endpoint_name}={endpoint}, payload={payload}, response is {response_content}"
             )
 
         if not success_codes:
             success_codes = [200]
 
@@ -356,7 +295,14 @@
 
 
 @enforce_types
 def urljoin(*args) -> str:
     trailing_slash = "/" if args[-1].endswith("/") else ""
 
     return "/".join(map(lambda x: str(x).strip("/"), args)) + trailing_slash
+
+
+def _remove_slash(path: str) -> str:
+    path = path[:-1] if path.endswith("/") else path
+    path = path[1:] if path.startswith("/") else path
+
+    return path
```

### Comparing `ocean-lib-2.2.3/ocean_lib/data_provider/data_encryptor.py` & `ocean-lib-2.2.4/ocean_lib/data_provider/data_encryptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,20 +31,20 @@
             data = json.dumps(objects_to_encrypt, separators=(",", ":"))
             payload = data.encode("utf-8")
         elif isinstance(objects_to_encrypt, str):
             payload = objects_to_encrypt.encode("utf-8")
         else:
             payload = objects_to_encrypt
 
-        _, encrypt_endpoint = DataServiceProviderBase.build_encrypt_endpoint(
-            provider_uri, chain_id
+        method, encrypt_endpoint = DataServiceProviderBase.build_endpoint(
+            "encrypt", provider_uri, {"chainId": chain_id}
         )
 
         response = DataServiceProviderBase._http_method(
-            "post",
+            method,
             encrypt_endpoint,
             data=payload,
             headers={"Content-type": "application/octet-stream"},
         )
 
         DataServiceProviderBase.check_response(
             response,
```

### Comparing `ocean-lib-2.2.3/ocean_lib/data_provider/data_service_provider.py` & `ocean-lib-2.2.4/ocean_lib/data_provider/data_service_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # Copyright 2023 Ocean Protocol Foundation
 # SPDX-License-Identifier: Apache-2.0
 #
 
 """Provider module."""
 import json
 import logging
+from datetime import datetime, timezone
 from json import JSONDecodeError
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
+from unittest.mock import Mock
 
-import requests
 from enforce_typing import enforce_types
 from requests.models import PreparedRequest, Response
 
 from ocean_lib.agreements.service_types import ServiceTypes
 from ocean_lib.data_provider.base import DataServiceProviderBase
 from ocean_lib.data_provider.fileinfo_provider import FileInfoProvider
-from ocean_lib.exceptions import DataProviderException
 from ocean_lib.http_requests.requests_session import get_requests_session
 from ocean_lib.models.compute_input import ComputeInput
 from ocean_lib.structures.algorithm_metadata import AlgorithmMetadata
 
 logger = logging.getLogger(__name__)
 
 
@@ -41,43 +41,35 @@
     def initialize(
         did: str,
         service: Any,  # Can not add Service typing due to enforce_type errors.
         consumer_address: str,
         userdata: Optional[Dict] = None,
     ) -> Response:
 
-        _, initialize_endpoint = DataServiceProvider.build_initialize_endpoint(
-            service.service_endpoint
+        method, initialize_endpoint = DataServiceProvider.build_endpoint(
+            "initialize", service.service_endpoint
         )
 
         payload = {
             "documentId": did,
             "serviceId": service.id,
             "consumerAddress": consumer_address,
         }
 
         if userdata is not None:
             userdata = json.dumps(userdata)
             payload["userdata"] = userdata
 
         response = DataServiceProvider._http_method(
-            "get", url=initialize_endpoint, params=payload
+            method, url=initialize_endpoint, params=payload
         )
-        if not response or not hasattr(response, "status_code"):
-            raise DataProviderException(
-                f"Failed to get a response for request: initializeEndpoint={initialize_endpoint}, payload={payload}, response is {response}"
-            )
 
-        if response.status_code != 200:
-            msg = (
-                f"Initialize service failed at the initializeEndpoint "
-                f"{initialize_endpoint}, reason {response.text}, status {response.status_code}"
-            )
-            logger.error(msg)
-            raise DataProviderException(msg)
+        DataServiceProviderBase.check_response(
+            response, "initializeEndpoint", initialize_endpoint, payload
+        )
 
         logger.info(
             f"Service initialized successfully"
             f" initializeEndpoint {initialize_endpoint}"
         )
 
         return response
@@ -94,30 +86,30 @@
     ) -> Response:
         """This function initializes compute services.
 
         To determine the Provider instance that will be called, we rely on the first dataset.
         The first dataset is also required to have a compute service.
         """
         (
-            _,
+            method,
             initialize_compute_endpoint,
-        ) = DataServiceProvider.build_initialize_compute_endpoint(service_endpoint)
+        ) = DataServiceProvider.build_endpoint("initializeCompute", service_endpoint)
 
         payload = {
             "datasets": datasets,
             "algorithm": algorithm_data,
             "compute": {
                 "env": compute_environment,
                 "validUntil": valid_until,
             },
             "consumerAddress": consumer_address,
         }
 
         response = DataServiceProvider._http_method(
-            "post",
+            method,
             initialize_compute_endpoint,
             data=json.dumps(payload),
             headers={"content-type": "application/json"},
         )
 
         DataServiceProviderBase.check_response(
             response, "initializeComputeEndpoint", initialize_compute_endpoint, payload
@@ -150,16 +142,16 @@
             assert isinstance(index, int), logger.error("index has to be an integer.")
             assert index >= 0, logger.error("index has to be 0 or a positive integer.")
             assert index < len(files), logger.error(
                 "index can not be bigger than the number of files"
             )
             indexes = [index]
 
-        _, download_endpoint = DataServiceProvider.build_download_endpoint(
-            service_endpoint
+        method, download_endpoint = DataServiceProvider.build_endpoint(
+            "download", service_endpoint
         )
 
         payload = {
             "documentId": did,
             "serviceId": service.id,
             "consumerAddress": consumer_wallet.address,
             "transferTxId": tx_id,
@@ -168,18 +160,19 @@
         if userdata:
             userdata = json.dumps(userdata)
             payload["userdata"] = userdata
 
         for i in indexes:
             payload["fileIndex"] = i
             payload["nonce"], payload["signature"] = DataServiceProvider.sign_message(
-                consumer_wallet, did
+                consumer_wallet,
+                did,
             )
             response = DataServiceProvider._http_method(
-                "get", url=download_endpoint, params=payload, stream=True, timeout=3
+                method, url=download_endpoint, params=payload, stream=True, timeout=3
             )
 
             DataServiceProviderBase.check_response(
                 response, "downloadEndpoint", download_endpoint, payload
             )
 
             DataServiceProvider.write_file(response, destination_folder, i)
@@ -230,19 +223,19 @@
             compute_environment=compute_environment,
             algorithm=algorithm,
             algorithm_meta=algorithm_meta,
             algorithm_custom_data=algorithm_custom_data,
             input_datasets=input_datasets,
         )
         logger.info(f"invoke start compute endpoint with this url: {payload}")
-        _, compute_endpoint = DataServiceProvider.build_compute_endpoint(
-            dataset_compute_service.service_endpoint
+        method, compute_endpoint = DataServiceProvider.build_endpoint(
+            "computeStart", dataset_compute_service.service_endpoint
         )
         response = DataServiceProvider._http_method(
-            "post",
+            method,
             compute_endpoint,
             data=json.dumps(payload),
             headers={"content-type": "application/json"},
         )
 
         logger.debug(
             f"got DataProvider execute response: {response.content} with status-code {response.status_code} "
@@ -276,16 +269,16 @@
         :param did: hex str the DDO id
         :param job_id: str id of compute job that was returned from `start_compute_job`
         :param dataset_compute_service:
         :param consumer of the consumer's account
 
         :return: bool whether the job was stopped successfully
         """
-        _, compute_stop_endpoint = DataServiceProvider.build_compute_endpoint(
-            dataset_compute_service.service_endpoint
+        _, compute_stop_endpoint = DataServiceProvider.build_endpoint(
+            "computeStop", dataset_compute_service.service_endpoint
         )
         return DataServiceProvider._send_compute_request(
             "put", did, job_id, compute_stop_endpoint, consumer
         )
 
     @staticmethod
     @enforce_types
@@ -300,19 +293,19 @@
         :param did: hex str the DDO id
         :param job_id: str id of compute job that was returned from `start_compute_job`
         :param dataset_compute_service:
         :param consumer of the consumer's account
 
         :return: bool whether the job was deleted successfully
         """
-        _, compute_delete_endpoint = DataServiceProvider.build_compute_endpoint(
-            dataset_compute_service.service_endpoint
+        method, compute_delete_endpoint = DataServiceProvider.build_endpoint(
+            "computeDelete", dataset_compute_service.service_endpoint
         )
         return DataServiceProvider._send_compute_request(
-            "delete", did, job_id, compute_delete_endpoint, consumer
+            method, did, job_id, compute_delete_endpoint, consumer
         )
 
     @staticmethod
     @enforce_types
     def compute_job_status(
         did: str,
         job_id: str,
@@ -325,19 +318,19 @@
         :param job_id: str id of compute job that was returned from `start_compute_job`
         :param dataset_compute_service:
         :param consumer of the consumer's account
 
         :return: dict of job_id to status info. When job_id is not provided, this will return
             status for each job_id that exist for the did
         """
-        _, compute_status_endpoint = DataServiceProvider.build_compute_endpoint(
-            dataset_compute_service.service_endpoint
+        method, compute_status_endpoint = DataServiceProvider.build_endpoint(
+            "computeStatus", dataset_compute_service.service_endpoint
         )
         return DataServiceProvider._send_compute_request(
-            "get", did, job_id, compute_status_endpoint, consumer
+            method, did, job_id, compute_status_endpoint, consumer
         )
 
     @staticmethod
     @enforce_types
     def compute_job_result(
         job_id: str, index: int, dataset_compute_service: Any, consumer
     ) -> bytes:
@@ -346,40 +339,39 @@
         :param job_id: str id of compute job that was returned from `start_compute_job`
         :param index: int compute result index
         :param dataset_compute_service:
         :param consumer of the consumer's account
 
         :return: dict of job_id to result urls.
         """
+
         nonce, signature = DataServiceProvider.sign_message(
-            consumer, f"{consumer.address}{job_id}{str(index)}"
+            consumer,
+            f"{consumer.address}{job_id}{str(index)}",
         )
 
         req = PreparedRequest()
         params = {
             "signature": signature,
             "nonce": nonce,
             "jobId": job_id,
             "index": index,
             "consumerAddress": consumer.address,
         }
 
-        (
-            _,
-            compute_job_result_endpoint,
-        ) = DataServiceProvider.build_compute_result_file_endpoint(
-            dataset_compute_service.service_endpoint
+        (method, compute_job_result_endpoint) = DataServiceProvider.build_endpoint(
+            "computeResult", dataset_compute_service.service_endpoint
         )
         req.prepare_url(compute_job_result_endpoint, params)
         compute_job_result_file_url = req.url
 
         logger.info(
             f"invoke the computeResult endpoint with this url: {compute_job_result_file_url}"
         )
-        response = DataServiceProvider._http_method("get", compute_job_result_file_url)
+        response = DataServiceProvider._http_method(method, compute_job_result_file_url)
 
         DataServiceProviderBase.check_response(
             response, "jobResultEndpoint", compute_job_result_endpoint, params
         )
 
         return response.content
 
@@ -418,16 +410,18 @@
         return function_result
 
     @staticmethod
     @enforce_types
     def _send_compute_request(
         http_method: str, did: str, job_id: str, service_endpoint: str, consumer
     ) -> Dict[str, Any]:
+
         nonce, signature = DataServiceProvider.sign_message(
-            consumer, f"{consumer.address}{job_id}{did}"
+            consumer,
+            f"{consumer.address}{job_id}{did}",
         )
 
         req = PreparedRequest()
         payload = {
             "consumerAddress": consumer.address,
             "documentId": did,
             "jobId": job_id,
@@ -443,16 +437,18 @@
         )
 
         DataServiceProviderBase.check_response(
             response, "compute Endpoint", req.url, payload
         )
 
         resp_content = json.loads(response.content.decode("utf-8"))
+
         if isinstance(resp_content, list):
             return resp_content[0]
+
         return resp_content
 
     @staticmethod
     # @enforce_types omitted due to subscripted generics error
     def _prepare_compute_payload(
         consumer,
         dataset: ComputeInput,
@@ -468,29 +464,25 @@
 
         if algorithm_meta:
             assert isinstance(algorithm_meta, AlgorithmMetadata), (
                 f"expecting a AlgorithmMetadata type "
                 f"for `algorithm_meta`, got {type(algorithm_meta)}"
             )
 
+        input_datasets = input_datasets if input_datasets else []
         _input_datasets = []
-        if input_datasets:
-            for _input in input_datasets:
-                assert _input.did, "The received dataset does not have a did."
-                assert (
-                    _input.transfer_tx_id
-                ), "The received dataset does not have a transaction id."
-                assert (
-                    _input.service_id
-                ), "The received dataset does not have a specified service id."
-                if _input.did != dataset.did:
-                    _input_datasets.append(_input.as_dictionary())
+        for _input in input_datasets:
+            for req_key in ["did", "transfer_tx_id", "service_id"]:
+                assert getattr(
+                    _input, req_key
+                ), f"The received dataset does not have a {req_key}."
 
         nonce, signature = DataServiceProvider.sign_message(
-            consumer, f"{consumer.address}{dataset.did}"
+            consumer,
+            f"{consumer.address}{dataset.did}",
         )
 
         payload = {
             "dataset": {
                 "documentId": dataset.did,
                 "serviceId": dataset.service_id,
                 "transferTxId": dataset.transfer_tx_id,
@@ -524,43 +516,35 @@
             payload["algorithm"] = algorithm_meta.as_dictionary()
 
         return payload
 
     @staticmethod
     @enforce_types
     def check_single_file_info(url_object: dict, provider_uri: str) -> bool:
-        _, endpoint = DataServiceProvider.build_fileinfo(provider_uri)
-        response = requests.post(endpoint, json=url_object)
+        method, endpoint = DataServiceProvider.build_endpoint("fileinfo", provider_uri)
+        response = DataServiceProvider._http_method(method, endpoint, json=url_object)
 
         if response.status_code != 200:
             return False
 
-        response = response.json()
-        for file_info in response:
-            return file_info["valid"]
-
-        return False
+        return any([file_info["valid"] for file_info in response.json()])
 
     @staticmethod
     @enforce_types
     def check_asset_file_info(
         did: str, service_id: str, provider_uri: str, userdata: Optional[dict] = None
     ) -> bool:
         if not did:
             return False
 
-        _, endpoint = DataServiceProvider.build_fileinfo(provider_uri)
+        method, endpoint = DataServiceProvider.build_endpoint("fileinfo", provider_uri)
         data = {"did": did, "serviceId": service_id}
 
         if userdata is not None:
             data["userdata"] = userdata
 
-        response = requests.post(endpoint, json=data)
+        response = DataServiceProvider._http_method(method, endpoint, json=data)
 
         if not response or response.status_code != 200:
             return False
 
-        response = response.json()
-        for ddo_info in response:
-            return ddo_info["valid"]
-
-        return False
+        return any([file_info["valid"] for file_info in response.json()])
```

### Comparing `ocean-lib-2.2.3/ocean_lib/data_provider/fileinfo_provider.py` & `ocean-lib-2.2.4/ocean_lib/data_provider/fileinfo_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,26 +31,28 @@
     @enforce_types
     def fileinfo(
         did: str,
         service: Any,
         with_checksum: bool = False,
         userdata: Optional[dict] = None,
     ) -> Response:  # Can not add Service typing due to enforce_type errors.
-        _, fileinfo_endpoint = DataServiceProviderBase.build_fileinfo(
-            service.service_endpoint
+        method, fileinfo_endpoint = DataServiceProviderBase.build_endpoint(
+            "fileinfo", service.service_endpoint
         )
+
         payload = {"did": did, "serviceId": service.id}
+
         if userdata is not None:
             payload["userdata"] = userdata
 
         if with_checksum:
             payload["checksum"] = 1
 
         response = DataServiceProviderBase._http_method(
-            "post", fileinfo_endpoint, json=payload
+            method, fileinfo_endpoint, json=payload
         )
 
         DataServiceProviderBase.check_response(
             response, "fileInfoEndpoint", fileinfo_endpoint, payload
         )
 
         logger.info(
```

### Comparing `ocean-lib-2.2.3/ocean_lib/example_config.py` & `ocean-lib-2.2.4/ocean_lib/example_config.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/exceptions.py` & `ocean-lib-2.2.4/ocean_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/http_requests/requests_session.py` & `ocean-lib-2.2.4/ocean_lib/http_requests/requests_session.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/compute_input.py` & `ocean-lib-2.2.4/ocean_lib/models/compute_input.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/data_nft.py` & `ocean-lib-2.2.4/ocean_lib/models/data_nft.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/data_nft_factory.py` & `ocean-lib-2.2.4/ocean_lib/models/data_nft_factory.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/datatoken1.py` & `ocean-lib-2.2.4/ocean_lib/models/datatoken1.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/datatoken2.py` & `ocean-lib-2.2.4/ocean_lib/models/datatoken2.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/datatoken_base.py` & `ocean-lib-2.2.4/ocean_lib/models/datatoken_base.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/dispenser.py` & `ocean-lib-2.2.4/ocean_lib/models/dispenser.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/models/fixed_rate_exchange.py` & `ocean-lib-2.2.4/ocean_lib/models/fixed_rate_exchange.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/ocean/crypto.py` & `ocean-lib-2.2.4/ocean_lib/ocean/crypto.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/ocean/mint_fake_ocean.py` & `ocean-lib-2.2.4/ocean_lib/ocean/mint_fake_ocean.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/ocean/ocean.py` & `ocean-lib-2.2.4/ocean_lib/ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/ocean/ocean_assets.py` & `ocean-lib-2.2.4/ocean_lib/ocean/ocean_assets.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/ocean/ocean_compute.py` & `ocean-lib-2.2.4/ocean_lib/ocean/ocean_compute.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/ocean/util.py` & `ocean-lib-2.2.4/ocean_lib/ocean/util.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/services/consumer_parameters.py` & `ocean-lib-2.2.4/ocean_lib/services/consumer_parameters.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/services/service.py` & `ocean-lib-2.2.4/ocean_lib/services/service.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/structures/abi_tuples.py` & `ocean-lib-2.2.4/ocean_lib/structures/abi_tuples.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/structures/algorithm_metadata.py` & `ocean-lib-2.2.4/ocean_lib/structures/algorithm_metadata.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/structures/file_objects.py` & `ocean-lib-2.2.4/ocean_lib/structures/file_objects.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/web3_internal/contract_base.py` & `ocean-lib-2.2.4/ocean_lib/web3_internal/contract_base.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/web3_internal/contract_utils.py` & `ocean-lib-2.2.4/ocean_lib/web3_internal/contract_utils.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib/web3_internal/utils.py` & `ocean-lib-2.2.4/ocean_lib/web3_internal/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #
 # Copyright 2023 Ocean Protocol Foundation
 # SPDX-License-Identifier: Apache-2.0
 #
 import logging
 from collections import namedtuple
-from typing import Any
+from typing import Any, Union
 
 import requests
 from brownie import network
 from brownie.network import chain
+from brownie.network.account import ClefAccount
 from enforce_typing import enforce_types
 from eth_keys import KeyAPI
 from eth_keys.backends import NativeECCBackend
 from hexbytes.main import HexBytes
 from web3.main import Web3
 
 Signature = namedtuple("Signature", ("v", "r", "s"))
@@ -28,20 +29,41 @@
     :param val:
     :return:
     """
     return Web3.toHex(Web3.toBytes(val).rjust(32, b"\0"))
 
 
 @enforce_types
-def sign_with_key(message_hash: HexBytes, key: str) -> str:
+def sign_with_clef(message_hash: str, wallet: ClefAccount) -> str:
+    message_hash = Web3.solidityKeccak(
+        ["bytes"],
+        [Web3.toBytes(text=message_hash)],
+    )
+
+    orig_sig = wallet._provider.make_request(
+        "account_signData", ["data/plain", wallet.address, message_hash.hex()]
+    )["result"]
+    return orig_sig
+
+
+@enforce_types
+def sign_with_key(message_hash: Union[HexBytes, str], key: str) -> str:
+    if isinstance(message_hash, str):
+        message_hash = Web3.solidityKeccak(
+            ["bytes"],
+            [Web3.toBytes(text=message_hash)],
+        )
+
     pk = keys.PrivateKey(Web3.toBytes(hexstr=key))
+
     prefix = "\x19Ethereum Signed Message:\n32"
     signable_hash = Web3.solidityKeccak(
         ["bytes", "bytes"], [Web3.toBytes(text=prefix), Web3.toBytes(message_hash)]
     )
+
     return keys.ecdsa_sign(message_hash=signable_hash, private_key=pk)
 
 
 @enforce_types
 def split_signature(signature: Any) -> Signature:
     """
```

### Comparing `ocean-lib-2.2.3/ocean_lib.egg-info/PKG-INFO` & `ocean-lib-2.2.4/ocean_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-lib
-Version: 2.2.3
+Version: 2.2.4
 Summary: 🐳 Ocean protocol library.
 Home-page: https://github.com/oceanprotocol/ocean.py
 Author: ocean-core-team
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Keywords: ocean-lib
 Classifier: Development Status :: 4 - Beta
@@ -74,27 +74,29 @@
 ### More types of data assets
 
 Each of the following shows how to publish & consume a particular type of data.
 - [C2D](READMEs/c2d-flow.md) - tokenize & monetize AI algorithms via Compute-to-Data
 - [REST API](READMEs/publish-flow-restapi.md) - Example on Binance ETH price feed
 - [GraphQL](READMEs/publish-flow-graphql.md) - Example on Ocean Data NFTs
 - [On-chain data](READMEs/publish-flow-onchain.md) - Example on Ocean swap fees
+- [Adding credentials](READMEs/publish-flow-credentials.md) - Example on publishing an asset with custom credentials
 
 ### Learn more
 - [Understand config parameters](READMEs/parameters.md) - envvars vs files
 - [Learn about off-chain services](READMEs/services.md) - Ocean Provider for data services, Aquarius metadata store
+- [Using hardware wallets with ocean.py](READMEs/using-clef.md) - Learn how to use hardware wallets with ocean.py via Brownie and Clef
 
 ## 🦑 Development
 
 - **[Developers flow](READMEs/developers.md)** - to further develop ocean.py
 - [Release process](READMEs/release-process.md) - to do a new release of ocean.py
 
 ## 🏛 License
 
-    Copyright ((C)) 2022 Ocean Protocol Foundation
+    Copyright ((C)) 2023 Ocean Protocol Foundation
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ocean-lib-2.2.3/ocean_lib.egg-info/SOURCES.txt` & `ocean-lib-2.2.4/ocean_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.3/ocean_lib.egg-info/requires.txt` & `ocean-lib-2.2.4/ocean_lib.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 bumpversion==0.6.0
 pkginfo==1.9.6
 twine==4.0.2
 watchdog==3.0.0
 isort==5.12.0
 flake8==6.0.0
 black
-pre-commit==3.2.2
+pre-commit==3.3.2
 licenseheaders==0.8.8
 codacy-coverage==1.3.11
-coverage==7.2.3
+coverage==7.2.5
 mccabe==0.7.0
 pytest==6.2.5
 pytest-watch==4.2.0
 pytest-env==0.6.2
 matplotlib
 mkcodes==0.1.1
 pytest-sugar==0.9.7
 
 [test]
 codacy-coverage==1.3.11
-coverage==7.2.3
+coverage==7.2.5
 mccabe==0.7.0
 pytest==6.2.5
 pytest-watch==4.2.0
 pytest-env==0.6.2
 matplotlib
 mkcodes==0.1.1
 pytest-sugar==0.9.7
```

### Comparing `ocean-lib-2.2.3/setup.py` & `ocean-lib-2.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     # See https://github.com/ethereum/web3.py/blob/master/setup.py
 ]
 # Required to run setup.py:
 setup_requirements = ["pytest-runner"]
 
 test_requirements = [
     "codacy-coverage==1.3.11",
-    "coverage==7.2.3",
+    "coverage==7.2.5",
     "mccabe==0.7.0",
     "pytest==6.2.5",
     "pytest-watch==4.2.0",
     "pytest-env==0.6.2",
     "matplotlib",  # just used in a readme test and unlikely to change, common dependency
     "mkcodes==0.1.1",
     "pytest-sugar==0.9.7",
@@ -52,15 +52,15 @@
     "bumpversion==0.6.0",
     "pkginfo==1.9.6",
     "twine==4.0.2",
     "watchdog==3.0.0",
     "isort==5.12.0",
     "flake8==6.0.0",
     "black",  # need to keep this up to date to brownie
-    "pre-commit==3.2.2",
+    "pre-commit==3.3.2",
     "licenseheaders==0.8.8",
 ]
 
 packages = find_namespace_packages(include=["ocean_lib*"], exclude=["*test*"])
 
 setup(
     author="ocean-core-team",
@@ -87,11 +87,11 @@
     packages=packages,
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/oceanprotocol/ocean.py",
     # fmt: off
     # bumpversion.sh needs single-quotes
-    version='2.2.3',
+    version='2.2.4',
     # fmt: on
     zip_safe=False,
 )
```

