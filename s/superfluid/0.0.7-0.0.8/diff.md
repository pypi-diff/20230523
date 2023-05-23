# Comparing `tmp/superfluid-0.0.7.tar.gz` & `tmp/superfluid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superfluid-0.0.7.tar", last modified: Tue May 23 16:22:57 2023, max compression
+gzip compressed data, was "superfluid-0.0.8.tar", last modified: Tue May 23 16:29:14 2023, max compression
```

## Comparing `superfluid-0.0.7.tar` & `superfluid-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:22:57.549868 superfluid-0.0.7/
--rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.7/LICENSE.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:22:57.549712 superfluid-0.0.7/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.7/README.md
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:22:57.542813 superfluid-0.0.7/main/
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:22:57.543359 superfluid-0.0.7/main/superfluid/
--rw-r--r--   0 godspowereze   (501) staff       (20)      118 2023-05-23 16:22:23.000000 superfluid-0.0.7/main/superfluid/__init__.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:22:57.549364 superfluid-0.0.7/main/superfluid/src/
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.0.7/main/superfluid/src/__init__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     5339 2023-05-23 07:38:08.000000 superfluid-0.0.7/main/superfluid/src/__types__.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     9367 2023-05-23 08:19:40.000000 superfluid-0.0.7/main/superfluid/src/cfa.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      709 2023-05-18 07:21:56.000000 superfluid-0.0.7/main/superfluid/src/constants.py
--rw-r--r--   0 godspowereze   (501) staff       (20)       84 2023-05-10 07:50:23.000000 superfluid-0.0.7/main/superfluid/src/errors.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1011 2023-05-23 06:52:12.000000 superfluid-0.0.7/main/superfluid/src/host.py
--rw-r--r--   0 godspowereze   (501) staff       (20)     1700 2023-05-23 06:54:22.000000 superfluid-0.0.7/main/superfluid/src/operation.py
--rw-r--r--   0 godspowereze   (501) staff       (20)      759 2023-05-23 07:47:53.000000 superfluid-0.0.7/main/superfluid/src/utils.py
-drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:22:57.546629 superfluid-0.0.7/main/superfluid.egg-info/
--rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:22:57.000000 superfluid-0.0.7/main/superfluid.egg-info/PKG-INFO
--rw-r--r--   0 godspowereze   (501) staff       (20)      497 2023-05-23 16:22:57.000000 superfluid-0.0.7/main/superfluid.egg-info/SOURCES.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:22:57.000000 superfluid-0.0.7/main/superfluid.egg-info/dependency_links.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 16:22:57.000000 superfluid-0.0.7/main/superfluid.egg-info/requires.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-23 16:22:57.000000 superfluid-0.0.7/main/superfluid.egg-info/top_level.txt
--rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:22:57.549906 superfluid-0.0.7/setup.cfg
--rw-r--r--   0 godspowereze   (501) staff       (20)      824 2023-05-23 16:22:31.000000 superfluid-0.0.7/setup.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.557785 superfluid-0.0.8/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1069 2023-05-23 08:08:26.000000 superfluid-0.0.8/LICENSE.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:29:14.557644 superfluid-0.0.8/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2329 2023-05-23 08:35:46.000000 superfluid-0.0.8/README.md
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.551634 superfluid-0.0.8/main/
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.552183 superfluid-0.0.8/main/superfluid/
+-rw-r--r--   0 godspowereze   (501) staff       (20)      118 2023-05-23 16:22:23.000000 superfluid-0.0.8/main/superfluid/__init__.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.557456 superfluid-0.0.8/main/superfluid/src/
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:15:40.000000 superfluid-0.0.8/main/superfluid/src/__init__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     5339 2023-05-23 07:38:08.000000 superfluid-0.0.8/main/superfluid/src/__types__.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     9372 2023-05-23 16:28:15.000000 superfluid-0.0.8/main/superfluid/src/cfa.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      709 2023-05-18 07:21:56.000000 superfluid-0.0.8/main/superfluid/src/constants.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)       84 2023-05-10 07:50:23.000000 superfluid-0.0.8/main/superfluid/src/errors.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1014 2023-05-23 16:28:39.000000 superfluid-0.0.8/main/superfluid/src/host.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)     1701 2023-05-23 16:28:48.000000 superfluid-0.0.8/main/superfluid/src/operation.py
+-rw-r--r--   0 godspowereze   (501) staff       (20)      760 2023-05-23 16:28:53.000000 superfluid-0.0.8/main/superfluid/src/utils.py
+drwxr-xr-x   0 godspowereze   (501) staff       (20)        0 2023-05-23 16:29:14.555054 superfluid-0.0.8/main/superfluid.egg-info/
+-rw-r--r--   0 godspowereze   (501) staff       (20)     2818 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/PKG-INFO
+-rw-r--r--   0 godspowereze   (501) staff       (20)      497 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/SOURCES.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)        1 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/dependency_links.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       32 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/requires.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       11 2023-05-23 16:29:14.000000 superfluid-0.0.8/main/superfluid.egg-info/top_level.txt
+-rw-r--r--   0 godspowereze   (501) staff       (20)       38 2023-05-23 16:29:14.557822 superfluid-0.0.8/setup.cfg
+-rw-r--r--   0 godspowereze   (501) staff       (20)      824 2023-05-23 16:29:13.000000 superfluid-0.0.8/setup.py
```

### Comparing `superfluid-0.0.7/LICENSE.txt` & `superfluid-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.7/PKG-INFO` & `superfluid-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.7 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.8 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
```

### Comparing `superfluid-0.0.7/README.md` & `superfluid-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.7/main/superfluid/src/__types__.py` & `superfluid-0.0.8/main/superfluid/src/__types__.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.7/main/superfluid/src/cfa.py` & `superfluid-0.0.8/main/superfluid/src/cfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict, Optional
 
 from web3 import Web3
 from web3.types import TxParams
 from web3.middleware import geth_poa_middleware
 
