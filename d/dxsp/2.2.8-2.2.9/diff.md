# Comparing `tmp/dxsp-2.2.8.tar.gz` & `tmp/dxsp-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.2.8.tar", max compression
+gzip compressed data, was "dxsp-2.2.9.tar", max compression
```

## Comparing `dxsp-2.2.8.tar` & `dxsp-2.2.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-14 17:38:32.580668 dxsp-2.2.8/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-14 17:38:32.580668 dxsp-2.2.8/README.md
--rw-r--r--   0        0        0       86 2023-05-14 17:38:33.232669 dxsp-2.2.8/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/config.py
--rw-r--r--   0        0        0     3139 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/default_settings.toml
--rw-r--r--   0        0        0    29552 2023-05-14 17:38:32.580668 dxsp-2.2.8/dxsp/main.py
--rw-r--r--   0        0        0     1825 2023-05-14 17:38:33.232669 dxsp-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 dxsp-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-15 12:54:04.853267 dxsp-2.2.9/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-15 12:54:04.853267 dxsp-2.2.9/README.md
+-rw-r--r--   0        0        0       86 2023-05-15 12:54:05.785266 dxsp-2.2.9/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/config.py
+-rw-r--r--   0        0        0     3139 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28625 2023-05-15 12:54:04.853267 dxsp-2.2.9/dxsp/main.py
+-rw-r--r--   0        0        0     1831 2023-05-15 12:54:05.785266 dxsp-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.9/PKG-INFO
```

### Comparing `dxsp-2.2.8/LICENSE` & `dxsp-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.8/README.md` & `dxsp-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.8/dxsp/assets/blockchains.py` & `dxsp-2.2.9/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.8/dxsp/default_settings.toml` & `dxsp-2.2.9/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.8/dxsp/main.py` & `dxsp-2.2.9/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,22 +33,22 @@
         self.chain_id = settings.dex_chain_id
         # USER
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
         self.private_key = settings.dex_private_key
 
         # UNISWAP 🦄
-        if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-            self.uniswap = Uniswap(
-                address=self.wallet_address,
-                private_key=self.private_key,
-                router_contract_addr=settings.dex_router_contract_addr,
-                version=2 if self.protocol_type == "uniswap_v2" else 3,
-                web3=self.w3,
-                default_slippage=settings.dex_trading_slippage)
+        # if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+        #     self.uniswap = Uniswap(
+        #         address=self.wallet_address,
+        #         private_key=self.private_key,
+        #         router_contract_addr=settings.dex_router_contract_addr,
+        #         version=2 if self.protocol_type == "uniswap_v2" else 3,
+        #         web3=self.w3,
+        #         default_slippage=settings.dex_trading_slippage)
 
         # COINGECKO 🦎
         try:
             self.cg = CoinGeckoAPI()
             assetplatform = self.cg.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
                            == int(self.chain_id)]
@@ -378,41 +378,32 @@
                 await self.get_approve_1inch(asset_out_address)
             elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 await self.get_approve_uniswap(asset_out_address)
         except Exception as e:
             self.logger.error("get_approve %s", e)
             return None
 
-    async def get_sign(self, order):
+    async def get_sign(self, transaction):
 
         try:
