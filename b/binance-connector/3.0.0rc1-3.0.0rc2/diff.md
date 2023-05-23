# Comparing `tmp/binance-connector-3.0.0rc1.tar.gz` & `tmp/binance-connector-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-connector-3.0.0rc1.tar", last modified: Tue Feb 14 00:59:05 2023, max compression
+gzip compressed data, was "binance-connector-3.0.0rc2.tar", last modified: Fri Apr 21 06:58:31 2023, max compression
```

## Comparing `binance-connector-3.0.0rc1.tar` & `binance-connector-3.0.0rc2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.810989 binance-connector-3.0.0rc1/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.810989 binance-connector-3.0.0rc1/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/lib/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/binance/spot/
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_blvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_bswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_c2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_fiat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_gift_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_loan.py
--rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_mining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_rebate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_savings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    30498 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_sub_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/spot/_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/binance/websocket/spot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/spot/websocket_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/binance_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-02-14 00:59:05.000000 binance-connector-3.0.0rc1/binance_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-14 00:59:05.000000 binance-connector-3.0.0rc1/binance_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 00:59:05.000000 binance-connector-3.0.0rc1/binance_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-14 00:59:05.000000 binance-connector-3.0.0rc1/binance_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-14 00:59:05.000000 binance-connector-3.0.0rc1/binance_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-14 00:59:05.814989 binance-connector-3.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-02-14 00:59:00.000000 binance-connector-3.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.581536 binance-connector-3.0.0rc2/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.581536 binance-connector-3.0.0rc2/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.585536 binance-connector-3.0.0rc2/binance/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_blvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_bswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_c2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_fiat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_gift_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_rebate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_savings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_sub_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.585536 binance-connector-3.0.0rc2/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.585536 binance-connector-3.0.0rc2/binance/websocket/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/binance_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/setup.py
```

### Comparing `binance-connector-3.0.0rc1/LICENSE.md` & `binance-connector-3.0.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/PKG-INFO` & `binance-connector-3.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-connector-3.0.0rc1/README.md` & `binance-connector-3.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/api.py` & `binance-connector-3.0.0rc2/binance/api.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/error.py` & `binance-connector-3.0.0rc2/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/lib/authentication.py` & `binance-connector-3.0.0rc2/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/lib/enums.py` & `binance-connector-3.0.0rc2/binance/lib/enums.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/lib/utils.py` & `binance-connector-3.0.0rc2/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/__init__.py` & `binance-connector-3.0.0rc2/binance/spot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,21 +193,21 @@
     from binance.spot._sub_account import sub_account_futures_account_summary
     from binance.spot._sub_account import sub_account_futures_position_risk
     from binance.spot._sub_account import sub_account_spot_transfer_history
     from binance.spot._sub_account import sub_account_enable_leverage_token
     from binance.spot._sub_account import managed_sub_account_deposit
     from binance.spot._sub_account import managed_sub_account_assets
     from binance.spot._sub_account import managed_sub_account_withdraw
-    from binance.spot._sub_account import sub_account_api_toggle_ip_restriction
-    from binance.spot._sub_account import sub_account_api_add_ip
+    from binance.spot._sub_account import sub_account_update_ip_restriction
     from binance.spot._sub_account import sub_account_api_get_ip_restriction
     from binance.spot._sub_account import sub_account_api_delete_ip
     from binance.spot._sub_account import managed_sub_account_get_snapshot
     from binance.spot._sub_account import managed_sub_account_investor_trans_log
     from binance.spot._sub_account import managed_sub_account_trading_trans_log
+    from binance.spot._sub_account import managed_sub_account_deposit_address
 
     # FUTURES
     from binance.spot._futures import futures_transfer
     from binance.spot._futures import futures_transfer_history
     from binance.spot._futures import futures_loan_borrow_history
     from binance.spot._futures import futures_loan_repay_history
     from binance.spot._futures import futures_loan_wallet
```

### Comparing `binance-connector-3.0.0rc1/binance/spot/_blvt.py` & `binance-connector-3.0.0rc2/binance/spot/_blvt.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_bswap.py` & `binance-connector-3.0.0rc2/binance/spot/_bswap.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_c2c.py` & `binance-connector-3.0.0rc2/binance/spot/_c2c.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_convert.py` & `binance-connector-3.0.0rc2/binance/spot/_convert.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_data_stream.py` & `binance-connector-3.0.0rc2/binance/spot/_data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_fiat.py` & `binance-connector-3.0.0rc2/binance/spot/_fiat.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_futures.py` & `binance-connector-3.0.0rc2/binance/spot/_futures.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_gift_card.py` & `binance-connector-3.0.0rc2/binance/spot/_gift_card.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_loan.py` & `binance-connector-3.0.0rc2/binance/spot/_loan.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_margin.py` & `binance-connector-3.0.0rc2/binance/spot/_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_market.py` & `binance-connector-3.0.0rc2/binance/spot/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_mining.py` & `binance-connector-3.0.0rc2/binance/spot/_mining.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_nft.py` & `binance-connector-3.0.0rc2/binance/spot/_nft.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_portfolio_margin.py` & `binance-connector-3.0.0rc2/binance/spot/_portfolio_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_savings.py` & `binance-connector-3.0.0rc2/binance/spot/_savings.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_staking.py` & `binance-connector-3.0.0rc2/binance/spot/_staking.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_sub_account.py` & `binance-connector-3.0.0rc2/binance/spot/_sub_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,87 +670,48 @@
     )
     payload = {"fromEmail": fromEmail, "asset": asset, "amount": amount, **kwargs}
     return self.limited_encoded_sign_request(
         "POST", "/sapi/v1/managed-subaccount/withdraw", payload
     )
 
 
