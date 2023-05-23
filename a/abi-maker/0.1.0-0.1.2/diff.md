# Comparing `tmp/abi_maker-0.1.0.tar.gz` & `tmp/abi_maker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi_maker-0.1.0.tar", max compression
+gzip compressed data, was "abi_maker-0.1.2.tar", max compression
```

## Comparing `abi_maker-0.1.0.tar` & `abi_maker-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       22 2022-09-19 16:48:25.849953 abi_maker-0.1.0/abi_maker/__init__.py
--rw-r--r--   0        0        0     2197 2023-01-05 19:00:58.646954 abi_maker-0.1.0/abi_maker/bin/abi_maker_cli.py
--rw-r--r--   0        0        0   456616 2023-01-05 19:54:50.895880 abi_maker-0.1.0/abi_maker/demo_abis/DFK_ABIS.json
--rw-r--r--   0        0        0    74637 2022-12-20 19:50:10.358139 abi_maker-0.1.0/abi_maker/demo_abis/EVO_ABIS.json
--rw-r--r--   0        0        0    19623 2022-12-20 19:44:21.122735 abi_maker-0.1.0/abi_maker/demo_abis/TREASURE_ABIS.json
--rw-r--r--   0        0        0    18930 2023-01-05 20:25:59.245380 abi_maker-0.1.0/abi_maker/make_wrapper.py
--rw-r--r--   0        0        0     5744 2023-01-05 19:00:59.870499 abi_maker-0.1.0/abi_maker/template_modules/abi_wrapper_contract.py
--rw-r--r--   0        0        0     1061 2022-11-18 22:47:37.086270 abi_maker-0.1.0/abi_maker/template_modules/credentials.py
--rw-r--r--   0        0        0      569 2023-01-05 19:15:30.402164 abi_maker-0.1.0/abi_maker/template_modules/solidity_types.py
--rw-r--r--   0        0        0      414 2022-12-13 04:00:54.457264 abi_maker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      817 2023-01-05 20:36:28.621971 abi_maker-0.1.0/setup.py
--rw-r--r--   0        0        0      373 2023-01-05 20:36:28.622123 abi_maker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-09-19 16:48:25.849953 abi_maker-0.1.2/abi_maker/__init__.py
+-rw-r--r--   0        0        0     2230 2023-04-25 16:34:05.704041 abi_maker-0.1.2/abi_maker/bin/abi_maker_cli.py
+-rw-r--r--   0        0        0   583935 2023-04-20 17:24:50.814186 abi_maker-0.1.2/abi_maker/demo_abis/DFK_ABIS.json
+-rw-r--r--   0        0        0    74637 2022-12-20 19:50:10.358139 abi_maker-0.1.2/abi_maker/demo_abis/EVO_ABIS.json
+-rw-r--r--   0        0        0    31404 2023-05-22 20:54:31.034183 abi_maker-0.1.2/abi_maker/demo_abis/Ponzi_ABIS.json
+-rw-r--r--   0        0        0    19623 2022-12-20 19:44:21.122735 abi_maker-0.1.2/abi_maker/demo_abis/TREASURE_ABIS.json
+-rw-r--r--   0        0        0    20942 2023-05-23 19:53:47.151399 abi_maker-0.1.2/abi_maker/make_wrapper.py
+-rw-r--r--   0        0        0     6293 2023-04-25 16:28:11.119967 abi_maker-0.1.2/abi_maker/template_modules/abi_contract_wrapper.py
+-rw-r--r--   0        0        0     1287 2023-04-25 16:26:44.262332 abi_maker-0.1.2/abi_maker/template_modules/abi_multi_contract_wrapper.py
+-rw-r--r--   0        0        0     2008 2023-04-07 21:54:10.156996 abi_maker-0.1.2/abi_maker/template_modules/credentials.py
+-rw-r--r--   0        0        0      819 2023-04-25 22:02:38.936676 abi_maker-0.1.2/abi_maker/template_modules/solidity_types.py
+-rw-r--r--   0        0        0      414 2023-05-23 20:05:44.056094 abi_maker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 abi_maker-0.1.2/PKG-INFO
```

### Comparing `abi_maker-0.1.0/abi_maker/bin/abi_maker_cli.py` & `abi_maker-0.1.2/abi_maker/bin/abi_maker_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 def main():
     args = parse_all_args()
     
     files_written = make_wrapper.write_project_wrapper( project_name=args.project, 
                                                         abi_json_path=args.json, 
                                                         output_dir=args.output,
                                                         overwrite_ok=args.force_overwrite)
