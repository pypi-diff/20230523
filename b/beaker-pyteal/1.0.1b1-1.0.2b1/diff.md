# Comparing `tmp/beaker_pyteal-1.0.1b1-py3-none-any.whl.zip` & `tmp/beaker_pyteal-1.0.2b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,41 @@
-Zip file size: 45657 bytes, number of entries: 36
--rw-r--r--  2.0 unx     1027 b- defN 80-Jan-01 00:00 beaker/__init__.py
--rw-r--r--  2.0 unx    44553 b- defN 80-Jan-01 00:00 beaker/application.py
--rw-r--r--  2.0 unx     1204 b- defN 80-Jan-01 00:00 beaker/build_options.py
+Zip file size: 47325 bytes, number of entries: 39
+-rw-r--r--  2.0 unx     1029 b- defN 80-Jan-01 00:00 beaker/__init__.py
+-rw-r--r--  2.0 unx    45518 b- defN 80-Jan-01 00:00 beaker/application.py
+-rw-r--r--  2.0 unx     2053 b- defN 80-Jan-01 00:00 beaker/build_options.py
 -rw-r--r--  2.0 unx      340 b- defN 80-Jan-01 00:00 beaker/client/__init__.py
--rw-r--r--  2.0 unx     3933 b- defN 80-Jan-01 00:00 beaker/client/api_providers.py
--rw-r--r--  2.0 unx    15852 b- defN 80-Jan-01 00:00 beaker/client/application_client.py
+-rw-r--r--  2.0 unx     4397 b- defN 80-Jan-01 00:00 beaker/client/api_providers.py
+-rw-r--r--  2.0 unx    16223 b- defN 80-Jan-01 00:00 beaker/client/application_client.py
 -rw-r--r--  2.0 unx     1239 b- defN 80-Jan-01 00:00 beaker/compilation.py
 -rw-r--r--  2.0 unx     1923 b- defN 80-Jan-01 00:00 beaker/consts.py
 -rw-r--r--  2.0 unx     2521 b- defN 80-Jan-01 00:00 beaker/decorators.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 beaker/lib/__init__.py
 -rw-r--r--  2.0 unx     1849 b- defN 80-Jan-01 00:00 beaker/lib/inline.py
 -rw-r--r--  2.0 unx      707 b- defN 80-Jan-01 00:00 beaker/lib/iter.py
 -rw-r--r--  2.0 unx     6449 b- defN 80-Jan-01 00:00 beaker/lib/math.py
 -rw-r--r--  2.0 unx      219 b- defN 80-Jan-01 00:00 beaker/lib/storage/__init__.py
 -rw-r--r--  2.0 unx     1968 b- defN 80-Jan-01 00:00 beaker/lib/storage/blob.py
 -rw-r--r--  2.0 unx     3308 b- defN 80-Jan-01 00:00 beaker/lib/storage/box_list.py
 -rw-r--r--  2.0 unx     3808 b- defN 80-Jan-01 00:00 beaker/lib/storage/box_mapping.py
 -rw-r--r--  2.0 unx     6841 b- defN 80-Jan-01 00:00 beaker/lib/storage/global_blob.py
 -rw-r--r--  2.0 unx     7631 b- defN 80-Jan-01 00:00 beaker/lib/storage/local_blob.py
 -rw-r--r--  2.0 unx     4226 b- defN 80-Jan-01 00:00 beaker/lib/strings.py
+-rw-r--r--  2.0 unx      239 b- defN 80-Jan-01 00:00 beaker/localnet/__init__.py
+-rw-r--r--  2.0 unx      736 b- defN 80-Jan-01 00:00 beaker/localnet/clients.py
+-rw-r--r--  2.0 unx     3578 b- defN 80-Jan-01 00:00 beaker/localnet/kmd.py
 -rw-r--r--  2.0 unx     5352 b- defN 80-Jan-01 00:00 beaker/logic_signature.py
 -rw-r--r--  2.0 unx    10620 b- defN 80-Jan-01 00:00 beaker/precompile.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 beaker/py.typed