-            # if not isinstance(order, dict):
-            #     raise ValueError("Transaction must be a dictionary")
-            self.logger.debug("get_sign: order %s", order)
+            self.logger.debug("get_sign: transaction %s", transaction)
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
-                order_params = {
+                transaction_params = {
                             'from': self.wallet_address,
-                            'gas': await self.get_gas(order),
-                            'gasPrice': await self.get_gasPrice(order),
+                            'gas': await self.get_gas(transaction),
+                            'gasPrice': await self.get_gasPrice(transaction),
                             'nonce': self.w3.eth.get_transaction_count(
                                 self.wallet_address),
                             }
-                order = order.build_transaction(order_params)
-            elif self.protocol_type in ["1inch", "1inch_limit"]:
-                order = order['tx']
-                order['gas'] = await self.get_gas(order)
-                order['nonce'] = self.w3.eth.get_transaction_count(
-                    self.wallet_address)
-                order['value'] = int(order['value'])
-                order['gasPrice'] = await self.get_gasPrice(order)
+                transaction = transaction.build_transaction(transaction_params)
             signed = self.w3.eth.account.sign_transaction(
-                order,
+                transaction,
                 settings.dex_private_key)
-            raw_order = signed.rawTransaction
-            return self.w3.eth.send_raw_transaction(raw_order)
+            tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
+            return tx_hash
         except (ValueError, TypeError, KeyError) as e:
             self.logger.error("get_sign: %s", e)
             raise
         except Exception as e:
             self.logger.error("get_sign: %s", e)
             raise RuntimeError("Failed to sign transaction")
 
@@ -553,27 +544,20 @@
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
         self.logger.debug("get_quote_uniswap")
         try:
-            # order_path_dex = [asset_out_address, asset_in_address]
-            # router_instance = await self.router()
-            # get_amount = router_instance.functions.getAmountsIn(
-            #     amount,
-            #     order_path_dex).call()
-            # self.logger.debug("get_amount: %s", get_amount)
-            # return get_amount[0]
-            quote = self.uniswap.get_price_output(
-                token0=asset_out_address,
-                token1=asset_in_address,
-                qty=amount)
-            self.logger.info("quoteuniswap %s", quote)
-            return quote
+            router_instance = await self.router()
+            quote = router_instance.functions.getAmountsOut(
+                amount,
+                [asset_in_address, asset_out_address]).call()
+
+            return quote[1]
         except Exception as e:
             self.logger.error("get_quote_uniswap %s", e)
             return
 
     async def get_approve_uniswap(self, asset_out_address):
 
         try:
@@ -585,20 +569,20 @@
                             self.w3.to_checksum_address(self.wallet_address),
                             self.w3.to_checksum_address(
                                 settings.dex_router_contract_addr)
                             ).call()
             self.logger.debug("approval_check %s", approval_check)
             if (approval_check == 0):
                 approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
-                approval_TX = asset_out_contract.functions.approve(
+                approval_transaction = asset_out_contract.functions.approve(
                                 self.w3.to_checksum_address(
                                     settings.dex_router_contract_addr),
                                 approved_amount)
-                self.logger.debug("approval_TX %s", approval_TX)
-                approval_txHash = await self.get_sign(approval_TX)
+                self.logger.debug("approval_TX %s", approval_transaction)
+                approval_txHash = await self.get_sign(approval_transaction)
                 self.logger.debug("approval_txHash %s", approval_txHash)
                 approval_txHash_complete = (
                     self.w3.eth.wait_for_transaction_receipt(
                         approval_txHash,
                         timeout=120,
                         poll_latency=0.1))
                 return approval_txHash_complete
@@ -608,33 +592,29 @@
 
     async def get_swap_uniswap(
         self,
         asset_out_address,
         asset_in_address,
         amount
     ):
-        return self.uniswap(
-            input_token=asset_in_address,
-            output_token=asset_out_address,
-            qty=amount
-        )
-        # order_path_dex = [asset_out_address, asset_in_address]
-
-        # deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-        # order_min_amount = self.get_quote_uniswap_v2(
-        #     asset_in_address,
-        #     asset_out_address)
-        # router_instance = await self.router()
-        # swap_order = router_instance.functions.swapExactTokensForTokens(
-        #                 amount,
-        #                 order_min_amount,
-        #                 order_path_dex,
-        #                 self.wallet_address,
-        #                 deadline)
-        # return swap_order
+        order_path_dex = [asset_out_address, asset_in_address]
+
+        deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
+        order_min_amount = self.get_quote_uniswap(
+            asset_in_address,
+            asset_out_address,
+            amount)[0]
+        router_instance = await self.router()
+        swap_order = router_instance.functions.swapExactTokensForTokens(
+                        amount,
+                        order_min_amount,
+                        order_path_dex,
+                        self.wallet_address,
+                        deadline)
+        return swap_order
 
 # 0️⃣x
     async def get_quote_0x(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
```

### Comparing `dxsp-2.2.8/pyproject.toml` & `dxsp-2.2.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.2.8"
+version = "2.2.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -14,17 +14,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 asyncio = "*"
 dynaconf = "*"
 web3 = ">=6.0.0"
 pycoingecko = "*"
-uniswap-python = "*"
-web3cli = "*"
-
+# uniswap-python = "*"
+# web3client = "*"
 #web3-ethereum-defi = "*"
 # web3client = ">=1.1.8"
 # # many-abis = ">=0.1.7"
 # apollox-connector-python = "*"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `dxsp-2.2.8/PKG-INFO` & `dxsp-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.2.8
+Version: 2.2.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
 Requires-Dist: pycoingecko
-Requires-Dist: uniswap-python
 Requires-Dist: web3 (>=6.0.0)
-Requires-Dist: web3cli
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
```