-    package_dir = args.output / args.project
+    # package_dir = args.output / args.project
+    package_dir = args.output 
     print(f'Wrote {len(files_written)} files to {package_dir}')
 
 
 def parse_all_args(args_in=None):
     ''' Set up argparser and return a namespace with named
     values from the command line arguments.  
     If help is requested (-h / --help) the help message will be printed
```

### Comparing `abi_maker-0.1.0/abi_maker/demo_abis/DFK_ABIS.json` & `abi_maker-0.1.2/abi_maker/demo_abis/DFK_ABIS.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9694177862637344%*

 * *Differences: {"'CONTRACTS'": "{'AirdropClaim': {'ADDRESS': {'sd': "*

 * *                "'0x0000000000000000000000000000000000000000'}}, 'AtonementCrystal': {'ADDRESS': "*

 * *                "{'sd': '0x0000000000000000000000000000000000000000'}}, 'Banker': {'ADDRESS': "*

 * *                "{'sd': '0x0000000000000000000000000000000000000000'}}, 'BirthdayCake': "*

 * *                "{'ADDRESS': {'sd': '0x0000000000000000000000000000000000000000'}}, 'CharityFund': "*

 * *                "{'ADDRESS': {'sd': '0x00000000000000000000000000000000 […]*

```diff
@@ -293,15 +293,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x947873092dc57C1A70704033c41cB110f4462a8B",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "Alchemist": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -3002,15 +3002,15 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x3A28E0D4eCF7558e1ba7357070032C5A6105B0C2",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "Banker": {
             "ABI": [
                 {
                     "inputs": [
                         {
@@ -3249,15 +3249,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x4b1F4C7981465F814c4A78d79be21558A60f57F2",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "BirthdayCake": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -3687,15 +3687,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x184223A0921B58F5a0ddFD6448d8b2715EcC87a7",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "CharityFund": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -4077,15 +4077,15 @@
                 {
                     "stateMutability": "payable",
                     "type": "receive"
                 }
             ],
             "ADDRESS": {
                 "cv": "0xABABB0A2c42274D0e81417B824CABca464F5c16C",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "CrystalCore": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -4236,24 +4236,138 @@
                     "name": "Paused",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "previousAdminRole",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "newAdminRole",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "RoleAdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleGranted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleRevoked",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": false,
                             "internalType": "address",
                             "name": "account",
                             "type": "address"
                         }
                     ],
                     "name": "Unpaused",
                     "type": "event"
                 },
                 {
+                    "inputs": [],
+                    "name": "CRYSTAL_MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "DEFAULT_ADMIN_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_recipient",
                             "type": "address"
                         },
                         {
@@ -4400,14 +4514,33 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "getRoleAdmin",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
                             "name": "_address",
                             "type": "address"
                         }
                     ],
                     "name": "getUserCrystals",
                     "outputs": [
@@ -4419,14 +4552,56 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "grantRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "hasRole",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
                             "name": "_heroCoreAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "address",
                             "name": "_statScienceAddress",
@@ -4494,14 +4669,50 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "renounceRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "revokeRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
                             "name": "_heroCoreAddress",
                             "type": "address"
                         }
                     ],
                     "name": "setHeroCore",
                     "outputs": [],
@@ -4531,14 +4742,33 @@
                     ],
                     "name": "setWaitBlocks",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
+                    "inputs": [
+                        {
+                            "internalType": "bytes4",
+                            "name": "interfaceId",
+                            "type": "bytes4"
+                        }
+                    ],
+                    "name": "supportsInterface",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [],
                     "name": "totalCrystals",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
@@ -7681,15 +7911,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x9EEaBBcf42F0c4900d302544Cce599811C2De2b9",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "DarkSummoning": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -7875,24 +8105,312 @@
                     "name": "EnhancementStoneAdded",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "feeAddress",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "feePercent",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "FeeAddressAdded",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeDeferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeDisbursed",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeLockedBurned",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "startTime",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "GlobalStartTimeSet",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": false,
                             "internalType": "uint8",
                             "name": "version",
                             "type": "uint8"
                         }
                     ],
                     "name": "Initialized",
                     "type": "event"
                 },
                 {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Paused",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "previousAdminRole",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "newAdminRole",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "RoleAdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleGranted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleRevoked",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Unpaused",
+                    "type": "event"
+                },
+                {
+                    "inputs": [],
+                    "name": "DEFAULT_ADMIN_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "",
                             "type": "address"
                         }
                     ],
@@ -8423,14 +8941,75 @@
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "getRoleAdmin",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "grantRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "hasRole",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [],
                     "name": "increasePerGen",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
@@ -8449,14 +9028,80 @@
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_crystalCoreAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_heroCoreAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_powerTokenAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_gaiaTearsAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_statScienceAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_graveyard",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_flagStorage",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_meditationCircle",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_assistingAuction",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "initialize",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "paused",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [],
                     "name": "powerToken",
                     "outputs": [
                         {
                             "internalType": "contract IPowerToken",
                             "name": "",
                             "type": "address"
@@ -8477,27 +9122,156 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "renounceRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "revokeRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address[]",
+                            "name": "_feeAddresses",
+                            "type": "address[]"
+                        },
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_feePercents",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "setFees",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_heroCoreAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setHeroCore",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_powerTokenAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setPowerToken",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_statScienceAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setStatScience",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_baseSummonFee",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_increasePerSummon",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_increasePerGen",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setSummonFees",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
                             "name": "_tearsAddress",
                             "type": "address"
                         }
                     ],
                     "name": "setTears",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "address",
+                            "name": "_tokenUnlockerAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setTokenUnlocker",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "uint256",
                             "name": "_summonerId",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_assistantId",
@@ -8524,19 +9298,76 @@
                             "type": "uint8"
                         }
                     ],
                     "name": "summonCrystal",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_summonerId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_assistantId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_summonerTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_assistantTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_enhancementStone",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint8",
+                            "name": "_rarityBonusCharges",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "summonCrystalWithLocked",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes4",
+                            "name": "interfaceId",
+                            "type": "bytes4"
+                        }
+                    ],
+                    "name": "supportsInterface",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x70908Fd7278aab183C7EfC4f3449184E98e2e305",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "DuelRankClaim": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -9282,15 +10113,15 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x89789a580fdE00319493BdCdB6C65959DAB1e517",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "ERC20": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -9631,14 +10462,295 @@
                 }
             ],
             "ADDRESS": {
                 "cv": null,
                 "sd": null
             }
         },
+        "FlagStorageV2": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint32",
+                                    "name": "levelCarryover",
+                                    "type": "uint32"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct DarkSummoning",
+                            "name": "values",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "DarkSummoningStorageSet",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "player",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint32",
+                                    "name": "summonRecord",
+                                    "type": "uint32"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledGameGenes",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledAppearanceGenes",
+                                    "type": "bool"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Gen0RerollSD",
+                            "name": "values",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "Gen0RerollSDStorageSet",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "previousOwner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "OwnershipTransferred",
+                    "type": "event"
+                },
+                {
+                    "inputs": [],
+                    "name": "owner",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "owner_",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "transferOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_access",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "setModerator",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_access",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "setUpdater",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getDarkSummoningStorage",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint32",
+                                    "name": "levelCarryover",
+                                    "type": "uint32"
+                                }
+                            ],
+                            "internalType": "struct DarkSummoning",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint32",
+                            "name": "_value",
+                            "type": "uint32"
+                        }
+                    ],
+                    "name": "setLevelCarryover",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getGen0RerollSDStorage",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "player",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint32",
+                                    "name": "summonRecord",
+                                    "type": "uint32"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledGameGenes",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledAppearanceGenes",
+                                    "type": "bool"
+                                }
+                            ],
+                            "internalType": "struct Gen0RerollSD",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "player",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint32",
+                                    "name": "summonRecord",
+                                    "type": "uint32"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledGameGenes",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "rerolledAppearanceGenes",
+                                    "type": "bool"
+                                }
+                            ],
+                            "internalType": "struct Gen0RerollSD",
+                            "name": "_reroll",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "setGen0RerollSDStorage",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x75d8ba2E4725633FcdcC165332dCA04c107915cA",
+                "sd": "0xeb9ff38209dCC4236DBFb3C275c0AAeEBf0B92Cf"
+            }
+        },
         "Gen0Airdrop": {
             "ABI": [
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_heroCoreAddress",
@@ -10010,15 +11122,15 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0xBd1f65e7f350C614d364AEFeB2d87F829b0E465d",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "Gen0Reroll": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -11628,15 +12740,3003 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x74934378840D77E36AeF1f031D301549b4e1a225",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
+            }
+        },
+        "GeneReroll": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "beforeHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "afterHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bool",
+                            "name": "craftingGenesRerolled",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "CraftingGenesRerolled",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "HeroRerollStarted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "heroBefore",
+                            "type": "tuple"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "heroAfter",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "HeroRerolled",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "version",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "Initialized",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "stat",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "increase",
+                            "type": "uint8"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "updateType",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "StatUp",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "beforeHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct Hero",
+                            "name": "afterHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8[]",
+                            "name": "geneIndex",
+                            "type": "uint8[]"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8[]",
+                            "name": "rankType",
+                            "type": "uint8[]"
+                        }
+                    ],
+                    "name": "TaintedGenesRerolled",
+                    "type": "event"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "cancelReroll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "endRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "heroToRerollData",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "internalType": "struct Hero",
+                            "name": "beforeHero",
+                            "type": "tuple"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "seedblock",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "finishTime",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "rerollStarted",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_heroIds",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "multiEndRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_heroIds",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "multiStartRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "startRoll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x4b98f4C73fadA8E9C3f573502713FCebfA5a98AC",
+                "sd": "0xD0E292bAfBB1F691fEAFa7ddE1050EAEa923b2e3"
             }
         },
         "HeroAuction": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -14039,42 +18139,14 @@
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "string",
-                            "name": "_name",
-                            "type": "string"
-                        },
-                        {
-                            "internalType": "string",
-                            "name": "_symbol",
-                            "type": "string"
-                        },
-                        {
-                            "internalType": "string",
-                            "name": "_url",
-                            "type": "string"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "_statScienceAddress",
-                            "type": "address"
-                        }
-                    ],
-                    "name": "initialize",
-                    "outputs": [],
-                    "stateMutability": "nonpayable",
-                    "type": "function"
-                },
-                {
-                    "inputs": [
-                        {
-                            "internalType": "string",
                             "name": "name",
                             "type": "string"
                         },
                         {
                             "internalType": "string",
                             "name": "symbol",
                             "type": "string"
@@ -14761,15 +18833,16 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0xEb9B61B145D6489Be575D3603F4a704810e143dF",
-                "sd": "0x268CC8248FFB72Cd5F3e73A9a20Fa2FF40EfbA61"
+                "sd": "0x268CC8248FFB72Cd5F3e73A9a20Fa2FF40EfbA61",
+                "sd1": "0x5F753dcDf9b1AD9AabC1346614D1f4746fd6Ce5C"
             }
         },
         "HeroSummoning": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -14795,14 +18868,75 @@
                     "name": "CrystalAirdrop",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "crystalId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "owner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "summonerId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "assistantId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "generation",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "createdBlock",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "summonerTears",
+                            "type": "uint8"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "assistantTears",
+                            "type": "uint8"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "enhancementStone",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "CrystalDarkSummoned",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": true,
                             "internalType": "address",
                             "name": "owner",
                             "type": "address"
                         },
                         {
                             "indexed": false,
@@ -14894,14 +19028,175 @@
                     "name": "EnhancementStoneAdded",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "feeAddress",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "feePercent",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "FeeAddressAdded",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeDeferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeDisbursed",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeLockedBurned",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "startTime",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "GlobalStartTimeSet",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": false,
                             "internalType": "uint8",
                             "name": "version",
                             "type": "uint8"
                         }
                     ],
                     "name": "Initialized",
@@ -14920,24 +19215,125 @@
                     "name": "Paused",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "previousAdminRole",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "newAdminRole",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "RoleAdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleGranted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleRevoked",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": false,
                             "internalType": "address",
                             "name": "account",
                             "type": "address"
                         }
                     ],
                     "name": "Unpaused",
                     "type": "event"
                 },
                 {
+                    "inputs": [],
+                    "name": "DEFAULT_ADMIN_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "",
                             "type": "address"
                         }
                     ],
@@ -15404,352 +19800,1684 @@
                                 }
                             ],
                             "internalType": "struct Hero",
                             "name": "_hero",
                             "type": "tuple"
                         }
                     ],
-                    "name": "calculateSummoningCost",
+                    "name": "calculateSummoningCost",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "cooldownPerGen",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "feeAddresses",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "feePercents",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "getRoleAdmin",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "grantRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "hasRole",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "increasePerGen",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "increasePerSummon",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "lastLockedSummon",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "lockedSummonCooldown",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "pause",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "paused",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "powerToken",
+                    "outputs": [
+                        {
+                            "internalType": "contract IPowerToken",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "removeEnhancementStone",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "renounceRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "revokeRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address[]",
+                            "name": "_feeAddresses",
+                            "type": "address[]"
+                        },
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_feePercents",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "setFees",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_heroCoreAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setHeroCore",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_lockedSummonCooldown",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setLockedSummonCooldown",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_powerTokenAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setPowerToken",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_statScienceAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setStatScience",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_baseCooldown",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_cooldownPerGen",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setSummonCooldowns",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_baseSummonFee",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_increasePerSummon",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_increasePerGen",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setSummonFees",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_tearsAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setTears",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_tokenUnlockerAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setTokenUnlocker",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_summonerId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_assistantId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_summonerTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_assistantTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_enhancementStone",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "summonCrystal",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_summonerId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_assistantId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_summonerTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_assistantTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_enhancementStone",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_assistingAuctionAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_hireAmount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "summonCrystalWithAuction",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_summonerId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_assistantId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_summonerTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_assistantTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_enhancementStone",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_assistingAuctionAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_hireAmount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "summonCrystalWithAuctionWithLocked",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_summonerId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_assistantId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_summonerTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_assistantTears",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_enhancementStone",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "summonCrystalWithLocked",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes4",
+                            "name": "interfaceId",
+                            "type": "bytes4"
+                        }
+                    ],
+                    "name": "supportsInterface",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "unpause",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0xBc36D18662Bb97F9e74B1EAA1B752aA7A44595A7",
+                "sd": "0xb086584f476Ad21B40aF0672f385a67334A0b294"
+            }
+        },
+        "ItemBridge": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "receiver",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "item",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "id",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "ERC1155Received",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "version",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "Initialized",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "bytes32",
+                            "name": "identifier",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "contractAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "ItemMapped",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "receiver",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "item",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "ItemReceived",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "MessageFailed",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "previousOwner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "OwnershipTransferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Paused",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "SetTrustedRemote",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Unpaused",
+                    "type": "event"
+                },
+                {
+                    "inputs": [],
+                    "name": "FUNCTION_TYPE_SEND",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [],
-                    "name": "cooldownPerGen",
+                    "name": "NO_EXTRA_GAS",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "address",
+                            "name": "_lzEndpoint",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "__NonblockingLzAppUpgradeable_init",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "__NonblockingLzAppUpgradeable_init_unchained",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
                             "internalType": "uint256",
-                            "name": "",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
                             "type": "uint256"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_useZro",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
                         }
                     ],
-                    "name": "feeAddresses",
+                    "name": "estimateFeeSendERC1155",
                     "outputs": [
                         {
-                            "internalType": "address",
+                            "internalType": "uint256",
                             "name": "",
-                            "type": "address"
+                            "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
                             "internalType": "uint256",
-                            "name": "",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
                             "type": "uint256"
                         }
                     ],
-                    "name": "feePercents",
+                    "name": "estimateFeeSendERC1155",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
-                    "inputs": [],
-                    "name": "increasePerGen",
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "estimateFeeSendERC20",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
-                    "inputs": [],
-                    "name": "increasePerSummon",
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "_useZro",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "estimateFeeSendERC20",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
-                            "internalType": "address",
-                            "name": "_crystalCoreAddress",
-                            "type": "address"
+                            "internalType": "uint16",
+                            "name": "",
+                            "type": "uint16"
                         },
                         {
-                            "internalType": "address",
-                            "name": "_heroCoreAddress",
-                            "type": "address"
+                            "internalType": "bytes",
+                            "name": "",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "failedMessages",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "forceResumeReceive",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_version",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint16",
+                            "name": "_chainId",
+                            "type": "uint16"
                         },
                         {
                             "internalType": "address",
-                            "name": "_powerTokenAddress",
+                            "name": "",
                             "type": "address"
                         },
                         {
+                            "internalType": "uint256",
+                            "name": "_configType",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getConfig",
+                    "outputs": [
+                        {
+                            "internalType": "bytes",
+                            "name": "",
+                            "type": "bytes"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "getGasLimit",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "gasLimit",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "pure",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
-                            "name": "_gaiaTearsAddress",
+                            "name": "_lzEndpoint",
                             "type": "address"
                         },
                         {
                             "internalType": "address",
-                            "name": "_statScienceAddress",
+                            "name": "_itemMinter",
                             "type": "address"
                         }
                     ],
                     "name": "initialize",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
-                    "inputs": [],
-                    "name": "paused",
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "isTrustedRemote",
                     "outputs": [
                         {
                             "internalType": "bool",
                             "name": "",
                             "type": "bool"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
-                    "inputs": [],
-                    "name": "powerToken",
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "itemAddresses",
                     "outputs": [
                         {
-                            "internalType": "contract IPowerToken",
+                            "internalType": "address",
                             "name": "",
                             "type": "address"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "address",
-                            "name": "_address",
+                            "name": "",
                             "type": "address"
                         }
                     ],
-                    "name": "removeEnhancementStone",
-                    "outputs": [],
-                    "stateMutability": "nonpayable",
+                    "name": "itemIdentifiers",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "lzEndpoint",
+                    "outputs": [
+                        {
+                            "internalType": "contract ILayerZeroEndpointUpgradeable",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
-                            "internalType": "address[]",
-                            "name": "_feeAddresses",
-                            "type": "address[]"
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
                         },
                         {
-                            "internalType": "uint256[]",
-                            "name": "_feePercents",
-                            "type": "uint256[]"
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
                         }
                     ],
-                    "name": "setFees",
+                    "name": "lzReceive",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "string",
+                            "name": "_identifier",
+                            "type": "string"
+                        },
+                        {
                             "internalType": "address",
-                            "name": "_heroCoreAddress",
+                            "name": "_contractAddress",
                             "type": "address"
                         }
                     ],
-                    "name": "setHeroCore",
+                    "name": "mapItem",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "uint16",
+                            "name": "",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "minDstGasLookup",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "nonblockingLzReceive",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "owner",
+                    "outputs": [
+                        {
                             "internalType": "address",
-                            "name": "_statScienceAddress",
+                            "name": "",
                             "type": "address"
                         }
                     ],
-                    "name": "setStatScience",
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "pause",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "paused",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "renounceOwnership",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_nonce",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_payload",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "retryMessage",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
                             "internalType": "uint256",
-                            "name": "_baseCooldown",
+                            "name": "_amount",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_cooldownPerGen",
+                            "name": "_id",
                             "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_zroPaymentAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
                         }
                     ],
-                    "name": "setSummonCooldowns",
+                    "name": "sendERC1155",
                     "outputs": [],
-                    "stateMutability": "nonpayable",
+                    "stateMutability": "payable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
-                            "internalType": "uint256",
-                            "name": "_baseSummonFee",
-                            "type": "uint256"
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_increasePerSummon",
+                            "name": "_amount",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_increasePerGen",
+                            "name": "_id",
                             "type": "uint256"
                         }
                     ],
-                    "name": "setSummonFees",
+                    "name": "sendERC1155",
                     "outputs": [],
-                    "stateMutability": "nonpayable",
+                    "stateMutability": "payable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
                             "internalType": "address",
-                            "name": "_tearsAddress",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_zroPaymentAddress",
                             "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_adapterParams",
+                            "type": "bytes"
                         }
                     ],
-                    "name": "setTears",
+                    "name": "sendERC20",
                     "outputs": [],
-                    "stateMutability": "nonpayable",
+                    "stateMutability": "payable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
-                            "internalType": "uint256",
-                            "name": "_summonerId",
-                            "type": "uint256"
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_receiver",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_item",
+                            "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_assistantId",
+                            "name": "_amount",
                             "type": "uint256"
-                        },
+                        }
+                    ],
+                    "name": "sendERC20",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
                         {
                             "internalType": "uint16",
-                            "name": "_summonerTears",
+                            "name": "_version",
                             "type": "uint16"
                         },
                         {
                             "internalType": "uint16",
-                            "name": "_assistantTears",
+                            "name": "_chainId",
                             "type": "uint16"
                         },
                         {
-                            "internalType": "address",
-                            "name": "_enhancementStone",
-                            "type": "address"
+                            "internalType": "uint256",
+                            "name": "_configType",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_config",
+                            "type": "bytes"
                         }
                     ],
-                    "name": "summonCrystal",
+                    "name": "setConfig",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "uint16",
+                            "name": "_dstChainId",
+                            "type": "uint16"
+                        },
+                        {
                             "internalType": "uint256",
-                            "name": "_summonerId",
+                            "name": "_type",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_assistantId",
+                            "name": "_dstGasAmount",
                             "type": "uint256"
-                        },
+                        }
+                    ],
+                    "name": "setMinDstGasLookup",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
                         {
                             "internalType": "uint16",
-                            "name": "_summonerTears",
+                            "name": "_version",
                             "type": "uint16"
-                        },
+                        }
+                    ],
+                    "name": "setReceiveVersion",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
                         {
                             "internalType": "uint16",
-                            "name": "_assistantTears",
+                            "name": "_version",
                             "type": "uint16"
-                        },
+                        }
+                    ],
+                    "name": "setSendVersion",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
                         {
-                            "internalType": "address",
-                            "name": "_enhancementStone",
-                            "type": "address"
+                            "internalType": "uint16",
+                            "name": "_srcChainId",
+                            "type": "uint16"
                         },
                         {
+                            "internalType": "bytes",
+                            "name": "_srcAddress",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "setTrustedRemote",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "_useCustomAdapterParams",
+                            "type": "bool"
+                        }
+                    ],
+                    "name": "setUseCustomAdapterParams",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
-                            "name": "_assistingAuctionAddress",
+                            "name": "newOwner",
                             "type": "address"
-                        },
+                        }
+                    ],
+                    "name": "transferOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
                         {
-                            "internalType": "uint256",
-                            "name": "_hireAmount",
-                            "type": "uint256"
+                            "internalType": "uint16",
+                            "name": "",
+                            "type": "uint16"
                         }
                     ],
-                    "name": "summonCrystalWithAuction",
+                    "name": "trustedRemoteLookup",
+                    "outputs": [
+                        {
+                            "internalType": "bytes",
+                            "name": "",
+                            "type": "bytes"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "unpause",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "useCustomAdapterParams",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
                 }
             ],
             "ADDRESS": {
-                "cv": "0xBc36D18662Bb97F9e74B1EAA1B752aA7A44595A7",
-                "sd": "0xb086584f476Ad21B40aF0672f385a67334A0b294"
+                "cv": "0x501CdC4ef10b63219704Bf6aDb785dfccb06deE2",
+                "sd": "0x6d5B86EaC9097EA4a94B2b69Cd4854678B89f839"
             }
         },
         "ItemConsumer": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -16629,22 +22357,46 @@
                             "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "buyPrice",
+                            "name": "startingPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "playerSellPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "minPrice",
                             "type": "uint256"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "sellPrice",
+                            "name": "deltaPriceIncrease",
                             "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "priceIncreaseDecay",
+                            "type": "uint64"
                         }
                     ],
                     "name": "ItemAdded",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
@@ -16691,75 +22443,93 @@
                             "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "buyPrice",
+                            "name": "currentPrice",
                             "type": "uint256"
                         },
                         {
                             "indexed": false,
                             "internalType": "uint256",
-                            "name": "sellPrice",
+                            "name": "playerSellPrice",
                             "type": "uint256"
                         },
                         {
                             "indexed": false,
-                            "internalType": "uint8",
-                            "name": "status",
-                            "type": "uint8"
-                        }
-                    ],
-                    "name": "ItemUpdated",
-                    "type": "event"
-                },
-                {
-                    "anonymous": false,
-                    "inputs": [
+                            "internalType": "uint256",
+                            "name": "minPrice",
+                            "type": "uint256"
+                        },
                         {
                             "indexed": false,
-                            "internalType": "address",
-                            "name": "account",
-                            "type": "address"
-                        }
-                    ],
-                    "name": "Paused",
-                    "type": "event"
-                },
-                {
-                    "anonymous": false,
-                    "inputs": [
+                            "internalType": "uint256",
+                            "name": "deltaPriceIncrease",
+                            "type": "uint256"
+                        },
                         {
                             "indexed": false,
-                            "internalType": "address",
-                            "name": "account",
-                            "type": "address"
+                            "internalType": "uint256",
+                            "name": "decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "priceIncreaseDecay",
+                            "type": "uint64"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "status",
+                            "type": "uint8"
                         }
                     ],
-                    "name": "Unpaused",
+                    "name": "ItemUpdated",
                     "type": "event"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_itemAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_buyPrice",
+                            "name": "_startingPrice",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_sellPrice",
                             "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_minPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_deltaPriceIncrease",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_priceIncreaseDecay",
+                            "type": "uint64"
                         }
                     ],
                     "name": "addTradeItem",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
@@ -16789,82 +22559,252 @@
                             "name": "_itemAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_quantity",
                             "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_maxPrice",
+                            "type": "uint256"
                         }
                     ],
                     "name": "buyItem",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
-                    "inputs": [],
-                    "name": "getTradeItems",
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_itemAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_quantity",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getNextPrice",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getTradeItem",
                     "outputs": [
                         {
                             "components": [
                                 {
                                     "internalType": "uint256",
                                     "name": "id",
                                     "type": "uint256"
                                 },
                                 {
-                                    "internalType": "contract IInventoryItem",
+                                    "internalType": "address",
                                     "name": "item",
                                     "type": "address"
                                 },
                                 {
                                     "internalType": "uint256",
-                                    "name": "buyPrice",
+                                    "name": "currentPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "playerSellPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "minPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "deltaPriceIncrease",
                                     "type": "uint256"
                                 },
                                 {
                                     "internalType": "uint256",
-                                    "name": "sellPrice",
+                                    "name": "decreaseRate",
                                     "type": "uint256"
                                 },
                                 {
+                                    "internalType": "uint64",
+                                    "name": "priceIncreaseDecay",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "lastPurchaseTimestamp",
+                                    "type": "uint64"
+                                },
+                                {
                                     "internalType": "uint8",
                                     "name": "status",
                                     "type": "uint8"
                                 }
                             ],
-                            "internalType": "struct ItemGoldTrader.TradeItem[]",
+                            "internalType": "struct TraderTypes.TradeItem",
                             "name": "",
-                            "type": "tuple[]"
+                            "type": "tuple"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "address",
-                            "name": "_dfkGoldAddress",
+                            "name": "_itemAddress",
                             "type": "address"
                         }
                     ],
-                    "name": "initialize",
-                    "outputs": [],
-                    "stateMutability": "nonpayable",
+                    "name": "getTradeItemByAddress",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "item",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "currentPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "playerSellPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "minPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "deltaPriceIncrease",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "decreaseRate",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "priceIncreaseDecay",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "lastPurchaseTimestamp",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint8",
+                                    "name": "status",
+                                    "type": "uint8"
+                                }
+                            ],
+                            "internalType": "struct TraderTypes.TradeItem",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [],
-                    "name": "paused",
+                    "name": "getTradeItems",
                     "outputs": [
                         {
-                            "internalType": "bool",
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "item",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "currentPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "playerSellPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "minPrice",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "deltaPriceIncrease",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "decreaseRate",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "priceIncreaseDecay",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint64",
+                                    "name": "lastPurchaseTimestamp",
+                                    "type": "uint64"
+                                },
+                                {
+                                    "internalType": "uint8",
+                                    "name": "status",
+                                    "type": "uint8"
+                                }
+                            ],
+                            "internalType": "struct TraderTypes.TradeItem[]",
                             "name": "",
-                            "type": "bool"
+                            "type": "tuple[]"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
@@ -16896,29 +22836,54 @@
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "id",
                             "type": "uint256"
                         },
                         {
-                            "internalType": "contract IInventoryItem",
+                            "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "buyPrice",
+                            "name": "currentPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "playerSellPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "minPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "deltaPriceIncrease",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "sellPrice",
+                            "name": "decreaseRate",
                             "type": "uint256"
                         },
                         {
+                            "internalType": "uint64",
+                            "name": "priceIncreaseDecay",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "lastPurchaseTimestamp",
+                            "type": "uint64"
+                        },
+                        {
                             "internalType": "uint8",
                             "name": "status",
                             "type": "uint8"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
@@ -16928,23 +22893,43 @@
                         {
                             "internalType": "address",
                             "name": "_itemAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "uint256",
-                            "name": "_buyPrice",
+                            "name": "_currentPrice",
                             "type": "uint256"
                         },
                         {
                             "internalType": "uint256",
                             "name": "_sellPrice",
                             "type": "uint256"
                         },
                         {
+                            "internalType": "uint256",
+                            "name": "_minPrice",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_deltaPriceIncrease",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_decreaseRate",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint64",
+                            "name": "_priceIncreaseDecay",
+                            "type": "uint64"
+                        },
+                        {
                             "internalType": "uint8",
                             "name": "_status",
                             "type": "uint8"
                         }
                     ],
                     "name": "updateTradeItem",
                     "outputs": [],
@@ -18851,15 +24836,15 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x77D991987ca85214f9686131C58c1ABE4C93E547",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "LandCore": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -22567,14 +28552,460 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0xD507b6b299d9FC835a0Df92f718920D13fA49B47",
                 "sd": "0xdbEE8C336B06f2d30a6d2bB3817a3Ae0E34f4900"
             }
         },
+        "Multicall3": {
+            "ABI": [
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "aggregate",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes[]",
+                            "name": "returnData",
+                            "type": "bytes[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "allowFailure",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call3[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "aggregate3",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "allowFailure",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "value",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call3Value[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "aggregate3Value",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "blockAndAggregate",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getBasefee",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "basefee",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getBlockHash",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getBlockNumber",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getChainId",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "chainid",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockCoinbase",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "coinbase",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockDifficulty",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "difficulty",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockGasLimit",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "gaslimit",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getCurrentBlockTimestamp",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "timestamp",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "addr",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "getEthBalance",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "balance",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getLastBlockHash",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "requireSuccess",
+                            "type": "bool"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "tryAggregate",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "requireSuccess",
+                            "type": "bool"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "address",
+                                    "name": "target",
+                                    "type": "address"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "callData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Call[]",
+                            "name": "calls",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "name": "tryBlockAndAggregate",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "blockNumber",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes32",
+                            "name": "blockHash",
+                            "type": "bytes32"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "success",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bytes",
+                                    "name": "returnData",
+                                    "type": "bytes"
+                                }
+                            ],
+                            "internalType": "struct Multicall3.Result[]",
+                            "name": "returnData",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0xcA11bde05977b3631167028862bE2a173976CA11",
+                "sd": "0xcA11bde05977b3631167028862bE2a173976CA11"
+            }
+        },
         "Pasture": {
             "ABI": [
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_petCore",
@@ -23656,14 +30087,428 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0x72F860bF73ffa3FC42B97BbcF43Ae80280CFcdc3",
                 "sd": "0x7aB1C574A8762bEde901F32670481c0427DdF626"
             }
         },
+        "PetBridge": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "previousAdmin",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "newAdmin",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "AdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "implementation",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "Upgraded",
+                    "type": "event"
+                },
+                {
+                    "stateMutability": "payable",
+                    "type": "fallback"
+                },
+                {
+                    "inputs": [],
+                    "name": "admin",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newAdmin",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "changeAdmin",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "implementation",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newImplementation",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "upgradeTo",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newImplementation",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "data",
+                            "type": "bytes"
+                        }
+                    ],
+                    "name": "upgradeToAndCall",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "stateMutability": "payable",
+                    "type": "receive"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "previousOwner",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "OwnershipTransferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "petId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "arrivalChainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "PetArrived",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "petId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "arrivalChainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "PetSent",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "_srcChainId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "bytes32",
+                            "name": "_srcAddress",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "SetTrustedRemote",
+                    "type": "event"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "_srcAddress",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_srcChainId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_message",
+                            "type": "bytes"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_executor",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "executeMessage",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_chainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getTrustedRemote",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "trustedRemote",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_messageBus",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_pets",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "initialize",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "messageBus",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "msgGasLimit",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "owner",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "pets",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "renounceOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_petId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_dstChainId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "sendPet",
+                    "outputs": [],
+                    "stateMutability": "payable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_messageBus",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setMessageBus",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_msgGasLimit",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "setMsgGasLimit",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_srcChainId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "bytes32",
+                            "name": "_srcAddress",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "setTrustedRemote",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "newOwner",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "transferOwnership",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "initialLogic",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "initialAdmin",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "bytes",
+                            "name": "_data",
+                            "type": "bytes"
+                        }
+                    ],
+                    "stateMutability": "payable",
+                    "type": "constructor"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0x36829ba54e6A0f11fB6e5A45aC5aD2742ec86a0B",
+                "sd": "0x5EcB820B32b60cCEd4506bd3b06C80BaFb879446"
+            }
+        },
         "PetCore": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
                             "indexed": true,
@@ -25395,14 +32240,162 @@
                     "name": "EggIncubated",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "feeAddress",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "uint256",
+                            "name": "feePercent",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "FeeAddressAdded",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeDeferred",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeDisbursed",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "source",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "from",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "to",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "token",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "amount",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint64",
+                            "name": "timestamp",
+                            "type": "uint64"
+                        }
+                    ],
+                    "name": "FeeLockedBurned",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": false,
                             "internalType": "uint8",
                             "name": "version",
                             "type": "uint8"
                         }
                     ],
                     "name": "Initialized",
@@ -25421,24 +32414,138 @@
                     "name": "Paused",
                     "type": "event"
                 },
                 {
                     "anonymous": false,
                     "inputs": [
                         {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "previousAdminRole",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "newAdminRole",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "RoleAdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleGranted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleRevoked",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
                             "indexed": false,
                             "internalType": "address",
                             "name": "account",
                             "type": "address"
                         }
                     ],
                     "name": "Unpaused",
                     "type": "event"
                 },
                 {
+                    "inputs": [],
+                    "name": "DEFAULT_ADMIN_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "HATCHING_MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [
                         {
                             "internalType": "uint256",
                             "name": "_eggId",
                             "type": "uint256"
                         }
                     ],
@@ -25492,14 +32599,52 @@
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
                             "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "feeAddresses",
+                    "outputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "feePercents",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
                             "name": "_eggId",
                             "type": "uint256"
                         }
                     ],
                     "name": "getEgg",
                     "outputs": [
                         {
@@ -25547,14 +32692,33 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "getRoleAdmin",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
                             "name": "_address",
                             "type": "address"
                         }
                     ],
                     "name": "getUserEggs",
                     "outputs": [
@@ -25566,14 +32730,56 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "grantRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "hasRole",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "uint8",
                             "name": "_eggType",
                             "type": "uint8"
                         },
                         {
                             "internalType": "uint8",
                             "name": "_tier",
@@ -25584,54 +32790,64 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [
                         {
+                            "internalType": "uint8",
+                            "name": "_eggType",
+                            "type": "uint8"
+                        },
+                        {
+                            "internalType": "uint8",
+                            "name": "_tier",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "incubateEggWithLocked",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
                             "internalType": "address",
                             "name": "_petCoreAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "address",
-                            "name": "_jewelTokenAddress",
+                            "name": "_powerTokenAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "address",
                             "name": "_goldAddress",
                             "type": "address"
                         },
                         {
                             "internalType": "address",
                             "name": "_gaiaTearsAddress",
                             "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_randomGeneratorAddress",
+                            "type": "address"
                         }
                     ],
                     "name": "initialize",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
                     "inputs": [],
-                    "name": "jewelToken",
-                    "outputs": [
-                        {
-                            "internalType": "contract IJewelToken",
-                            "name": "",
-                            "type": "address"
-                        }
-                    ],
-                    "stateMutability": "view",
-                    "type": "function"
-                },
-                {
-                    "inputs": [],
                     "name": "originId",
                     "outputs": [
                         {
                             "internalType": "uint8",
                             "name": "",
                             "type": "uint8"
                         }
@@ -25656,26 +32872,39 @@
                             "type": "bool"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
+                    "inputs": [],
+                    "name": "powerToken",
+                    "outputs": [
+                        {
+                            "internalType": "contract IPowerToken",
+                            "name": "",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
                         }
                     ],
                     "name": "priceTiers",
                     "outputs": [
                         {
                             "internalType": "uint8",
-                            "name": "jewelCost",
+                            "name": "powerTokenCost",
                             "type": "uint8"
                         },
                         {
                             "internalType": "uint16",
                             "name": "goldCost",
                             "type": "uint16"
                         },
@@ -25695,14 +32924,50 @@
                             "type": "uint16"
                         }
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 },
                 {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "renounceRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "revokeRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
                     "inputs": [],
                     "name": "season",
                     "outputs": [
                         {
                             "internalType": "uint8",
                             "name": "",
                             "type": "uint8"
@@ -25840,15 +33105,15 @@
                             "name": "_priceTierIndex",
                             "type": "uint8"
                         },
                         {
                             "components": [
                                 {
                                     "internalType": "uint8",
-                                    "name": "jewelCost",
+                                    "name": "powerTokenCost",
                                     "type": "uint8"
                                 },
                                 {
                                     "internalType": "uint16",
                                     "name": "goldCost",
                                     "type": "uint16"
                                 },
@@ -25875,14 +33140,46 @@
                     ],
                     "name": "setPriceTiers",
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 },
                 {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_tokenUnlockerAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "setTokenUnlocker",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes4",
+                            "name": "interfaceId",
+                            "type": "bytes4"
+                        }
+                    ],
+                    "name": "supportsInterface",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
                     "inputs": [],
                     "name": "totalEggs",
                     "outputs": [
                         {
                             "internalType": "uint256",
                             "name": "",
                             "type": "uint256"
@@ -26768,14 +34065,1918 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0x04b9dA42306B023f3572e106B11D82aAd9D32EBb",
                 "sd": "0xB3F5867E277798b50ba7A71C0b24FDcA03045eDF"
             }
         },
+        "PowerUpManager": {
+            "ABI": [
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "Canceled",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "Deactivated",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "Expired",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "HeroAssigned",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "HeroRemoved",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "isActivated",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "emergencyWithdrawHappened",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "openHeroSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancellationHeldSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heldSlotExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "govTokenHoldExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "owner",
+                                    "type": "address"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct PowerUpUserData",
+                            "name": "userData",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "IncreasedTier",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "uint8",
+                            "name": "version",
+                            "type": "uint8"
+                        }
+                    ],
+                    "name": "Initialized",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "string",
+                                    "name": "name",
+                                    "type": "string"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "powerUpType",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tiers",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heroesPerTier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "lockTimeRequiredToAcquire",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancelDelay",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256[]",
+                                    "name": "govTokenPerTier",
+                                    "type": "uint256[]"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct PowerUp",
+                            "name": "powerup",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "PowerUpAdded",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "string",
+                                    "name": "name",
+                                    "type": "string"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "powerUpType",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tiers",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heroesPerTier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "lockTimeRequiredToAcquire",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancelDelay",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256[]",
+                                    "name": "govTokenPerTier",
+                                    "type": "uint256[]"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct PowerUp",
+                            "name": "powerup",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "PowerUpRemoved",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "string",
+                                    "name": "name",
+                                    "type": "string"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "powerUpType",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tiers",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heroesPerTier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "lockTimeRequiredToAcquire",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancelDelay",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256[]",
+                                    "name": "govTokenPerTier",
+                                    "type": "uint256[]"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct PowerUp",
+                            "name": "powerup",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "PowerUpUpdated",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "previousAdminRole",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "newAdminRole",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "RoleAdminChanged",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleGranted",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": true,
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": true,
+                            "internalType": "address",
+                            "name": "sender",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "RoleRevoked",
+                    "type": "event"
+                },
+                {
+                    "anonymous": false,
+                    "inputs": [
+                        {
+                            "indexed": false,
+                            "internalType": "address",
+                            "name": "player",
+                            "type": "address"
+                        },
+                        {
+                            "indexed": false,
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "isActivated",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "emergencyWithdrawHappened",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "openHeroSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancellationHeldSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heldSlotExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "govTokenHoldExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "owner",
+                                    "type": "address"
+                                }
+                            ],
+                            "indexed": false,
+                            "internalType": "struct PowerUpUserData",
+                            "name": "userData",
+                            "type": "tuple"
+                        }
+                    ],
+                    "name": "Subscribed",
+                    "type": "event"
+                },
+                {
+                    "inputs": [],
+                    "name": "CANCELER_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "DEFAULT_ADMIN_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "MODERATOR_ROLE",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "activePowerUps",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_id",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "string",
+                            "name": "_name",
+                            "type": "string"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_type",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_tiers",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroesPerTier",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_lockTimeRequiredToAcquire",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_cancelHoldDelay",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_govTokenPerTier",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "addPowerUp",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "assignHero",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_powerUpIds",
+                            "type": "uint256[]"
+                        },
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_heroIds",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "assignHeroes",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "cancel",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "cleanUpHeroAssignments",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_user",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "deactivatePowerUps",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "emergencyCancelAll",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "getActivePowerUps",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "string",
+                                    "name": "name",
+                                    "type": "string"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "powerUpType",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tiers",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heroesPerTier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "lockTimeRequiredToAcquire",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancelDelay",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256[]",
+                                    "name": "govTokenPerTier",
+                                    "type": "uint256[]"
+                                }
+                            ],
+                            "internalType": "struct PowerUp[]",
+                            "name": "",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_account",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getAssignedHeroIds",
+                    "outputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_account",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getAssignedHeroes",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "id",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonedTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "nextSummonTime",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "summonerId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "assistantId",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "summons",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "maxSummons",
+                                            "type": "uint32"
+                                        }
+                                    ],
+                                    "internalType": "struct SummoningInfo",
+                                    "name": "summoningInfo",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "statGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "visualGenes",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "enum Rarity",
+                                            "name": "rarity",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "bool",
+                                            "name": "shiny",
+                                            "type": "bool"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "generation",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "firstName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint32",
+                                            "name": "lastName",
+                                            "type": "uint32"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "shinyStyle",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "class",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "subClass",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroInfo",
+                                    "name": "info",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "staminaFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "hpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint256",
+                                            "name": "mpFullAt",
+                                            "type": "uint256"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "level",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint64",
+                                            "name": "xp",
+                                            "type": "uint64"
+                                        },
+                                        {
+                                            "internalType": "address",
+                                            "name": "currentQuest",
+                                            "type": "address"
+                                        },
+                                        {
+                                            "internalType": "uint8",
+                                            "name": "sp",
+                                            "type": "uint8"
+                                        },
+                                        {
+                                            "internalType": "enum HeroStatus",
+                                            "name": "status",
+                                            "type": "uint8"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroState",
+                                    "name": "state",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mp",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "stamina",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStats",
+                                    "name": "stats",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "primaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "strength",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "intelligence",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "wisdom",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "luck",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "agility",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "vitality",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "endurance",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "dexterity",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "hpLg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpSm",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpRg",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mpLg",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroStatGrowth",
+                                    "name": "secondaryStatGrowth",
+                                    "type": "tuple"
+                                },
+                                {
+                                    "components": [
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "mining",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "gardening",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "foraging",
+                                            "type": "uint16"
+                                        },
+                                        {
+                                            "internalType": "uint16",
+                                            "name": "fishing",
+                                            "type": "uint16"
+                                        }
+                                    ],
+                                    "internalType": "struct HeroProfessions",
+                                    "name": "professions",
+                                    "type": "tuple"
+                                }
+                            ],
+                            "internalType": "struct Hero[]",
+                            "name": "",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getPowerUpHeroData",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "powerUpId",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heroId",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "assignedSlot",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "owner",
+                                    "type": "address"
+                                }
+                            ],
+                            "internalType": "struct PowerUpHeroData",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "name": "getRoleAdmin",
+                    "outputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "",
+                            "type": "bytes32"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "getUserPowerUpData",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "isActivated",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "emergencyWithdrawHappened",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "openHeroSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancellationHeldSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heldSlotExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "govTokenHoldExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "owner",
+                                    "type": "address"
+                                }
+                            ],
+                            "internalType": "struct PowerUpUserData",
+                            "name": "",
+                            "type": "tuple"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_address",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "getUserPowerUpDataForActivePowerUps",
+                    "outputs": [
+                        {
+                            "components": [
+                                {
+                                    "internalType": "bool",
+                                    "name": "isActivated",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "bool",
+                                    "name": "emergencyWithdrawHappened",
+                                    "type": "bool"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "tier",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "openHeroSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "cancellationHeldSlots",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "heldSlotExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "govTokenHoldExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "address",
+                                    "name": "owner",
+                                    "type": "address"
+                                }
+                            ],
+                            "internalType": "struct PowerUpUserData[]",
+                            "name": "",
+                            "type": "tuple[]"
+                        },
+                        {
+                            "components": [
+                                {
+                                    "internalType": "uint256",
+                                    "name": "powerUpId",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "govTokens",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "end",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "govTokenHoldExpiration",
+                                    "type": "uint256"
+                                },
+                                {
+                                    "internalType": "uint256",
+                                    "name": "usedBalance",
+                                    "type": "uint256"
+                                }
+                            ],
+                            "internalType": "struct PowerUpLock[]",
+                            "name": "",
+                            "type": "tuple[]"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "grantRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "hasRole",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_tier",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "increaseTier",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_voteEscrowRewardPoolAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_heroCoreAddress",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "_questCoreAddress",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "initialize",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_user",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "isHeroPowerUpActive",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_user",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "isUserPowerUpActive",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "powerUpHeroData",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "heroId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "assignedSlot",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "owner",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "powerUpHeroesAssigned",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "powerUps",
+                    "outputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "id",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "string",
+                            "name": "name",
+                            "type": "string"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "powerUpType",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "tiers",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "heroesPerTier",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "lockTimeRequiredToAcquire",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "cancelDelay",
+                            "type": "uint256"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "removeHero",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_user",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "removeHeroFromAllType3",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_heroId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "removeHeroFromAllType3ForSender",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_powerUpIds",
+                            "type": "uint256[]"
+                        },
+                        {
+                            "internalType": "uint256[]",
+                            "name": "_heroIds",
+                            "type": "uint256[]"
+                        }
+                    ],
+                    "name": "removeHeroes",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "renounceRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes32",
+                            "name": "role",
+                            "type": "bytes32"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "account",
+                            "type": "address"
+                        }
+                    ],
+                    "name": "revokeRole",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_tier",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "subscribe",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "bytes4",
+                            "name": "interfaceId",
+                            "type": "bytes4"
+                        }
+                    ],
+                    "name": "supportsInterface",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "",
+                            "type": "bool"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "userPowerUpData",
+                    "outputs": [
+                        {
+                            "internalType": "bool",
+                            "name": "isActivated",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "emergencyWithdrawHappened",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "tier",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "openHeroSlots",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "cancellationHeldSlots",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "heldSlotExpiration",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "govTokenHoldExpiration",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "owner",
+                            "type": "address"
+                        }
+                    ],
+                    "stateMutability": "view",
+                    "type": "function"
+                },
+                {
+                    "inputs": [],
+                    "name": "verifyAllPowerUps",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "verifyPowerUp",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                },
+                {
+                    "inputs": [
+                        {
+                            "internalType": "address",
+                            "name": "_user",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "uint256",
+                            "name": "_powerUpId",
+                            "type": "uint256"
+                        }
+                    ],
+                    "name": "verifyPowerUpForUser",
+                    "outputs": [],
+                    "stateMutability": "nonpayable",
+                    "type": "function"
+                }
+            ],
+            "ADDRESS": {
+                "cv": "0xc20a268bc7c4dB28f1f6e1703676513Db06C1B93",
+                "sd": "0xcd26DfD7EdAe42eD525266D9a53b466db4Ed4f7b"
+            }
+        },
         "Profiles": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
                             "indexed": false,
@@ -29670,15 +38871,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x6a56222A67df18FC282CD58dCDF12e61Be812f97",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "RaffleTicket": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -30108,15 +39309,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0xBbd7c4Be2e54fF5e013471162e1ABAD7AB74c3C3",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "StoneCarver": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -30503,15 +39704,15 @@
                     ],
                     "stateMutability": "view",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0xc32A0e963e50AAAED273A75425fC39902b0d0b3b",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "Stylist": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
@@ -31134,15 +40335,15 @@
                     "outputs": [],
                     "stateMutability": "nonpayable",
                     "type": "function"
                 }
             ],
             "ADDRESS": {
                 "cv": "0x123165B3a30fdA3655B30cfC10135C1CA3C21bFC",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         },
         "UniswapV2Factory": {
             "ABI": [
                 {
                     "inputs": [
                         {
@@ -31332,15 +40533,15 @@
                 }
             ],
             "ADDRESS": {
                 "cv": "0x794C07912474351b3134E6D6B3B7b3b4A07cbAAa",
                 "sd": "0x36fAE766e51f17F8218C735f58426E293498Db2B"
             }
         },
-        "UniswapV2Router02": {
+        "UniswapV2Router": {
             "ABI": [
                 {
                     "inputs": [
                         {
                             "internalType": "address",
                             "name": "_factory",
                             "type": "address"
@@ -33115,15 +42316,15 @@
                 {
                     "stateMutability": "payable",
                     "type": "receive"
                 }
             ],
             "ADDRESS": {
                 "cv": "0xED6dC9FD092190C08e4afF8611496774Ded19D54",
-                "sd": ""
+                "sd": "0x0000000000000000000000000000000000000000"
             }
         }
     },
     "DEFAULT_RPC": {
         "cv": "https://subnets.avax.network/defi-kingdoms/dfk-chain/rpc",
         "sd": "https://klaytn.rpc.defikingdoms.com/"
     },
```

### Comparing `abi_maker-0.1.0/abi_maker/demo_abis/EVO_ABIS.json` & `abi_maker-0.1.2/abi_maker/demo_abis/EVO_ABIS.json`

 * *Files identical despite different names*

### Comparing `abi_maker-0.1.0/abi_maker/demo_abis/TREASURE_ABIS.json` & `abi_maker-0.1.2/abi_maker/demo_abis/TREASURE_ABIS.json`

 * *Files identical despite different names*

### Comparing `abi_maker-0.1.0/abi_maker/make_wrapper.py` & `abi_maker-0.1.2/abi_maker/make_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,31 +16,53 @@
 
 PACKAGE_DIR = Path(__file__).parent
 TEMPLATES_DIR = PACKAGE_DIR / 'template_modules'
 
 SNAKE_CASE_RE_1 = re.compile(r'(.)([A-Z][a-z]+)')
 SNAKE_CASE_RE_2 = re.compile(r'([a-z0-9])([A-Z])')
 
+# These functions, from OpenZeppelin's Access Control libraries or related to 
+# Diamond storage, are not needed in the wrapper module. Unless there's a good 
+# reason, we should exclude them from wrappers
+INFRASTRUCTURE_FUNCTIONS = [
+    'Initialized', 'Paused', 'Unpaused', 
+    'initialize', 'paused', 'togglePause', 'unpause', 'pause', 
+    'DiamondCut', 
+    'diamondCut', 'facetAddress', 'facetAddresses', 'facetFunctionSelectors', 'facets',
+    'RoleAdminChanged', 'RoleGranted', 'RoleRevoked', 
+    'previousAdminRole', 'newAdminRole', 'getRoleAdmin', 'grantRole', 'hasRole', 
+    'renounceRole', 'revokeRole', 'supportsInterface',
+]
+
 # FIXME: Function polymorphism is legal in Solidity but not in Python. 
 # Having two functions, with the same name but different arguments A(arg1) & A(arg2, arg3) 
 # is fine in Solidity but in Python will silently fail and only the last function
 # will be valid.
 # Proposal: number any duplicate-named functions (e.g. A(arg1), A1(arg2, arg3))
 
+# See also: https://web3py.readthedocs.io/en/v5/contracts.html#invoke-ambiguous-contract-functions-example
+# There's capacity to disambiguate functions based on their argument signatures,
+# but I'm not sure how to incorporate that into this project
+# - Athiriyya 12 January 2023
+
+# (What I've done so far is just to manually remove the ABI JSON for duplicate-named functions)
+
+
 # ===============
 # = ENTRY POINT =
 # ===============
 def write_project_wrapper(project_name:str, abi_json_path:Path, output_dir:Path, overwrite_ok=False) -> List[Path]:
     if not abi_json_path.exists():
         raise ValueError(f"No ABI file present for project {project_name} at expected path {abi_json_path}")
     abis_by_name = json.loads(abi_json_path.read_text())
 
     # Make project dir, erasing any previous dir
     # Warn before overwriting a dir. If overwrite_ok is True, proceed.
-    project_dir = output_dir / project_name
+    # project_dir = output_dir / project_name
+    project_dir = output_dir 
     if project_dir.exists():
         overwrite_ok = overwrite_ok or yes_no_prompt(f'Overwrite project dir? ({project_dir})')
         if overwrite_ok:
             shutil.rmtree(project_dir)
         else:
             print(f'Refusing to overwrite project dir at {project_dir}. '
                   f'\nMove the directory or pass the -f command line option to continue')
@@ -70,41 +92,41 @@
     written_paths:List[Path] = []
 
     contracts_dir =  project_dir / 'contracts'
     
     contracts_dir.mkdir(exist_ok=True, parents=True)
 
     # TODO: we might make some provisions for a customizable superclass    
-    # superclass_name = f'{project_name.capitalize()}Contract'
-    superclass_name = 'ABIWrapperContract'
+
     for contract_name, contract_info in project_dict['CONTRACTS'].items():
         # Note that this address may be a single hex address or a dict of addresses
         # for multi-chain contracts
         address = contract_info.get('ADDRESS')
         abi = contract_info['ABI']
-        path = write_contract_wrapper_module(contract_name, abi, address, superclass_name, contracts_dir)
+        path = write_contract_wrapper_module(contract_name, abi, address, contracts_dir)
         written_paths.append(path)
     
     return written_paths
 
 def write_contract_wrapper_module(contract_name:str, 
                                   contract_dicts:Sequence[Dict], 
                                   contract_address:Union[HexAddress, Dict[str, HexAddress]], 
-                                  superclass_name:str, 
                                   super_dir:Path) -> Path:
 
     abi_str = ',\n    '.join((json.dumps(d) for d in contract_dicts))
     abi_str = indent(abi_str, INDENT)
 
-    superclass_module = to_snake_case(superclass_name)
+    multichain = isinstance(contract_address, dict)
+    custom_contract = (contract_address is None or multichain and None in contract_address.values())
+
+    superclass_name = 'ABIMultiContractWrapper' if custom_contract else 'ABIContractWrapper' 
     module_str = python_class_str_for_contract_dicts(contract_name, 
                                                 contract_dicts, 
                                                 contract_address, 
                                                 abi_str,
-                                                superclass_module,
                                                 superclass_name)
 
 
     contract_path = (super_dir / to_snake_case(contract_name)).with_suffix('.py')
     contract_path.write_text(module_str)
     return contract_path
 
@@ -113,28 +135,35 @@
                                 contract_paths:Sequence[Path],
                                 project_dir:Path) -> Path:
     init_strs = []
     import_strs = []
 
     contract_dicts = project_dict['CONTRACTS']
     # Figure out if this is a multichain contract
-    single_dict = next(iter(contract_dicts.values()))
+    single_dict:Dict = next(iter(contract_dicts.values()))
     is_multichain = isinstance(single_dict.get('ADDRESS'), dict)
     chain_arg = ''
     chain_type_arg = ''
     chain_self = ''
     if is_multichain:
         chain_arg = 'self.chain_key, '
         chain_type_arg = 'chain_key:str, '
         chain_self = '\n        self.chain_key = chain_key'
 
     default_rpc = project_dict.get('DEFAULT_RPC', None)
 
     for class_name, module_path in zip(contract_dicts.keys(), contract_paths):
         module_name = module_path.stem
+        address_desc = contract_dicts[class_name]['ADDRESS']
+        custom_contracts = ((is_multichain and not any(dict(address_desc).values()))
+                            or (not is_multichain and not address_desc))
+        # subclasses of AbiMultiContractWrapper (== ERC20, for now)
+        # don't have a chain key or contract as part of their args
+        chain_arg = '' if custom_contracts else 'self.chain_key, '
+
         import_strs.append(f'from .contracts.{module_name} import {class_name}')
         init_strs.append(indent(f'self.{module_name} = {class_name}({chain_arg}self.rpc)', INDENT*2))
 
     imports = '\n'.join(import_strs)
     inits = '\n'.join(init_strs)
     default_rpc_declaration = ''
     default_rpc_setting = ''
@@ -152,76 +181,83 @@
 #! /usr/bin/env python
 
 {imports}
 {default_rpc_declaration}
 
 class All{project_name.capitalize()}Contracts:
     # TODO: we might want to be able to specify other traits, like gas fees or timeout
-    def __init__(self, {chain_type_arg}rpc:str=None):
+    def __init__(self, {chain_type_arg}rpc:str | None = None):
         self.rpc = rpc{default_rpc_setting}{chain_self}
 
 {inits}
 
 '''
 )
 
     all_contract_path = project_dir / f'all_{project_name.lower()}_contracts.py'
     all_contract_path.write_text(class_str)
     return all_contract_path
 
 def python_class_str_for_contract_dicts(contract_name:str, 
                                         contract_dicts:Sequence[Dict], 
-                                        contract_address:Optional[HexAddress],
+                                        contract_address:Union[None, HexAddress, Dict[str, HexAddress]],
                                         abi_str:str, 
-                                        superclass_module: str='abi_wrapper_contract',
-                                        superclass_name:str = 'ABIWrapperContract' ) -> str:
+                                        superclass_name:str = 'ABIContractWrapper' ) -> str:
     # There are two binary options for how we write contracts:
     # - contract may or may not be multichain, in which case CONTRACT_ADDRESS 
     #   is written as a dictionary rather than a single string, or
     # - contract may or may not be for an ERC20-style token, where a custom address
     #   is passed to every function call
     # 
     # We handle both circumstances below, but it's a little involved.    