--rw-r--r--  2.0 unx      243 b- defN 80-Jan-01 00:00 beaker/sandbox/__init__.py
--rw-r--r--  2.0 unx      734 b- defN 80-Jan-01 00:00 beaker/sandbox/clients.py
--rw-r--r--  2.0 unx     3578 b- defN 80-Jan-01 00:00 beaker/sandbox/kmd.py
+-rw-r--r--  2.0 unx      343 b- defN 80-Jan-01 00:00 beaker/sandbox/__init__.py
+-rw-r--r--  2.0 unx      370 b- defN 80-Jan-01 00:00 beaker/sandbox/clients.py
+-rw-r--r--  2.0 unx      693 b- defN 80-Jan-01 00:00 beaker/sandbox/kmd.py
 -rw-r--r--  2.0 unx      837 b- defN 80-Jan-01 00:00 beaker/state/__init__.py
 -rw-r--r--  2.0 unx      751 b- defN 80-Jan-01 00:00 beaker/state/_abc.py
 -rw-r--r--  2.0 unx     3489 b- defN 80-Jan-01 00:00 beaker/state/_aggregate.py
 -rw-r--r--  2.0 unx     3904 b- defN 80-Jan-01 00:00 beaker/state/blob.py
 -rw-r--r--  2.0 unx    10370 b- defN 80-Jan-01 00:00 beaker/state/primitive.py
 -rw-r--r--  2.0 unx     6335 b- defN 80-Jan-01 00:00 beaker/state/reserved.py
--rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 beaker_pyteal-1.0.1b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2875 b- defN 80-Jan-01 00:00 beaker_pyteal-1.0.1b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 beaker_pyteal-1.0.1b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2904 b- defN 16-Jan-01 00:00 beaker_pyteal-1.0.1b1.dist-info/RECORD
-36 files, 162743 bytes uncompressed, 41065 bytes compressed:  74.8%
+-rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 beaker_pyteal-1.0.2b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2871 b- defN 80-Jan-01 00:00 beaker_pyteal-1.0.2b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 beaker_pyteal-1.0.2b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     3147 b- defN 16-Jan-01 00:00 beaker_pyteal-1.0.2b1.dist-info/RECORD
+39 files, 167037 bytes uncompressed, 42355 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -54,14 +54,23 @@
 
 Filename: beaker/lib/storage/local_blob.py
 Comment: 
 
 Filename: beaker/lib/strings.py
 Comment: 
 
+Filename: beaker/localnet/__init__.py
+Comment: 
+
+Filename: beaker/localnet/clients.py
+Comment: 
+
+Filename: beaker/localnet/kmd.py
+Comment: 
+
 Filename: beaker/logic_signature.py
 Comment: 
 
 Filename: beaker/precompile.py
 Comment: 
 
 Filename: beaker/py.typed
@@ -90,20 +99,20 @@
 
 Filename: beaker/state/primitive.py
 Comment: 
 
 Filename: beaker/state/reserved.py
 Comment: 
 
-Filename: beaker_pyteal-1.0.1b1.dist-info/LICENSE
+Filename: beaker_pyteal-1.0.2b1.dist-info/LICENSE
 Comment: 
 
-Filename: beaker_pyteal-1.0.1b1.dist-info/METADATA
+Filename: beaker_pyteal-1.0.2b1.dist-info/METADATA
 Comment: 
 
-Filename: beaker_pyteal-1.0.1b1.dist-info/WHEEL
+Filename: beaker_pyteal-1.0.2b1.dist-info/WHEEL
 Comment: 
 
-Filename: beaker_pyteal-1.0.1b1.dist-info/RECORD
+Filename: beaker_pyteal-1.0.2b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beaker/__init__.py

```diff
@@ -1,8 +1,8 @@
-from . import client, consts, lib, sandbox
+from . import client, consts, lib, localnet
 from .application import (
     Application,
     precompiled,
     this_app,
     unconditional_create_approval,
     unconditional_opt_in_approval,
 )
@@ -34,12 +34,12 @@
     "ReservedLocalStateValue",
     "client",
     "consts",
     "identity_key_gen",
     "lib",
     "precompiled",
     "prefix_key_gen",
-    "sandbox",
+    "localnet",
     "this_app",
     "unconditional_create_approval",
     "unconditional_opt_in_approval",
 ]
```

## beaker/application.py