-def sub_account_api_toggle_ip_restriction(
-    self, email: str, subAccountApiKey: str, ipRestrict: bool, **kwargs
+def sub_account_update_ip_restriction(
+    self, email: str, subAccountApiKey: str, status: str, **kwargs
 ):
-    """Enable or Disable IP Restriction for a Sub-account API Key (For Master Account)
+    """Update IP Restriction for Sub-Account API key (For Master Account)
 
-    POST /sapi/v1/sub-account/subAccountApi/ipRestriction
+    POST /sapi/v2/sub-account/subAccountApi/ipRestriction
 
-    https://binance-docs.github.io/apidocs/spot/en/#enable-or-disable-ip-restriction-for-a-sub-account-api-key-for-master-account
+    https://binance-docs.github.io/apidocs/spot/en/#update-ip-restriction-for-sub-account-api-key-for-master-account
 
     Args:
         email (str): Sub-account email
         subAccountApiKey (str)
-        ipRestrict (bool): True or False
+        status (str) : IP Restriction status. 1 = IP Unrestricted. 2 = Restrict access to trusted IPs only.
     Keyword Args:
-        thirdParty (bool, optional): False by default
+        ipAddress (str, optional): Can be added in batches, separated by commas
         recvWindow (int, optional)
     """
 
     check_required_parameters(
         [
             [email, "email"],
             [subAccountApiKey, "subAccountApiKey"],
-            [ipRestrict, "ipRestrict"],
+            [status, "status"],
         ]
     )
     payload = {
         "email": email,
         "subAccountApiKey": subAccountApiKey,
-        "ipRestrict": ipRestrict,
+        "status": status,
         **kwargs,
     }
 
     return self.limited_encoded_sign_request(
-        "POST", "/sapi/v1/sub-account/subAccountApi/ipRestriction", payload
-    )
-
-
-def sub_account_api_add_ip(
-    self, email: str, subAccountApiKey: str, ipAddress: str, **kwargs
-):
-    """Add IP List for a Sub-account API Key (For Master Account)
-
-    Before the usage of this endpoint, please ensure POST /sapi/v1/sub-account/subAccountApi/ipRestriction was used to enable the IP restriction.
-
-    POST /sapi/v1/sub-account/subAccountApi/ipRestriction/ipList
-
-    https://binance-docs.github.io/apidocs/spot/en/#add-ip-list-for-a-sub-account-api-key-for-master-account
-
-    Args:
-        email (str): Sub-account email
-        subAccountApiKey (str)
-        ipAddress (str): Can be added in batches, separated by commas
-    Keyword Args:
-        thirdPartyName (str, optional)
-        recvWindow (int, optional)
-    """
-
-    check_required_parameters(
-        [
-            [email, "email"],
-            [subAccountApiKey, "subAccountApiKey"],
-            [ipAddress, "ipAddress"],
-        ]
-    )
-    payload = {
-        "email": email,
-        "subAccountApiKey": subAccountApiKey,
-        "ipAddress": ipAddress,
-        **kwargs,
-    }
-
-    return self.limited_encoded_sign_request(
-        "POST", "/sapi/v1/sub-account/subAccountApi/ipRestriction/ipList", payload
+        "POST", "/sapi/v2/sub-account/subAccountApi/ipRestriction", payload
     )
 
 
 def sub_account_api_get_ip_restriction(
     self, email: str, subAccountApiKey: str, **kwargs
 ):
     """Get IP Restriction for a Sub-account API Key (For Master Account)
@@ -930,7 +891,39 @@
         "limit": limit,
         **kwargs,
     }
 
     return self.limited_encoded_sign_request(
         "GET", "/sapi/v1/managed-subaccount/queryTransLogForTradeParent", payload
     )
+
+
+def managed_sub_account_deposit_address(self, email: str, coin: str, **kwargs):
+    """Get Managed Sub-account Deposit Address (For Investor Master Account) (USER_DATA)
+
+    GET /sapi/v1/managed-subaccount/deposit/address (HMAC SHA256)
+
+    https://binance-docs.github.io/apidocs/spot/en/#get-managed-sub-account-deposit-address-for-investor-master-account-user_data
+
+    Args:
+        email (str): email
+        coin (str): coin
+    Keyword Args:
+        network (str, optional)
+        recvWindow (int, optional)
+    """
+
+    check_required_parameters(
+        [
+            [email, "email"],
+            [coin, "coin"],
+        ]
+    )
+    payload = {
+        "email": email,
+        "coin": coin,
+        **kwargs,
+    }
+
+    return self.limited_encoded_sign_request(
+        "GET", "/sapi/v1/managed-subaccount/deposit/address", payload
+    )
```

### Comparing `binance-connector-3.0.0rc1/binance/spot/_trade.py` & `binance-connector-3.0.0rc2/binance/spot/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/spot/_wallet.py` & `binance-connector-3.0.0rc2/binance/spot/_wallet.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/binance_socket_manager.py` & `binance-connector-3.0.0rc2/binance/websocket/binance_socket_manager.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/__init__.py` & `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_account.py` & `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_market.py` & `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_trade.py` & `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/spot/websocket_api/_user_data.py` & `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_user_data.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/spot/websocket_stream.py` & `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance/websocket/websocket_client.py` & `binance-connector-3.0.0rc2/binance/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/binance_connector.egg-info/PKG-INFO` & `binance-connector-3.0.0rc2/binance_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-connector-3.0.0rc1/binance_connector.egg-info/SOURCES.txt` & `binance-connector-3.0.0rc2/binance_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc1/setup.py` & `binance-connector-3.0.0rc2/setup.py`

 * *Files identical despite different names*