-from host import Host
-from constants import CFA_V1_ABI, CFA_V1_FORWARDER_ABI, RPC_FOR_MUMBAI, CFA_V1_ADDRESS, CFA_V1_FORWARDER_ADDRESS, HOST_ADDRESS, PRIVATE_KEY
-from __types__ import GetFlowParams, GetAccountFlowInfoParams, GetFlowOperatorDataParams, GetFlowOperatorDataParamsByID, CreateFlowParams, UpdateFlowParams, DeleteFlowParams, Web3FlowInfo, UpdateFlowParams, Web3FlowOperatorData
-from errors import SFError
-from operation import Operation
+from .host import Host
+from .constants import CFA_V1_ABI, CFA_V1_FORWARDER_ABI, RPC_FOR_MUMBAI, CFA_V1_ADDRESS, CFA_V1_FORWARDER_ADDRESS, HOST_ADDRESS, PRIVATE_KEY
+from .__types__ import GetFlowParams, GetAccountFlowInfoParams, GetFlowOperatorDataParams, GetFlowOperatorDataParamsByID, CreateFlowParams, UpdateFlowParams, DeleteFlowParams, Web3FlowInfo, UpdateFlowParams, Web3FlowOperatorData
+from .errors import SFError
+from .operation import Operation
 
 
 class CFA_V1:
 
     web3 = None
     host = None
     contract = None
```

### Comparing `superfluid-0.0.7/main/superfluid/src/constants.py` & `superfluid-0.0.8/main/superfluid/src/constants.py`

 * *Files identical despite different names*

### Comparing `superfluid-0.0.7/main/superfluid/src/host.py` & `superfluid-0.0.8/main/superfluid/src/host.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, Type
 
 from web3 import Web3
 from web3.contract.contract import ContractFunction
 from web3.middleware import geth_poa_middleware
 
-from constants import HOST_ABI
-from operation import Operation
-from __types__ import BatchOperationType
+from .constants import HOST_ABI
+from .operation import Operation
+from .__types__ import BatchOperationType
 
 
 class Host:
 
     contract = None
 
     def __init__(self, rpc: str, host_address: str) -> None:
```

### Comparing `superfluid-0.0.7/main/superfluid/src/operation.py` & `superfluid-0.0.8/main/superfluid/src/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from web3.types import TxParams
 from web3.contract.contract import ContractFunction
 from web3 import Web3
 from eth_typing import HexStr
 from eth_account import Account
 
-from __types__ import BatchOperationType
+from .__types__ import BatchOperationType
 
 
 class Operation:
 
     agreement_call: ContractFunction = None
     type: BatchOperationType = None
     forwarder_txn: TxParams = None
```

### Comparing `superfluid-0.0.7/main/superfluid/src/utils.py` & `superfluid-0.0.8/main/superfluid/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from eth_typing import HexAddress
 from web3 import Web3
 
-from errors import InvalidAddressError
+from .errors import InvalidAddressError
 
 
 def to_bytes32(string: str) -> bytes:
     encoded_string = string.encode('utf-8')
     if len(encoded_string) > 32:
         raise ValueError("Input string is too long for bytes32")
     padding_length = 32 - len(encoded_string)
```

### Comparing `superfluid-0.0.7/main/superfluid.egg-info/PKG-INFO` & `superfluid-0.0.8/main/superfluid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superfluid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SDK for the Superfluid Protocol
 Home-page: https://github.com/Godspower-Eze/superfluid.py
 Author: Godspower-Eze
 Author-email: Godspowereze260@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: superfluid Version: 0.0.7 Summary: Python SDK for
+Metadata-Version: 2.1 Name: superfluid Version: 0.0.8 Summary: Python SDK for
 the Superfluid Protocol Home-page: https://github.com/Godspower-Eze/
 superfluid.py Author: Godspower-Eze Author-email: Godspowereze260@gmail.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE.txt
               ****** Welcome to Superfluid Python SDK ð ******
```

### Comparing `superfluid-0.0.7/setup.py` & `superfluid-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="superfluid",
-    version="0.0.7",
+    version="0.0.8",
     description="Python SDK for the Superfluid Protocol",
     package_dir={"": "main"},
     packages=find_packages(where="main"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Godspower-Eze/superfluid.py",
     author="Godspower-Eze",
```