```diff
@@ -1128,25 +1128,44 @@
                                 for k, v in abi_external.actions.items()
                             },
                         )
                     ),
                 )
                 hints[abi_external.method.method_signature()] = abi_external.hints
 
-            # Compile approval and clear programs
-            approval_program, clear_program, contract = router.compile_program(
+                # Compile approval and clear programs
+            compile_results = router.compile(
+                algod_client=client,
                 version=self.build_options.avm_version,
                 assemble_constants=self.build_options.assemble_constants,
                 optimize=self.build_options.optimize_options,
+                with_sourcemaps=self.build_options.with_sourcemaps,
+                pcs_in_sourcemap=bool(client),
+                annotate_teal=self.build_options.annotate_teal,
+                annotate_teal_headers=self.build_options.annotate_teal_headers,
+                annotate_teal_concise=self.build_options.annotate_teal_concise,
             )
 
+            approval_prog: str = compile_results.approval_teal
+            clear_prog: str = compile_results.clear_teal
+
+            if compile_results.approval_sourcemap is not None:
+                approval_sm = compile_results.approval_sourcemap
+                if approval_sm.annotated_teal is not None:
+                    approval_prog = approval_sm.annotated_teal
+
+            if compile_results.clear_sourcemap is not None:
+                clear_sm = compile_results.clear_sourcemap
+                if clear_sm.annotated_teal is not None:
+                    clear_prog = clear_sm.annotated_teal
+
         return ApplicationSpecification(
-            approval_program=approval_program,
-            clear_program=clear_program,
-            contract=contract,
+            approval_program=approval_prog,
+            clear_program=clear_prog,
+            contract=compile_results.abi_contract,
             hints=hints,
             schema={
                 "global": self._global_state.dictify(),
                 "local": self._local_state.dictify(),
             },
             global_state_schema=self._global_state.schema,
             local_state_schema=self._local_state.schema,
```

## beaker/build_options.py

```diff
@@ -20,13 +20,26 @@
     assemble_constants: bool = True
     """When true, the compiler will produce a program with fully
         assembled constants, rather than using the pseudo-ops `int`, `byte`, and `addr`. These
         constants will be assembled in the most space-efficient way, so enabling this may reduce
         the compiled program's size. Enabling this option requires a minimum AVM version of 3.
         Defaults to True."""
 
+    with_sourcemaps: bool = False
+    """When `True`, the compiler will produce a source map that associates
+        each line of the generated TEAL program back to the original PyTeal source code. Defaults to `False`.  """
+    annotate_teal: bool = False
+    """When `True`, the compiler will produce a TEAL program with comments
+        that describe the PyTeal source code that generated each line of the program. Defaults to `False`."""
+    annotate_teal_headers: bool = False
+    """When `True` along with `annotate_teal` being `True`, a header
+        line with column names will be added at the top of the annotated teal. Defaults to `False`."""
+    annotate_teal_concise: bool = False
+    """When `True` along with `annotate_teal` being `True`, the compiler
+        will provide fewer columns in the annotated teal. Defaults to `False`."""
+
     @property
     def optimize_options(self) -> OptimizeOptions:
         return OptimizeOptions(
             scratch_slots=self.scratch_slots,
             frame_pointers=self.frame_pointers,
         )
```

## beaker/client/api_providers.py

