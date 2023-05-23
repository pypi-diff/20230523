# Comparing `tmp/cryptos-2.0.7.tar.gz` & `tmp/cryptos-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptos-2.0.7.tar", last modified: Fri May  5 13:14:13 2023, max compression
+gzip compressed data, was "cryptos-2.0.8.tar", last modified: Tue May 23 16:19:10 2023, max compression
```

## Comparing `cryptos-2.0.7.tar` & `cryptos-2.0.8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.229498 cryptos-2.0.7/
--rw-rw-rw-   0        0        0     1293 2022-10-03 10:19:24.000000 cryptos-2.0.7/LICENSE
--rw-rw-rw-   0        0        0      112 2023-05-05 12:53:53.000000 cryptos-2.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    36041 2023-05-05 13:14:13.227497 cryptos-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    35326 2023-05-05 13:08:32.000000 cryptos-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.046558 cryptos-2.0.7/crypto_scripts/
--rw-rw-rw-   0        0        0        0 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/__init__.py
--rw-rw-rw-   0        0        0      889 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/broadcast.py
--rw-rw-rw-   0        0        0     1891 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/convert_private_key.py
--rw-rw-rw-   0        0        0     1472 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/create_private_key.py
--rw-rw-rw-   0        0        0     2987 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/cryptosend.py
--rw-rw-rw-   0        0        0     8917 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/explorer.py
--rw-rw-rw-   0        0        0     1088 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/get_block_sizes.py
--rw-rw-rw-   0        0        0     3471 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/subscribe.py
--rw-rw-rw-   0        0        0     3637 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/view_private_key_addresses.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.091058 cryptos-2.0.7/cryptos/
--rw-rw-rw-   0        0        0      275 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/blocks.py
--rw-rw-rw-   0        0        0     6798 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/cashaddr.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.120321 cryptos-2.0.7/cryptos/coins/
--rw-rw-rw-   0        0        0      153 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/__init__.py
--rw-rw-rw-   0        0        0    16705 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/base.py
--rw-rw-rw-   0        0        0      162 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/bitcoin.py
--rw-rw-rw-   0        0        0      183 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/bitcoin_cash.py
--rw-rw-rw-   0        0        0      147 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/dash.py
--rw-rw-rw-   0        0        0      151 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/dogecoin.py
--rw-rw-rw-   0        0        0      167 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/litecoin.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.136436 cryptos-2.0.7/cryptos/coins_async/
--rw-rw-rw-   0        0        0      124 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/__init__.py
--rw-rw-rw-   0        0        0    50159 2023-04-03 17:25:43.000000 cryptos-2.0.7/cryptos/coins_async/base.py
--rw-rw-rw-   0        0        0     1252 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/bitcoin.py
--rw-rw-rw-   0        0        0     1352 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/bitcoin_cash.py
--rw-rw-rw-   0        0        0      746 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/dash.py
--rw-rw-rw-   0        0        0      931 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/dogecoin.py
--rw-rw-rw-   0        0        0      976 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/litecoin.py
--rw-rw-rw-   0        0        0     1657 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/composite.py
--rw-rw-rw-   0        0        0      402 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/constants.py
--rw-rw-rw-   0        0        0     8911 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/deterministic.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.142500 cryptos-2.0.7/cryptos/electrumx_client/
--rw-rw-rw-   0        0        0       37 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/__init__.py
--rw-rw-rw-   0        0        0    22725 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/client.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.162771 cryptos-2.0.7/cryptos/electrumx_client/servers/
--rw-rw-rw-   0        0        0    10969 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin.json
--rw-rw-rw-   0        0        0     3618 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_cash.json
--rw-rw-rw-   0        0        0     1093 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json
--rw-rw-rw-   0        0        0      936 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_testnet.json
--rw-rw-rw-   0        0        0      384 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/dash.json
--rw-rw-rw-   0        0        0      486 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/dash_testnet.json
--rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/doge.json
--rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/doge_testnet.json
--rw-rw-rw-   0        0        0      973 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/litecoin.json
--rw-rw-rw-   0        0        0      283 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/litecoin_testnet.json
--rw-rw-rw-   0        0        0      257 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/testing.json
--rw-rw-rw-   0        0        0     2400 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/types.py
--rw-rw-rw-   0        0        0    15164 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/english.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.182148 cryptos-2.0.7/cryptos/explorers/
--rw-rw-rw-   0        0        0      644 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/explorers/base_insight.py
--rw-rw-rw-   0        0        0      338 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/bitpay.py
--rw-rw-rw-   0        0        0     4045 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/explorers/blockchain.py
--rw-rw-rw-   0        0        0     1074 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/blockcypher.py
--rw-rw-rw-   0        0        0     1280 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/blockdozer.py
--rw-rw-rw-   0        0        0     1264 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/btg_explorer.py
--rw-rw-rw-   0        0        0     1242 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/dash_siampm.py
--rw-rw-rw-   0        0        0     3047 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/sochain.py
--rw-rw-rw-   0        0        0      559 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/utils.py
--rw-rw-rw-   0        0        0    18584 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/keystore.py
--rw-rw-rw-   0        0        0    19302 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/main.py
--rw-rw-rw-   0        0        0     8436 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/mnemonic.py
--rw-rw-rw-   0        0        0     2838 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/opcodes.py
--rw-rw-rw-   0        0        0     3494 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/py3specials.py
--rw-rw-rw-   0        0        0    15159 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/ripemd.py
--rw-rw-rw-   0        0        0      364 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/script_utils.py
--rw-rw-rw-   0        0        0     6099 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/segwit_addr.py
--rw-rw-rw-   0        0        0     3777 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/stealth.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.187822 cryptos-2.0.7/cryptos/testing/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/testing/__init__.py
--rw-rw-rw-   0        0        0    33902 2023-04-03 12:02:39.000000 cryptos-2.0.7/cryptos/testing/testcases.py
--rw-rw-rw-   0        0        0    56461 2023-04-03 12:02:39.000000 cryptos-2.0.7/cryptos/testing/testcases_async.py
--rw-rw-rw-   0        0        0    21694 2023-04-03 17:25:43.000000 cryptos-2.0.7/cryptos/transaction.py
--rw-rw-rw-   0        0        0     2414 2023-04-03 17:25:43.000000 cryptos-2.0.7/cryptos/types.py
--rw-rw-rw-   0        0        0     2040 2023-03-24 21:15:30.000000 cryptos-2.0.7/cryptos/utils.py
--rw-rw-rw-   0        0        0    12253 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/wallet.py
--rw-rw-rw-   0        0        0     6746 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/wallet_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.105193 cryptos-2.0.7/cryptos.egg-info/
--rw-rw-rw-   0        0        0    36041 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3093 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      438 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 13:14:13.229498 cryptos-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1801 2023-05-05 12:51:31.000000 cryptos-2.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.199933 cryptos-2.0.7/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/__init__.py
--rw-rw-rw-   0        0        0     5596 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/electrum_subscribe_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.204117 cryptos-2.0.7/tests/test_coins/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins/__init__.py
--rw-rw-rw-   0        0        0    13157 2023-04-03 13:33:46.000000 cryptos-2.0.7/tests/test_coins/test_bitcoin_testnet.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.224498 cryptos-2.0.7/tests/test_coins_async/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/__init__.py
--rw-rw-rw-   0        0        0    16130 2023-04-03 17:25:43.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin.py
--rw-rw-rw-   0        0        0    11403 2023-03-24 22:06:15.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash.py
--rw-rw-rw-   0        0        0     8815 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash_testnet.py
--rw-rw-rw-   0        0        0    10667 2023-04-03 12:02:39.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin_testnet.py
--rw-rw-rw-   0        0        0     5932 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_dash.py
--rw-rw-rw-   0        0        0     5829 2023-04-03 12:02:39.000000 cryptos-2.0.7/tests/test_coins_async/test_dash_testnet.py
--rw-rw-rw-   0        0        0     7355 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_dogecoin.py
--rw-rw-rw-   0        0        0     5694 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_dogecoin_testnet.py
--rw-rw-rw-   0        0        0    13843 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_litecoin.py
--rw-rw-rw-   0        0        0     9245 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_litecoin_testnet.py
--rw-rw-rw-   0        0        0    26157 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_electrum_client.py
--rw-rw-rw-   0        0        0    28702 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_general.py
--rw-rw-rw-   0        0        0     4366 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_stealth.py
--rw-rw-rw-   0        0        0    32352 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_wallet.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.468214 cryptos-2.0.8/
+-rw-rw-rw-   0        0        0     1293 2022-10-03 10:19:24.000000 cryptos-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-05-05 12:53:53.000000 cryptos-2.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    41635 2023-05-23 16:19:10.468214 cryptos-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    40920 2023-05-23 16:18:56.000000 cryptos-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.256192 cryptos-2.0.8/crypto_scripts/
+-rw-rw-rw-   0        0        0        0 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/__init__.py
+-rw-rw-rw-   0        0        0      889 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/broadcast.py
+-rw-rw-rw-   0        0        0     1888 2023-05-23 16:18:56.000000 cryptos-2.0.8/crypto_scripts/convert_private_key.py
+-rw-rw-rw-   0        0        0     1472 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/create_private_key.py
+-rw-rw-rw-   0        0        0     2987 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/cryptosend.py
+-rw-rw-rw-   0        0        0     8914 2023-05-23 16:18:56.000000 cryptos-2.0.8/crypto_scripts/explorer.py
+-rw-rw-rw-   0        0        0     1088 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/get_block_sizes.py
+-rw-rw-rw-   0        0        0     3471 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/subscribe.py
+-rw-rw-rw-   0        0        0     3631 2023-05-23 16:18:56.000000 cryptos-2.0.8/crypto_scripts/view_private_key_addresses.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.299362 cryptos-2.0.8/cryptos/
+-rw-rw-rw-   0        0        0      275 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/blocks.py
+-rw-rw-rw-   0        0        0     6798 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/cashaddr.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.324510 cryptos-2.0.8/cryptos/coins/
+-rw-rw-rw-   0        0        0      153 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/__init__.py
+-rw-rw-rw-   0        0        0    18357 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/coins/base.py
+-rw-rw-rw-   0        0        0      162 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/bitcoin.py
+-rw-rw-rw-   0        0        0      183 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/bitcoin_cash.py
+-rw-rw-rw-   0        0        0      147 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/dash.py
+-rw-rw-rw-   0        0        0      151 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/dogecoin.py
+-rw-rw-rw-   0        0        0      167 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/litecoin.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.340786 cryptos-2.0.8/cryptos/coins_async/
+-rw-rw-rw-   0        0        0      124 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/__init__.py
+-rw-rw-rw-   0        0        0    50144 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/coins_async/base.py
+-rw-rw-rw-   0        0        0     1252 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/bitcoin.py
+-rw-rw-rw-   0        0        0     1352 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/bitcoin_cash.py
+-rw-rw-rw-   0        0        0      746 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/dash.py
+-rw-rw-rw-   0        0        0      931 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/dogecoin.py
+-rw-rw-rw-   0        0        0      976 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/litecoin.py
+-rw-rw-rw-   0        0        0     1657 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/composite.py
+-rw-rw-rw-   0        0        0      402 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/constants.py
+-rw-rw-rw-   0        0        0     8911 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/deterministic.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.340786 cryptos-2.0.8/cryptos/electrumx_client/
+-rw-rw-rw-   0        0        0       37 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/__init__.py
+-rw-rw-rw-   0        0        0    22725 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/client.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.356047 cryptos-2.0.8/cryptos/electrumx_client/servers/
+-rw-rw-rw-   0        0        0    10969 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin.json
+-rw-rw-rw-   0        0        0     3618 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash.json
+-rw-rw-rw-   0        0        0     1093 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json
+-rw-rw-rw-   0        0        0      936 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_testnet.json
+-rw-rw-rw-   0        0        0      384 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/dash.json
+-rw-rw-rw-   0        0        0      486 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/dash_testnet.json
+-rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/doge.json
+-rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/doge_testnet.json
+-rw-rw-rw-   0        0        0      973 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/litecoin.json
+-rw-rw-rw-   0        0        0      283 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/litecoin_testnet.json
+-rw-rw-rw-   0        0        0      257 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/testing.json
+-rw-rw-rw-   0        0        0     2400 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/types.py
+-rw-rw-rw-   0        0        0    15164 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/english.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.368055 cryptos-2.0.8/cryptos/explorers/
+-rw-rw-rw-   0        0        0      644 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/explorers/base_insight.py
+-rw-rw-rw-   0        0        0      338 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/bitpay.py
+-rw-rw-rw-   0        0        0     4045 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/explorers/blockchain.py
+-rw-rw-rw-   0        0        0     1074 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/blockcypher.py
+-rw-rw-rw-   0        0        0     1280 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/blockdozer.py
+-rw-rw-rw-   0        0        0     1264 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/btg_explorer.py
+-rw-rw-rw-   0        0        0     1242 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/dash_siampm.py
+-rw-rw-rw-   0        0        0     3047 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/sochain.py
+-rw-rw-rw-   0        0        0      559 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/utils.py
+-rw-rw-rw-   0        0        0    18584 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/keystore.py
+-rw-rw-rw-   0        0        0    19302 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/main.py
+-rw-rw-rw-   0        0        0     8436 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/mnemonic.py
+-rw-rw-rw-   0        0        0     2838 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/opcodes.py
+-rw-rw-rw-   0        0        0     3494 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/py3specials.py
+-rw-rw-rw-   0        0        0    15159 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/ripemd.py
+-rw-rw-rw-   0        0        0      364 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/script_utils.py
+-rw-rw-rw-   0        0        0     6099 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/segwit_addr.py
+-rw-rw-rw-   0        0        0     3777 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/stealth.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.385707 cryptos-2.0.8/cryptos/testing/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/testing/__init__.py
+-rw-rw-rw-   0        0        0    33904 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/testing/testcases.py
+-rw-rw-rw-   0        0        0    56457 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/testing/testcases_async.py
+-rw-rw-rw-   0        0        0    21694 2023-04-03 17:25:43.000000 cryptos-2.0.8/cryptos/transaction.py
+-rw-rw-rw-   0        0        0     2414 2023-04-03 17:25:43.000000 cryptos-2.0.8/cryptos/types.py
+-rw-rw-rw-   0        0        0     2040 2023-03-24 21:15:30.000000 cryptos-2.0.8/cryptos/utils.py
+-rw-rw-rw-   0        0        0    12247 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/wallet.py
+-rw-rw-rw-   0        0        0     6746 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/wallet_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.316905 cryptos-2.0.8/cryptos.egg-info/
+-rw-rw-rw-   0        0        0    41635 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3093 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      438 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 16:19:10.468214 cryptos-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1801 2023-05-23 16:18:56.000000 cryptos-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.401375 cryptos-2.0.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     5596 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/electrum_subscribe_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.401375 cryptos-2.0.8/tests/test_coins/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins/__init__.py
+-rw-rw-rw-   0        0        0    13157 2023-04-03 13:33:46.000000 cryptos-2.0.8/tests/test_coins/test_bitcoin_testnet.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.468214 cryptos-2.0.8/tests/test_coins_async/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/__init__.py
+-rw-rw-rw-   0        0        0    16130 2023-04-03 17:25:43.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin.py
+-rw-rw-rw-   0        0        0    11403 2023-03-24 22:06:15.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash.py
+-rw-rw-rw-   0        0        0     8815 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash_testnet.py
+-rw-rw-rw-   0        0        0    10667 2023-04-03 12:02:39.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin_testnet.py
+-rw-rw-rw-   0        0        0     5932 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_dash.py
+-rw-rw-rw-   0        0        0     5829 2023-04-03 12:02:39.000000 cryptos-2.0.8/tests/test_coins_async/test_dash_testnet.py
+-rw-rw-rw-   0        0        0     7355 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_dogecoin.py
+-rw-rw-rw-   0        0        0     5694 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_dogecoin_testnet.py
+-rw-rw-rw-   0        0        0    14402 2023-05-23 16:18:56.000000 cryptos-2.0.8/tests/test_coins_async/test_litecoin.py
+-rw-rw-rw-   0        0        0     9245 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_litecoin_testnet.py
+-rw-rw-rw-   0        0        0    26157 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_electrum_client.py
+-rw-rw-rw-   0        0        0    28702 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_general.py
+-rw-rw-rw-   0        0        0     4366 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_stealth.py
+-rw-rw-rw-   0        0        0    32352 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_wallet.py
```

### Comparing `cryptos-2.0.7/LICENSE` & `cryptos-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/PKG-INFO` & `cryptos-2.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: cryptos
-Version: 2.0.7
-Summary: Python Crypto Coin Tools
-Home-page: http://github.com/primal100/pybitcointools
-Author: Paul Martin
-Author-email: greatestloginnameever@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Security :: Cryptography
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Pycryptotools, Python library for Crypto coins signatures and transactions
 
 This is a fork of Vitalik Buterin's original [pybitcointools](https://github.com/vbuterin/pybitcointools) library.
 
 After a lot of work, the library is finally active again and being actively updated. This took a lot of work and unfortunately some backward imcompatible changes may have been introduced in v2. If you run into issues after upgrading open an issue and will try to help. If it's reasonable to do so we can consider restoring the previous behaviour in v2, otherwise will assist with migration.
 
 Installation:
