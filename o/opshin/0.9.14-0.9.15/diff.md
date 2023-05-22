# Comparing `tmp/opshin-0.9.14.tar.gz` & `tmp/opshin-0.9.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opshin-0.9.14.tar", max compression
+gzip compressed data, was "opshin-0.9.15.tar", max compression
```

## Comparing `opshin-0.9.14.tar` & `opshin-0.9.15.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-03-18 21:52:55.536442 opshin-0.9.14/LICENSE.txt
--rw-r--r--   0        0        0    10198 2023-03-18 21:52:55.536442 opshin-0.9.14/README.md
--rw-r--r--   0        0        0      398 2023-03-18 21:52:55.544443 opshin-0.9.14/opshin/__init__.py
--rw-r--r--   0        0        0     8107 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/__main__.py
--rw-r--r--   0        0        0    34621 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/compiler.py
--rw-r--r--   0        0        0        0 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/ledger/__init__.py
--rw-r--r--   0        0        0     2936 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/ledger/interval.py
--rw-r--r--   0        0        0        1 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/optimize/__init__.py
--rw-r--r--   0        0        0     6451 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/optimize/optimize_remove_deadvars.py
--rw-r--r--   0        0        0      253 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/optimize/optimize_remove_pass.py
--rw-r--r--   0        0        0     2528 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/optimize/optimize_varlen.py
--rw-r--r--   0        0        0    12190 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/prelude.py
--rw-r--r--   0        0        0        0 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/__init__.py
--rw-r--r--   0        0        0      630 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_augassign.py
--rw-r--r--   0        0        0      704 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_forbidden_overwrites.py
--rw-r--r--   0        0        0     2791 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_import.py
--rw-r--r--   0        0        0     1763 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_import_dataclasses.py
--rw-r--r--   0        0        0     2681 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_import_hashlib.py
--rw-r--r--   0        0        0     2012 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_import_plutusdata.py
--rw-r--r--   0        0        0     1183 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_import_typing.py
--rw-r--r--   0        0        0     1167 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_inject_builtin_constr.py
--rw-r--r--   0        0        0      961 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_inject_builtins.py
--rw-r--r--   0        0        0      851 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_remove_type_stuff.py
--rw-r--r--   0        0        0     1104 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/rewrite/rewrite_tuple_assign.py
--rw-r--r--   0        0        0        0 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/__init__.py
--rw-r--r--   0        0        0    14906 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/test_builtins.py
--rw-r--r--   0        0        0        0 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/test_ledger/__init__.py
--rw-r--r--   0        0        0     5729 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/test_ledger/test_interval.py
--rw-r--r--   0        0        0    29714 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/test_misc.py
--rw-r--r--   0        0        0    17394 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/test_ops.py
--rw-r--r--   0        0        0     6472 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/tests/test_stdlib.py
--rw-r--r--   0        0        0    28198 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/type_inference.py
--rw-r--r--   0        0        0    39748 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/typed_ast.py
--rw-r--r--   0        0        0    21723 2023-03-18 21:52:55.548442 opshin-0.9.14/opshin/util.py
--rw-r--r--   0        0        0     1240 2023-03-18 21:52:55.548442 opshin-0.9.14/pyproject.toml
--rw-r--r--   0        0        0    11217 1970-01-01 00:00:00.000000 opshin-0.9.14/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-20 15:57:32.630155 opshin-0.9.15/LICENSE.txt
+-rw-r--r--   0        0        0    10198 2023-03-20 15:57:32.630155 opshin-0.9.15/README.md
+-rw-r--r--   0        0        0      426 2023-03-20 15:57:32.638155 opshin-0.9.15/opshin/__init__.py
+-rw-r--r--   0        0        0     7295 2023-03-20 15:57:32.638155 opshin-0.9.15/opshin/__main__.py
+-rw-r--r--   0        0        0     2172 2023-03-20 15:57:32.638155 opshin-0.9.15/opshin/builder.py
+-rw-r--r--   0        0        0    34700 2023-03-20 15:57:32.638155 opshin-0.9.15/opshin/compiler.py
+-rw-r--r--   0        0        0        0 2023-03-20 15:57:32.638155 opshin-0.9.15/opshin/ledger/__init__.py
+-rw-r--r--   0        0        0     2936 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/ledger/interval.py
+-rw-r--r--   0        0        0        1 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/optimize/__init__.py
+-rw-r--r--   0        0        0     6451 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/optimize/optimize_remove_deadvars.py
+-rw-r--r--   0        0        0      253 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/optimize/optimize_remove_pass.py
+-rw-r--r--   0        0        0     2528 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/optimize/optimize_varlen.py
+-rw-r--r--   0        0        0    12190 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/prelude.py
+-rw-r--r--   0        0        0        0 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/__init__.py
+-rw-r--r--   0        0        0      630 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_augassign.py
+-rw-r--r--   0        0        0      704 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_forbidden_overwrites.py
+-rw-r--r--   0        0        0     2791 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_import.py
+-rw-r--r--   0        0        0     1763 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_import_dataclasses.py
+-rw-r--r--   0        0        0     2681 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_import_hashlib.py
+-rw-r--r--   0        0        0     2012 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_import_plutusdata.py
+-rw-r--r--   0        0        0     1183 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_import_typing.py
+-rw-r--r--   0        0        0     1167 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_inject_builtin_constr.py
+-rw-r--r--   0        0        0      961 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_inject_builtins.py
+-rw-r--r--   0        0        0      851 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_remove_type_stuff.py
+-rw-r--r--   0        0        0     1104 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_tuple_assign.py
+-rw-r--r--   0        0        0     1498 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/rewrite/rewrite_zero_ary.py
+-rw-r--r--   0        0        0        0 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/__init__.py
+-rw-r--r--   0        0        0    14906 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/test_builtins.py
+-rw-r--r--   0        0        0        0 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/test_ledger/__init__.py
+-rw-r--r--   0        0        0     5729 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/test_ledger/test_interval.py
+-rw-r--r--   0        0        0    31050 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/test_misc.py
+-rw-r--r--   0        0        0    17394 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/test_ops.py
+-rw-r--r--   0        0        0     6472 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/tests/test_stdlib.py
+-rw-r--r--   0        0        0    28322 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/type_inference.py
+-rw-r--r--   0        0        0    39748 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/typed_ast.py
+-rw-r--r--   0        0        0    21723 2023-03-20 15:57:32.642156 opshin-0.9.15/opshin/util.py
+-rw-r--r--   0        0        0     1240 2023-03-20 15:57:32.642156 opshin-0.9.15/pyproject.toml
+-rw-r--r--   0        0        0    11217 1970-01-01 00:00:00.000000 opshin-0.9.15/PKG-INFO
```

### Comparing `opshin-0.9.14/LICENSE.txt` & `opshin-0.9.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/README.md` & `opshin-0.9.15/README.md`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/__main__.py` & `opshin-0.9.15/opshin/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 import importlib
 import json
 import pathlib
 import sys
 import typing
 import ast
 
-import cbor2
-import pyaiken
 import pycardano
 import uplc
 import uplc.ast
 
-from opshin import __version__, compiler
+from opshin import __version__, compiler, builder
 from opshin.util import CompilerError, data_from_json
 
 
 class Command(enum.Enum):
     compile_pluto = "compile_pluto"
     compile = "compile"
     eval = "eval"
@@ -174,46 +172,25 @@
                     "Please supply an output directory if no input file is specified."
                 )
                 exit(-1)
             target_dir = pathlib.Path("build") / pathlib.Path(input_file).stem
         else:
             target_dir = pathlib.Path(args.output_directory)
         target_dir.mkdir(exist_ok=True, parents=True)
-        uplc_dump = code.dumps()
-        cbor_hex = pyaiken.uplc.flat(uplc_dump)
-        # create cbor file for use with pycardano/lucid
+        artifacts = builder._build(code)
         with (target_dir / "script.cbor").open("w") as fp:
-            fp.write(cbor_hex)
-        cbor = bytes.fromhex(cbor_hex)
-        # double wrap
-        cbor_wrapped = cbor2.dumps(cbor)
-        cbor_wrapped_hex = cbor_wrapped.hex()
-        # create plutus file
-        d = {
-            "type": "PlutusScriptV2",
-            "description": f"opshin {__version__} Smart Contract",
-            "cborHex": cbor_wrapped_hex,
-        }
+            fp.write(artifacts.cbor_hex)
         with (target_dir / "script.plutus").open("w") as fp:
-            json.dump(d, fp)
-        script_hash = pycardano.plutus_script_hash(pycardano.PlutusV2Script(cbor))
-        # generate policy ids
+            fp.write(artifacts.plutus_json)
         with (target_dir / "script.policy_id").open("w") as fp:
-            fp.write(script_hash.to_primitive().hex())
-        addr_mainnet = pycardano.Address(
-            script_hash, network=pycardano.Network.MAINNET
-        ).encode()
-        # generate addresses
+            fp.write(artifacts.policy_id)
         with (target_dir / "mainnet.addr").open("w") as fp:
-            fp.write(addr_mainnet)
-        addr_testnet = pycardano.Address(
-            script_hash, network=pycardano.Network.TESTNET
-        ).encode()
+            fp.write(artifacts.mainnet_addr)
         with (target_dir / "testnet.addr").open("w") as fp:
-            fp.write(addr_testnet)
+            fp.write(artifacts.testnet_addr)
 
         print(f"Wrote script artifacts to {target_dir}/")
         return
     if command == Command.eval_uplc:
         print("Starting execution")
         print("------------------")
         assert isinstance(code, uplc.ast.Program)
```