```diff
@@ -18,25 +18,29 @@
 
     algod_hosts: dict[Network, str] = {}
     indexer_hosts: dict[Network, str] = {}
 
     def __init__(self, network: Network):
         self.network = network
 
-    def algod(self, token: str = "") -> AlgodClient:
+    def algod(
+        self, token: str = "", headers: dict[str, str] | None = None
+    ) -> AlgodClient:
         """return an algod client based on the provider used and network it was initialized with"""
         if self.network not in self.algod_hosts:
             raise Exception(f"Unrecognized network: {self.network}")
-        return AlgodClient(token, self.algod_hosts[self.network])
+        return AlgodClient(token, self.algod_hosts[self.network], headers)
 
-    def indexer(self, token: str = "") -> IndexerClient:
+    def indexer(
+        self, token: str = "", headers: dict[str, str] | None = None
+    ) -> IndexerClient:
         """return an indexer client based on the provider used and network it was initialized with"""
         if self.network not in self.indexer_hosts:
             raise Exception(f"Unrecognized network: {self.network}")
-        return IndexerClient(token, self.indexer_hosts[self.network])
+        return IndexerClient(token, self.indexer_hosts[self.network], headers)
 
 
 class AlgoNode(APIProvider):
     algod_hosts = {
         Network.MainNet: "https://mainnet-api.algonode.cloud",
         Network.TestNet: "https://testnet-api.algonode.cloud",
         Network.BetaNet: "https://betanet-api.algonode.cloud",
@@ -76,33 +80,45 @@
         Network.BetaNet: "https://betanet-algorand.api.purestake.io/idx2",
     }
 
     token_header = "X-API-Key"
 
     # Purestake requires a different header, so we override the
     # existing methods but re-use them to generate the client
-    def algod(self, token: str = "") -> AlgodClient:
-        algod_client = super().algod()
-        algod_client.headers = {self.token_header: token}  # type: ignore[misc]
+    def algod(
+        self, token: str = "", headers: dict[str, str] | None = None
+    ) -> AlgodClient:
+        _headers = {self.token_header: token}
+        if headers is not None:
+            _headers |= headers
+        algod_client = super().algod(token, _headers)
         return algod_client
 
-    def indexer(self, token: str = "") -> IndexerClient:
-        indexer_client = super().indexer()
-        indexer_client.headers = {self.token_header: token}
+    def indexer(
+        self, token: str = "", headers: dict[str, str] | None = None
+    ) -> IndexerClient:
+        _headers = {self.token_header: token}
+        if headers is not None:
+            _headers |= headers
+        indexer_client = super().indexer(token, _headers)
         return indexer_client
 
 
 class Sandbox(APIProvider):
     default_host = "http://localhost"
     default_algod_port: int = 4001
     default_indexer_port: int = 8980
     default_token: str = "a" * 64
 
     # purposely doesn't check which network because it may
     # be set up to use mainnet/testnet
-    def algod(self, token: str = default_token) -> AlgodClient:
+    def algod(
+        self, token: str = default_token, headers: dict[str, str] | None = None
+    ) -> AlgodClient:
         address = f"{self.default_host}:{self.default_algod_port}"
-        return AlgodClient(token, address)
+        return AlgodClient(token, address, headers)
 
-    def indexer(self, token: str = default_token) -> IndexerClient:
+    def indexer(
+        self, token: str = default_token, headers: dict[str, str] | None = None
+    ) -> IndexerClient:
         address = f"{self.default_host}:{self.default_indexer_port}"
-        return IndexerClient(token, address)
+        return IndexerClient(token, address, headers)
```

## beaker/client/application_client.py

```diff
@@ -7,14 +7,15 @@
 from algokit_utils import ApplicationClient as AlgokitApplicationClient
 from algokit_utils import (
     ApplicationSpecification,
     CommonCallParameters,
     CreateCallParameters,
     OnCompleteCallParameters,
     Program,
+    get_sender_from_signer,
 )
 from algosdk import transaction
 from algosdk.abi import Method
 from algosdk.atomic_transaction_composer import (
     ABIResult,
     AtomicTransactionComposer,
     AtomicTransactionResponse,
@@ -51,14 +52,16 @@
                 app_spec = ApplicationSpecification.from_json(
                     path.read_text(encoding="utf8")
                 )
             case str():
                 app_spec = ApplicationSpecification.from_json(app)
             case _:
                 raise Exception(f"Unexpected app type: {app}")
+        # algokit client does not get sender from signer on init, do so here to keep original beaker client behaviour
+        sender = sender or get_sender_from_signer(signer)
         self._app_client = AlgokitApplicationClient(
             client,
             app_spec,
             app_id=app_id,
             signer=signer,
             sender=sender,
             suggested_params=suggested_params,
@@ -108,22 +111,26 @@
     def approval(self) -> Program | None:
         return self._app_client.approval
 
     @property
     def clear(self) -> Program | None:
         return self._app_client.clear
 
+    @property
+    def algokit_app_client(self) -> AlgokitApplicationClient:
+        return self._app_client
+
     def get_sender(
         self, sender: str | None = None, signer: TransactionSigner | None = None
     ) -> str:
-        signer, sender = self._app_client._resolve_signer_sender(signer, sender)
+        _, sender = self._app_client.resolve_signer_sender(signer, sender)
         return sender
 
     def get_signer(self, signer: TransactionSigner | None = None) -> TransactionSigner:
-        signer, sender = self._app_client._resolve_signer_sender(signer, None)
+        signer, _ = self._app_client.resolve_signer_sender(signer, "ignored")
         return signer
 
     def get_suggested_params(
         self,
         sp: transaction.SuggestedParams | None = None,
     ) -> transaction.SuggestedParams:
 
@@ -416,24 +423,24 @@
     def prepare(
         self,
         signer: TransactionSigner | None = None,
         sender: str | None = None,
         app_id: int | None = None,
     ) -> "ApplicationClient":
         """makes a copy of the current ApplicationClient and the fields passed"""
-        signer = self.get_signer(signer)
-        sender = self.get_sender(sender, signer)
+        signer, sender = self._app_client.get_signer_sender(signer, sender)
         copy = ApplicationClient(
             self.client,
             self._app_client.app_spec,
             app_id=self.app_id if app_id is None else app_id,
             signer=signer,
             sender=sender,
             suggested_params=self.suggested_params,
         )
+        # also make a copy of inner client so any cached programs are retained
         copy._app_client = copy._app_client.prepare(
             signer=signer, sender=sender, app_id=app_id
         )
         return copy
 
 
 def _extract_kwargs(
```