@@ -502,40 +483,101 @@
 
 The arguments are the private key of the sender, the receiver's address and the fee (default 10000). Change will be returned to the sender. 
 
 ### Listing of main coin-specific methods:
 
 * privtopub            : (privkey) -> pubkey
 * pubtoaddr            : (pubkey) -> address
-* privtoaddr           : (privkey) -> address
+* privtoaddr           : (privkey) -> Convert a wif encoded private key to correct address, if not wif encoded then p2pkh
+* privtop2pkh          : (privkey) -> p2pkh address
 * encode_privkey       : (privkey, format, script_type="p2pkh") -> privkey
 * sign                 : (txobj, i, privkey) -> create digital signature of tx with privkey and add to input i
 * signall              : (txobj, privkey) -> create digital signature of tx with privkey for all inputs
-* history              : (address, merkle_proof=False) -> tx history and balance of an address
+* history              : (address, merkle_proof=False) -> tx history of an address
+* get_histories        : (*addresses, merkle_proof=False) -> tx histories of an address
 * unspent              : (address, merkle_proof=False) -> unspent outputs for an addresses
-* pushtx               : (hex or bin tx) -> push a transaction to the blockchain
-* get_tx               : (txhash) -> fetch a tx from the blockchain
+* get_unspents         : (addresses, merkle_proof=False) -> unspent outputs for multiple addresses
+* pushtx               : (hex or tx object) -> push a transaction to the blockchain
+* get_raw_tx           : (txid) -> Get the raw hex of a transaction id
+* get_tx               : (txid) -> fetch a tx from the blockchain
+* get_verbose_tx       : (txid) -> Transaction details verbose output
+* get_txs              : (*txids) -> Fetch multiple transaction details
+* calculate_fee        : (Tx) -> Calculate the fee of a transaction
 * send                 : (privkey, frm, to, value, change_addr=None, fee=None, estimate_fee_blocks: int = 6) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
 * send_to_multiple_receivers_tx          : (privkey, addr outs:value pairs, change_addr=None,fee=10000,, estimate_fee_blocks: int = 6) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
 * preparetx            : (frm, to, value, fee, estimate_fee_blocks: int = 6,change_addr=None): -> create unsigned txobj with change output
 * preparemultitx       : (frm, outs:value pairs, change_addr=None, fee=None, estimate_fee_blocks: int = 6): -> create unsigned txobj with multiple outputs and additional change output
 * preparesignedtx      : (privkey, frm, to, value, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with change output
 * preparesignedmultirecipienttx : (privkey, frm, outs: value pairs, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with multiple outputs and additional change output
-* mktx                 : (inputs, outputs, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
+* mktx                 : (inputs, outputs, locktifme=0, sequence=0xFFFFFFFF) -> create unsigned txobj
 * mktx_with_change     : (inputs, outputs, change_addr=None, fee=None, estimate_fee_blocks=6, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
-* mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multsig script and address pubkeys
+* mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multisig script and address
+* multisign            : (txobj, i, script, privkey) -> signature
+* apply_multisignatures: (txobj, i, script, sigs) -> tx with index i signed with sigs
+* mk_multsig_segwit_address : (pubkeys, M)- Returns both M-of-N multisig script and native segwit address
+* mk_multsig_cash_address: (pubkeys, M)- Returns both M-of-N multisig script and Bitcoin Cash address
 * pubtop2w             : (pub) -> pay to witness script hash (segwit address)
 * privtop2w            : (priv) -> pay to witness script hash (segwit address)
+* pubtop2wpkh_p2sh     : (pub) -> Convert a public key to a segwit address encoded in a p2sh script
+* privtop2wpkh_p2sh    : (priv) -> Convert a private key to a segwit address encoded in a p2sh script
+* hash_to_segwit_addr  : (hash) -. Convert a public key hash to a native segwit address
+* scripthash_to_segwit_addr: (hash) -> Convert the hash of a p2sh script to a native segwit address
 * is_address           : (addr) -> true if addr is a valid address for this network
+* is_p2pkh              : (address) -> Return true if an address is in p2pkh format
 * is_p2sh              : (addr) -> true if addr is a pay to script hash for this network
 * is_segwit            : (priv, addr) -> true if priv-addr pair represent a pay to witness script hash
+* is_cash_or_legacy_p2pkh_address : (address) -> Returns true if an address is a legacy p2pkh address or a Bitcoin Cash formatted p2pkh address
+* is_native_segwit      : (address) -> Returns true if an address is of native segwit type
+* is_cash_address       : (address) -> Returns true if an address is of Bitcoin Cash address format
+* maybe_legacy_segwit   : (address) -> Returns true if address is likely a legacy segwit p2sh address
+* is_p2wsh              : (address) -> Returns true is address is a Pay To Witness Script Address
+* is_segwit_or_p2sh     : (address) -> Returns true if an address is a Pay to Witness or Pay to Script address
 * current_block_height : () -> Latest block height
 * block_height         : (txhash) -> Block height containing the txhash
 * inspect              : (tx_hex) -> Deserialize a transaction and decode and ins and outs
 * merkle_prove         : (txhash) -> Proves a transaction is valid and returns txhash, merkle siblings and block header.
+* estimate_fee_per_kb  : (numblocks) -> Get estimated fee kb to get transaction confirmed within numblocks number of blocks
+* tx_size              : (tx) -> Estimate final transaction size of an unsigned transaction
+* estimate_fee         : (tx, numblocks=6) -> Estimate required fee of an unsigned transaction
+* raw_block_header     : (height) -> Get the raw data of a block header
+* block_header         : (height) -> Get the decoded details of a block header
+* block_headers        : (*heights) -> Get a list of decoded block headers
+* subscribe_to_block_headers: (callback(height, raw_header, decoded_header)) -> Run a callback whenever a new block is added to the blockchain
+* unsubscribe_from_block_headers: () -> Remove all subscriptions to block headers
+* confirmations        : (height) -> Number of confirmations a transaction at this height has
+* subscribe_to_address : (callback(addr, status), addr) -> Run a callback every time there is an activity on an address
+* subscribe_to_address_transactions : (callback(address: str, txs, newly_confirmed, history, unspent, confirmed, unconfirmed, proven), addr) -> Run a callback every time there is an activity on an address with details transaction and balance information already retrieved
+* unsubscribe_from_address: (addr) -> Remove all subscriptions for this address
+* get_balance           : (addr) -> Get the balance, confirmed and unconfirmed, for an address
+* get_balances          : (*addrs) -> Get the balance, confirmed and unconfirmed, for multiple addresses
+* get_merkle            : (tx) -> Get the merkle root of a transaction
+* merkle_prove          : (tx) -> Prove a transaction is valid
+* merkle_prove_by_txid  : (txid) -> Prove a transaction id is valid
+* balance_merkle_proven : (addr) -> Get the merkle proven balance for an address
+* balance_merkle_proven : (*addrs) -> Get the merkle proven balance for multiple addresses
+* get_address_variations: (addr) -> Return alternative formats for an address (e.g. Standard + Bitcoin Cash address)
+* pub_is_for_p2pkh_addr : (pub, addr) -> Returns true if the p2pkh address for pub is addr
+* wiftoaddr             : (priv) -> Convert a private key in WIF format to the correct address type
+* electrum_address      : (masterkey, n, for_change) -> Electrum Address (for old Electrum seeds)
+* encode_privkey        : (privkey, format, script_type) -> Convert a private key to a different format or script types
+* output_script_to_address : (script) -> Convert an output script to an address
+* scripttoaddr          : (script)  -> Convert an input script to an address 
+* addrtoscript          : (address) -> Convert an address to an output script
+* addrtoscripthash      : (address) -> Convert an address to scripthash as required by ElectrumX servers
+* p2sh_scriptaddr       : (script) -> Convert an output P2SH script to a P2SH address
+* p2sh_segwit_addr      : (script) -> Convert an output P2SH script to a native segwit P2WSH address
+* pubtosegwitaddress    : (pub) -> Convert a public key to a native segwit address
+* privtosegwitaddress   : (priv) -> Convert a private key to a native segwit address
+* scripthash_to_cash_addr: (scripthash) -> Convert a scripthash to a Bitcoin Cash address
+* pubtocashaddress      : (pub) -> Convert a public key to a Bitcoin Cash address
+* privtocashaddress     : (priv) -> Convert a private key to a Bitcoin Cash address 
+* p2sh_cash_addr        : (script) -> Convert an script to a Bitcoin Cash address
+* hash_to_cash_addr     : (hash) -> Convert the hash of a p2sh script to a Bitcoin Cash address
+* legacy_addr_to_cash_address: (addr) -> Convert a legacy P2PKH address to a Bitcoin Cash address
+* cash_address_to_legacy_addr: (addr) -> Convert a Bitcoin Cash address to a legalcy P2PKH address
 
 ### Listing of main non-coin specific commands:
 
 * add                  : (key1, key2) -> key1 + key2 (works on privkeys or pubkeys)
 * multiply             : (pubkey, privkey) -> returns pubkey * privkey
 
 * ecdsa_sign           : (message, privkey) -> sig
@@ -553,19 +595,15 @@
 * bip32_master_key     : (seed) -> bip32 master key
 * bip32_ckd            : (private or public bip32 key, i) -> child key
 * bip32_privtopub      : (private bip32 key) -> public bip32 key
 * bip32_extract_key    : (private or public bip32_key) -> privkey or pubkey
 
 * deserialize          : (hex or bin transaction) -> JSON tx
 * serialize            : (JSON tx) -> hex or bin tx
-* multisign            : (txobj, i, script, privkey) -> signature
-* apply_multisignatures: (txobj, i, script, sigs) -> tx with index i signed with sigs
-* scriptaddr           : (script) -> P2SH address
-* mk_multisig_script   : (pubkeys, M) -> M-of-N multisig script from pubkeys
-* verify_tx_input      : (tx, i, script, sig, pub) -> True/False
+s* verify_tx_input      : (tx, i, script, sig, pub) -> True/False
 * tx_hash              : (hex or bin tx) -> hash
 
 * access               : (json list/object, prop) -> desired property of that json object
 * multiaccess          : (json list, prop) -> like access, but mapped across each list element
 * slice                : (json list, start, end) -> given slice of the list
 * count                : (json list) -> number of elements
 * sum                  : (json list) -> sum of all values
@@ -578,8 +616,8 @@
 on the mainnet. The original pybitcointools had issues opened in Github where people lost money either due to 
 not understanding what they were doing or because of bugs. 
 
 
 ### Working together
 
 If you wish to work together on crypto or other software related projects you can contact me using social links on my Github profile.
-I can very easily and quickly build software tools on top of this pybitcointools library.
+I can very easily and quickly build software tools on top of this pybitcointools library.
```

### Comparing `cryptos-2.0.7/README.md` & `cryptos-2.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: cryptos
+Version: 2.0.8
+Summary: Python Crypto Coin Tools
+Home-page: http://github.com/primal100/pybitcointools
+Author: Paul Martin
+Author-email: greatestloginnameever@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Security :: Cryptography
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Pycryptotools, Python library for Crypto coins signatures and transactions
 
 This is a fork of Vitalik Buterin's original [pybitcointools](https://github.com/vbuterin/pybitcointools) library.
 
 After a lot of work, the library is finally active again and being actively updated. This took a lot of work and unfortunately some backward imcompatible changes may have been introduced in v2. If you run into issues after upgrading open an issue and will try to help. If it's reasonable to do so we can consider restoring the previous behaviour in v2, otherwise will assist with migration.
 
 Installation:
@@ -483,40 +502,101 @@
 
 The arguments are the private key of the sender, the receiver's address and the fee (default 10000). Change will be returned to the sender. 
 
 ### Listing of main coin-specific methods:
 
 * privtopub            : (privkey) -> pubkey
 * pubtoaddr            : (pubkey) -> address
-* privtoaddr           : (privkey) -> address
+* privtoaddr           : (privkey) -> Convert a wif encoded private key to correct address, if not wif encoded then p2pkh
+* privtop2pkh          : (privkey) -> p2pkh address
 * encode_privkey       : (privkey, format, script_type="p2pkh") -> privkey
 * sign                 : (txobj, i, privkey) -> create digital signature of tx with privkey and add to input i
 * signall              : (txobj, privkey) -> create digital signature of tx with privkey for all inputs
-* history              : (address, merkle_proof=False) -> tx history and balance of an address
+* history              : (address, merkle_proof=False) -> tx history of an address
+* get_histories        : (*addresses, merkle_proof=False) -> tx histories of an address
 * unspent              : (address, merkle_proof=False) -> unspent outputs for an addresses
-* pushtx               : (hex or bin tx) -> push a transaction to the blockchain
-* get_tx               : (txhash) -> fetch a tx from the blockchain
+* get_unspents         : (addresses, merkle_proof=False) -> unspent outputs for multiple addresses
+* pushtx               : (hex or tx object) -> push a transaction to the blockchain
+* get_raw_tx           : (txid) -> Get the raw hex of a transaction id
+* get_tx               : (txid) -> fetch a tx from the blockchain
+* get_verbose_tx       : (txid) -> Transaction details verbose output
+* get_txs              : (*txids) -> Fetch multiple transaction details
+* calculate_fee        : (Tx) -> Calculate the fee of a transaction
 * send                 : (privkey, frm, to, value, change_addr=None, fee=None, estimate_fee_blocks: int = 6) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
 * send_to_multiple_receivers_tx          : (privkey, addr outs:value pairs, change_addr=None,fee=10000,, estimate_fee_blocks: int = 6) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
 * preparetx            : (frm, to, value, fee, estimate_fee_blocks: int = 6,change_addr=None): -> create unsigned txobj with change output
 * preparemultitx       : (frm, outs:value pairs, change_addr=None, fee=None, estimate_fee_blocks: int = 6): -> create unsigned txobj with multiple outputs and additional change output
 * preparesignedtx      : (privkey, frm, to, value, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with change output
 * preparesignedmultirecipienttx : (privkey, frm, outs: value pairs, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with multiple outputs and additional change output
-* mktx                 : (inputs, outputs, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
+* mktx                 : (inputs, outputs, locktifme=0, sequence=0xFFFFFFFF) -> create unsigned txobj
 * mktx_with_change     : (inputs, outputs, change_addr=None, fee=None, estimate_fee_blocks=6, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
-* mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multsig script and address pubkeys
+* mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multisig script and address
+* multisign            : (txobj, i, script, privkey) -> signature
+* apply_multisignatures: (txobj, i, script, sigs) -> tx with index i signed with sigs
+* mk_multsig_segwit_address : (pubkeys, M)- Returns both M-of-N multisig script and native segwit address
+* mk_multsig_cash_address: (pubkeys, M)- Returns both M-of-N multisig script and Bitcoin Cash address
 * pubtop2w             : (pub) -> pay to witness script hash (segwit address)
 * privtop2w            : (priv) -> pay to witness script hash (segwit address)
+* pubtop2wpkh_p2sh     : (pub) -> Convert a public key to a segwit address encoded in a p2sh script
+* privtop2wpkh_p2sh    : (priv) -> Convert a private key to a segwit address encoded in a p2sh script
+* hash_to_segwit_addr  : (hash) -. Convert a public key hash to a native segwit address
+* scripthash_to_segwit_addr: (hash) -> Convert the hash of a p2sh script to a native segwit address
 * is_address           : (addr) -> true if addr is a valid address for this network
+* is_p2pkh              : (address) -> Return true if an address is in p2pkh format
 * is_p2sh              : (addr) -> true if addr is a pay to script hash for this network
 * is_segwit            : (priv, addr) -> true if priv-addr pair represent a pay to witness script hash
+* is_cash_or_legacy_p2pkh_address : (address) -> Returns true if an address is a legacy p2pkh address or a Bitcoin Cash formatted p2pkh address
+* is_native_segwit      : (address) -> Returns true if an address is of native segwit type
+* is_cash_address       : (address) -> Returns true if an address is of Bitcoin Cash address format
+* maybe_legacy_segwit   : (address) -> Returns true if address is likely a legacy segwit p2sh address
+* is_p2wsh              : (address) -> Returns true is address is a Pay To Witness Script Address
+* is_segwit_or_p2sh     : (address) -> Returns true if an address is a Pay to Witness or Pay to Script address
 * current_block_height : () -> Latest block height
 * block_height         : (txhash) -> Block height containing the txhash
 * inspect              : (tx_hex) -> Deserialize a transaction and decode and ins and outs
 * merkle_prove         : (txhash) -> Proves a transaction is valid and returns txhash, merkle siblings and block header.
+* estimate_fee_per_kb  : (numblocks) -> Get estimated fee kb to get transaction confirmed within numblocks number of blocks
+* tx_size              : (tx) -> Estimate final transaction size of an unsigned transaction
+* estimate_fee         : (tx, numblocks=6) -> Estimate required fee of an unsigned transaction
+* raw_block_header     : (height) -> Get the raw data of a block header
+* block_header         : (height) -> Get the decoded details of a block header
+* block_headers        : (*heights) -> Get a list of decoded block headers
+* subscribe_to_block_headers: (callback(height, raw_header, decoded_header)) -> Run a callback whenever a new block is added to the blockchain
+* unsubscribe_from_block_headers: () -> Remove all subscriptions to block headers
+* confirmations        : (height) -> Number of confirmations a transaction at this height has
+* subscribe_to_address : (callback(addr, status), addr) -> Run a callback every time there is an activity on an address
+* subscribe_to_address_transactions : (callback(address: str, txs, newly_confirmed, history, unspent, confirmed, unconfirmed, proven), addr) -> Run a callback every time there is an activity on an address with details transaction and balance information already retrieved
+* unsubscribe_from_address: (addr) -> Remove all subscriptions for this address
+* get_balance           : (addr) -> Get the balance, confirmed and unconfirmed, for an address
+* get_balances          : (*addrs) -> Get the balance, confirmed and unconfirmed, for multiple addresses
+* get_merkle            : (tx) -> Get the merkle root of a transaction
+* merkle_prove          : (tx) -> Prove a transaction is valid
+* merkle_prove_by_txid  : (txid) -> Prove a transaction id is valid
+* balance_merkle_proven : (addr) -> Get the merkle proven balance for an address
+* balance_merkle_proven : (*addrs) -> Get the merkle proven balance for multiple addresses
+* get_address_variations: (addr) -> Return alternative formats for an address (e.g. Standard + Bitcoin Cash address)
+* pub_is_for_p2pkh_addr : (pub, addr) -> Returns true if the p2pkh address for pub is addr
+* wiftoaddr             : (priv) -> Convert a private key in WIF format to the correct address type
+* electrum_address      : (masterkey, n, for_change) -> Electrum Address (for old Electrum seeds)
+* encode_privkey        : (privkey, format, script_type) -> Convert a private key to a different format or script types
+* output_script_to_address : (script) -> Convert an output script to an address
+* scripttoaddr          : (script)  -> Convert an input script to an address 
+* addrtoscript          : (address) -> Convert an address to an output script
+* addrtoscripthash      : (address) -> Convert an address to scripthash as required by ElectrumX servers
+* p2sh_scriptaddr       : (script) -> Convert an output P2SH script to a P2SH address
+* p2sh_segwit_addr      : (script) -> Convert an output P2SH script to a native segwit P2WSH address
+* pubtosegwitaddress    : (pub) -> Convert a public key to a native segwit address
+* privtosegwitaddress   : (priv) -> Convert a private key to a native segwit address
+* scripthash_to_cash_addr: (scripthash) -> Convert a scripthash to a Bitcoin Cash address
+* pubtocashaddress      : (pub) -> Convert a public key to a Bitcoin Cash address
+* privtocashaddress     : (priv) -> Convert a private key to a Bitcoin Cash address 
+* p2sh_cash_addr        : (script) -> Convert an script to a Bitcoin Cash address
+* hash_to_cash_addr     : (hash) -> Convert the hash of a p2sh script to a Bitcoin Cash address
+* legacy_addr_to_cash_address: (addr) -> Convert a legacy P2PKH address to a Bitcoin Cash address
+* cash_address_to_legacy_addr: (addr) -> Convert a Bitcoin Cash address to a legalcy P2PKH address
 
 ### Listing of main non-coin specific commands:
 
 * add                  : (key1, key2) -> key1 + key2 (works on privkeys or pubkeys)
 * multiply             : (pubkey, privkey) -> returns pubkey * privkey
 
 * ecdsa_sign           : (message, privkey) -> sig
@@ -534,19 +614,15 @@
 * bip32_master_key     : (seed) -> bip32 master key
 * bip32_ckd            : (private or public bip32 key, i) -> child key
 * bip32_privtopub      : (private bip32 key) -> public bip32 key
 * bip32_extract_key    : (private or public bip32_key) -> privkey or pubkey
 
 * deserialize          : (hex or bin transaction) -> JSON tx
 * serialize            : (JSON tx) -> hex or bin tx
-* multisign            : (txobj, i, script, privkey) -> signature
-* apply_multisignatures: (txobj, i, script, sigs) -> tx with index i signed with sigs
-* scriptaddr           : (script) -> P2SH address
-* mk_multisig_script   : (pubkeys, M) -> M-of-N multisig script from pubkeys
-* verify_tx_input      : (tx, i, script, sig, pub) -> True/False
+s* verify_tx_input      : (tx, i, script, sig, pub) -> True/False
 * tx_hash              : (hex or bin tx) -> hash
 
 * access               : (json list/object, prop) -> desired property of that json object
 * multiaccess          : (json list, prop) -> like access, but mapped across each list element
 * slice                : (json list, start, end) -> given slice of the list
 * count                : (json list) -> number of elements
 * sum                  : (json list) -> sum of all values
@@ -559,8 +635,8 @@
 on the mainnet. The original pybitcointools had issues opened in Github where people lost money either due to 
 not understanding what they were doing or because of bugs. 
 
 
 ### Working together
 
 If you wish to work together on crypto or other software related projects you can contact me using social links on my Github profile.
-I can very easily and quickly build software tools on top of this pybitcointools library.
+I can very easily and quickly build software tools on top of this pybitcointools library.
```

### Comparing `cryptos-2.0.7/crypto_scripts/broadcast.py` & `cryptos-2.0.8/crypto_scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/crypto_scripts/convert_private_key.py` & `cryptos-2.0.8/crypto_scripts/convert_private_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     print(f'Private key {output_format_str} format: {encoded_priv_key}')
     public_key = privtopub(encoded_priv_key)
     print(f'Public key: {public_key}')
     if script_type == "p2pkh":
         address = coin.pubtoaddr(public_key)
         print(f'P2PKH Address: {address}')
     elif script_type == "p2wpkh" and coin.segwit_supported:
-        native_segwit_address = coin.pub_to_segwit_address(public_key)
+        native_segwit_address = coin.pubtosegwitaddress(public_key)
         print(f'P2WPKH Native Segwit address: {native_segwit_address}')
     elif script_type == "p2wpkh-p2sh" and coin.segwit_supported:
         p2pkhw_p2sh = coin.pubtop2wpkh_p2sh(public_key)
         print(f'P2PKHW_P2SH Address: {p2pkhw_p2sh}')
 
 
 if __name__ == "__main__":
```

### Comparing `cryptos-2.0.7/crypto_scripts/create_private_key.py` & `cryptos-2.0.8/crypto_scripts/create_private_key.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/crypto_scripts/cryptosend.py` & `cryptos-2.0.8/crypto_scripts/cryptosend.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/crypto_scripts/explorer.py` & `cryptos-2.0.8/crypto_scripts/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     if witness := inp.get('txinwitness'):
         pubkey_or_script = witness[-1]
         if coin.is_p2wsh(address):
             return coin.p2sh_segwit_addr(pubkey_or_script) == address
         elif coin.is_segwit_or_p2sh(address):
             if is_pubkey(pubkey_or_script):
                 return any(addr == address for addr in (                                    # P2W
-                    coin.pub_to_segwit_address(pubkey_or_script),
+                    coin.pubtosegwitaddress(pubkey_or_script),
                     coin.pubtop2wpkh_p2sh(pubkey_or_script),
                 ))
         return False
     elif scriptSig := inp.get('scriptSig', {}).get('hex'):
         if scriptSig.startswith('00'):
             script = script_sig_script(scriptSig)
             if coin.is_p2sh(address):
```

### Comparing `cryptos-2.0.7/crypto_scripts/get_block_sizes.py` & `cryptos-2.0.8/crypto_scripts/get_block_sizes.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/crypto_scripts/subscribe.py` & `cryptos-2.0.8/crypto_scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/crypto_scripts/view_private_key_addresses.py` & `cryptos-2.0.8/crypto_scripts/view_private_key_addresses.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         native_segwit_address = coin.privtosegwitaddress(p2wpkh_wif)
         native_segwit_compressed_address = coin.privtosegwitaddress(p2wpkh_wif_compressed)
 
         print(f'P2WPKH Native Segwit Address: {native_segwit_address}')
 
         assert native_segwit_address == native_segwit_compressed_address
 
-        native_segwit_address2 = coin.pub_to_segwit_address(public_key)
-        native_segwit_compressed_address2 = coin.pub_to_segwit_address(compressed_public_key)
+        native_segwit_address2 = coin.pubtosegwitaddress(public_key)
+        native_segwit_compressed_address2 = coin.pubtosegwitaddress(compressed_public_key)
 
         assert native_segwit_address2 == native_segwit_compressed_address2
 
         assert native_segwit_address == native_segwit_address2
 
         assert native_segwit_address == coin.privtoaddr(p2wpkh_wif)
         assert native_segwit_address == coin.privtoaddr(p2wpkh_wif_compressed)
```

### Comparing `cryptos-2.0.7/cryptos/blocks.py` & `cryptos-2.0.8/cryptos/blocks.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/cashaddr.py` & `cryptos-2.0.8/cryptos/cashaddr.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/coins/base.py` & `cryptos-2.0.8/cryptos/coins/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,20 +89,20 @@
     def close(self):
         self.is_closing = True
         if self._loop_is_started.is_set():
             fut = Future()
             self._request_queue.sync_q.put((fut, "close", (), {}))
             fut.result(timeout=100)
 
-    def tx_size(self, txobj: Tx) -> float:
-        return self._async_coin.tx_size(txobj)
-
     def estimate_fee_per_kb(self, numblocks: int = 6) -> float:
         return self._run_async("estimate_fee_per_kb", numblocks=numblocks)
 
+    def tx_size(self, txobj: Tx) -> float:
+        return self._async_coin.tx_size(txobj)
+
     def estimate_fee(self, txobj: Tx, numblocks: int = 6) -> int:
         return self._run_async("estimate_fee", txobj, numblocks=numblocks)
 
     def raw_block_header(self, height: int) -> str:
         return self._run_async("raw_block_header", height)
 
     def block_header(self, height: int) -> BlockHeader:
@@ -165,19 +165,19 @@
 
     def get_histories(self, *args: str, merkle_proof: bool = False) -> List[ElectrumXMultiTxResponse]:
         return self._run_async("get_histories", *args, merkle_proof=merkle_proof)
 
     def get_raw_tx(self, tx_hash: str) -> str:
         return self._run_async("get_raw_tx", tx_hash)
 
-    def get_tx(self, tx_hash: str) -> Tx:
-        return self._run_async("get_tx", tx_hash)
+    def get_tx(self, txid: str) -> Tx:
+        return self._run_async("get_tx", txid)
 
-    def get_verbose_tx(self, tx_hash: str) -> Dict[str, Any]:       # Make TypedDict
-        return self._run_async("get_verbose_tx", tx_hash)
+    def get_verbose_tx(self, txid: str) -> Dict[str, Any]:       # Make TypedDict
+        return self._run_async("get_verbose_tx", txid)
 
     def get_txs(self, *args: str) -> List[Tx]:
         return self._run_async("get_txs", *args)
 
     def pushtx(self, tx: Union[str, Tx]):
         return self._run_async("pushtx", tx)
 
@@ -186,14 +186,23 @@
 
     def pubtoaddr(self, pubkey: PubKeyType) -> str:
         return self._async_coin.pubtoaddr(pubkey)
 
     def privtoaddr(self, privkey: PrivkeyType) -> str:
         return self._async_coin.privtoaddr(privkey)
 
+    def privtop2pkh(self, privkey: PrivkeyType) -> str:
+        return self._async_coin.privtop2pkh(privkey)
+
+    def pub_is_for_p2pkh_addr(self, pubkey: PubKeyType, address: str) -> bool:
+        return self._async_coin.pub_is_for_p2pkh_addr(pubkey, address)
+
+    def wiftoaddr(self, privkey: PrivkeyType) -> str:
+        return self._async_coin.wiftoaddr(privkey)
+
     def electrum_address(self, masterkey: AnyStr, n: int, for_change: int = 0) -> str:
         return self._async_coin.electrum_address(masterkey, n, for_change=for_change)
 
     def encode_privkey(self, privkey: PrivkeyType, formt: str, script_type: str = "p2pkh") -> PrivkeyType:
         return self._async_coin.encode_privkey(privkey, formt, script_type)
 
     def is_p2pkh(self, addr: str) -> bool:
@@ -204,49 +213,70 @@
 
     def is_native_segwit(self, addr: str) -> bool:
         return self._async_coin.is_native_segwit(addr)
 
     def is_address(self, addr: str) -> bool:
         return self._async_coin.is_address(addr)
 
-    def is_legacy_segwit_or_multisig(self, addr: str) -> bool:
+    def is_cash_or_legacy_p2pkh_address(self, addr: str)-> bool:
+        return self._async_coin.is_cash_or_legacy_p2pkh_address(addr)
+
+    def maybe_legacy_segwit(self, addr: str) -> bool:
         return self._async_coin.maybe_legacy_segwit(addr)
 
+    def is_p2wsh(self, addr: str) -> bool:
+        return self._async_coin.is_p2wsh(addr)
+
+    def is_segwit_or_p2sh(self, addr: str) -> bool:
+        return self._async_coin.is_segwit_or_p2sh(addr)
+
     def is_segwit_or_multisig(self, addr: str) -> bool:
         return self._async_coin.is_segwit_or_p2sh(addr)
 
     def output_script_to_address(self, script: str) -> str:
         return self._async_coin.output_script_to_address(script)
 
     def scripttoaddr(self, script: str) -> str:
         return self._async_coin.scripttoaddr(script)
 
     def p2sh_scriptaddr(self, script: str) -> str:
         return self._async_coin.p2sh_scriptaddr(script)
 
+    def p2sh_segwit_addr(self, script: str) -> str:
+        return self._async_coin.p2sh_segwit_addr(script)
+
     def addrtoscript(self, addr: str) -> str:
         return self._async_coin.addrtoscript(addr)
 
     def addrtoscripthash(self, addr: str) -> str:
         return self._async_coin.addrtoscripthash(addr)
 
-    def pubtop2w(self, pub: str) -> str:
+    def pubtop2wpkh_p2sh(self, pub: str) -> str:
         return self._async_coin.pubtop2wpkh_p2sh(pub)
 
+    def privtop2wpkh_p2sh(self, priv: str) -> str:
+        return self._async_coin.privtop2wpkh_p2sh(priv)
+
     def hash_to_segwit_addr(self, pub_hash: str) -> str:
         return self._async_coin.hash_to_segwit_addr(pub_hash)
 
-    def pub_to_segwit_address(self, pubkey) -> str:
-        return self._async_coin.pub_to_segwit_address(pubkey)
+    def scripthash_to_segwit_addr(self, script_hash: AnyStr) -> str:
+        return self._async_coin.scripthash_to_segwit_addr(script_hash)
+
+    def pubtosegwitaddress(self, pubkey) -> str:
+        return self._async_coin.pubtosegwitaddress(pubkey)
 
     def script_to_p2wsh(self, script) -> str:
         return self._async_coin.script_to_p2wsh(script)
 
-    def mk_multsig_address(self, *args: str, num_required: int = None) -> Tuple[str, str]:
-        return self._async_coin.mk_multsig_address(*args, num_required=num_required)
+    def mk_multisig_address(self, *args: str, num_required: int = None) -> Tuple[str, str]:
+        return self._async_coin.mk_multisig_address(*args, num_required=num_required)
+
+    def mk_multsig_segwit_address(self, *args: str, num_required: int = None) -> Tuple[str, str]:
+        return self._async_coin.mk_multsig_segwit_address(*args, num_required=num_required)
 
     def sign(self, txobj: Union[Tx, AnyStr], i: int, priv: PrivkeyType) -> Tx:
         return self._async_coin.sign(txobj, i, priv)
 
     def signall(self, txobj: Union[str, Tx], priv: PrivateKeySignAllType) -> Tx:
         return self._async_coin.signall(txobj, priv)
 
@@ -329,27 +359,36 @@
 
     def is_cash_address(self, addr: str) -> bool:
         return self._async_coin.is_cash_address(addr)
 
     def scripthash_to_cash_addr(self, scripthash: bytes) -> str:
         return self._async_coin.scripthash_to_cash_addr(scripthash)
 
+    def p2sh_cash_addr(self, script: str) -> str:
+        return self._async_coin.p2sh_cash_addr(script)
+
     def hash_to_cash_addr(self, pub_hash: AnyStr) -> str:
         return self._async_coin.hash_to_cash_addr(pub_hash)
 
-    def pub_to_cash_address(self, pubkey: str) -> str:
-        return self._async_coin.pub_to_cash_address(pubkey)
+    def pubtocashaddress(self, pubkey: str) -> str:
+        return self._async_coin.pubtocashaddress(pubkey)
 
     def privtocashaddress(self, privkey: PrivkeyType) -> str:
         return self._async_coin.privtocashaddress(privkey)
 
     def legacy_addr_to_cash_address(self, addr: str) -> str:
         return self._async_coin.legacy_addr_to_cash_address(addr)
 
     def cash_address_to_legacy_addr(self, addr: str) -> str:
         return self._async_coin.cash_address_to_legacy_addr(addr)
 
     def mk_multsig_cash_address(self, *args: str, num_required: int = None) -> Tuple[str, str]:
         return self._async_coin.mk_multsig_cash_address(*args, num_required=num_required)
 
+    def apply_multisignatures(self, txobj: Tx, i: int, script, *args):
+        return self._async_coin.apply_multisignatures(txobj, i, script, *args)
+
     def calculate_fee(self, tx: Tx) -> int:
         return self._run_async("calculate_fee", tx)
+
+    def privtosegwitaddress(self, privkey: PrivkeyType) -> str:
+        return self._async_coin.privtosegwitaddress(privkey)
```

### Comparing `cryptos-2.0.7/cryptos/coins_async/base.py` & `cryptos-2.0.8/cryptos/coins_async/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,48 +436,48 @@
 
     async def get_raw_tx(self, tx_hash: str) -> str:
         """
         Fetch transaction from the blockchain
         """
         return await self.client.get_tx(tx_hash)
 
-    async def get_tx(self, tx_hash: str) -> Tx:
+    async def get_tx(self, txid: str) -> Tx:
         """
         Fetch transaction from the blockchain and deserialise it to a dictionary
         """
-        tx = await self.get_raw_tx(tx_hash)
+        tx = await self.get_raw_tx(txid)
         deserialized_tx = deserialize(tx)
         return deserialized_tx
 
-    async def get_verbose_tx(self, tx_hash: str) -> ElectrumXVerboseTX:
+    async def get_verbose_tx(self, txid: str) -> ElectrumXVerboseTX:
         """
         Fetch transaction from the blockchain in verbose form
         """
-        return await self.client.get_tx(tx_hash, verbose=True)
+        return await self.client.get_tx(txid, verbose=True)
 
     async def get_txs(self, *args: str) -> AsyncGenerator[Tx, None]:
         for tx in await asyncio.gather(*[self.get_tx(tx_hash) for tx_hash in args]):
             yield tx
 
-    async def ensure_values(self, tx: Tx) -> Tx:
+    async def _ensure_values(self, tx: Tx) -> Tx:
         if not all(inp.get('value') for inp in tx['ins']):
             tx_hashes = list(dict.fromkeys([inp['tx_hash'] for inp in tx['ins'] if not inp.get('value')]))
             try:
                 txs = await alist(self.get_txs(*tx_hashes))
             except RuntimeError as e:  # Not sure what causes this intermittent error
                 txs = []
             for inp in tx['ins']:
                 pos = inp['tx_pos']
                 prev_tx = next(filter(lambda t: txhash(serialize(t)) == inp['tx_hash'], txs))
                 inp['value'] = prev_tx['outs'][pos]['value']
         return tx
 
     async def calculate_fee(self, tx: Tx) -> int:
         try:
-            tx = await self.ensure_values(tx)
+            tx = await self._ensure_values(tx)
         except RuntimeError:
             pass
         in_value = sum(i['value'] for i in tx['ins'])
         out_value = sum(o['value'] for o in tx['outs'])
         return in_value - out_value
 
     async def pushtx(self, tx: Union[str, Tx]):
@@ -517,15 +517,15 @@
             else:
                 return [self.legacy_addr_to_cash_address(address), address]
         else:
             return [address]
 
     def pub_is_for_p2pkh_addr(self, pubkey: PubKeyType, address: str) -> bool:
         return self.pubtoaddr(pubkey) == address or (
-                self.cash_address_supported and self.pub_to_cash_address(pubkey) == address)
+                self.cash_address_supported and self.pubtocashaddress(pubkey) == address)
 
     def wiftoaddr(self, privkey: PrivkeyType) -> str:
         magicbyte, priv = b58check_to_bin(privkey)
         wif_magicbyte = magicbyte - self.wif_prefix
         if self.wif_script_types['p2pkh'] == wif_magicbyte:
             return self.privtop2pkh(privkey)
         if self.wif_script_types['p2wpkh-p2sh'] == wif_magicbyte:
@@ -613,15 +613,15 @@
         """
         segwit_hrp = self.segwit_hrp if self.segwit_supported else None
         cash_hrp = self.cash_hrp if self.cash_address_supported else None
         return output_script_to_address(script, self.magicbyte, self.script_magicbyte, segwit_hrp, cash_hrp)
 
     def scripttoaddr(self, script: str) -> str:
         """
-        Convert an input public key hash to an address
+        Convert an input public key has or script to an address
         """
         if is_hex(script):
             script = binascii.unhexlify(script)
         # 0x14 is expected pubkey hash length
         pubkey_hash_prefix = binascii.unhexlify(opcodes.OP_DUP.hex() + opcodes.OP_HASH160.hex() + '14')
         pubkey_hash_suffix = binascii.unhexlify(opcodes.OP_EQUALVERIFY.hex() + opcodes.OP_CHECKSIG.hex())
         if script[:3] == pubkey_hash_prefix and script[-2:] == pubkey_hash_suffix and len(script) == 25:
@@ -726,27 +726,27 @@
             raise NotImplementedError(f"{self.display_name} does not support cash addresses")
         return cashaddr.encode_full(self.cash_hrp, cashaddr.PUBKEY_TYPE, pub_hash)
 
     def privtosegwitaddress(self, privkey: PrivkeyType) -> str:
         """
         Convert a private key to the new segwit address format outlined in BIP01743
         """
-        return self.pub_to_segwit_address(self.privtopub(privkey))
+        return self.pubtosegwitaddress(self.privtopub(privkey))
 
-    def pub_to_cash_address(self, pubkey: str) -> str:
+    def pubtocashaddress(self, pubkey: str) -> str:
         """
         Convert a public key to a cash address
         """
         return self.hash_to_cash_addr(pubkey_to_hash(pubkey))
 
     def privtocashaddress(self, privkey: PrivkeyType) -> str:
         """
         Convert a private key to a cash address
         """
-        return self.pub_to_cash_address(self.privtopub(privkey))
+        return self.pubtocashaddress(self.privtopub(privkey))
 
     def legacy_addr_to_cash_address(self, addr: str) -> str:
         """
         Convert a legacy Bitcoin Address to a Bitcoin cash address
         """
         magicbyte, pubkey_hash = b58check_to_bin(addr)
         if magicbyte == self.magicbyte:
@@ -761,21 +761,21 @@
         Convert a Bitcoin cash address to a legacy Bitcoin address
         """
         prefix, kind, pubkey_hash = cashaddr.decode(addr)
         if kind == 0:
             return bin_to_b58check(pubkey_hash, self.magicbyte)
         return bin_to_b58check(pubkey_hash, self.script_magicbyte)
 
-    def pub_to_segwit_address(self, pubkey: str) -> str:
+    def pubtosegwitaddress(self, pubkey: str) -> str:
         """
         Convert a public key to the new segwit address format outlined in BIP01743
         """
         return self.hash_to_segwit_addr(pubkey_to_hash(compress(pubkey)))
 
-    def mk_multsig_address(self, *args: str, num_required: int = None) -> Tuple[str, str]:
+    def mk_multisig_address(self, *args: str, num_required: int = None) -> Tuple[str, str]:
         """
         :param args: List of public keys to used to create multisig
         :param num_required: The number of signatures required to spend (defaults to number of public keys provided)
         :return: multisig script
         """
         num_required = num_required or len(args)
         script = mk_multisig_script(*args, num_required)
```

### Comparing `cryptos-2.0.7/cryptos/coins_async/bitcoin.py` & `cryptos-2.0.8/cryptos/coins_async/bitcoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/coins_async/bitcoin_cash.py` & `cryptos-2.0.8/cryptos/coins_async/bitcoin_cash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/coins_async/dash.py` & `cryptos-2.0.8/cryptos/coins_async/dash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/coins_async/dogecoin.py` & `cryptos-2.0.8/cryptos/coins_async/dogecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/coins_async/litecoin.py` & `cryptos-2.0.8/cryptos/coins_async/litecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/composite.py` & `cryptos-2.0.8/cryptos/composite.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/deterministic.py` & `cryptos-2.0.8/cryptos/deterministic.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/client.py` & `cryptos-2.0.8/cryptos/electrumx_client/client.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin.json` & `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_cash.json` & `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json` & `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_testnet.json` & `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_testnet.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/servers/litecoin.json` & `cryptos-2.0.8/cryptos/electrumx_client/servers/litecoin.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/electrumx_client/types.py` & `cryptos-2.0.8/cryptos/electrumx_client/types.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/english.txt` & `cryptos-2.0.8/cryptos/english.txt`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/__init__.py` & `cryptos-2.0.8/cryptos/explorers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/base_insight.py` & `cryptos-2.0.8/cryptos/explorers/base_insight.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/blockchain.py` & `cryptos-2.0.8/cryptos/explorers/blockchain.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/blockcypher.py` & `cryptos-2.0.8/cryptos/explorers/blockcypher.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/blockdozer.py` & `cryptos-2.0.8/cryptos/explorers/blockdozer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/btg_explorer.py` & `cryptos-2.0.8/cryptos/explorers/btg_explorer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/dash_siampm.py` & `cryptos-2.0.8/cryptos/explorers/dash_siampm.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/sochain.py` & `cryptos-2.0.8/cryptos/explorers/sochain.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/explorers/utils.py` & `cryptos-2.0.8/cryptos/explorers/utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/keystore.py` & `cryptos-2.0.8/cryptos/keystore.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/main.py` & `cryptos-2.0.8/cryptos/main.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/mnemonic.py` & `cryptos-2.0.8/cryptos/mnemonic.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/opcodes.py` & `cryptos-2.0.8/cryptos/opcodes.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/py3specials.py` & `cryptos-2.0.8/cryptos/py3specials.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/ripemd.py` & `cryptos-2.0.8/cryptos/ripemd.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/segwit_addr.py` & `cryptos-2.0.8/cryptos/segwit_addr.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/stealth.py` & `cryptos-2.0.8/cryptos/stealth.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/testing/testcases.py` & `cryptos-2.0.8/cryptos/testing/testcases.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,18 +537,18 @@
     def assertGetSegwitTxsOK(self):
         txs = self._coin.get_txs(self.txid)
         self.assertListEqual(list(txs[0].keys()),
                              ['ins', 'outs', 'version', 'marker', 'flag', 'witness', 'locktime'])
 
     def assertMultiSigTransactionOK(self):
         pubs = [privtopub(priv) for priv in self.privkeys]
-        script, address1 = self._coin.mk_multsig_address(*pubs, num_required=2)
+        script, address1 = self._coin.mk_multisig_address(*pubs, num_required=2)
         self.assertEqual(address1, self.multisig_addresses[0])
         pubs2 = [privtopub(priv) for priv in self.privkeys[0:2]]
-        script2, address2 = self._coin.mk_multsig_address(*pubs2)
+        script2, address2 = self._coin.mk_multisig_address(*pubs2)
         self.assertEqual(address2, self.multisig_addresses[1])
 
         # Find which of the three addresses currently has the most coins and choose that as the sender
         max_value = 0
         sender = None
 
         for i, addr in enumerate(self.multisig_addresses):
```

### Comparing `cryptos-2.0.7/cryptos/testing/testcases_async.py` & `cryptos-2.0.8/cryptos/testing/testcases_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,16 +128,16 @@
     def assertP2WPKH_WIFOK(self):
         for privkey, expected_wif, address in zip(self.privkeys, self.privkey_native_segwit_wifs, self.native_segwit_addresses):
             wif = self._coin.encode_privkey(privkey, formt="wif_compressed", script_type="p2wpkh")
             self.assertEqual(wif, expected_wif)
             self.assertEqual(self._coin.privtosegwitaddress(privkey), address)
             self.assertEqual(self._coin.privtosegwitaddress(wif), address)
             self.assertEqual(self._coin.privtoaddr(wif), address)
-            self.assertEqual(self._coin.pub_to_segwit_address(privtopub(privkey)), address)
-            self.assertEqual(self._coin.pub_to_segwit_address(privtopub(wif)), address)
+            self.assertEqual(self._coin.pubtosegwitaddress(privtopub(privkey)), address)
+            self.assertEqual(self._coin.pubtosegwitaddress(privtopub(wif)), address)
             self.assertTrue(self._coin.is_native_segwit(address))
             self.assertTrue(self._coin.is_address(address))
             self.assertFalse(self._coin.is_p2sh(address))
             self.assertFalse(self._coin.is_p2pkh(address))
 
     async def assertBalanceOK(self):
         result = await self._coin.get_balance(self.unspent_addresses[0])
@@ -800,18 +800,18 @@
     async def assertGetSegwitTxsOK(self):
         txs = await alist(self._coin.get_txs(self.txid))
         self.assertListEqual(list(txs[0].keys()),
                              ['ins', 'outs', 'version', 'marker', 'flag', 'witness', 'locktime'])
 
     async def assertMultiSigTransactionOK(self, expected_tx_id: str = None):
         pubs = [privtopub(priv) for priv in self.privkeys]
-        script1, address1 = self._coin.mk_multsig_address(*pubs, num_required=2)
+        script1, address1 = self._coin.mk_multisig_address(*pubs, num_required=2)
         self.assertEqual(address1, self.multisig_addresses[0])
         pubs2 = pubs[0:2]
-        script2, address2 = self._coin.mk_multsig_address(*pubs2)
+        script2, address2 = self._coin.mk_multisig_address(*pubs2)
         self.assertEqual(address2, self.multisig_addresses[1])
 
         # Find which of the three addresses currently has the most coins and choose that as the sender
         max_value = 0
         sender = None
         unspents = []
```

### Comparing `cryptos-2.0.7/cryptos/transaction.py` & `cryptos-2.0.8/cryptos/transaction.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/types.py` & `cryptos-2.0.8/cryptos/types.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/utils.py` & `cryptos-2.0.8/cryptos/utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos/wallet.py` & `cryptos-2.0.8/cryptos/wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self.address_derivations[address] = pubkey
         return address
 
     def pubtoaddr(self, pubkey):
         if self.xtype == "p2pkh":
             return self.coin.pubtoaddr(pubkey)
         elif self.xtype == "p2wpkh":
-            return self.coin.pub_to_segwit_address(pubkey)
+            return self.coin.pubtosegwitaddress(pubkey)
         elif self.xtype == "p2wpkh-p2sh":
             return self.coin.pubtop2wpkh_p2sh(pubkey)
 
     @property
     def addresses(self):
         return [self.pubtoaddr(pub) for pub in self.keystore.keypairs.keys()]
 
@@ -220,15 +220,15 @@
     def pubkey_change(self, index):
         return self.keystore.derive_pubkey(1, index)
 
     def pubtoaddr(self, pubkey):
         if self.xtype == "p2pkh":
             return self.coin.pubtoaddr(pubkey)
         elif self.xtype == "p2wpkh":
-            return self.coin.pub_to_segwit_address(pubkey)
+            return self.coin.pubtosegwitaddress(pubkey)
         elif self.xtype == "p2wpkh-p2sh":
             return self.coin.pubtop2wpkh_p2sh(pubkey)
 
     def receiving_address(self, index):
         pubkey = self.pubkey_receiving(index)
         address = self.pubtoaddr(pubkey)
         self.address_derivations[address] = (0, index)
```

### Comparing `cryptos-2.0.7/cryptos/wallet_utils.py` & `cryptos-2.0.8/cryptos/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/cryptos.egg-info/PKG-INFO` & `cryptos-2.0.8/cryptos.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptos
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python Crypto Coin Tools
 Home-page: http://github.com/primal100/pybitcointools
 Author: Paul Martin
 Author-email: greatestloginnameever@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -502,40 +502,101 @@
 
 The arguments are the private key of the sender, the receiver's address and the fee (default 10000). Change will be returned to the sender. 
 
 ### Listing of main coin-specific methods:
 
 * privtopub            : (privkey) -> pubkey
 * pubtoaddr            : (pubkey) -> address
-* privtoaddr           : (privkey) -> address
+* privtoaddr           : (privkey) -> Convert a wif encoded private key to correct address, if not wif encoded then p2pkh
+* privtop2pkh          : (privkey) -> p2pkh address
 * encode_privkey       : (privkey, format, script_type="p2pkh") -> privkey
 * sign                 : (txobj, i, privkey) -> create digital signature of tx with privkey and add to input i
 * signall              : (txobj, privkey) -> create digital signature of tx with privkey for all inputs
-* history              : (address, merkle_proof=False) -> tx history and balance of an address
+* history              : (address, merkle_proof=False) -> tx history of an address
+* get_histories        : (*addresses, merkle_proof=False) -> tx histories of an address
 * unspent              : (address, merkle_proof=False) -> unspent outputs for an addresses
-* pushtx               : (hex or bin tx) -> push a transaction to the blockchain
-* get_tx               : (txhash) -> fetch a tx from the blockchain
+* get_unspents         : (addresses, merkle_proof=False) -> unspent outputs for multiple addresses
+* pushtx               : (hex or tx object) -> push a transaction to the blockchain
+* get_raw_tx           : (txid) -> Get the raw hex of a transaction id
+* get_tx               : (txid) -> fetch a tx from the blockchain
+* get_verbose_tx       : (txid) -> Transaction details verbose output
+* get_txs              : (*txids) -> Fetch multiple transaction details
+* calculate_fee        : (Tx) -> Calculate the fee of a transaction
 * send                 : (privkey, frm, to, value, change_addr=None, fee=None, estimate_fee_blocks: int = 6) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
 * send_to_multiple_receivers_tx          : (privkey, addr outs:value pairs, change_addr=None,fee=10000,, estimate_fee_blocks: int = 6) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
 * preparetx            : (frm, to, value, fee, estimate_fee_blocks: int = 6,change_addr=None): -> create unsigned txobj with change output
 * preparemultitx       : (frm, outs:value pairs, change_addr=None, fee=None, estimate_fee_blocks: int = 6): -> create unsigned txobj with multiple outputs and additional change output
 * preparesignedtx      : (privkey, frm, to, value, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with change output
 * preparesignedmultirecipienttx : (privkey, frm, outs: value pairs, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with multiple outputs and additional change output
-* mktx                 : (inputs, outputs, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
+* mktx                 : (inputs, outputs, locktifme=0, sequence=0xFFFFFFFF) -> create unsigned txobj
 * mktx_with_change     : (inputs, outputs, change_addr=None, fee=None, estimate_fee_blocks=6, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
-* mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multsig script and address pubkeys
+* mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multisig script and address
+* multisign            : (txobj, i, script, privkey) -> signature
+* apply_multisignatures: (txobj, i, script, sigs) -> tx with index i signed with sigs
+* mk_multsig_segwit_address : (pubkeys, M)- Returns both M-of-N multisig script and native segwit address
+* mk_multsig_cash_address: (pubkeys, M)- Returns both M-of-N multisig script and Bitcoin Cash address
 * pubtop2w             : (pub) -> pay to witness script hash (segwit address)
 * privtop2w            : (priv) -> pay to witness script hash (segwit address)
+* pubtop2wpkh_p2sh     : (pub) -> Convert a public key to a segwit address encoded in a p2sh script
+* privtop2wpkh_p2sh    : (priv) -> Convert a private key to a segwit address encoded in a p2sh script
+* hash_to_segwit_addr  : (hash) -. Convert a public key hash to a native segwit address
+* scripthash_to_segwit_addr: (hash) -> Convert the hash of a p2sh script to a native segwit address
 * is_address           : (addr) -> true if addr is a valid address for this network
+* is_p2pkh              : (address) -> Return true if an address is in p2pkh format
 * is_p2sh              : (addr) -> true if addr is a pay to script hash for this network
 * is_segwit            : (priv, addr) -> true if priv-addr pair represent a pay to witness script hash
+* is_cash_or_legacy_p2pkh_address : (address) -> Returns true if an address is a legacy p2pkh address or a Bitcoin Cash formatted p2pkh address
+* is_native_segwit      : (address) -> Returns true if an address is of native segwit type
+* is_cash_address       : (address) -> Returns true if an address is of Bitcoin Cash address format
+* maybe_legacy_segwit   : (address) -> Returns true if address is likely a legacy segwit p2sh address
+* is_p2wsh              : (address) -> Returns true is address is a Pay To Witness Script Address
+* is_segwit_or_p2sh     : (address) -> Returns true if an address is a Pay to Witness or Pay to Script address
 * current_block_height : () -> Latest block height
 * block_height         : (txhash) -> Block height containing the txhash
 * inspect              : (tx_hex) -> Deserialize a transaction and decode and ins and outs
 * merkle_prove         : (txhash) -> Proves a transaction is valid and returns txhash, merkle siblings and block header.
+* estimate_fee_per_kb  : (numblocks) -> Get estimated fee kb to get transaction confirmed within numblocks number of blocks
+* tx_size              : (tx) -> Estimate final transaction size of an unsigned transaction
+* estimate_fee         : (tx, numblocks=6) -> Estimate required fee of an unsigned transaction
+* raw_block_header     : (height) -> Get the raw data of a block header
+* block_header         : (height) -> Get the decoded details of a block header
+* block_headers        : (*heights) -> Get a list of decoded block headers
+* subscribe_to_block_headers: (callback(height, raw_header, decoded_header)) -> Run a callback whenever a new block is added to the blockchain
+* unsubscribe_from_block_headers: () -> Remove all subscriptions to block headers
+* confirmations        : (height) -> Number of confirmations a transaction at this height has
+* subscribe_to_address : (callback(addr, status), addr) -> Run a callback every time there is an activity on an address
+* subscribe_to_address_transactions : (callback(address: str, txs, newly_confirmed, history, unspent, confirmed, unconfirmed, proven), addr) -> Run a callback every time there is an activity on an address with details transaction and balance information already retrieved
+* unsubscribe_from_address: (addr) -> Remove all subscriptions for this address
+* get_balance           : (addr) -> Get the balance, confirmed and unconfirmed, for an address
+* get_balances          : (*addrs) -> Get the balance, confirmed and unconfirmed, for multiple addresses
+* get_merkle            : (tx) -> Get the merkle root of a transaction
+* merkle_prove          : (tx) -> Prove a transaction is valid
+* merkle_prove_by_txid  : (txid) -> Prove a transaction id is valid
+* balance_merkle_proven : (addr) -> Get the merkle proven balance for an address
+* balance_merkle_proven : (*addrs) -> Get the merkle proven balance for multiple addresses
+* get_address_variations: (addr) -> Return alternative formats for an address (e.g. Standard + Bitcoin Cash address)
+* pub_is_for_p2pkh_addr : (pub, addr) -> Returns true if the p2pkh address for pub is addr
+* wiftoaddr             : (priv) -> Convert a private key in WIF format to the correct address type
+* electrum_address      : (masterkey, n, for_change) -> Electrum Address (for old Electrum seeds)
+* encode_privkey        : (privkey, format, script_type) -> Convert a private key to a different format or script types
+* output_script_to_address : (script) -> Convert an output script to an address
+* scripttoaddr          : (script)  -> Convert an input script to an address 
+* addrtoscript          : (address) -> Convert an address to an output script
+* addrtoscripthash      : (address) -> Convert an address to scripthash as required by ElectrumX servers
+* p2sh_scriptaddr       : (script) -> Convert an output P2SH script to a P2SH address
+* p2sh_segwit_addr      : (script) -> Convert an output P2SH script to a native segwit P2WSH address
+* pubtosegwitaddress    : (pub) -> Convert a public key to a native segwit address
+* privtosegwitaddress   : (priv) -> Convert a private key to a native segwit address
+* scripthash_to_cash_addr: (scripthash) -> Convert a scripthash to a Bitcoin Cash address
+* pubtocashaddress      : (pub) -> Convert a public key to a Bitcoin Cash address
+* privtocashaddress     : (priv) -> Convert a private key to a Bitcoin Cash address 
+* p2sh_cash_addr        : (script) -> Convert an script to a Bitcoin Cash address
+* hash_to_cash_addr     : (hash) -> Convert the hash of a p2sh script to a Bitcoin Cash address
+* legacy_addr_to_cash_address: (addr) -> Convert a legacy P2PKH address to a Bitcoin Cash address
+* cash_address_to_legacy_addr: (addr) -> Convert a Bitcoin Cash address to a legalcy P2PKH address
 
 ### Listing of main non-coin specific commands:
 
 * add                  : (key1, key2) -> key1 + key2 (works on privkeys or pubkeys)
 * multiply             : (pubkey, privkey) -> returns pubkey * privkey
 
 * ecdsa_sign           : (message, privkey) -> sig
@@ -553,19 +614,15 @@
 * bip32_master_key     : (seed) -> bip32 master key
 * bip32_ckd            : (private or public bip32 key, i) -> child key
 * bip32_privtopub      : (private bip32 key) -> public bip32 key
 * bip32_extract_key    : (private or public bip32_key) -> privkey or pubkey
 
 * deserialize          : (hex or bin transaction) -> JSON tx
 * serialize            : (JSON tx) -> hex or bin tx
-* multisign            : (txobj, i, script, privkey) -> signature
-* apply_multisignatures: (txobj, i, script, sigs) -> tx with index i signed with sigs
-* scriptaddr           : (script) -> P2SH address
-* mk_multisig_script   : (pubkeys, M) -> M-of-N multisig script from pubkeys
-* verify_tx_input      : (tx, i, script, sig, pub) -> True/False
+s* verify_tx_input      : (tx, i, script, sig, pub) -> True/False
 * tx_hash              : (hex or bin tx) -> hash
 
 * access               : (json list/object, prop) -> desired property of that json object
 * multiaccess          : (json list, prop) -> like access, but mapped across each list element
 * slice                : (json list, start, end) -> given slice of the list
 * count                : (json list) -> number of elements
 * sum                  : (json list) -> sum of all values
```

### Comparing `cryptos-2.0.7/cryptos.egg-info/SOURCES.txt` & `cryptos-2.0.8/cryptos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/setup.py` & `cryptos-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(name='cryptos',
-      version='2.0.7',
+      version='2.0.8',
       description='Python Crypto Coin Tools',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Paul Martin',
       author_email='greatestloginnameever@gmail.com',
       url='http://github.com/primal100/pybitcointools',
       packages=find_packages(),
```

### Comparing `cryptos-2.0.7/tests/electrum_subscribe_mock_server.py` & `cryptos-2.0.8/tests/electrum_subscribe_mock_server.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins/test_bitcoin_testnet.py` & `cryptos-2.0.8/tests/test_coins/test_bitcoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_bitcoin.py` & `cryptos-2.0.8/tests/test_coins_async/test_bitcoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash.py` & `cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash_testnet.py` & `cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_bitcoin_testnet.py` & `cryptos-2.0.8/tests/test_coins_async/test_bitcoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_dash.py` & `cryptos-2.0.8/tests/test_coins_async/test_dash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_dash_testnet.py` & `cryptos-2.0.8/tests/test_coins_async/test_dash_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_dogecoin.py` & `cryptos-2.0.8/tests/test_coins_async/test_dogecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_dogecoin_testnet.py` & `cryptos-2.0.8/tests/test_coins_async/test_dogecoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_litecoin.py` & `cryptos-2.0.8/tests/test_coins_async/test_litecoin.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                                              "TBuuGEcqFBYxir6Y4df3AMq4nSgYckooED1MT2MyyuHTcFPhEP7W",
                                              "TJBomHjQjYxQ62GE1SbrQNrjcEfTh8bhfABhW3mXdRUryzB2UR2g"]
     fee: int = 54400
     max_fee: int = fee
     testnet: bool = False
 
     unspent_addresses: List[str] = ["LSdTvMHRm8sScqwCi6x9wzYQae8JeZhx6y"]
-    balance: ElectrumXMultiBalanceResponse = {'confirmed': 83515295, 'unconfirmed': 0}
+    balance: ElectrumXMultiBalanceResponse = {'confirmed': 83571855, 'unconfirmed': 0}
     balances: List[ElectrumXMultiBalanceResponse] = [{'address': unspent_addresses[0]} | dict(balance)]
     unspent: List[ElectrumXTx] = [{'address': 'LSdTvMHRm8sScqwCi6x9wzYQae8JeZhx6y',
                                   'height': 1495972,
                                   'tx_hash': '6cf532663cd14013aa6ccb394f86d64aa48fce4d6aa8a175f9b75ea486465ca9',
                                   'tx_pos': 0,
                                   'value': 1984},
                                  {'address': 'LSdTvMHRm8sScqwCi6x9wzYQae8JeZhx6y',
@@ -89,15 +89,21 @@
                                   'tx_hash': '43eb70acc4c8c6bdbfabdf76cdbf0a6a969b82051514d105f8c00dff23e715c6',
                                   'tx_pos': 0,
                                   'value': 200000},
                                  {'address': 'LSdTvMHRm8sScqwCi6x9wzYQae8JeZhx6y',
                                   'height': 2352771,
                                   'tx_hash': '7158c6f05ef2b06a40cd00b64647da6735d2eb3908f958fcbc5d0584f34be460',
                                   'tx_pos': 0,
-                                  'value': 1121169}]
+                                  'value': 1121169},
+                                 {'address': 'LSdTvMHRm8sScqwCi6x9wzYQae8JeZhx6y',
+                                  'height': 2454373,
+                                  'tx_hash': '02c0665f6ddaed09a365ddafdff05b188969ee754acf6867b9dd1b970d254a8b',
+                                  'tx_pos': 0,
+                                  'value': 56560
+                                  }]
     history: List[ElectrumXTx] = [{'height': 1495972,
                                    'tx_hash': '6cf532663cd14013aa6ccb394f86d64aa48fce4d6aa8a175f9b75ea486465ca9'},
                                   {'height': 1509957,
                                    'tx_hash': '4987fcebf1643d6a254e6352b72867de1c64a0f5b9e6e1e83c103be419ed9914'},
                                   {'height': 1514616,
                                    'tx_hash': '107cc3d3bf8f1977f9c60b80d02c6e44b1e272a8ebe0d43f712762113bb47c43'},
                                   {'height': 1710946,
@@ -109,15 +115,17 @@
                                   {'height': 1800218,
                                    'tx_hash': '68f98cd415c0586c917e4ba6c78747e7281adca09837048ff8fa211cab9326cd'},
                                   {'height': 2192455,
                                    'tx_hash': '8391ba465fe818e7041a2316e508731b6e20bf9488c0b7579bfd7de46c6e9ab3'},
                                   {'height': 2262951,
                                    'tx_hash': '43eb70acc4c8c6bdbfabdf76cdbf0a6a969b82051514d105f8c00dff23e715c6'},
                                   {'height': 2352771,
-                                   'tx_hash': '7158c6f05ef2b06a40cd00b64647da6735d2eb3908f958fcbc5d0584f34be460'}]
+                                   'tx_hash': '7158c6f05ef2b06a40cd00b64647da6735d2eb3908f958fcbc5d0584f34be460'},
+                                  {'height': 2454373,
+                                   'tx_hash': '02c0665f6ddaed09a365ddafdff05b188969ee754acf6867b9dd1b970d254a8b'}]
     histories: List[ElectrumXTx] = [dict(h) | {'address': "LSdTvMHRm8sScqwCi6x9wzYQae8JeZhx6y"} for h in history]
     unspents: List[ElectrumXTx] = unspent
     min_latest_height: int = 2360220
     txheight: int = 509045
     block_hash: str = "3bfd5d7f95a28e1af34cc50a36aee92c4aa4c317d4d0f7795034f7a8fc74b6c9"
     txid: str = "0c2d49e00dd1372a7219fbc4378611b39f54790bbd597b4c29517f0d93c9faa2"
     txinputs: List[TxInput] = [{'output': 'b3105972beef05e88cf112fd9718d32c270773462d62e4659dc9b4a2baafc038:0', 'value': 1157763509}]
@@ -174,54 +182,54 @@
 
     async def test_balances_merkle_proven(self):
         await self.assertBalancesMerkleProvenOK()
 
     async def test_transaction(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
-            await self.assertTransactionOK("9e60e1f5257950837bbbe7f2ca84410a59d9b6326823c4e0defdb01fb115df97")
+            await self.assertTransactionOK("5f2bee84fdd62038a5f34848cd427cca3ed278d990d7ed4e50d7f62378c23757")
 
     async def test_transaction_segwit(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
             await self.assertSegwitTransactionOK(
-                "c263194aed2d18f3289105f99636b2187f7228c0a5d3b0c757d68a7a9099a4c4")
+                "1956512ac84a0624d1c771463ed08c19b9e4add2d7f23975b4c4fcd9c6d0a006")
 
     async def test_transaction_native_segwit(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
             await self.assertNativeSegwitTransactionOK(
-                "41c45ea2381ec4da825712d1cee6d598247edac93e8fedb79ff6d426bfb2af6f")
+                "eab7dcbf60408c9a72bfd5f60ffcef3c266e8b9a0f159686f97334740ff2b88c")
 
     async def test_transaction_mixed_segwit(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
             await self.assertMixedSegwitTransactionOK(
-                "5e918bfc41e912b581adb513efe4f480d37950c386842ad1bbd052b3fb5c1a48")
+                "69678157448b00cfdafaf07bf7825072094552c5f5f3626152845118b3b30969")
 
     async def test_transaction_multisig(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
             await self.assertMultiSigTransactionOK(
-                "a0c54d9e45a7bd3ab224d154760f08c7fcfc8aeaecbb46914796ff52e27e6c85")
+                "6ecbbfe2af2744b3000e02e21f70c96d5e2128a04db07e3d1c983036f7683d70")
 
     async def test_transaction_native_segwit_multisig(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
-            await self.assertNativeSegwitMultiSigTransactionOK("37d3c7f0ff6846a34bbd69a472cadb83ee631b5ea1bc7695cfe52a3442ed7397")
+            await self.assertNativeSegwitMultiSigTransactionOK("27fb482d29a85b3141141622dde4015499cdf17ecc41b57c01dc387e9e87431e")
 
     async def test_sendmulti_recipient_tx(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
-            await self.assertSendMultiRecipientsTXOK("c85e3e899b43c5a1f68647c852ee13f9e3e2b409b4cc73cce131d70dba1a793d")
+            await self.assertSendMultiRecipientsTXOK("b714d2614e05ae9442c44f39faa82cc41ef4d37348d04075e5315f41b9467071")
 
     async def test_send(self):
         with mock.patch('cryptos.electrumx_client.client.NotificationSession.send_request',
                         side_effect=self.mock_electrumx_send_request):
-            await self.assertSendOK("6d2cfbc85d56284f0ee88f977979d20e8e66017b48737568d1b23ae597594e2d")
+            await self.assertSendOK("ba75fb9bafeb6dd02d044b7814f3da917037bedf3d187eae4b94c10a6559e7d1")
 
     async def test_subscribe_block_headers(self):
         await self.assertSubscribeBlockHeadersOK()
 
     async def test_subscribe_block_headers_sync(self):
         await self.assertSubscribeBlockHeadersSyncCallbackOK()
```

### Comparing `cryptos-2.0.7/tests/test_coins_async/test_litecoin_testnet.py` & `cryptos-2.0.8/tests/test_coins_async/test_litecoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_electrum_client.py` & `cryptos-2.0.8/tests/test_electrum_client.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_general.py` & `cryptos-2.0.8/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_stealth.py` & `cryptos-2.0.8/tests/test_stealth.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.7/tests/test_wallet.py` & `cryptos-2.0.8/tests/test_wallet.py`

 * *Files identical despite different names*