### Comparing `opshin-0.9.14/opshin/compiler.py` & `opshin-0.9.15/opshin/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .rewrite.rewrite_import_hashlib import RewriteImportHashlib
 from .rewrite.rewrite_import_plutusdata import RewriteImportPlutusData
 from .rewrite.rewrite_import_typing import RewriteImportTyping
 from .rewrite.rewrite_inject_builtins import RewriteInjectBuiltins
 from .rewrite.rewrite_inject_builtin_constr import RewriteInjectBuiltinsConstr
 from .rewrite.rewrite_remove_type_stuff import RewriteRemoveTypeStuff
 from .rewrite.rewrite_tuple_assign import RewriteTupleAssign
+from .rewrite.rewrite_zero_ary import RewriteZeroAry
 from .optimize.optimize_remove_pass import OptimizeRemovePass
 from .optimize.optimize_remove_deadvars import OptimizeRemoveDeadvars
 from .optimize.optimize_varlen import OptimizeVarlen
 from .type_inference import *
 from .util import CompilingNodeTransformer, PowImpl
 from .typed_ast import transform_ext_params_map, transform_output_map, RawPlutoExpr
 
@@ -853,14 +854,15 @@
         RewriteImportTyping(),
         RewriteForbiddenOverwrites(),
         RewriteImportDataclasses(),
         RewriteInjectBuiltins(),
         # The type inference needs to be run after complex python operations were rewritten
         AggressiveTypeInferencer(),
         # Rewrites that circumvent the type inference or use its results