## beaker/sandbox/__init__.py

```diff
@@ -1,10 +1,14 @@
+from warnings import warn
+
 from .clients import get_algod_client, get_indexer_client
 from .kmd import SandboxAccount, add_account, get_accounts
 
 __all__ = [
     "SandboxAccount",
     "add_account",
     "get_accounts",
     "get_algod_client",
     "get_indexer_client",
 ]
+
+warn("beaker.sandbox is being deprecated, use beaker.localnet instead")
```

## beaker/sandbox/clients.py

```diff
@@ -1,22 +1,17 @@
-from algosdk.v2client.algod import AlgodClient
-from algosdk.v2client.indexer import IndexerClient
-
-DEFAULT_ALGOD_ADDRESS = "http://localhost:4001"
-DEFAULT_ALGOD_TOKEN = "a" * 64
-
-DEFAULT_INDEXER_ADDRESS = "http://localhost:8980"
-DEFAULT_INDEXER_TOKEN = "a" * 64
-
-
-def get_algod_client(
-    address: str = DEFAULT_ALGOD_ADDRESS, token: str = DEFAULT_ALGOD_TOKEN
-) -> AlgodClient:
-    """creates a new algod client using the default sandbox parameters"""
-    return AlgodClient(token, address)
-
-
-def get_indexer_client(
-    address: str = DEFAULT_INDEXER_ADDRESS, token: str = DEFAULT_INDEXER_TOKEN
-) -> IndexerClient:
-    """creates a new indexer client using the default sandbox parameters"""
-    return IndexerClient(token, address)
+from ..localnet.clients import (
+    DEFAULT_ALGOD_ADDRESS,
+    DEFAULT_ALGOD_TOKEN,
+    DEFAULT_INDEXER_ADDRESS,
+    DEFAULT_INDEXER_TOKEN,
+    get_algod_client,
+    get_indexer_client,
+)
+
+__all__ = [
+    "get_algod_client",
+    "get_indexer_client",
+    "DEFAULT_ALGOD_ADDRESS",
+    "DEFAULT_ALGOD_TOKEN",
+    "DEFAULT_INDEXER_ADDRESS",
+    "DEFAULT_INDEXER_TOKEN",
+]
```

## beaker/sandbox/kmd.py