-
+    superclass_module = to_snake_case(superclass_name)
 
     # If contract_address is None/null, this is a token contract like ERC20
     # where the address of the token will be supplied as well as normal args, 
     # so a custom contract will be made for each call. 
     multichain = isinstance(contract_address, dict)
     custom_contract = (contract_address is None or multichain and None in contract_address.values())
 
     chain_type_arg = ''
     contract_setter = ''
     if multichain:
         address_str = indent(json.dumps(contract_address, indent=4), '    ' )
         address_str = address_str.replace('null', 'None')
-        chain_type_arg = 'chain_key:str, '
-        contract_setter = '.get(chain_key)'
+        if not custom_contract:
+            chain_type_arg = 'chain_key:str, '
+            contract_setter = 'contract_address = CONTRACT_ADDRESS[chain_key]'
     else:
         address_str = 'None' if custom_contract else f'"{contract_address}"'
 
+    custom_contract_init = dedent(f'''    def __init__(self, rpc:str):
+                super().__init__(abi=ABI, rpc=rpc)
+    ''')
+
+    fixed_contract_init = dedent(f'''    def __init__(self, {chain_type_arg}rpc:str):
+                {contract_setter}
+                super().__init__(contract_address=contract_address, abi=ABI, rpc=rpc)
+    ''')
+
+    init_str = custom_contract_init if custom_contract else fixed_contract_init
+
     class_str = dedent(
     f'''
     from ..{superclass_module} import {superclass_name}
     from ..solidity_types import *
     from ..credentials import Credentials
 
     CONTRACT_ADDRESS = {address_str}
 
     ABI = """[
     {abi_str}
     ]
     """     
 
     class {inflection.camelize(contract_name)}({superclass_name}):
-
-        def __init__(self, {chain_type_arg}rpc:str=None):
-            contract_address = CONTRACT_ADDRESS{contract_setter}
-            super().__init__(contract_address=contract_address, abi=ABI, rpc=rpc)
-    ''')
+        {init_str}''')
     func_strs = [function_body(d, custom_contract) for d in contract_dicts]
     # remove empty strs
     func_strs = [f for f in func_strs if f]
 
     class_str += f'\n'.join(func_strs)
     return class_str
 
@@ -265,15 +301,15 @@
                 contract = self.get_custom_contract(contract_address, abi=self.abi)
                 tx = contract.functions.{contract_func_name}({solidity_args_str})
                 return self.send_transaction(tx, cred)''')
     else:
         if is_view:
             body = dedent(f'''
             {def_func}
-                return self.contract.functions.{contract_func_name}({solidity_args_str}).call()''')
+                return self.contract.functions.{contract_func_name}({solidity_args_str}).call(block_identifier=block_identifier)''')
         else:
             body = dedent(f'''
             {def_func}
                 tx = self.contract.functions.{contract_func_name}({solidity_args_str})
                 return self.send_transaction(tx, cred)''')
     return indent(body, INDENT)
 
@@ -318,62 +354,67 @@
 
     substitute_arg_name = 'a'
     for arg_dict in function_dict['inputs']:
         arg_name = solidity_arg_name_to_pep_8(arg_dict['name'])
         if not arg_name:
             arg_name = substitute_arg_name
             substitute_arg_name = chr(ord(substitute_arg_name) + 1)
-        arg_type = abi_type_to_hint(arg_dict)
+        arg_type = abi_type_to_hint(arg_dict, is_output=False)
         inputs.append(f'{arg_name}:{arg_type}')
 
+    if not is_transaction:
+        inputs.append(f"block_identifier:BlockIdentifier = 'latest'")
+
     inputs_str = ', '.join(inputs)
 
     sig = f'def {func_name}({inputs_str}){return_type}:'
     return sig
 
 def get_output_types(outputs_list:Sequence[Dict]) -> str:
     if len(outputs_list) == 0:
         return 'None'
     else:
         if len(outputs_list) == 1:
-            return abi_type_to_hint(outputs_list[0])
+            return abi_type_to_hint(outputs_list[0], is_output=True)
         else:
-            out_types_str = ', '.join([abi_type_to_hint(o) for o in outputs_list])
+            out_types_str = ', '.join([abi_type_to_hint(o, is_output=True) for o in outputs_list])
             return f'Tuple[{out_types_str}]'
 
-def abi_type_to_hint(arg_dict:Dict) -> str:
+def abi_type_to_hint(arg_dict:Dict, is_output=False) -> str:
     type_in = arg_dict['type']
     
     # Figure out if this is a (possibly nested) list type
     bracket_pair_re = re.compile(r'\[\d*\]')
     list_depth = len(bracket_pair_re.findall(type_in))
     if list_depth > 0:
         match = bracket_pair_re.search(type_in)
         if match:
             type_in = type_in[:match.start()]
 
     # Nest lists as needed
     type_out = type_in
     for i in range(list_depth):
-        type_out = f'Sequence[{type_out}]'
+        if is_output:
+            type_out = f'List[{type_out}]'
+        else:
+            type_out = f'Sequence[{type_out}]'
 
     return type_out
 
-def to_snake_case(name:str=None) -> str:
+def to_snake_case(name:str | None = None) -> str:
     # See: https://stackoverflow.com/a/1176023/3592884
     # name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     # return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
     if not name:
         return ''
     name = SNAKE_CASE_RE_1.sub(r'\1_\2', name)
     return SNAKE_CASE_RE_2.sub(r'\1_\2', name).lower()
 
-def is_role_func(d:Dict) -> bool:
-    res = ('role' in d.get('name', '').lower() or d.get('name') == 'supportsInterface')    
-    return res
+def is_infra_func(d:Dict) -> bool:
+    return d.get('name') in INFRASTRUCTURE_FUNCTIONS
 
 # ===========================
 # = # DICT & ABI FORMATTING =
 # ===========================
 def write_abis_to_readable_file(abis:Dict[str, List[Dict]], abi_path:Path, exclude_role_funcs=True) -> Dict[str, List[Dict]]:
     # Write ABI JSON out in a way designed to be human-readable, 
     # neither all in one condensed line,
@@ -389,21 +430,20 @@
     #     "abi_contract_2": [
     #         {"etc": "etc"}
     #     ]
     # }
     
     # Also, order the entries in each ABI dict with name and type first
     ordered_abis = {k:make_ordered_dict(v, exclude_role_funcs) for k,v in abis.items()}
-
-    out_str = '{\n' + ',\n\n'.join([f'"{k}":{one_dict_per_line(d)}' for k,d in ordered_abis.items()]) + '\n}'
+    out_str = '{\n' + ',\n\n'.join([f'"{k}":{one_dict_per_line(d)}' for k,d in ordered_abis.items()]) + '\n}' #type: ignore
     # TODO: I think this is a better way to nest dicts, but would need to test a little
     # out_str = json_nest_dict_to_depth(ordered_abis, flatten_after_level=3)
     abi_path.write_text(out_str)  
     print(f'Wrote ABI data to {abi_path}')
-    return ordered_abis
+    return ordered_abis # type:ignore
 
 def one_dict_per_line(dict_list:Sequence[Dict]) -> str:
     '''
     Render a list of dicts like so:
     [
         {'dict_a': 1},
         {'dict_b': 2}
@@ -418,54 +458,54 @@
         return json.dumps(elt)
 
     if isinstance(elt, dict):
         kv_strings = [f'"{k}": {json_nest_dict_to_depth(v, flatten_after_level, depth+1)}' for k, v in elt.items()]
         kvs = indent(',\n'.join(kv_strings), INDENT)
         return f'{{\n{kvs}\n}}'
     elif isinstance(elt, (list, tuple)):
-        elts = [json_nest_dict_to_depth(e, flatten_after_level, depth+1) for e in elt]
+        elts = [str(json_nest_dict_to_depth(e, flatten_after_level, depth+1)) for e in elt]
         es = indent(',\n'.join(elts), INDENT)
         return f'[\n{es}\n]'
     else:
         return json.dumps(elt)
 
-def make_ordered_dict(d: Union[List, Dict], exclude_role_funcs=True) -> Union[List, Dict]:
+def make_ordered_dict(d: Union[List, Dict], exclude_infra_funcs=True) -> Union[List, Dict]:
     # Given a dict or list of dicts, output a data structure with the same
     # contents, but with keys alphabetized and with the "name" field of any sub-dict
     # made first, so that ABI dicts are more easily readable.
 
     # exclude_role_funcs:  if True, don't include ABI functions that include the word 'role'
     # Lots of contracts use OpenZeppelin's role-access code, which includes about
     # 10 functions relating to roles which aren't usually usable by code clients,
     # so they clutter up ABIs. If requested, don't include these in the dicts we
     # output
 
     if not isinstance(d, (list, dict)):
         return d
 
     if isinstance(d, list):
-        if exclude_role_funcs:
-            new_list = list([make_ordered_dict(d2, exclude_role_funcs) for d2 in d if not is_role_func(d2)])
+        if exclude_infra_funcs:
+            new_list = list([make_ordered_dict(d2, exclude_infra_funcs) for d2 in d if not is_infra_func(d2)])
         else:
-            new_list = list([make_ordered_dict(d2, exclude_role_funcs) for d2 in d])
+            new_list = list([make_ordered_dict(d2, exclude_infra_funcs) for d2 in d])
         # Sort list entries alphabetically. In practice, this ends up sorting by
         # method names, which has the side effect of separating Solidity events 
         # (which start with a capital letter) from Solidity functions
         return sorted(new_list, key=lambda d:str(d))
         
     elif isinstance(d, dict):
         # Output a new dictionary with `priority_keys` first if present, 
         # then all other keys sorted alphabetically
         priority_keys = ['name', 'type', 'inputs', 'outputs']
         keys = set(d.keys())
         to_sort = keys - set(priority_keys)
         priorities_present = [k for k in priority_keys if k in keys]
         sorted_keys = priorities_present + sorted(to_sort)
 
-        new_dict = {k:make_ordered_dict(d[k], exclude_role_funcs) for k in sorted_keys}
+        new_dict = {k:make_ordered_dict(d[k], exclude_infra_funcs) for k in sorted_keys}
 
     return new_dict
 
 # ===========
 # = HELPERS =
 # ===========
 def yes_no_prompt(prompt: str, default: bool = False) -> bool:
```

### Comparing `abi_maker-0.1.0/abi_maker/template_modules/abi_wrapper_contract.py` & `abi_maker-0.1.2/abi_maker/template_modules/abi_contract_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,150 +1,153 @@
 #! /usr/bin/env python
-
-import traceback
-
-import web3
 from web3 import Web3
-from web3.datastructures import AttributeDict
-from web3.middleware import geth_poa_middleware
+from web3.middleware.geth_poa import geth_poa_middleware
+from web3.logs import DISCARD
 
 from .credentials import Credentials
 
-from .solidity_types import *
-from web3.contract import Contract
-from typing import Dict, Tuple, Union, Optional, Any
+from .solidity_types import (address, ChecksumAddress, TxReceipt, AttributeDict)
+from web3.contract.contract import Contract
+from typing import Dict, Tuple, Union, Optional, Any, Sequence
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_MAX_GAS = 50
 DEFAULT_MAX_PRIORITY_GAS = 3
 
 W3_INSTANCES: Dict[str, Web3] = {}
 
-class ABIWrapperContract:
+class ABIContractWrapper:
     def __init__(self, 
-                 contract_address:Optional[address], 
+                 contract_address:str, 
                  abi:str,
                  rpc:str,
                  max_gas_gwei:float=DEFAULT_MAX_GAS,
                  max_priority_gwei:float=DEFAULT_MAX_PRIORITY_GAS):
         self.rpc = rpc
-        self.contract_address = contract_address
+        # self.contract_address = contract_address
         self.abi = abi
-        self.contract = None
         self.nonces: Dict[address, int] = {}
         self.timeout = DEFAULT_TIMEOUT
 
         # This one superclass may be used by many contracts, who don't all need to
         # create separate Web3 instances. Just use one per RPC
         global W3_INSTANCES
         w3 = W3_INSTANCES.get(self.rpc, None)
         if not w3:
             w3 = Web3(Web3.HTTPProvider(self.rpc))
             w3.middleware_onion.inject(geth_poa_middleware, layer=0)
             W3_INSTANCES[self.rpc] = w3
         self.w3 = w3
+        self.contract_address:ChecksumAddress = self.w3.to_checksum_address(contract_address)
 
-        self.max_gas_wei = self.w3.toWei(max_gas_gwei, 'gwei')
-        self.max_priority_wei = self.w3.toWei(max_priority_gwei, 'gwei')
+        self.max_gas_wei = self.w3.to_wei(max_gas_gwei, 'gwei')
+        self.max_priority_wei = self.w3.to_wei(max_priority_gwei, 'gwei')
 
-        if self.contract_address:
-            self.contract = self.w3.eth.contract(self.contract_address, abi=self.abi)
+        self.contract = self.w3.eth.contract(self.contract_address, abi=self.abi)
 
     def get_nonce_and_update(self, address:address, force_fetch=True) -> int:
         # FIXME: I think there's a bug in the caching logic below that lets
         # nonces run ahead of where they should be and causes transactions to
         # fail.
         # So force_fetch is set to true, which fetches the appropriate nonce for
         # every transaction
         # - Athiriyya 13 December 2022
 
         # We keep track of our own nonce, and only re-fetch it if a 'nonce too low'
         # error gets thrown       
         nonce = self.nonces.get(address, 0) 
         if force_fetch or nonce == 0:
-            nonce = self.w3.eth.getTransactionCount( address, 'pending')
+            nonce = self.w3.eth.get_transaction_count( address, 'pending')
 
         # Store the next nonce this address will use, and return the current one
         self.nonces[address] = nonce + 1
         return nonce
 
-    def get_gas_dict_and_update(self, address:address) -> Dict[str, float]:
+    def get_gas_dict_and_update(self, address:address) -> Dict[str, int]:
         nonce = self.get_nonce_and_update(address)
          
         legacy = False
         if legacy:
             # TODO: it's expensive to query for fees with every transaction. 
             # Maybe query only once a minute?
             gas, gas_price = self.get_legacy_gas_fee()
-            gas_dict = {'gas': gas, 'gasPrice':gas_price, 'nonce':nonce}
+            gas_dict = {
+                'gas': gas, 
+                'gasPrice':gas_price, 
+                'nonce':nonce
+            }
         else:
             gas_dict = {
                 'from': address, 
-                'maxFeePerGas': self.max_gas_wei, 
-                'maxPriorityFeePerGas': self.max_priority_wei, 
+                'maxFeePerGas': int(self.max_gas_wei), 
+                'maxPriorityFeePerGas': int(self.max_priority_wei), 
                 'nonce': nonce
             }
         return gas_dict
 
     def call_contract_function(self, function_name:str, *args) -> Any:
         contract_func = getattr(self.contract, function_name)
         return contract_func(*args).call()
 
-    def get_custom_contract(self, contract_address:address, abi:str=None) -> Contract:
+    def get_custom_contract(self, contract_address:ChecksumAddress, abi:str | None=None) -> Contract:
         # TODO: Many custom contracts for e.g. ERC20 tokens could
         # be re-used by caching a contracts dictionary keyed by address
         # For now, just return a new contract
         abi = abi or self.abi
-        contract = self.w3.eth.contract(contract_address, abi=abi)
+        checked_addr = self.w3.to_checksum_address(contract_address)
+        contract = self.w3.eth.contract(checked_addr, abi=abi)
         return contract
 
     def send_transaction(self,
                          tx,
                          cred:Credentials,
-                         nonce=None
-                        ) -> Optional[TxReceipt]:
-
+                         extra_dict:Dict[str,Any] | None = None
+                        ) -> TxReceipt:
+        # Some transactions require extra information or fees when building 
+        # the transaction. e.g. bridging functions need a {'value': <bridge_fee_in_wei>}
+        # argument. If supplied, add that extra info
         address = cred.address  
         gas_dict = self.get_gas_dict_and_update(address)
