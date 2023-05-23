# Comparing `tmp/quorum_eth_py-0.3.1.tar.gz` & `tmp/quorum_eth_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_eth_py-0.3.1.tar", last modified: Wed May 17 05:09:41 2023, max compression
+gzip compressed data, was "quorum_eth_py-0.4.0.tar", last modified: Tue May 23 07:48:53 2023, max compression
```

## Comparing `quorum_eth_py-0.3.1.tar` & `quorum_eth_py-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.871835 quorum_eth_py-0.3.1/
--rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-17 05:09:41.869862 quorum_eth_py-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.809709 quorum_eth_py-0.3.1/quorum_eth_py/
--rw-rw-rw-   0        0        0      445 2023-05-17 05:09:03.000000 quorum_eth_py-0.3.1/quorum_eth_py/__init__.py
--rw-rw-rw-   0        0        0     1746 2023-05-17 04:45:00.000000 quorum_eth_py-0.3.1/quorum_eth_py/_browser.py
--rw-rw-rw-   0        0        0     7497 2023-05-17 05:08:52.000000 quorum_eth_py-0.3.1/quorum_eth_py/_eth.py
--rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.3.1/quorum_eth_py/_gateway.py
--rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.3.1/quorum_eth_py/_http.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.867841 quorum_eth_py-0.3.1/quorum_eth_py/contract/
--rw-rw-rw-   0        0        0    23212 2023-05-14 05:42:29.000000 quorum_eth_py-0.3.1/quorum_eth_py/contract/RumERC20.py
--rw-rw-rw-   0        0        0      138 2023-05-15 07:09:49.000000 quorum_eth_py-0.3.1/quorum_eth_py/contract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 05:09:41.861251 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-17 05:09:41.000000 quorum_eth_py-0.3.1/quorum_eth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 05:09:41.871835 quorum_eth_py-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-05-17 05:09:03.000000 quorum_eth_py-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.162515 quorum_eth_py-0.4.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-23 07:48:53.161519 quorum_eth_py-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.102683 quorum_eth_py-0.4.0/quorum_eth_py/
+-rw-rw-rw-   0        0        0      343 2023-05-23 02:53:26.000000 quorum_eth_py-0.4.0/quorum_eth_py/__init__.py
+-rw-rw-rw-   0        0        0     1746 2023-05-17 04:45:00.000000 quorum_eth_py-0.4.0/quorum_eth_py/_browser.py
+-rw-rw-rw-   0        0        0      149 2023-05-22 12:44:15.000000 quorum_eth_py-0.4.0/quorum_eth_py/_constants.py
+-rw-rw-rw-   0        0        0     6276 2023-05-23 07:43:44.000000 quorum_eth_py-0.4.0/quorum_eth_py/_eth.py
+-rw-rw-rw-   0        0        0      470 2023-04-28 13:05:38.000000 quorum_eth_py-0.4.0/quorum_eth_py/_gateway.py
+-rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.4.0/quorum_eth_py/_http.py
+-rw-rw-rw-   0        0        0     6150 2023-05-23 07:39:54.000000 quorum_eth_py-0.4.0/quorum_eth_py/_paid_group.py
+-rw-rw-rw-   0        0        0     2177 2023-05-23 07:02:25.000000 quorum_eth_py-0.4.0/quorum_eth_py/_rum_erc20.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.159523 quorum_eth_py-0.4.0/quorum_eth_py/contract/
+-rw-rw-rw-   0        0        0    38405 2023-05-22 11:47:48.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/PaidGroup.py
+-rw-rw-rw-   0        0        0    38871 2023-05-23 06:31:13.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/PaidGroupV2.py
+-rw-rw-rw-   0        0        0    23212 2023-05-22 10:47:15.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/RumERC20.py
+-rw-rw-rw-   0        0        0      280 2023-05-22 11:47:45.000000 quorum_eth_py-0.4.0/quorum_eth_py/contract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:48:53.151544 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 07:48:52.000000 quorum_eth_py-0.4.0/quorum_eth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:48:53.162515 quorum_eth_py-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1134 2023-05-23 02:30:10.000000 quorum_eth_py-0.4.0/setup.py
```

### Comparing `quorum_eth_py-0.3.1/LICENSE` & `quorum_eth_py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.1/PKG-INFO` & `quorum_eth_py-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_eth_py
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.3.1/quorum_eth_py/_browser.py` & `quorum_eth_py-0.4.0/quorum_eth_py/_browser.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.1/quorum_eth_py/_eth.py` & `quorum_eth_py-0.4.0/quorum_eth_py/_eth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,201 +1,160 @@
-import asyncio
-import logging
-
-from quorum_mininode_py import create_pvtkey
-from web3 import Web3
-from web3.middleware import geth_poa_middleware
-
-from quorum_eth_py.contract.RumERC20 import abi as RumERC20_abi
-from quorum_eth_py.contract.RumERC20 import bytecode as RumERC20_bytecode
-
-logger = logging.getLogger(__name__)
-
-
-RUM_ETH_HTTP_PROVIDER = "http://149.56.22.113:8545"
-RUM_ETH_CHAINID = 19890609
-
-
-class RumEthChain:
-    """https://github.com/rumsystem/rum-eth-mvm/blob/main/RUM-ETH.md"""
-
-    def __init__(self, pvtkey: str = None):
-        pvtkey = pvtkey or create_pvtkey()
-        self.w3 = Web3(Web3.HTTPProvider(RUM_ETH_HTTP_PROVIDER))
-        self.w3.middleware_onion.inject(geth_poa_middleware, layer=0)
-        self.is_connected()
-        self.account = self.w3.eth.account.from_key(pvtkey)
-        self.w3.eth.default_account = self.account.address
-        logger.info("account address: %s", self.account.address)
-
-    def is_connected(self):
-        status = self.w3.is_connected()
-        logger.info("connected to rum-eth-chain: %s", status)
-        return status
-
-    def get_balance(self, address: str = None):
-        """get the balance of address, default is the account address"""
-        address = address or self.account.address
-        address = self.w3.to_checksum_address(address)
-        balance_wei = self.w3.eth.get_balance(address)
-        balance = self.w3.from_wei(balance_wei, "ether")
-        return balance
-
-    def _transction(self, tx: dict):
-        signed_tx = self.w3.eth.account.sign_transaction(
-            tx, private_key=self.account.key
-        )
-        tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-        tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
-        return tx_receipt
-
-    def transfer(self, to_address: str, num):
-        """transfer rum to address, the rum is origin token of poa chain, used as gas feed"""
-        # check balance of account
-        if num <= 0:
-            raise Exception("transfer num must be positive")
-        to_address = self.w3.to_checksum_address(to_address)
-        if self.get_balance() < num:
-            raise Exception(f"balance not enough {self.get_balance()}")
-        tx = {
-            "nonce": self.w3.eth.get_transaction_count(self.account.address),
-            "to": to_address,
-            "value": self.w3.to_wei(num, "ether"),
-            "gasPrice": self.w3.to_wei("10", "gwei"),
-            "gas": 50000,
-            "chainId": RUM_ETH_CHAINID,
-        }
-        gas_limit = self.w3.eth.estimate_gas(tx)
-        if gas_limit > tx["gas"]:
-            tx["gas"] = gas_limit
-        tx_receipt = self._transction(tx)
-        tid = tx_receipt.transactionHash.hex()
-        return tid
-
-    def contract_instance(self, abi, contract_address):
-        contract_instance = self.w3.eth.contract(contract_address, abi=abi)
-        return contract_instance
-
-    def deploy_erc20(
-        self, name, symbol, total_supply, minter_address=None, abi=None, bytecode=None
-    ):
-        """deploy new erc20 contract"""
-        abi = abi or RumERC20_abi
-        bytecode = bytecode or RumERC20_bytecode
-        contract = self.w3.eth.contract(abi=abi, bytecode=bytecode)
-        cap = self.w3.to_wei(total_supply, "ether")
-        minter = self.w3.to_checksum_address(minter_address or self.account.address)
-
-        tx = {
-            "from": self.account.address,
-            "nonce": self.w3.eth.get_transaction_count(self.account.address),
-            "gasPrice": self.w3.to_wei("10", "gwei"),
-            "gas": 50000,
-            "chainId": RUM_ETH_CHAINID,
-        }
-        gas_limit = contract.constructor(
-            cap=cap, name_=name, symbol_=symbol, minter=minter
-        ).estimate_gas()
-        if gas_limit > tx["gas"]:
-            tx["gas"] = gas_limit
-
-        if self.get_balance() < self.w3.from_wei(tx["gas"], "ether"):
-            raise Exception(f"not enough for gas fee {self.get_balance()}")
-
-        build_tx = contract.constructor(
-            cap=cap, name_=name, symbol_=symbol, minter=minter
-        ).build_transaction(tx)
-        tx_receipt = self._transction(build_tx)
-        contract_address = tx_receipt.contractAddress
-        logger.info("deploy new erc20 contract: %s", contract_address)
-        return contract_address
-
-    def get_trx(self, tx_id_hex: str):
-        receipt = self.w3.eth.get_transaction_receipt(tx_id_hex)
-        return receipt
-
-    async def check_trx(self, tx_id_hex, times=10):
-        for i in range(times):
-            try:
-                receipt = self.w3.eth.get_transaction_receipt(tx_id_hex)
-            except Exception as e:
-                logger.error(e)
-                receipt = None
-            if receipt:
-                if receipt["status"] == 1:
-                    msg = "Transaction completed successfully"
-                    status = True
-                else:
-                    msg = "Transaction failed"
-                    status = False
-            else:
-                msg = "Transaction not found"
-                status = False
-            if status:
-                break
-            await asyncio.sleep(1)
-        return msg, status
-
-
-class RumERC20Instance:
-    """
-    https://github.com/rumsystem/rum-eth-mvm/blob/main/dapps/RumERC20/contracts/RumERC20.sol
-    """
-
-    def __init__(
-        self, contract_address, pvtkey=None, chain: RumEthChain = None, abi=None
-    ):
-        abi = abi or RumERC20_abi
-        self.chain = chain or RumEthChain(pvtkey)
-        self.w3 = self.chain.w3
-        self.account = self.chain.account
-        self.erc20 = self.chain.w3.eth.contract(contract_address, abi=abi)
-        self.funcs = self.erc20.functions
-
-    def name(self):
-        return self.funcs.name().call()
-
-    def symbol(self):
-        return self.funcs.symbol().call()
-
-    def decimals(self):
-        return self.funcs.decimals().call()
-
-    def total_supply(self):
-        unit256 = self.funcs.totalSupply().call()
-        return self.w3.from_wei(unit256, "ether")
-
-    def get_balance(self, address=None):
-        address = address or self.account.address
-        address = self.w3.to_checksum_address(address)
-        unit256 = self.funcs.balanceOf(address).call()
-        return self.w3.from_wei(unit256, "ether")
-
-    def get_rum_balance(self, address=None):
-        address = address or self.account.address
-        return self.chain.get_balance(address)
-
-    def transfer(self, to_address, num):
-        """transfter num of token to address"""
-        to_address = self.w3.to_checksum_address(to_address)
-        amount = self.w3.to_wei(num, "ether")
-
-        options = {
-            "gas": 53000,
-            "gasPrice": self.w3.to_wei("1", "gwei"),
-            "from": self.account.address,
-            "nonce": self.w3.eth.get_transaction_count(self.account.address),
-        }
-        gas_limit = self.w3.eth.estimate_gas(options)
-        if gas_limit > options["gas"]:
-            options["gas"] = gas_limit
-
-        tx = self.funcs.transfer(to_address, amount).build_transaction(options)
-        signed = self.w3.eth.account.sign_transaction(tx, private_key=self.account.key)
-        tx_hash = self.w3.eth.send_raw_transaction(signed.rawTransaction)
-        tx_receipt = self.w3.eth.wait_for_transaction_receipt(tx_hash)
-        tid = tx_receipt.transactionHash.hex()
-        logger.info("transfer to %s is done by trx: %s", to_address, tid)
-        return tid
-
-    def get_trx(self, tx_id_hex: str):
-        return self.chain.get_trx(tx_id_hex)
+import logging
+
+from quorum_mininode_py import create_pvtkey
+from web3 import Web3
+from web3.middleware import geth_poa_middleware
+
+from quorum_eth_py._constants import RUM_ETH_CHAINID, RUM_ETH_HTTP_PROVIDER
+from quorum_eth_py.contract.PaidGroupV2 import abi as PaidGroup_abiv2
+from quorum_eth_py.contract.PaidGroupV2 import bytecode as PaidGroup_bytecodev2
+from quorum_eth_py.contract.RumERC20 import abi as RumERC20_abi
+from quorum_eth_py.contract.RumERC20 import bytecode as RumERC20_bytecode
+
+logger = logging.getLogger(__name__)
+
+
+class RumEthChain:
+    """https://github.com/rumsystem/rum-eth-mvm/blob/main/RUM-ETH.md"""
+
+    def __init__(self, pvtkey: str = None):
+        pvtkey = pvtkey or create_pvtkey()
+        self.w3 = Web3(Web3.HTTPProvider(RUM_ETH_HTTP_PROVIDER))
+        self.w3.middleware_onion.inject(geth_poa_middleware, layer=0)
+        self.is_connected()
+        self.account = self.w3.eth.account.from_key(pvtkey)
+        self.w3.eth.default_account = self.account.address
+        logger.info("account address: %s", self.account.address)
+
+    def is_connected(self):
+        status = self.w3.is_connected()
+        logger.info("connected to rum-eth-chain: %s", status)
+        return status
+
+    def get_balance(self, address: str = None):
+        """get the balance of address, default is the account address"""
+        address = address or self.account.address
+        address = self.w3.to_checksum_address(address)
+        balance_wei = self.w3.eth.get_balance(address)
+        balance = self.w3.from_wei(balance_wei, "ether")
+        return balance
+
+    def send_transction(self, trx: dict):
+        signed_trx = self.w3.eth.account.sign_transaction(
+            trx, private_key=self.account.key
+        )
+        trx_hash = self.w3.eth.send_raw_transaction(signed_trx.rawTransaction)
+        trx_receipt = self.w3.eth.wait_for_transaction_receipt(trx_hash)
+
+        tid = self.get_trx_id(trx_receipt)
+        if trx_receipt["status"] == 1:
+            logger.info("send_transction success: %s", tid)
+        else:
+            logger.error("send_transction failed: %s", tid)
+        return trx_receipt
+
+    def init_gas_options(self, to: str = None, value: float = None, gas: int = 10000):
+        """init gas options"""
+        options = {
+            "from": self.account.address,
+            "nonce": self.w3.eth.get_transaction_count(self.account.address),
+            "gasPrice": self.w3.to_wei("1", "gwei"),
+            "gas": gas,
+            "chainId": RUM_ETH_CHAINID,
+        }
+        if to:
+            options.update({"to": self.w3.to_checksum_address(to)})
+        if value:
+            options.update({"value": self.w3.to_wei(value, "ether")})
+            if self.get_balance() < value:
+                raise Exception(f"balance not enough {self.get_balance()}")
+
+        gas_limit = self.w3.eth.estimate_gas(options) + 5000
+        if gas_limit > options["gas"]:
+            options["gas"] = gas_limit
+        logger.info("gas options: %s", options["gas"])
+
+        if self.get_balance() < self.w3.from_wei(options["gas"], "ether"):
+            raise Exception(f"not enough for gas fee {self.get_balance()}")
+
+        return options
+
+    def transfer(self, to_address: str, num: float):
+        """transfer rum to address, the rum is origin token of poa chain, used as gas feed"""
+        # check balance of account
+        if num <= 0:
+            raise Exception("transfer num must be positive")
+        to_address = self.w3.to_checksum_address(to_address)
+        options = self.init_gas_options(to=to_address, value=num)
+        return self.send_transction(options)
+
+    def get_trx(self, tx_id_hex: str):
+        receipt = self.w3.eth.get_transaction_receipt(tx_id_hex)
+        return receipt
+
+    def get_trx_id(self, tx_receipt):
+        return tx_receipt.transactionHash.hex()
+
+    def contract_instance(self, contract_address, abi):
+        return self.w3.eth.contract(contract_address, abi=abi)
+
+    def deploy_erc20(
+        self,
+        name: str,
+        symbol: str,
+        total_supply: int,
+        minter_address: str = None,
+        abi=RumERC20_abi,
+        bytecode=RumERC20_bytecode,
+    ):
+        """deploy new erc20 contract"""
+        contract = self.w3.eth.contract(abi=abi, bytecode=bytecode)
+        options = self.init_gas_options(gas=2000000)
+        con = contract.constructor(
+            cap=self.w3.to_wei(total_supply, "ether"),
+            name_=name,
+            symbol_=symbol,
+            minter=self.w3.to_checksum_address(minter_address or self.account.address),
+        )
+        _gas = con.estimate_gas() + 10000
+        if _gas > options["gas"]:
+            logger.info("gas options: %s → %s", options["gas"], _gas)
+            options["gas"] = _gas
+        receipt = self.send_transction(con.build_transaction(options))
+        logger.info("deploy erc20 contract success: %s", receipt.contractAddress)
+        return receipt
+
+    def deploy_paidgroup_v2(
+        self,
+        name: str,
+        receive_addr: str,
+        invoke_fee: float = 0.001,
+        share_ratio=95,
+        version: str = "0.1.0",
+        abi=PaidGroup_abiv2,
+        bytecode=PaidGroup_bytecodev2,
+    ):
+        # deploy contract
+        pg = self.w3.eth.contract(abi=abi, bytecode=bytecode)
+        payload = (
+            version,
+            self.w3.to_wei(invoke_fee, "ether"),
+            share_ratio,
+            receive_addr,
+            name,
+            self.account.address,
+        )
+        options = self.init_gas_options()
+        con = pg.constructor(*payload)
+        _gas = con.estimate_gas() + 10000
+        if _gas > options["gas"]:
+            options["gas"] = _gas
+        receipt = self.send_transction(con.build_transaction(options))
+        # init contract
+        pg = self.contract_instance(receipt.contractAddress, abi)
+        options = self.init_gas_options(gas=3500000)
+        init = pg.functions.initialize(*payload)
+        _gas = init.estimate_gas() + 10000
+        if _gas > options["gas"]:
+            options["gas"] = _gas
+        self.send_transction(init.build_transaction(options))
+        return receipt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quorum_eth_py-0.3.1/quorum_eth_py/_http.py` & `quorum_eth_py-0.4.0/quorum_eth_py/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.1/quorum_eth_py/contract/RumERC20.py` & `quorum_eth_py-0.4.0/quorum_eth_py/contract/RumERC20.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.3.1/quorum_eth_py.egg-info/PKG-INFO` & `quorum_eth_py-0.4.0/quorum_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-eth-py
-Version: 0.3.1
+Version: 0.4.0
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.3.1/setup.py` & `quorum_eth_py-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_eth_py",
-    version="0.3.1",
+    version="0.4.0",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A python sdk for quorum-eth chain",
     keywords=["rumsystem", "quorum", "eth", "sdk", "blockchain"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_eth_py",
```