```diff
@@ -1,106 +1,34 @@
-import contextlib
-from collections.abc import Iterator
-from dataclasses import dataclass
-from functools import cached_property
-
-from algosdk.atomic_transaction_composer import AccountTransactionSigner
-from algosdk.kmd import KMDClient
-from algosdk.wallet import Wallet
-
-DEFAULT_KMD_ADDRESS = "http://localhost:4002"
-DEFAULT_KMD_TOKEN = "a" * 64
-DEFAULT_KMD_WALLET_NAME = "unencrypted-default-wallet"
-DEFAULT_KMD_WALLET_PASSWORD = ""
-
-
-def get_client() -> KMDClient:
-    """creates a new kmd client using the default sandbox parameters"""
-    return KMDClient(kmd_token=DEFAULT_KMD_TOKEN, kmd_address=DEFAULT_KMD_ADDRESS)
-
-
-def get_sandbox_default_wallet() -> Wallet:
-    """returns the default sandbox kmd wallet"""
-    return Wallet(
-        wallet_name=DEFAULT_KMD_WALLET_NAME,
-        wallet_pswd=DEFAULT_KMD_WALLET_PASSWORD,
-        kmd_client=get_client(),
-    )
-
-
-@dataclass(kw_only=True)
-class SandboxAccount:
-    """SandboxAccount is a simple dataclass to hold a sandbox account details"""
-
-    #: The address of a sandbox account
-    address: str
-    #: The base64 encoded private key of the account
-    private_key: str
-
-    #: An AccountTransactionSigner that can be used as a TransactionSigner
-    @cached_property
-    def signer(self) -> AccountTransactionSigner:
-        return AccountTransactionSigner(self.private_key)
-
-
-def get_accounts(
-    kmd_address: str = DEFAULT_KMD_ADDRESS,
-    kmd_token: str = DEFAULT_KMD_TOKEN,
-    wallet_name: str = DEFAULT_KMD_WALLET_NAME,
-    wallet_password: str = DEFAULT_KMD_WALLET_PASSWORD,
-) -> list[SandboxAccount]:
-    """gets all the accounts in the sandbox kmd, defaults
-    to the `unencrypted-default-wallet` created on private networks automatically"""
-    kmd = KMDClient(kmd_token, kmd_address)
-    with wallet_handle_by_name(kmd, wallet_name, wallet_password) as wallet_handle:
-        return [
-            SandboxAccount(
-                address=address,
-                private_key=kmd.export_key(wallet_handle, wallet_password, address),
-            )
-            for address in kmd.list_keys(wallet_handle)
-        ]
-
-
-def add_account(
-    private_key: str,
-    kmd_address: str = DEFAULT_KMD_ADDRESS,
-    kmd_token: str = DEFAULT_KMD_TOKEN,
-    wallet_name: str = DEFAULT_KMD_WALLET_NAME,
-    wallet_password: str = DEFAULT_KMD_WALLET_PASSWORD,
-) -> str:
-    """Adds a new account to the sandbox kmd"""
-    kmd = KMDClient(kmd_token, kmd_address)
-    with wallet_handle_by_name(kmd, wallet_name, wallet_password) as wallet_handle:
-        return kmd.import_key(wallet_handle, private_key)
-
-
-def delete_account(
-    address: str,
-    kmd_address: str = DEFAULT_KMD_ADDRESS,
-    kmd_token: str = DEFAULT_KMD_TOKEN,
-    wallet_name: str = DEFAULT_KMD_WALLET_NAME,
-    wallet_password: str = DEFAULT_KMD_WALLET_PASSWORD,
-) -> None:
-    """Deletes an existing account from the sandbox kmd"""
-    kmd = KMDClient(kmd_token, kmd_address)
-    with wallet_handle_by_name(kmd, wallet_name, wallet_password) as wallet_handle:
-        kmd.delete_key(wallet_handle, wallet_password, address)
-
-
-@contextlib.contextmanager
-def wallet_handle_by_name(
-    kmd: KMDClient, wallet_name: str, wallet_password: str
-) -> Iterator[str]:
-
-    wallets = kmd.list_wallets()
-
-    try:
-        wallet_id = next(iter(w["id"] for w in wallets if w["name"] == wallet_name))
-    except StopIteration:
-        raise Exception(f"Wallet not found: {wallet_name}") from None
-
-    wallet_handle = kmd.init_wallet_handle(wallet_id, wallet_password)
-    try:
-        yield wallet_handle
-    finally:
-        kmd.release_wallet_handle(wallet_handle)
+from ..localnet.kmd import (
+    DEFAULT_KMD_ADDRESS,
+    DEFAULT_KMD_TOKEN,
+    DEFAULT_KMD_WALLET_NAME,
+    DEFAULT_KMD_WALLET_PASSWORD,
+    LocalAccount,
+    add_account,
+    delete_account,
+    get_accounts,
+    get_client,
+    get_localnet_default_wallet,
+    wallet_handle_by_name,
+)
+
+get_sandbox_default_wallet = get_localnet_default_wallet
+
+
+class SandboxAccount(LocalAccount):
+    pass
+
+
+__all__ = [
+    "get_client",
+    "get_sandbox_default_wallet",
+    "SandboxAccount",
+    "get_accounts",
+    "add_account",
+    "delete_account",
+    "wallet_handle_by_name",
+    "DEFAULT_KMD_ADDRESS",
+    "DEFAULT_KMD_TOKEN",
+    "DEFAULT_KMD_WALLET_NAME",
+    "DEFAULT_KMD_WALLET_PASSWORD",
+]
```