+        RewriteZeroAry(),
         RewriteInjectBuiltinsConstr(),
         RewriteRemoveTypeStuff(),
     ]
     for s in rewrite_steps:
         prog = s.visit(prog)
         prog = fix_missing_locations(prog)
```

### Comparing `opshin-0.9.14/opshin/ledger/interval.py` & `opshin-0.9.15/opshin/ledger/interval.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/optimize/optimize_remove_deadvars.py` & `opshin-0.9.15/opshin/optimize/optimize_remove_deadvars.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/optimize/optimize_varlen.py` & `opshin-0.9.15/opshin/optimize/optimize_varlen.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/prelude.py` & `opshin-0.9.15/opshin/prelude.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_augassign.py` & `opshin-0.9.15/opshin/rewrite/rewrite_augassign.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_forbidden_overwrites.py` & `opshin-0.9.15/opshin/rewrite/rewrite_forbidden_overwrites.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_import.py` & `opshin-0.9.15/opshin/rewrite/rewrite_import.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_import_dataclasses.py` & `opshin-0.9.15/opshin/rewrite/rewrite_import_dataclasses.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_import_hashlib.py` & `opshin-0.9.15/opshin/rewrite/rewrite_import_hashlib.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_import_plutusdata.py` & `opshin-0.9.15/opshin/rewrite/rewrite_import_plutusdata.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_import_typing.py` & `opshin-0.9.15/opshin/rewrite/rewrite_import_typing.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_inject_builtin_constr.py` & `opshin-0.9.15/opshin/rewrite/rewrite_inject_builtin_constr.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_inject_builtins.py` & `opshin-0.9.15/opshin/rewrite/rewrite_inject_builtins.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_remove_type_stuff.py` & `opshin-0.9.15/opshin/rewrite/rewrite_remove_type_stuff.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/rewrite/rewrite_tuple_assign.py` & `opshin-0.9.15/opshin/rewrite/rewrite_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/tests/test_builtins.py` & `opshin-0.9.15/opshin/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/tests/test_ledger/test_interval.py` & `opshin-0.9.15/opshin/tests/test_ledger/test_interval.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/tests/test_misc.py` & `opshin-0.9.15/opshin/tests/test_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -740,7 +740,59 @@
     b: int = x
     return b
 """
         ast = compiler.parse(source_code)
         code = compiler.compile(ast).compile()
         res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0))).value
         self.assertEqual(res, 0)
+
+    def test_zero_ary(self):
+        source_code = """
+def a() -> None:
+    assert False, "Executed a"
+
+def validator(x: None) -> None:
+    b = a
+    if False:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    @unittest.expectedFailure
+    def test_zero_ary_exec(self):
+        source_code = """
+def a() -> None:
+    assert False, "Executed a"
+
+def validator(x: None) -> None:
+    b = a
+    if True:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    def test_zero_ary_method(self):
+        source_code = """
+def validator(x: None) -> None:
+    b = b"\\xFF".decode
+    if False:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
+
+    @unittest.expectedFailure
+    def test_zero_ary_method_exec(self):
+        source_code = """
+def validator(x: None) -> None:
+    b = b"\\xFF".decode
+    if True:
+        b()
+"""
+        ast = compiler.parse(source_code)
+        code = compiler.compile(ast).compile()
+        res = uplc_eval(uplc.Apply(code, uplc.PlutusInteger(0)))
```

### Comparing `opshin-0.9.14/opshin/tests/test_ops.py` & `opshin-0.9.15/opshin/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/tests/test_stdlib.py` & `opshin-0.9.15/opshin/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/type_inference.py` & `opshin-0.9.15/opshin/type_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,19 +503,19 @@
             )
         if isinstance(tc.func.typ, InstanceType) and isinstance(
             tc.func.typ.typ, FunctionType
         ):
             functyp = tc.func.typ.typ
             assert len(tc.args) == len(
                 functyp.argtyps
-            ), f"Signature of function {ast.dump(node)} does not match number of arguments"
+            ), f"Signature of function does not match number of arguments. Expected {len(functyp.argtyps)} arguments with these types: {functyp.argtyps}"
             # all arguments need to be supertypes of the given type
             assert all(
                 ap >= a.typ for a, ap in zip(tc.args, functyp.argtyps)
-            ), f"Signature of function {ast.dump(node)} does not match arguments"
+            ), f"Signature of function does not match arguments. Expected {len(functyp.argtyps)} arguments with these types: {functyp.argtyps}"
             tc.typ = functyp.rettyp
             return tc
         raise TypeInferenceError("Could not infer type of call")
 
     def visit_Pass(self, node: Pass) -> TypedPass:
         tp = copy(node)
         return tp
```

### Comparing `opshin-0.9.14/opshin/typed_ast.py` & `opshin-0.9.15/opshin/typed_ast.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/opshin/util.py` & `opshin-0.9.15/opshin/util.py`

 * *Files identical despite different names*

### Comparing `opshin-0.9.14/pyproject.toml` & `opshin-0.9.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opshin"
-version = "0.9.14"
+version = "0.9.15"
 description = "A simple pythonic programming language for Smart Contracts on Cardano"
 authors = ["nielstron <n.muendler@web.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/opshin/opshin"
 documentation = "https://opshin.opshin.dev/"
 keywords = ["python", "language", "programming-language", "compiler", "validator", "smart-contracts", "cardano"]
```

### Comparing `opshin-0.9.14/PKG-INFO` & `opshin-0.9.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opshin
-Version: 0.9.14
+Version: 0.9.15
 Summary: A simple pythonic programming language for Smart Contracts on Cardano
 Home-page: https://github.com/opshin/opshin
 License: MIT
 Keywords: python,language,programming-language,compiler,validator,smart-contracts,cardano
 Author: nielstron
 Author-email: n.muendler@web.de
 Requires-Python: >=3.8,<3.9
```