-        tx_dict = tx.buildTransaction(gas_dict)    
+        if extra_dict:
+            gas_dict.update(extra_dict)
+        tx_dict = tx.build_transaction(gas_dict)    
         signed_tx = self.w3.eth.account.sign_transaction(tx_dict, private_key=cred.private_key)
         try:
             self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
 
         except Exception as e:
             if 'nonce too low' in str(e):
                 nonce = self.get_nonce_and_update(address, force_fetch=True)
                 return self.send_transaction( tx, cred)
-
-            traceback.print_exc()
-            return None
+            # otherwise, raise
+            raise(e)
 
         receipt = self.w3.eth.wait_for_transaction_receipt(
             transaction_hash=signed_tx.hash,
             poll_latency=1,
             timeout=self.timeout,
         )
         return receipt
 
     def get_legacy_gas_fee(self) ->Tuple[int, int]:
         # See: https://web3py.readthedocs.io/en/stable/gas_price.html#gas-price-api
         # Some transactions may require a gas dict with the keys {'gasPrice': x_wei, '': y_wei}
-        block = self.w3.eth.getBlock("pending")
-        base_gas = block.gasUsed + self.w3.toWei(50, 'gwei')
-        gas_limit =block.gasLimit
+        block = self.w3.eth.get_block("pending")
+        base_gas = block.get('gasUsed', 2_500_000) + self.w3.to_wei(50, 'gwei')
+        gas_limit =block.get('gasLimit', 2_500_000)
 
         return base_gas, gas_limit
 
     def tx_receipt_for_hash(self, tx_hash:address) -> TxReceipt:
         tx_receipt = self.w3.eth.get_transaction_receipt(tx_hash)
         return tx_receipt
 
-    def parse_events(self, tx_receipt:TxReceipt, event_names:Sequence[str]=None) -> Dict[str, AttributeDict]:
+    def parse_events(self, tx_receipt:TxReceipt, event_names:Sequence[str] | None = None) -> Dict[str, AttributeDict]:
         event_dicts = {}
-        for event in self.contract.events:
-            eds = event().processReceipt(tx_receipt, errors=web3.logs.DISCARD)
+        for event in self.contract.events: # type: ignore
+            eds = event().process_receipt(tx_receipt, errors=DISCARD)
             if eds:
                 for ed in eds:
                     event_dicts.setdefault(ed.event,[]).append(ed)
         if event_names:
             event_dicts = {k:v for k,v in event_dicts.items() if k in event_names}
         return event_dicts
```