## Comparing `beaker_pyteal-1.0.1b1.dist-info/LICENSE` & `beaker_pyteal-1.0.2b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beaker_pyteal-1.0.1b1.dist-info/METADATA` & `beaker_pyteal-1.0.2b1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: beaker-pyteal
-Version: 1.0.1b1
+Version: 1.0.2b1
 Summary: A Framework for building PyTeal Applications
 Home-page: https://beaker.algo.xyz
 License: MIT
 Keywords: pyteal,algorand
 Author: Ben Guidarelli
 Author-email: ben@algorand.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: algokit-utils (>=1.0.0,<2.0.0)
+Requires-Dist: algokit-utils (>=1.0.2,<2.0.0)
 Requires-Dist: py-algorand-sdk (>=2.0.0)
-Requires-Dist: pyteal (>=0.23.0,<0.24.0)
+Requires-Dist: pyteal (>=0.24,<0.25)
 Project-URL: Repository, https://github.com/algorand-devrel/beaker
 Description-Content-Type: text/markdown
 
 Beaker
 ------
 <img align="left" src="https://raw.githubusercontent.com/algorand-devrel/beaker/master/beaker.png" margin="10px" >
```

## Comparing `beaker_pyteal-1.0.1b1.dist-info/RECORD` & `beaker_pyteal-1.0.2b1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-beaker/__init__.py,sha256=tXSQjGQJo35KdLcemNYY5mYaHwiZ0OfQijsnOudjBzI,1027
-beaker/application.py,sha256=oPjTCdppmDelP-xw5jZbSHgKQrO3GVoPcU1Ljj9Cm98,44553
-beaker/build_options.py,sha256=4A42BiGXu1bxb9IPv3iRRmDVRMVwTOsvTyHHujUow9g,1204
+beaker/__init__.py,sha256=Zafo6SvJS0NuCF7YRoS76_eYXEEyXb17SJheL1fs3uw,1029
+beaker/application.py,sha256=U6PYMuLE1pqi6ZtxqndsBOjXa9y2lJCwQ28KfAXOsBY,45518
+beaker/build_options.py,sha256=kBy7fYzTTLy7Ik3OHrO5qiJUilohNB2rBwB90T0pbr0,2053
 beaker/client/__init__.py,sha256=I8qm-6zAR91ppLXeEMoB6n0hgb4OtuBoYyYdqBDlRD4,340
-beaker/client/api_providers.py,sha256=jYqo3vIwLMaVOEMcOhxbU1Irf_YXsatBuwcsczHxde4,3933
-beaker/client/application_client.py,sha256=rExM6KtGSeQtUXeq9k8CTDK2IemSNN4aLgH_ngsR1FY,15852
+beaker/client/api_providers.py,sha256=oo43FWdGYk97sYS3B9-uPaX-oRA1tuInXDQ1f_ZvHIE,4397
+beaker/client/application_client.py,sha256=iqOdmK5_HyaeI4r6prlM4Jzfyb6P2zxv02l8OmPW_N8,16223
 beaker/compilation.py,sha256=tGwhSY4igShDZPuH6BXSyarYK3norBFZKLXEPDgVWo0,1239
 beaker/consts.py,sha256=Tb8D_rPKTqG1_7-zEEyx567qMPwdCiQ-V2Hbbco2ABc,1923
 beaker/decorators.py,sha256=oV__PUkcf9w4VBZ0WzOa4FJ9vshzlyLxDPwBr1dD_88,2521
 beaker/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beaker/lib/inline.py,sha256=bCtunBew8mjlYm9imFveMAPxF8-y48Dq-iv8lX3JInE,1849
 beaker/lib/iter.py,sha256=ruBqc7YR0KL4cIvo5Gcx117w6i6VT2e4DuYQJtRxOJQ,707
 beaker/lib/math.py,sha256=P7YOD3QAq2dpmd-fuiqTIZ5bvtk8gnVYY10h86NI8tM,6449
 beaker/lib/storage/__init__.py,sha256=7VfJiPHvtf4fahidKeQQQ4e17KASqzN4HEnqJYgIsOE,219
 beaker/lib/storage/blob.py,sha256=is1HC-FmaqkbcRnLIVRpFRrKgnOyHEhhAfvz3q-yV9A,1968
 beaker/lib/storage/box_list.py,sha256=2hP2H9NBCFkJTU6erZ0cj8W_APkfs5-OkCK2YjICA7Y,3308
 beaker/lib/storage/box_mapping.py,sha256=ejRpiG0RCb59hoWTsKARZCluenOTKWwFXjx15nagvMA,3808
 beaker/lib/storage/global_blob.py,sha256=5L3SLtaYaZ_rnIragHfXNHlpi0QYt6cFKFk6-0e9EkU,6841
 beaker/lib/storage/local_blob.py,sha256=3Iql4q6vWu9nx7E6tWAdL9tYX6GLa2YihEoe4bMI2_Y,7631
 beaker/lib/strings.py,sha256=NAlnfa_IMvMSY-p-ZFI0IzFnDa_rzOSAHCejENEF3GI,4226
+beaker/localnet/__init__.py,sha256=HZM_thVlWIVwZ-of4vaCEYfasUYLYyL2Me3DUh3cVF0,239
+beaker/localnet/clients.py,sha256=RDhQl_iYJvsn_wWE1GZaDyn7dmn8zbyyt_7hDmAE5LA,736
+beaker/localnet/kmd.py,sha256=q6womWe1UoDQyK7tHDrxWrPuT8NuAERZm9tPD6VyAQw,3578
 beaker/logic_signature.py,sha256=fV9N_6EPpXa5bbmPAxrJ0NR1FcQUyU_yUZKNTHMFQtg,5352
 beaker/precompile.py,sha256=qQGRWu1Vhce9zdLvDC6UYnPG-pVN9yL-sdG9Bdn3UPY,10620
 beaker/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-beaker/sandbox/__init__.py,sha256=jf2CdWxkVixeaQqvYwxQgDm9wlVDfJBs9V_mCjWe90Y,243
-beaker/sandbox/clients.py,sha256=YoOhrosbAMz-fKcZBDdncNnfZBisp15tCGEgLtL5CKY,734
-beaker/sandbox/kmd.py,sha256=Z0JnMLemRhXmPRsyRwL-RAv6sLtxeM8bWgm-F31D_Ho,3578
+beaker/sandbox/__init__.py,sha256=CJiKdNtRuFb-IqrLWleJ9aNXW6N1gy_umVVFqGsyTZA,343
+beaker/sandbox/clients.py,sha256=mzxHT-Z6r-59nKnIiosMloCJENL6BYIOTUP4sko7GU4,370
+beaker/sandbox/kmd.py,sha256=Vv5RcqtckOcp5r118Bv-Dx7-4wCCes-6ZqPfVi2U07M,693
 beaker/state/__init__.py,sha256=iYUSAH3te00kKwgC1sSV72cxRzv1BNcWcGJlPHRQr5k,837
 beaker/state/_abc.py,sha256=voWExtCshDtcPdPIYP6xIdIvuaM6EdL_Bh57a2V5WUk,751
 beaker/state/_aggregate.py,sha256=82HK---a8yfcupP_Z_rG2ig-fYTLiq8O59LAGCIMGlM,3489
 beaker/state/blob.py,sha256=gECzmITgSnsd_7qKtLCpxjZRf6E8Fx136i_Sy2cmXXM,3904
 beaker/state/primitive.py,sha256=RtGQTdZtLoAmHV85hg50czJ0B5A0jEGtPrkUgdx0-JE,10370
 beaker/state/reserved.py,sha256=YoEZAjxK_cSFRbb5vldX8RhXKoy3g6XeQVJWAEaW5I4,6335
-beaker_pyteal-1.0.1b1.dist-info/LICENSE,sha256=kvKjEpeo_RzCoWYr0x-mWqdClWMyaqC1DZQpI30hq5E,1065
-beaker_pyteal-1.0.1b1.dist-info/METADATA,sha256=E0MduEQzi85pY1WPqI2zpTJi27KXu3UaJDdpRw-OuA8,2875
-beaker_pyteal-1.0.1b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-beaker_pyteal-1.0.1b1.dist-info/RECORD,,
+beaker_pyteal-1.0.2b1.dist-info/LICENSE,sha256=kvKjEpeo_RzCoWYr0x-mWqdClWMyaqC1DZQpI30hq5E,1065
+beaker_pyteal-1.0.2b1.dist-info/METADATA,sha256=2aEIcnnSZYhkKCCzfaV6tTL-CgYKj4eDixX7AtMKanw,2871
+beaker_pyteal-1.0.2b1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+beaker_pyteal-1.0.2b1.dist-info/RECORD,,
```

