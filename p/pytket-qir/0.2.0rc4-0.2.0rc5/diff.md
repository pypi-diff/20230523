# Comparing `tmp/pytket_qir-0.2.0rc4-py3-none-any.whl.zip` & `tmp/pytket_qir-0.2.0rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17408 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      882 b- defN 23-May-21 16:36 pytket/qir/__init__.py
--rw-rw-rw-  2.0 fat       71 b- defN 23-May-21 16:37 pytket/qir/_metadata.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-May-21 16:36 pytket/qir/conversion/__init__.py
--rw-rw-rw-  2.0 fat     1946 b- defN 23-May-21 16:36 pytket/qir/conversion/api.py
--rw-rw-rw-  2.0 fat    28077 b- defN 23-May-21 16:36 pytket/qir/conversion/conversion.py
--rw-rw-rw-  2.0 fat     4237 b- defN 23-May-21 16:36 pytket/qir/conversion/gatesets.py
--rw-rw-rw-  2.0 fat     1529 b- defN 23-May-21 16:36 pytket/qir/conversion/module.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-21 16:37 pytket_qir-0.2.0rc4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4296 b- defN 23-May-21 16:37 pytket_qir-0.2.0rc4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-21 16:37 pytket_qir-0.2.0rc4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-21 16:37 pytket_qir-0.2.0rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1017 b- defN 23-May-21 16:37 pytket_qir-0.2.0rc4.dist-info/RECORD
-12 files, 54445 bytes uncompressed, 15686 bytes compressed:  71.2%
+Zip file size: 17629 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      862 b- defN 23-May-23 13:48 pytket/qir/__init__.py
+-rw-r--r--  2.0 unx       69 b- defN 23-May-23 13:48 pytket/qir/_metadata.py
+-rw-r--r--  2.0 unx      715 b- defN 23-May-23 13:48 pytket/qir/conversion/__init__.py
+-rw-r--r--  2.0 unx     2519 b- defN 23-May-23 13:48 pytket/qir/conversion/api.py
+-rw-r--r--  2.0 unx    27522 b- defN 23-May-23 13:48 pytket/qir/conversion/conversion.py
+-rw-r--r--  2.0 unx     4082 b- defN 23-May-23 13:48 pytket/qir/conversion/gatesets.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-May-23 13:48 pytket/qir/conversion/module.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-23 13:48 pytket_qir-0.2.0rc5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4183 b- defN 23-May-23 13:48 pytket_qir-0.2.0rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 13:48 pytket_qir-0.2.0rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-23 13:48 pytket_qir-0.2.0rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1017 b- defN 23-May-23 13:48 pytket_qir-0.2.0rc5.dist-info/RECORD
+12 files, 53906 bytes uncompressed, 15907 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pytket/qir/conversion/gatesets.py
 Comment: 
 
 Filename: pytket/qir/conversion/module.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc4.dist-info/LICENSE
+Filename: pytket_qir-0.2.0rc5.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qir-0.2.0rc4.dist-info/METADATA
+Filename: pytket_qir-0.2.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qir-0.2.0rc4.dist-info/WHEEL
+Filename: pytket_qir-0.2.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_qir-0.2.0rc4.dist-info/top_level.txt
+Filename: pytket_qir-0.2.0rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_qir-0.2.0rc4.dist-info/RECORD
+Filename: pytket_qir-0.2.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/qir/__init__.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Backends for processing pytket circuits with Quantinuum devices
-"""
-
-# _metadata.py is copied to the folder after installation.
-from ._metadata import __extension_version__, __extension_name__  # type: ignore
-from .conversion import pytket_to_qir, ReturnTypeQIR
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Backends for processing pytket circuits with Quantinuum devices
+"""
+
+# _metadata.py is copied to the folder after installation.
+from ._metadata import __extension_version__, __extension_name__  # type: ignore
+from .conversion import pytket_to_qir, ReturnTypeQIR
```

## pytket/qir/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.2.0rc4"
-__extension_name__ = "pytket-qir"
+__extension_version__ = "0.2.0rc5"
+__extension_name__ = "pytket-qir"
```

## pytket/qir/conversion/__init__.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""Backends for processing pytket circuits with Quantinuum devices
-"""
-
-from .api import pytket_to_qir, ReturnTypeQIR
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""Backends for processing pytket circuits with Quantinuum devices
+"""
+
+from .api import pytket_to_qir, ReturnTypeQIR
```

## pytket/qir/conversion/api.py

```diff
@@ -1,66 +1,85 @@
-# Copyright 2020-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""
-public api for qir conversion from pytket
-"""
-
-from enum import Enum
-from typing import Union
-
-from pytket.circuit import Circuit
-
-from .conversion import QirGenerator
-from .module import tketqirModule
-
-
-class ReturnTypeQIR(Enum):
-    BINARY = 0
-    STRING = 1
-
-
-def pytket_to_qir(
-    circ: Circuit,
-    name: str = "Generated from input pytket circuit",
-    returntype: ReturnTypeQIR = ReturnTypeQIR.BINARY,
-) -> Union[str, bytes, None]:
-    """converts give pytket circuit to qir
-    :param name: name for the qir module created
-    :type name: str
-    :param returntype: format of the generated qir, defaut value is binary
-    :type returntype: ReturnTypeQIR
-    """
-
-    m = tketqirModule(
-        name=name,
-        num_qubits=circ.n_qubits,
-        num_results=circ.n_qubits,
-    )
-
-    qir_generator = QirGenerator(
-        circuit=circ,
-        module=m,
-        wasm_int_type=32,
-        qir_int_type=64,
-    )
-
-    populated_module = qir_generator.circuit_to_module(
-        qir_generator.circuit, qir_generator.module, True
-    )
-    if returntype == ReturnTypeQIR.BINARY:
-        return populated_module.module.bitcode()
-    elif returntype == ReturnTypeQIR.STRING:
-        return populated_module.module.ir()
-    else:
-        ValueError("unsupported return type")
+# Copyright 2020-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""
+public api for qir conversion from pytket
+"""
+
+from enum import Enum
+from typing import Union
+
+from pytket.circuit import Circuit
+
+from .conversion import QirGenerator
+from .module import tketqirModule
+
+
+class ReturnTypeQIR(Enum):
+    """Return types qir, options are BINARY for a binary
+    output and STRING for a string output
+    """
+
+    BINARY = 0
+    STRING = 1
+
+
+def pytket_to_qir(
+    circ: Circuit,
+    name: str = "Generated from input pytket circuit",
+    returntype: ReturnTypeQIR = ReturnTypeQIR.BINARY,
+) -> Union[str, bytes, None]:
+    """converts given pytket circuit to qir
+    :param circ: given circuit
+    :type circ: pytket circuit
+    :param name: name for the qir module created
+    :type name: str
+    :param returntype: format of the generated qir, defaut value is binary
+    :type returntype: ReturnTypeQIR
+    """
+
+    if len(circ.q_registers) > 1:
+        raise ValueError(
+            """The circuit that should be converted should only have one
+            quantum register, you can convert it with using the pytket
+              compilerpass `FlattenRelabelRegistersPass`"""
+        )
+
+    for creg in circ.c_registers:
+        if creg.size > 64:
+            raise ValueError(
+                "each of the classical register must not have more than 64 bits"
+            )
+
+    m = tketqirModule(
+        name=name,
+        num_qubits=circ.n_qubits,
+        num_results=circ.n_qubits,
+    )
+
+    qir_generator = QirGenerator(
+        circuit=circ,
+        module=m,
+        wasm_int_type=32,
+        qir_int_type=64,
+    )
+
+    populated_module = qir_generator.circuit_to_module(
+        qir_generator.circuit, qir_generator.module, True
+    )
+    if returntype == ReturnTypeQIR.BINARY:
+        return populated_module.module.bitcode()
+    elif returntype == ReturnTypeQIR.STRING:
+        return populated_module.module.ir()
+    else:
+        raise ValueError("unsupported return type")
```

## pytket/qir/conversion/conversion.py

```diff
@@ -1,714 +1,724 @@
-# Copyright 2019-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""
-This module contains all functionality to generate QIR files
-from pytket circuits.
-"""
-
-from functools import partial
-from typing import cast, Dict, List, Optional, Sequence, Tuple, Union
-
-from pyqir import Value, IntPredicate
-import pyqir
-
-from pytket import Circuit, OpType, Bit, Qubit  # type: ignore
-from pytket.qasm.qasm import _retrieve_registers  # type: ignore
-from pytket.circuit import (  # type: ignore
-    BitRegister,
-    ClassicalExpBox,
-    Command,
-    Conditional,
-    RangePredicateOp,
-    CopyBitsOp,
-    Op,
-    MetaOp,
-    SetBitsOp,
-    WASMOp,
-    OpType,
-)
-
-from pytket.circuit.logic_exp import (  # type: ignore
-    BitWiseOp,
-    RegAdd,
-    RegAnd,
-    RegEq,
-    RegGeq,
-    RegGt,
-    RegLeq,
-    RegLt,
-    RegNeq,
-    RegSub,
-    RegMul,
-    RegOr,
-    RegLsh,
-    RegRsh,
-    RegXor,
-    BitOr,
-    BitXor,
-    BitNeq,
-    BitEq,
-    BitAnd,
-)
-
-from pytket.passes import auto_rebase_pass  # type: ignore
-
-from .gatesets import (
-    FuncSpec,
-)
-
-from .module import tketqirModule
-
-
-_TK_CLOPS_TO_PYQIR_REG: Dict = {
-    RegAnd: lambda b: b.and_,
-    RegOr: lambda b: b.or_,
-    RegXor: lambda b: b.xor,
-    RegAdd: lambda b: b.add,
-    RegSub: lambda b: b.sub,
-    RegMul: lambda b: b.mul,
-    RegLsh: lambda b: b.shl,
-    RegRsh: lambda b: b.lshr,
-}
-
-_TK_CLOPS_TO_PYQIR_REG_BOOL: Dict = {
-    RegEq: lambda b: partial(b.icmp, IntPredicate.EQ),
-    RegNeq: lambda b: partial(b.icmp, IntPredicate.NE),
-    RegGt: lambda b: partial(b.icmp, IntPredicate.UGT),
-    RegGeq: lambda b: partial(b.icmp, IntPredicate.UGE),
-    RegLt: lambda b: partial(b.icmp, IntPredicate.ULT),
-    RegLeq: lambda b: partial(b.icmp, IntPredicate.ULE),
-}
-
-_TK_CLOPS_TO_PYQIR_BIT: Dict = {
-    BitAnd: lambda b: b.and_,
-    BitOr: lambda b: b.or_,
-    BitXor: lambda b: b.xor,
-    BitNeq: lambda b: partial(b.icmp, IntPredicate.NE),
-    BitEq: lambda b: partial(b.icmp, IntPredicate.EQ),
-}
-
-
-class QirGenerator:
-    """Generate QIR from a pytket circuit."""
-
-    def __init__(
-        self,
-        circuit: Circuit,
-        module: tketqirModule,
-        wasm_int_type: int,
-        qir_int_type: int,
-    ) -> None:
-        self.circuit = circuit
-        self.module = module
-        self.wasm_int_type = pyqir.IntType(self.module.context, wasm_int_type)
-        self.qir_int_type = pyqir.IntType(self.module.context, qir_int_type)
-        self.qubit_type = pyqir.qubit_type(self.module.context)
-        self.result_type = pyqir.result_type(self.module.context)
-
-        self.cregs = _retrieve_registers(self.circuit.bits, BitRegister)
-        self.target_gateset = self.module.gateset.base_gateset
-
-        # Will throw an exception if the rebase can not handle the target gateset.
-        self.rebase_to_gateset = auto_rebase_pass(self.target_gateset)
-
-        self.set_cregs: Dict[str, List] = {}  # Keep track of set registers.
-        self.ssa_vars: Dict[str, Value] = {}  # Keep track of set ssa variables.
-
-        # i1 read_bit_from_reg(i64 reg, i64 index)
-        self.read_bit_from_reg = self.module.module.add_external_function(
-            "read_bit_from_reg",
-            pyqir.FunctionType(
-                pyqir.IntType(self.module.module.context, 1),
-                [self.qir_int_type] * 2,
-            ),
-        )
-
-        # void set_one_bit_in_reg(i64 reg, i64 index, i1 value)
-        self.set_one_bit_in_reg = self.module.module.add_external_function(
-            "set_one_bit_in_reg",
-            pyqir.FunctionType(
-                pyqir.Type.void(self.module.module.context),
-                [
-                    self.qir_int_type,
-                    self.qir_int_type,
-                    pyqir.IntType(self.module.module.context, 1),
-                ],
-            ),
-        )
-
-        # void set_all_bits_in_reg(i64 reg, i64 value)
-        self.set_all_bits_in_reg = self.module.module.add_external_function(
-            "set_all_bits_in_reg",
-            pyqir.FunctionType(
-                pyqir.Type.void(self.module.module.context),
-                [
-                    self.qir_int_type,
-                    self.qir_int_type,
-                ],
-            ),
-        )
-
-        # __quantum__qis__read_result__body(result)
-        self.read_bit_from_result = self.module.module.add_external_function(
-            "__quantum__qis__read_result__body",
-            pyqir.FunctionType(
-                pyqir.IntType(self.module.module.context, 1),
-                [pyqir.result_type(self.module.module.context)],
-            ),
-        )
-
-        # i64 reg2var(i1, i1, i1, ...)
-        self.reg2var = self.module.module.add_external_function(
-            "reg2var",
-            pyqir.FunctionType(
-                pyqir.IntType(self.module.module.context, qir_int_type),
-                [pyqir.IntType(self.module.module.context, 1)] * qir_int_type,
-            ),
-        )
-
-        # void __quantum__rt__int_record_output(i64)
-        self.record_output = self.module.module.add_external_function(
-            "__quantum__rt__int_record_output",
-            pyqir.FunctionType(
-                pyqir.Type.void(self.module.module.context),
-                [pyqir.IntType(self.module.module.context, qir_int_type)],
-            ),
-        )
-
-        self.barrier: List[Optional[pyqir.Function]] = [None]
-        self.order: List[Optional[pyqir.Function]] = [None]
-        self.group: List[Optional[pyqir.Function]] = [None]
-        self.sleep: List[Optional[pyqir.Function]] = [None]
-
-        # __quantum__qis__barrier1__body()
-        for i in range(1, self.circuit.n_qubits):
-            funcnameb = f"__quantum__qis__barrier{i}__body"
-            funcnameo = f"__quantum__qis__order{i}__body"
-            funcnameg = f"__quantum__qis__group{i}__body"
-            funcnames = f"__quantum__qis__sleep{i}__body"
-
-            self.barrier.append(
-                self.module.module.add_external_function(
-                    funcnameb,
-                    pyqir.FunctionType(
-                        pyqir.Type.void(self.module.module.context),
-                        [pyqir.qubit_type(self.module.module.context)] * i,
-                    ),
-                )
-            )
-
-            self.order.append(
-                self.module.module.add_external_function(
-                    funcnameo,
-                    pyqir.FunctionType(
-                        pyqir.Type.void(self.module.module.context),
-                        [pyqir.qubit_type(self.module.module.context)] * i,
-                    ),
-                )
-            )
-
-            self.group.append(
-                self.module.module.add_external_function(
-                    funcnameg,
-                    pyqir.FunctionType(
-                        pyqir.Type.void(self.module.module.context),
-                        [pyqir.qubit_type(self.module.module.context)] * i,
-                    ),
-                )
-            )
-
-            self.sleep.append(
-                self.module.module.add_external_function(
-                    funcnames,
-                    pyqir.FunctionType(
-                        pyqir.Type.void(self.module.module.context),
-                        [pyqir.qubit_type(self.module.module.context)] * i,
-                    ),
-                )
-            )
-
-        for creg in self.circuit.c_registers:
-            self._reg2ssa_var(creg, qir_int_type)
-
-    def _rebase_command_to_gateset(self, command: Command) -> Optional[Circuit]:
-        """Rebase to the target gateset if needed."""
-        optype = command.op.type
-        params = command.op.params
-        args = command.args
-        if optype not in self.module.gateset.base_gateset:
-            circuit = Circuit(self.circuit.n_qubits, self.circuit.n_bits)
-            circuit.add_gate(optype, params, args)
-            self.rebase_to_gateset.apply(circuit)
-            return circuit
-        return None
-
-    def _rebase_op_to_gateset(self, op: OpType, args: List) -> Optional[Circuit]:
-        """Rebase an op to the target gateset if needed."""
-        optype = op.type
-        if op.type == OpType.ClassicalExpBox:
-            circuit = Circuit(self.circuit.n_qubits)
-            for cr in self.circuit.c_registers:
-                circuit.add_c_register(cr.name, cr.size)
-
-            circuit.add_gate(op, args)
-            return circuit
-        else:
-            params = op.params
-            circuit = Circuit(self.circuit.n_qubits, self.circuit.n_bits)
-            circuit.add_gate(optype, params, args)
-            self.rebase_to_gateset.apply(circuit)
-            return circuit
-
-    def _get_optype_and_params(self, op: Op) -> Tuple[OpType, Sequence[float]]:
-        optype = op.type
-        params: List = []
-        if optype == OpType.ExplicitPredicate:
-            if op.get_name() == "AND":
-                optype = BitWiseOp.AND
-            elif op.get_name() == "OR":
-                optype = BitWiseOp.OR
-            elif op.get_name() == "XOR":
-                optype = BitWiseOp.XOR
-        elif optype in [OpType.Barrier, OpType.CopyBits]:
-            pass
-        else:
-            params = op.params
-        return (optype, params)
-
-    def _to_qis_qubits(self, qubits: List[Qubit]) -> Sequence[Qubit]:
-        return [self.module.module.qubits[qubit.index[0]] for qubit in qubits]
-
-    def _to_qis_results(self, bits: List[Bit]) -> Optional[Value]:
-        if bits:
-            return self.module.module.results[bits[0].index[0]]  # type: ignore
-        return None
-
-    def _to_qis_bits(self, args: List[Bit]) -> Sequence[Value]:
-        for b in args:
-            assert b.name == "c"
-        if args:
-            return [self.module.module.results[bit.index[0]] for bit in args[:-1]]
-        return []
-
-    def _reg2ssa_var(self, bit_reg: BitRegister, int_size: int) -> Value:
-        """Convert a BitRegister to an SSA variable using pyqir types."""
-        reg_name = bit_reg[0].reg_name
-        if (
-            reg_name not in self.ssa_vars.keys()
-        ):  # Check if the register has been previously set.
-            # Check if the register has been previously set. If not, initialise to 0.
-            if reg_value := self.set_cregs.get(reg_name):
-                bit_reg = reg_value
-                value = sum([n * 2**k for k, n in enumerate(reg_value)])
-                return pyqir.const(self.qir_int_type, value)
-            else:
-                bit_reg = [False] * len(bit_reg)
-            if (size := len(bit_reg)) <= int_size:  # Widening by zero-padding.
-                bool_reg = bit_reg + [False] * (int_size - size)
-            else:  # Narrowing by truncation.
-                bool_reg = bit_reg[:int_size]
-            ssa_var = cast(Value, self.module.builder.call(self.reg2var, [*bool_reg]))  # type: ignore
-            self.ssa_vars[reg_name] = ssa_var
-            # reg_name = bit_reg[0].reg_name
-            return ssa_var
-        else:
-            return cast(Value, self.ssa_vars[reg_name])  # type: ignore
-
-    def _get_c_regs_from_com(self, command: Command) -> Tuple[List[str], List[str]]:
-        """Get classical registers from command op types."""
-        op = command.op
-        args = command.args
-        inputs: List[str] = []
-        outputs: List[str] = []
-
-        if isinstance(op, WASMOp):
-            for reglist, sizes in [
-                (inputs, op.input_widths),
-                (outputs, op.output_widths),
-            ]:
-                for in_width in sizes:
-                    assert in_width > 0
-                    com_bits = args[:in_width]
-                    args = args[in_width:]
-                    regname = com_bits[0].reg_name
-                    if com_bits != list(self.cregs[regname]):
-                        raise ValueError("WASM ops must act on entire registers.")
-                    reglist.append(regname)
-        elif isinstance(op, ClassicalExpBox):
-            # remove this
-            for reglist, sizes in [
-                (
-                    inputs,
-                    list(
-                        map(
-                            lambda obj: obj.size  # type: ignore
-                            if isinstance(obj, BitRegister)
-                            else None,
-                            op.get_exp().args,
-                        )
-                    ),
-                ),
-                (outputs, [op.get_n_o()]),
-            ]:
-                for in_width in sizes:
-                    if in_width == 0:
-                        raise ValueError(
-                            "ClassicalExpBox op input or output \
-                            registers have empty widths."
-                        )
-                    com_bits = args[:in_width]
-                    args = args[in_width:]
-                    regname = com_bits[0].reg_name
-                    if com_bits != list(self.cregs[regname]):
-                        raise ValueError(
-                            "ClassicalExpBox ops must act on entire registers."
-                        )
-                    reglist.append(regname)
-        elif isinstance(op, SetBitsOp):
-            for reglist, sizes in [
-                (outputs, [op.n_outputs]),
-            ]:
-                for in_width in sizes:
-                    if in_width == 0:
-                        raise ValueError(
-                            "A value is getting assigned to an empty register."
-                        )
-                    com_bits = args[:in_width]
-                    args = args[in_width:]
-                    regname = com_bits[0].reg_name
-                    if com_bits != list(self.cregs[regname]):
-                        raise ValueError("SetBitOp must act on entire registers.")
-                    reglist.append(regname)
-        return inputs, outputs
-
-    def _get_ssa_from_cl_reg_op(
-        self, reg: Union[BitRegister, RegAnd, RegOr, RegXor], module: tketqirModule
-    ) -> Value:
-
-        if type(reg) in _TK_CLOPS_TO_PYQIR_REG:
-            assert len(reg.args) == 2
-
-            ssa_left = self._get_ssa_from_cl_reg_op(reg.args[0], module)
-            ssa_right = self._get_ssa_from_cl_reg_op(reg.args[1], module)
-
-            # add function to module
-            output_instruction = _TK_CLOPS_TO_PYQIR_REG[type(reg)](module.builder)(
-                ssa_left, ssa_right
-            )
-            return output_instruction  # type: ignore
-        elif type(reg) == BitRegister:
-            return self.ssa_vars[reg.name]
-        else:
-            raise ValueError("unsupported classical register operaton")
-
-    def _get_ssa_from_cl_bit_op(
-        self, bit: Union[Bit, BitAnd, BitOr, BitXor], module: tketqirModule
-    ) -> Value:
-
-        if type(bit) == Bit:
-
-            result = module.builder.call(
-                self.read_bit_from_reg,
-                [
-                    self.ssa_vars[bit.reg_name],
-                    pyqir.const(self.qir_int_type, bit.index[0]),
-                ],
-            )
-
-            return result
-        elif type(bit) in _TK_CLOPS_TO_PYQIR_BIT:
-
-            assert len(bit.args) == 2
-
-            ssa_left = self._get_ssa_from_cl_bit_op(bit.args[0], module)
-            ssa_right = self._get_ssa_from_cl_bit_op(bit.args[1], module)
-
-            # add function to module
-            output_instruction = _TK_CLOPS_TO_PYQIR_BIT[type(bit)](module.builder)(
-                ssa_left, ssa_right
-            )
-
-            return output_instruction  # type: ignore
-        else:
-            raise ValueError("unsupported bisewise operation")
-
-    def circuit_to_module(
-        self, circuit: Circuit, module: tketqirModule, record_output: bool = False
-    ) -> tketqirModule:
-        """Populate a PyQir module from a pytket circuit."""
-
-        for command in circuit:
-            op = command.op
-
-            if isinstance(op, RangePredicateOp):
-                lower_qir = pyqir.const(self.qir_int_type, op.lower)
-                upper_qir = pyqir.const(self.qir_int_type, op.upper)
-
-                registername = command.args[0].reg_name
-
-                lower_cond = module.module.builder.icmp(
-                    pyqir.IntPredicate.SGT, lower_qir, self.ssa_vars[registername]
-                )
-                upper_cond = module.module.builder.icmp(
-                    pyqir.IntPredicate.SGT, self.ssa_vars[registername], upper_qir
-                )
-
-                result = module.module.builder.and_(lower_cond, upper_cond)
-
-                condition_bit_index = command.args[-1].index[0]
-                registername = command.args[-1].reg_name
-
-                self.module.builder.call(
-                    self.set_one_bit_in_reg,
-                    [
-                        self.ssa_vars[registername],
-                        pyqir.const(self.qir_int_type, condition_bit_index),
-                        result,
-                    ],
-                )
-
-            elif isinstance(op, Conditional):
-                assert op.width == 1  # only one conditional bit
-                conditional_circuit = self._rebase_op_to_gateset(
-                    op.op, command.args[op.width :]
-                )
-                condition_bit_index = command.args[0].index[0]
-                condition_name = command.args[0].reg_name
-
-                def condition_block_true() -> None:
-                    """
-                    Populate recursively the module with the contents of the conditional
-                    sub-circuit when the condition is True.
-                    """
-                    if op.value == 1:
-                        self.circuit_to_module(conditional_circuit, module)
-
-                def condition_block_false() -> None:
-                    """
-                    Populate recursively the module with the contents of the conditional
-                    sub-circuit when the condition is False.
-                    """
-                    if op.value == 0:
-                        self.circuit_to_module(conditional_circuit, module)
-
-                if condition_name in self.ssa_vars:
-
-                    ssabool = module.builder.call(
-                        self.read_bit_from_reg,
-                        [
-                            self.ssa_vars[condition_name],
-                            pyqir.const(self.qir_int_type, condition_bit_index),
-                        ],
-                    )
-
-                    module.module.builder.if_(
-                        ssabool,
-                        true=lambda: condition_block_true(),  # type: ignore
-                        false=lambda: condition_block_false(),  # type: ignore
-                    )
-
-                else:
-                    ValueError(
-                        "circuit contruction with special condition not yet supported"
-                    )
-                    # this should be an assertion when working
-
-            elif isinstance(op, WASMOp):
-                raise ValueError("WASM not supported yet")
-            elif op.type == OpType.Measure:
-
-                assert len(command.bits) == 1
-                assert len(command.qubits) == 1
-                assert command.qubits[0].reg_name == "q"
-
-                module.qis.mz(
-                    module.module.qubits[command.qubits[0].index[0]],
-                    module.module.results[command.qubits[0].index[0]],
-                )
-
-                ssa_measureresult = self.module.builder.call(
-                    self.read_bit_from_result,
-                    [
-                        module.module.results[command.qubits[0].index[0]],
-                    ],
-                )
-
-                self.module.builder.call(
-                    self.set_one_bit_in_reg,
-                    [
-                        self.ssa_vars[command.bits[0].reg_name],
-                        pyqir.const(self.qir_int_type, command.bits[0].index[0]),
-                        ssa_measureresult,
-                    ],
-                )
-
-            elif isinstance(op, ClassicalExpBox):
-
-                returntypebool = False
-                result_index = 0
-                outputs = command.args[-1].reg_name
-                ssa_left = self.ssa_vars[list(self.ssa_vars)[0]]  # set default value
-                ssa_right = self.ssa_vars[list(self.ssa_vars)[0]]  # set default value
-
-                if type(op.get_exp()) in _TK_CLOPS_TO_PYQIR_REG:
-                    # do something with register things
-                    ssa_left = self._get_ssa_from_cl_reg_op(
-                        op.get_exp().args[0], module
-                    )
-                    ssa_right = self._get_ssa_from_cl_reg_op(
-                        op.get_exp().args[1], module
-                    )
-
-                    # add function to module
-                    output_instruction = _TK_CLOPS_TO_PYQIR_REG[type(op.get_exp())](
-                        module.builder
-                    )(ssa_left, ssa_right)
-
-                elif type(op.get_exp()) in _TK_CLOPS_TO_PYQIR_BIT:
-                    ssa_left = self._get_ssa_from_cl_bit_op(
-                        op.get_exp().args[0], module
-                    )
-                    ssa_right = self._get_ssa_from_cl_bit_op(
-                        op.get_exp().args[1], module
-                    )
-
-                    # add function to module
-                    returntypebool = True
-                    result_index = command.args[-1].index[0]  # todo
-                    output_instruction = _TK_CLOPS_TO_PYQIR_BIT[type(op.get_exp())](
-                        module.builder
-                    )(ssa_left, ssa_right)
-
-                elif type(op.get_exp()) in _TK_CLOPS_TO_PYQIR_REG_BOOL:
-                    ssa_left = self._get_ssa_from_cl_reg_op(
-                        op.get_exp().args[0], module
-                    )
-                    ssa_right = self._get_ssa_from_cl_reg_op(
-                        op.get_exp().args[1], module
-                    )
-
-                    # add function to module
-                    returntypebool = True
-                    output_instruction = _TK_CLOPS_TO_PYQIR_REG_BOOL[
-                        type(op.get_exp())
-                    ](module.builder)(ssa_left, ssa_right)
-
-                else:
-                    raise ValueError(" unexpected classical op")
-
-                if returntypebool:
-                    # the return value of the some classical ops is bool in qir,
-                    # so the return value can only be written to one entry
-                    # of the register this implementation write the value
-                    # to the 0-th entry
-                    # of the register, this could be changed to a user given value
-
-                    self.module.builder.call(
-                        self.set_one_bit_in_reg,
-                        [
-                            self.ssa_vars[outputs],
-                            pyqir.const(self.qir_int_type, result_index),
-                            output_instruction,
-                        ],
-                    )
-                else:
-                    self.module.builder.call(
-                        self.set_all_bits_in_reg,
-                        [self.ssa_vars[outputs], output_instruction],
-                    )
-
-            elif isinstance(op, SetBitsOp):
-                _, outputs = self._get_c_regs_from_com(command)
-                for out in outputs:
-                    self.set_cregs[out] = command.op.values
-            elif isinstance(op, MetaOp):
-
-                assert command.qubits[0].reg_name == "q"
-
-                qir_qubits = self._to_qis_qubits(command.qubits)
-
-                if command.op.data == "":
-                    self.module.builder.call(
-                        self.barrier[len(command.qubits)],  # type: ignore
-                        [*qir_qubits],
-                    )
-                elif command.op.data[0:5] == "order":
-                    self.module.builder.call(
-                        self.order[len(command.qubits)],  # type: ignore
-                        [*qir_qubits],
-                    )
-                elif command.op.data[0:5] == "group":
-                    self.module.builder.call(
-                        self.group[len(command.qubits)],  # type: ignore
-                        [*qir_qubits],
-                    )
-                elif command.op.data[0:5] == "sleep":
-                    self.module.builder.call(
-                        self.sleep[len(command.qubits)],  # type: ignore
-                        [*qir_qubits],
-                    )
-                else:
-                    raise ValueError("Meta op is not supported yet")
-
-            elif isinstance(op, CopyBitsOp):
-                input_reg = command.args[0]
-                output_reg = command.args[1]
-                output_name = output_reg.reg_name
-                optype, _ = self._get_optype_and_params(op)
-                gate = module.gateset.tk_to_gateset(optype)
-                ssa_var = cast(Value, self.module.module.results[input_reg.index[0]])
-                get_gate = getattr(module, gate.func_name.value)
-                output_instr = module.builder.call(get_gate, [ssa_var])
-                ssa_var_result = output_instr
-                self.set_all_bits_in_reg(self.ssa_vars[output_name], ssa_var_result)  # type: ignore
-
-            else:
-                rebased_circ = self._rebase_command_to_gateset(
-                    command
-                )  # Check if the command must be rebased.
-                if rebased_circ is not None:
-                    self.circuit_to_module(rebased_circ, module)
-                else:
-                    optype, params = self._get_optype_and_params(op)
-                    qubits = self._to_qis_qubits(command.qubits)
-                    results = self._to_qis_results(command.bits)
-                    bits: Optional[Sequence[Value]] = None
-                    if type(optype) == BitWiseOp:
-                        bits = self._to_qis_bits(command.args)
-                    gate = module.gateset.tk_to_gateset(optype)
-                    if not gate.func_spec == FuncSpec.BODY:
-                        func_name = gate.func_name.value + "_" + gate.func_spec.value
-                        get_gate = getattr(module.qis, func_name)
-                    else:
-                        get_gate = getattr(module.qis, gate.func_name.value)
-                    if bits:
-                        get_gate(*bits)
-                    elif params:
-                        get_gate(*params, *qubits)
-                    elif results:
-                        get_gate(*qubits, results)
-                    else:
-                        get_gate(*qubits)
-        if record_output:
-            for creg in self.circuit.c_registers:
-                reg_name = creg[0].reg_name
-                self.module.builder.call(
-                    self.record_output,
-                    [
-                        self.ssa_vars[reg_name],
-                    ],
-                )
-
-        return module
+# Copyright 2019-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""
+This module contains all functionality to generate QIR files
+from pytket circuits.
+"""
+
+from functools import partial
+from typing import cast, Dict, List, Optional, Sequence, Tuple, Union
+
+from pyqir import Value, IntPredicate
+import pyqir
+
+from pytket import Circuit, OpType, Bit, Qubit  # type: ignore
+from pytket.qasm.qasm import _retrieve_registers  # type: ignore
+from pytket.circuit import (  # type: ignore
+    BitRegister,
+    ClassicalExpBox,
+    Command,
+    Conditional,
+    RangePredicateOp,
+    CopyBitsOp,
+    Op,
+    MetaOp,
+    SetBitsOp,
+    WASMOp,
+    OpType,
+)
+
+from pytket.circuit.logic_exp import (  # type: ignore
+    BitWiseOp,
+    RegAdd,
+    RegAnd,
+    RegEq,
+    RegGeq,
+    RegGt,
+    RegLeq,
+    RegLt,
+    RegNeq,
+    RegSub,
+    RegMul,
+    RegOr,
+    RegLsh,
+    RegRsh,
+    RegXor,
+    BitOr,
+    BitXor,
+    BitNeq,
+    BitEq,
+    BitAnd,
+)
+
+from pytket.passes import auto_rebase_pass  # type: ignore
+
+from .gatesets import (
+    FuncSpec,
+)
+
+from .module import tketqirModule
+
+
+_TK_CLOPS_TO_PYQIR_REG: Dict = {
+    RegAnd: lambda b: b.and_,
+    RegOr: lambda b: b.or_,
+    RegXor: lambda b: b.xor,
+    RegAdd: lambda b: b.add,
+    RegSub: lambda b: b.sub,
+    RegMul: lambda b: b.mul,
+    RegLsh: lambda b: b.shl,
+    RegRsh: lambda b: b.lshr,
+}
+
+_TK_CLOPS_TO_PYQIR_REG_BOOL: Dict = {
+    RegEq: lambda b: partial(b.icmp, IntPredicate.EQ),
+    RegNeq: lambda b: partial(b.icmp, IntPredicate.NE),
+    RegGt: lambda b: partial(b.icmp, IntPredicate.UGT),
+    RegGeq: lambda b: partial(b.icmp, IntPredicate.UGE),
+    RegLt: lambda b: partial(b.icmp, IntPredicate.ULT),
+    RegLeq: lambda b: partial(b.icmp, IntPredicate.ULE),
+}
+
+_TK_CLOPS_TO_PYQIR_BIT: Dict = {
+    BitAnd: lambda b: b.and_,
+    BitOr: lambda b: b.or_,
+    BitXor: lambda b: b.xor,
+    BitNeq: lambda b: partial(b.icmp, IntPredicate.NE),
+    BitEq: lambda b: partial(b.icmp, IntPredicate.EQ),
+}
+
+
+class QirGenerator:
+    """Generate QIR from a pytket circuit."""
+
+    def __init__(
+        self,
+        circuit: Circuit,
+        module: tketqirModule,
+        wasm_int_type: int,
+        qir_int_type: int,
+    ) -> None:
+        self.circuit = circuit
+        self.module = module
+        self.wasm_int_type = pyqir.IntType(self.module.context, wasm_int_type)
+        self.qir_int_type = pyqir.IntType(self.module.context, qir_int_type)
+        self.qubit_type = pyqir.qubit_type(self.module.context)
+        self.result_type = pyqir.result_type(self.module.context)
+
+        self.cregs = _retrieve_registers(self.circuit.bits, BitRegister)
+        self.target_gateset = self.module.gateset.base_gateset
+
+        # Will throw an exception if the rebase can not handle the target gateset.
+        self.rebase_to_gateset = auto_rebase_pass(self.target_gateset)
+
+        self.set_cregs: Dict[str, List] = {}  # Keep track of set registers.
+        self.ssa_vars: Dict[str, Value] = {}  # Keep track of set ssa variables.
+
+        # i1 read_bit_from_reg(i64 reg, i64 index)
+        self.read_bit_from_reg = self.module.module.add_external_function(
+            "read_bit_from_reg",
+            pyqir.FunctionType(
+                pyqir.IntType(self.module.module.context, 1),
+                [self.qir_int_type] * 2,
+            ),
+        )
+
+        # void set_one_bit_in_reg(i64 reg, i64 index, i1 value)
+        self.set_one_bit_in_reg = self.module.module.add_external_function(
+            "set_one_bit_in_reg",
+            pyqir.FunctionType(
+                pyqir.Type.void(self.module.module.context),
+                [
+                    self.qir_int_type,
+                    self.qir_int_type,
+                    pyqir.IntType(self.module.module.context, 1),
+                ],
+            ),
+        )
+
+        # void set_all_bits_in_reg(i64 reg, i64 value)
+        self.set_all_bits_in_reg = self.module.module.add_external_function(
+            "set_all_bits_in_reg",
+            pyqir.FunctionType(
+                pyqir.Type.void(self.module.module.context),
+                [
+                    self.qir_int_type,
+                    self.qir_int_type,
+                ],
+            ),
+        )
+
+        # __quantum__qis__read_result__body(result)
+        self.read_bit_from_result = self.module.module.add_external_function(
+            "__quantum__qis__read_result__body",
+            pyqir.FunctionType(
+                pyqir.IntType(self.module.module.context, 1),
+                [pyqir.result_type(self.module.module.context)],
+            ),
+        )
+
+        # i64 reg2var(i1, i1, i1, ...)
+        self.reg2var = self.module.module.add_external_function(
+            "reg2var",
+            pyqir.FunctionType(
+                pyqir.IntType(self.module.module.context, qir_int_type),
+                [pyqir.IntType(self.module.module.context, 1)] * qir_int_type,
+            ),
+        )
+
+        # void __quantum__rt__int_record_output(i64)
+        self.record_output = self.module.module.add_external_function(
+            "__quantum__rt__int_record_output",
+            pyqir.FunctionType(
+                pyqir.Type.void(self.module.module.context),
+                [pyqir.IntType(self.module.module.context, qir_int_type)],
+            ),
+        )
+
+        self.barrier: List[Optional[pyqir.Function]] = [None] * (
+            self.circuit.n_qubits + 1
+        )
+        self.order: List[Optional[pyqir.Function]] = [None] * (
+            self.circuit.n_qubits + 1
+        )
+        self.group: List[Optional[pyqir.Function]] = [None] * (
+            self.circuit.n_qubits + 1
+        )
+        self.sleep: List[Optional[pyqir.Function]] = [None] * (
+            self.circuit.n_qubits + 1
+        )
+
+        for creg in self.circuit.c_registers:
+            self._reg2ssa_var(creg, qir_int_type)
+
+    def _add_barrier_op(
+        self, module: tketqirModule, index: int, qir_qubits: Sequence
+    ) -> None:
+        # __quantum__qis__barrier1__body()
+        if self.barrier[index] == None:
+            self.barrier[index] = self.module.module.add_external_function(
+                f"__quantum__qis__barrier{index}__body",
+                pyqir.FunctionType(
+                    pyqir.Type.void(self.module.module.context),
+                    [pyqir.qubit_type(self.module.module.context)] * index,
+                ),
+            )
+
+        module.builder.call(
+            self.barrier[index],  # type: ignore
+            [*qir_qubits],
+        )
+
+    def _add_group_op(
+        self, module: tketqirModule, index: int, qir_qubits: Sequence
+    ) -> None:
+        # __quantum__qis__group1__body()
+        if self.group[index] == None:
+            self.group[index] = self.module.module.add_external_function(
+                f"__quantum__qis__group{index}__body",
+                pyqir.FunctionType(
+                    pyqir.Type.void(self.module.module.context),
+                    [pyqir.qubit_type(self.module.module.context)] * index,
+                ),
+            )
+
+        module.builder.call(
+            self.group[index],  # type: ignore
+            [*qir_qubits],
+        )
+
+    def _add_order_op(
+        self, module: tketqirModule, index: int, qir_qubits: Sequence
+    ) -> None:
+        # __quantum__qis__order1__body()
+        if self.order[index] == None:
+            self.order[index] = self.module.module.add_external_function(
+                f"__quantum__qis__order{index}__body",
+                pyqir.FunctionType(
+                    pyqir.Type.void(self.module.module.context),
+                    [pyqir.qubit_type(self.module.module.context)] * index,
+                ),
+            )
+
+        module.builder.call(
+            self.order[index],  # type: ignore
+            [*qir_qubits],
+        )
+
+    def _add_sleep_op(
+        self, module: tketqirModule, index: int, qir_qubits: Sequence, duration: float
+    ) -> None:
+        # __quantum__qis__sleep1__body()
+        if self.sleep[index] == None:
+            paramlist = [pyqir.qubit_type(self.module.module.context)] * index
+            paramlist.append(
+                pyqir.Type.double(self.module.module.context)
+            )  # add float parameter
+            self.sleep[index] = self.module.module.add_external_function(
+                f"__quantum__qis__sleep{index}__body",
+                pyqir.FunctionType(
+                    pyqir.Type.void(self.module.module.context),
+                    paramlist,
+                ),
+            )
+
+        module.builder.call(
+            self.sleep[index],  # type: ignore
+            [
+                *qir_qubits,
+                pyqir.const(pyqir.Type.double(self.module.module.context), duration),
+            ],
+        )
+
+    def _rebase_command_to_gateset(self, command: Command) -> Optional[Circuit]:
+        """Rebase to the target gateset if needed."""
+        optype = command.op.type
+        params = command.op.params
+        args = command.args
+        if optype not in self.module.gateset.base_gateset:
+            circuit = Circuit(self.circuit.n_qubits, self.circuit.n_bits)
+            circuit.add_gate(optype, params, args)
+            self.rebase_to_gateset.apply(circuit)
+            return circuit
+        return None
+
+    def _rebase_op_to_gateset(self, op: OpType, args: List) -> Optional[Circuit]:
+        """Rebase an op to the target gateset if needed."""
+        optype = op.type
+        if op.type == OpType.ClassicalExpBox:
+            circuit = Circuit(self.circuit.n_qubits)
+            for cr in self.circuit.c_registers:
+                circuit.add_c_register(cr.name, cr.size)
+
+            circuit.add_gate(op, args)
+            return circuit
+        else:
+            params = op.params
+            circuit = Circuit(self.circuit.n_qubits, self.circuit.n_bits)
+            circuit.add_gate(optype, params, args)
+            self.rebase_to_gateset.apply(circuit)
+            return circuit
+
+    def _get_optype_and_params(self, op: Op) -> Tuple[OpType, Sequence[float]]:
+        optype = op.type
+        params: List = []
+        if optype == OpType.ExplicitPredicate:
+            if op.get_name() == "AND":
+                optype = BitWiseOp.AND
+            elif op.get_name() == "OR":
+                optype = BitWiseOp.OR
+            elif op.get_name() == "XOR":
+                optype = BitWiseOp.XOR
+        elif optype in [OpType.Barrier, OpType.CopyBits]:
+            pass
+        else:
+            params = op.params
+        return (optype, params)
+
+    def _to_qis_qubits(self, qubits: List[Qubit]) -> Sequence[Qubit]:
+        return [self.module.module.qubits[qubit.index[0]] for qubit in qubits]
+
+    def _to_qis_results(self, bits: List[Bit]) -> Optional[Value]:
+        if bits:
+            return self.module.module.results[bits[0].index[0]]  # type: ignore
+        return None
+
+    def _to_qis_bits(self, args: List[Bit]) -> Sequence[Value]:
+        for b in args:
+            assert b.name == "c"
+        if args:
+            return [self.module.module.results[bit.index[0]] for bit in args[:-1]]
+        return []
+
+    def _reg2ssa_var(self, bit_reg: BitRegister, int_size: int) -> Value:
+        """Convert a BitRegister to an SSA variable using pyqir types."""
+        reg_name = bit_reg[0].reg_name
+        if (
+            reg_name not in self.ssa_vars.keys()
+        ):  # Check if the register has been previously set.
+            # Check if the register has been previously set. If not, initialise to 0.
+            if reg_value := self.set_cregs.get(reg_name):
+                bit_reg = reg_value
+                value = sum([n * 2**k for k, n in enumerate(reg_value)])
+                return pyqir.const(self.qir_int_type, value)
+            else:
+                bit_reg = [False] * len(bit_reg)
+            if (size := len(bit_reg)) <= int_size:  # Widening by zero-padding.
+                bool_reg = bit_reg + [False] * (int_size - size)
+            else:  # Narrowing by truncation.
+                bool_reg = bit_reg[:int_size]
+            ssa_var = cast(Value, self.module.builder.call(self.reg2var, [*bool_reg]))  # type: ignore
+            self.ssa_vars[reg_name] = ssa_var
+            return ssa_var
+        else:
+            return cast(Value, self.ssa_vars[reg_name])  # type: ignore
+
+    def _get_c_regs_from_com(self, command: Command) -> Tuple[List[str], List[str]]:
+        """Get classical registers from command op types."""
+        op = command.op
+        args = command.args
+        inputs: List[str] = []
+        outputs: List[str] = []
+
+        if isinstance(op, WASMOp):
+            for reglist, sizes in [
+                (inputs, op.input_widths),
+                (outputs, op.output_widths),
+            ]:
+                for in_width in sizes:
+                    assert in_width > 0
+                    com_bits = args[:in_width]
+                    args = args[in_width:]
+                    regname = com_bits[0].reg_name
+                    if com_bits != list(self.cregs[regname]):
+                        raise ValueError("WASM ops must act on entire registers.")
+                    reglist.append(regname)
+        elif isinstance(op, SetBitsOp):
+            for reglist, sizes in [
+                (outputs, [op.n_outputs]),
+            ]:
+                for in_width in sizes:
+                    if in_width == 0:
+                        raise ValueError(
+                            "A value is getting assigned to an empty register."
+                        )
+                    com_bits = args[:in_width]
+                    args = args[in_width:]
+                    regname = com_bits[0].reg_name
+                    if com_bits != list(self.cregs[regname]):
+                        raise ValueError("SetBitOp must act on entire registers.")
+                    reglist.append(regname)
+        return inputs, outputs
+
+    def _get_ssa_from_cl_reg_op(
+        self, reg: Union[BitRegister, RegAnd, RegOr, RegXor], module: tketqirModule
+    ) -> Value:
+
+        if type(reg) in _TK_CLOPS_TO_PYQIR_REG:
+            assert len(reg.args) == 2
+
+            ssa_left = self._get_ssa_from_cl_reg_op(reg.args[0], module)
+            ssa_right = self._get_ssa_from_cl_reg_op(reg.args[1], module)
+
+            # add function to module
+            output_instruction = _TK_CLOPS_TO_PYQIR_REG[type(reg)](module.builder)(
+                ssa_left, ssa_right
+            )
+            return output_instruction  # type: ignore
+        elif type(reg) == BitRegister:
+            return self.ssa_vars[reg.name]
+        else:
+            raise ValueError("unsupported classical register operaton")
+
+    def _get_ssa_from_cl_bit_op(
+        self, bit: Union[Bit, BitAnd, BitOr, BitXor], module: tketqirModule
+    ) -> Value:
+
+        if type(bit) == Bit:
+
+            result = module.builder.call(
+                self.read_bit_from_reg,
+                [
+                    self.ssa_vars[bit.reg_name],
+                    pyqir.const(self.qir_int_type, bit.index[0]),
+                ],
+            )
+
+            return result
+        elif type(bit) in _TK_CLOPS_TO_PYQIR_BIT:
+
+            assert len(bit.args) == 2
+
+            ssa_left = self._get_ssa_from_cl_bit_op(bit.args[0], module)
+            ssa_right = self._get_ssa_from_cl_bit_op(bit.args[1], module)
+
+            # add function to module
+            output_instruction = _TK_CLOPS_TO_PYQIR_BIT[type(bit)](module.builder)(
+                ssa_left, ssa_right
+            )
+
+            return output_instruction  # type: ignore
+        else:
+            raise ValueError("unsupported bisewise operation")
+
+    def circuit_to_module(
+        self, circuit: Circuit, module: tketqirModule, record_output: bool = False
+    ) -> tketqirModule:
+        """Populate a PyQir module from a pytket circuit."""
+
+        for command in circuit:
+            op = command.op
+
+            if isinstance(op, RangePredicateOp):
+                lower_qir = pyqir.const(self.qir_int_type, op.lower)
+                upper_qir = pyqir.const(self.qir_int_type, op.upper)
+
+                registername = command.args[0].reg_name
+
+                lower_cond = module.module.builder.icmp(
+                    pyqir.IntPredicate.SGT, lower_qir, self.ssa_vars[registername]
+                )
+                upper_cond = module.module.builder.icmp(
+                    pyqir.IntPredicate.SGT, self.ssa_vars[registername], upper_qir
+                )
+
+                result = module.module.builder.and_(lower_cond, upper_cond)
+
+                condition_bit_index = command.args[-1].index[0]
+                registername = command.args[-1].reg_name
+
+                self.module.builder.call(
+                    self.set_one_bit_in_reg,
+                    [
+                        self.ssa_vars[registername],
+                        pyqir.const(self.qir_int_type, condition_bit_index),
+                        result,
+                    ],
+                )
+
+            elif isinstance(op, Conditional):
+                assert op.width == 1  # only one conditional bit
+                conditional_circuit = self._rebase_op_to_gateset(
+                    op.op, command.args[op.width :]
+                )
+                condition_bit_index = command.args[0].index[0]
+                condition_name = command.args[0].reg_name
+
+                def condition_block_true() -> None:
+                    """
+                    Populate recursively the module with the contents of the conditional
+                    sub-circuit when the condition is True.
+                    """
+                    if op.value == 1:
+                        self.circuit_to_module(conditional_circuit, module)
+
+                def condition_block_false() -> None:
+                    """
+                    Populate recursively the module with the contents of the conditional
+                    sub-circuit when the condition is False.
+                    """
+                    if op.value == 0:
+                        self.circuit_to_module(conditional_circuit, module)
+
+                if condition_name in self.ssa_vars:
+
+                    ssabool = module.builder.call(
+                        self.read_bit_from_reg,
+                        [
+                            self.ssa_vars[condition_name],
+                            pyqir.const(self.qir_int_type, condition_bit_index),
+                        ],
+                    )
+
+                    module.module.builder.if_(
+                        ssabool,
+                        true=lambda: condition_block_true(),  # type: ignore
+                        false=lambda: condition_block_false(),  # type: ignore
+                    )
+
+                else:
+                    ValueError(
+                        "circuit contruction with special condition not yet supported"
+                    )
+                    # this should be an assertion when working
+
+            elif isinstance(op, WASMOp):
+                raise ValueError(
+                    "WASM not supported yet, support expected with pytket-qir==0.3.0"
+                )
+            elif op.type == OpType.Measure:
+
+                assert len(command.bits) == 1
+                assert len(command.qubits) == 1
+                assert command.qubits[0].reg_name == "q"
+
+                module.qis.mz(
+                    module.module.qubits[command.qubits[0].index[0]],
+                    module.module.results[command.qubits[0].index[0]],
+                )
+
+                ssa_measureresult = self.module.builder.call(
+                    self.read_bit_from_result,
+                    [
+                        module.module.results[command.qubits[0].index[0]],
+                    ],
+                )
+
+                self.module.builder.call(
+                    self.set_one_bit_in_reg,
+                    [
+                        self.ssa_vars[command.bits[0].reg_name],
+                        pyqir.const(self.qir_int_type, command.bits[0].index[0]),
+                        ssa_measureresult,
+                    ],
+                )
+
+            elif isinstance(op, ClassicalExpBox):
+
+                returntypebool = False
+                result_index = (
+                    0  # defines the default value for ops that returns bool, see below
+                )
+                outputs = command.args[-1].reg_name
+                ssa_left = self.ssa_vars[list(self.ssa_vars)[0]]  # set default value
+                ssa_right = self.ssa_vars[list(self.ssa_vars)[0]]  # set default value
+
+                #
+
+                if type(op.get_exp()) in _TK_CLOPS_TO_PYQIR_REG:
+                    # classical ops acting on registers returning register
+                    ssa_left = self._get_ssa_from_cl_reg_op(
+                        op.get_exp().args[0], module
+                    )
+                    ssa_right = self._get_ssa_from_cl_reg_op(
+                        op.get_exp().args[1], module
+                    )
+
+                    # add function to module
+                    output_instruction = _TK_CLOPS_TO_PYQIR_REG[type(op.get_exp())](
+                        module.builder
+                    )(ssa_left, ssa_right)
+
+                elif type(op.get_exp()) in _TK_CLOPS_TO_PYQIR_BIT:
+                    # classical ops acting on bits returning bit
+                    ssa_left = self._get_ssa_from_cl_bit_op(
+                        op.get_exp().args[0], module
+                    )
+                    ssa_right = self._get_ssa_from_cl_bit_op(
+                        op.get_exp().args[1], module
+                    )
+
+                    # add function to module
+                    returntypebool = True
+                    result_index = command.args[-1].index[0]  # todo
+                    output_instruction = _TK_CLOPS_TO_PYQIR_BIT[type(op.get_exp())](
+                        module.builder
+                    )(ssa_left, ssa_right)
+
+                elif type(op.get_exp()) in _TK_CLOPS_TO_PYQIR_REG_BOOL:
+                    # classical ops acting on registers returning bit
+                    ssa_left = self._get_ssa_from_cl_reg_op(
+                        op.get_exp().args[0], module
+                    )
+                    ssa_right = self._get_ssa_from_cl_reg_op(
+                        op.get_exp().args[1], module
+                    )
+
+                    # add function to module
+                    returntypebool = True
+                    output_instruction = _TK_CLOPS_TO_PYQIR_REG_BOOL[
+                        type(op.get_exp())
+                    ](module.builder)(ssa_left, ssa_right)
+
+                else:
+                    raise ValueError(" unexpected classical op")
+
+                if returntypebool:
+                    # the return value of the some classical ops is bool in qir,
+                    # so the return value can only be written to one entry
+                    # of the register this implementation write the value
+                    # to the 0-th entry
+                    # of the register, this could be changed to a user given value
+
+                    self.module.builder.call(
+                        self.set_one_bit_in_reg,
+                        [
+                            self.ssa_vars[outputs],
+                            pyqir.const(self.qir_int_type, result_index),
+                            output_instruction,
+                        ],
+                    )
+                else:
+                    self.module.builder.call(
+                        self.set_all_bits_in_reg,
+                        [self.ssa_vars[outputs], output_instruction],
+                    )
+
+            elif isinstance(op, SetBitsOp):
+                _, outputs = self._get_c_regs_from_com(command)
+                for out in outputs:
+                    self.set_cregs[out] = command.op.values
+            elif isinstance(op, MetaOp):
+
+                assert command.qubits[0].reg_name == "q"
+
+                qir_qubits = self._to_qis_qubits(command.qubits)
+
+                if command.op.data == "":
+                    self._add_barrier_op(module, len(command.qubits), qir_qubits)
+                elif command.op.data[0:5] == "order":
+                    self._add_order_op(module, len(command.qubits), qir_qubits)
+                elif command.op.data[0:5] == "group":
+                    self._add_group_op(module, len(command.qubits), qir_qubits)
+                elif command.op.data[0:5] == "sleep":
+                    self._add_sleep_op(
+                        module,
+                        len(command.qubits),
+                        qir_qubits,
+                        float(command.op.data[6:-1]),
+                    )
+                else:
+                    raise ValueError("Meta op is not supported yet")
+
+            elif isinstance(op, CopyBitsOp):
+                input_reg = command.args[0]
+                output_reg = command.args[1]
+                output_name = output_reg.reg_name
+                optype, _ = self._get_optype_and_params(op)
+                gate = module.gateset.tk_to_gateset(optype)
+                ssa_var = cast(Value, self.module.module.results[input_reg.index[0]])
+                get_gate = getattr(module, gate.func_name.value)
+                output_instr = module.builder.call(get_gate, [ssa_var])
+                ssa_var_result = output_instr
+                self.set_all_bits_in_reg(self.ssa_vars[output_name], ssa_var_result)  # type: ignore
+
+            else:
+                rebased_circ = self._rebase_command_to_gateset(
+                    command
+                )  # Check if the command must be rebased.
+                if rebased_circ is not None:
+                    self.circuit_to_module(rebased_circ, module)
+                else:
+                    optype, params = self._get_optype_and_params(op)
+                    qubits = self._to_qis_qubits(command.qubits)
+                    results = self._to_qis_results(command.bits)
+                    bits: Optional[Sequence[Value]] = None
+                    if type(optype) == BitWiseOp:
+                        bits = self._to_qis_bits(command.args)
+                    gate = module.gateset.tk_to_gateset(optype)
+                    if not gate.func_spec == FuncSpec.BODY:
+                        func_name = gate.func_name.value + "_" + gate.func_spec.value
+                        get_gate = getattr(module.qis, func_name)
+                    else:
+                        get_gate = getattr(module.qis, gate.func_name.value)
+                    if bits:
+                        get_gate(*bits)
+                    elif params:
+                        get_gate(*params, *qubits)
+                    elif results:
+                        get_gate(*qubits, results)
+                    else:
+                        get_gate(*qubits)
+        if record_output:
+            for creg in self.circuit.c_registers:
+                reg_name = creg[0].reg_name
+                self.module.builder.call(
+                    self.record_output,
+                    [
+                        self.ssa_vars[reg_name],
+                    ],
+                )
+
+        return module
```

## pytket/qir/conversion/gatesets.py

 * *Ordering differences only*

```diff
@@ -1,155 +1,155 @@
-# Copyright 2019-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-from string import Template
-
-from dataclasses import dataclass
-from enum import Enum
-from string import Template
-from typing import Callable, Dict, List, NamedTuple, Set, Union, Any
-
-from pytket import OpType  # type: ignore
-
-# PyQirParameterType = any  # Union[Double, Int, Qubit, Result] # todo
-# PyQirReturnType = any  # Union[Int, Result, Void] # todo
-
-
-class FuncNat(Enum):
-    QIS = "qis"
-    CIS = "cis"
-    HYBRID = "hybrid"
-    RT = "rt"
-
-
-class FuncName(Enum):
-    H = "h"
-    X = "x"
-    Y = "y"
-    Z = "z"
-    S = "s"
-    T = "t"
-    RESET = "reset"
-    CNOT = "cnot"
-    CX = "cx"
-    CZ = "cz"
-    MEASURE = "m"
-    MEASUREZ = "mz"
-    Rx = "rx"
-    Ry = "ry"
-    Rz = "rz"
-    PHASEDX = "u1q"
-    ZZPHASE = "rzz"
-    ZZMAX = "zz"
-    AND = "and"
-    OR = "or"
-    XOR = "xor"
-    INT = "integer"
-    BOOL = "bool"
-    RES = "result"
-    READ_RES = "read_result"
-
-
-class FuncSpec(Enum):
-    BODY = "body"
-    ADJ = "adj"
-    CTL = "ctl"
-    CTLADJ = "ctladj"
-    REC_OUT = "record_output"
-
-
-@dataclass(frozen=True)
-class QirGate:
-    func_nat: FuncNat
-    func_name: Union[FuncName, Enum]
-    func_spec: FuncSpec
-
-
-@dataclass(frozen=True)
-class CustomQirGate(QirGate):
-    function_signature: List
-    return_type: Any
-
-
-CustomGateSet = NamedTuple(
-    "CustomGateSet",
-    [
-        ("name", str),
-        ("template", Template),
-        ("base_gateset", Set[OpType]),
-        ("gateset", Dict[str, CustomQirGate]),
-        ("tk_to_gateset", Callable),
-    ],
-)
-
-
-_TK_TO_PYQIR = {
-    OpType.H: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.H, func_spec=FuncSpec.BODY
-    ),
-    OpType.X: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.X, func_spec=FuncSpec.BODY
-    ),
-    OpType.Y: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.Y, func_spec=FuncSpec.BODY
-    ),
-    OpType.Z: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.Z, func_spec=FuncSpec.BODY
-    ),
-    OpType.S: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.S, func_spec=FuncSpec.BODY
-    ),
-    OpType.Sdg: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.S, func_spec=FuncSpec.ADJ
-    ),
-    OpType.T: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.T, func_spec=FuncSpec.BODY
-    ),
-    OpType.Tdg: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.T, func_spec=FuncSpec.ADJ
-    ),
-    OpType.Reset: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.RESET, func_spec=FuncSpec.BODY
-    ),
-    OpType.CX: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.CX, func_spec=FuncSpec.BODY
-    ),
-    OpType.CZ: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.CZ, func_spec=FuncSpec.BODY
-    ),
-    OpType.Measure: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.MEASUREZ, func_spec=FuncSpec.BODY
-    ),
-    OpType.Rx: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.Rx, func_spec=FuncSpec.BODY
-    ),
-    OpType.Ry: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.Ry, func_spec=FuncSpec.BODY
-    ),
-    OpType.Rz: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.Rz, func_spec=FuncSpec.BODY
-    ),
-    OpType.CopyBits: QirGate(
-        func_nat=FuncNat.QIS, func_name=FuncName.READ_RES, func_spec=FuncSpec.BODY
-    ),
-}
-
-
-PYQIR_GATES = CustomGateSet(
-    name="PyQir",
-    template=Template("__quantum__${func_nat}__${func_name}__${func_spec}"),
-    base_gateset=set(_TK_TO_PYQIR.keys()),
-    gateset={},
-    tk_to_gateset=lambda optype: _TK_TO_PYQIR[optype],
-)
+# Copyright 2019-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+
+from string import Template
+
+from dataclasses import dataclass
+from enum import Enum
+from string import Template
+from typing import Callable, Dict, List, NamedTuple, Set, Union, Any
+
+from pytket import OpType  # type: ignore
+
+# PyQirParameterType = any  # Union[Double, Int, Qubit, Result] # todo
+# PyQirReturnType = any  # Union[Int, Result, Void] # todo
+
+
+class FuncNat(Enum):
+    QIS = "qis"
+    CIS = "cis"
+    HYBRID = "hybrid"
+    RT = "rt"
+
+
+class FuncName(Enum):
+    H = "h"
+    X = "x"
+    Y = "y"
+    Z = "z"
+    S = "s"
+    T = "t"
+    RESET = "reset"
+    CNOT = "cnot"
+    CX = "cx"
+    CZ = "cz"
+    MEASURE = "m"
+    MEASUREZ = "mz"
+    Rx = "rx"
+    Ry = "ry"
+    Rz = "rz"
+    PHASEDX = "u1q"
+    ZZPHASE = "rzz"
+    ZZMAX = "zz"
+    AND = "and"
+    OR = "or"
+    XOR = "xor"
+    INT = "integer"
+    BOOL = "bool"
+    RES = "result"
+    READ_RES = "read_result"
+
+
+class FuncSpec(Enum):
+    BODY = "body"
+    ADJ = "adj"
+    CTL = "ctl"
+    CTLADJ = "ctladj"
+    REC_OUT = "record_output"
+
+
+@dataclass(frozen=True)
+class QirGate:
+    func_nat: FuncNat
+    func_name: Union[FuncName, Enum]
+    func_spec: FuncSpec
+
+
+@dataclass(frozen=True)
+class CustomQirGate(QirGate):
+    function_signature: List
+    return_type: Any
+
+
+CustomGateSet = NamedTuple(
+    "CustomGateSet",
+    [
+        ("name", str),
+        ("template", Template),
+        ("base_gateset", Set[OpType]),
+        ("gateset", Dict[str, CustomQirGate]),
+        ("tk_to_gateset", Callable),
+    ],
+)
+
+
+_TK_TO_PYQIR = {
+    OpType.H: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.H, func_spec=FuncSpec.BODY
+    ),
+    OpType.X: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.X, func_spec=FuncSpec.BODY
+    ),
+    OpType.Y: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.Y, func_spec=FuncSpec.BODY
+    ),
+    OpType.Z: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.Z, func_spec=FuncSpec.BODY
+    ),
+    OpType.S: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.S, func_spec=FuncSpec.BODY
+    ),
+    OpType.Sdg: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.S, func_spec=FuncSpec.ADJ
+    ),
+    OpType.T: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.T, func_spec=FuncSpec.BODY
+    ),
+    OpType.Tdg: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.T, func_spec=FuncSpec.ADJ
+    ),
+    OpType.Reset: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.RESET, func_spec=FuncSpec.BODY
+    ),
+    OpType.CX: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.CX, func_spec=FuncSpec.BODY
+    ),
+    OpType.CZ: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.CZ, func_spec=FuncSpec.BODY
+    ),
+    OpType.Measure: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.MEASUREZ, func_spec=FuncSpec.BODY
+    ),
+    OpType.Rx: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.Rx, func_spec=FuncSpec.BODY
+    ),
+    OpType.Ry: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.Ry, func_spec=FuncSpec.BODY
+    ),
+    OpType.Rz: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.Rz, func_spec=FuncSpec.BODY
+    ),
+    OpType.CopyBits: QirGate(
+        func_nat=FuncNat.QIS, func_name=FuncName.READ_RES, func_spec=FuncSpec.BODY
+    ),
+}
+
+
+PYQIR_GATES = CustomGateSet(
+    name="PyQir",
+    template=Template("__quantum__${func_nat}__${func_name}__${func_spec}"),
+    base_gateset=set(_TK_TO_PYQIR.keys()),
+    gateset={},
+    tk_to_gateset=lambda optype: _TK_TO_PYQIR[optype],
+)
```

## pytket/qir/conversion/module.py

 * *Ordering differences only*

```diff
@@ -1,48 +1,48 @@
-# Copyright 2019-2023 Cambridge Quantum Computing
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-"""
-This module defines an extension for the PyQir SimpleModule
-for the needs of generating QIR from Pytket circuits.
-"""
-
-from typing import Optional
-
-from pyqir import SimpleModule, BasicQisBuilder  # type: ignore
-
-from pytket.wasm import WasmFileHandler
-
-from .gatesets import PYQIR_GATES
-
-
-class tketqirModule:
-    """
-    PyQir module extension to account for custom defined input gate set
-    and calls to WASM files.
-    """
-
-    def __init__(
-        self,
-        name: str,
-        num_qubits: int,
-        num_results: int,
-        wasm_handler: Optional[WasmFileHandler] = None,
-    ) -> None:
-        self.module = SimpleModule(name, num_qubits, num_results)
-
-        self.builder = self.module.builder
-        self.context = self.module.context
-        self.qis = BasicQisBuilder(self.builder)
-        self.gateset = PYQIR_GATES
-        self.wasm_handler = wasm_handler
+# Copyright 2019-2023 Cambridge Quantum Computing
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+"""
+This module defines an extension for the PyQir SimpleModule
+for the needs of generating QIR from Pytket circuits.
+"""
+
+from typing import Optional
+
+from pyqir import SimpleModule, BasicQisBuilder  # type: ignore
+
+from pytket.wasm import WasmFileHandler
+
+from .gatesets import PYQIR_GATES
+
+
+class tketqirModule:
+    """
+    PyQir module extension to account for custom defined input gate set
+    and calls to WASM files.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        num_qubits: int,
+        num_results: int,
+        wasm_handler: Optional[WasmFileHandler] = None,
+    ) -> None:
+        self.module = SimpleModule(name, num_qubits, num_results)
+
+        self.builder = self.module.builder
+        self.context = self.module.context
+        self.qis = BasicQisBuilder(self.builder)
+        self.gateset = PYQIR_GATES
+        self.wasm_handler = wasm_handler
```

## Comparing `pytket_qir-0.2.0rc4.dist-info/LICENSE` & `pytket_qir-0.2.0rc5.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `pytket_qir-0.2.0rc4.dist-info/METADATA` & `pytket_qir-0.2.0rc5.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-Metadata-Version: 2.1
-Name: pytket-qir
-Version: 0.2.0rc4
-Summary: Extension for pytket, providing functions for conversion into to qir
-Author: TKET development team
-Author-email: tket-support@cambridgequantum.com
-License: Apache 2
-Project-URL: Documentation, https://cqcl.github.io/pytket-qir/api/index.html
-Project-URL: Source, https://github.com/CQCL/pytket-qir
-Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pytket (~=1.14)
-Requires-Dist: pyqir (==0.8.1)
-Requires-Dist: pyqir-generator (==0.7.0)
-Requires-Dist: pyqir-evaluator (==0.7.0)
-Requires-Dist: pyqir-parser (==0.7.0)
-
-# Pytket Extensions
-
-# this is currently work in progress
-
-This repository contains the pytket-qir extension, using Quantinuum's
-[pytket](https://cqcl.github.io/tket/pytket/api/index.html) quantum SDK.
-
-# pytket-qir
-
-[Pytket](https://cqcl.github.io/tket/pytket/api/index.html) is a python module for interfacing
-with tket, a quantum computing toolkit and optimisation compiler developed by Quantinuum.
-
-`pytket-qir` is an extension to `pytket` that allows `pytket` circuits to
-be converted to qir.
-
-## Getting started
-
-`pytket-qir` is available for Python 3.9, 3.10 and 3.11, on Linux, MacOS
-and Windows. To install, run:
-
-```pip install pytket-qir```
-
-This will install `pytket` if it isn't already installed, and add new classes
-and methods into the `pytket.extensions` namespace.
-
-The [example notebooks](https://github.com/CQCL/pytket-qir/tree/develop/examples) also demonstrate some of the key features of pytket-qir.
-
-## Bugs, support and feature requests
-
-Please file bugs and feature requests on the Github
-[issue tracker](https://github.com/CQCL/pytket-qir/issues).
-
-There is also a Slack channel for discussion and support. Click [here](https://tketusers.slack.com/join/shared_invite/zt-18qmsamj9-UqQFVdkRzxnXCcKtcarLRA#/shared-invite/email) to join.
-
-## Development
-
-To install this extension in editable mode, simply change to this directory, and run:
-
-```shell
-pip install -e .
-```
-
-## Contributing
-
-Pull requests are welcome. To make a PR, first fork the repo, make your proposed
-changes on the `develop` branch, and open a PR from your fork. If it passes
-tests and is accepted after review, it will be merged in.
-
-### Code style
-
-#### Formatting
-
-All code should be formatted using
-[black](https://black.readthedocs.io/en/stable/), with default options. This is
-checked on the CI. The CI is currently using version 20.8b1.
-
-#### Type annotation
-
-On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
-type checker and all submissions must pass its checks. You should therefore run
-`mypy` locally on any changed files before submitting a PR. Because of the way
-extension modules embed themselves into the `pytket` namespace this is a little
-complicated, but it should be sufficient to run the script `modules/mypy-check`
-(passing as a single argument the root directory of the module to test). The
-script requires `mypy` 0.800 or above.
-
-#### Linting
-
-We use [pylint](https://pypi.org/project/pylint/) on the CI to check compliance
-with a set of style requirements (listed in `.pylintrc`). You should run
-`pylint` over any changed files before submitting a PR, to catch any issues.
-
-### Tests
-
-To run the tests:
-
-1. `cd` into the `tests` directory;
-2. ensure you have installed `pytest`, `hypothesis`, and any modules listed in
-the `test-requirements.txt` file (all via `pip`);
-3. run `pytest`.
-
-When adding a new feature, please add a test for it. When fixing a bug, please
-add a test that demonstrates the fix.
+Metadata-Version: 2.1
+Name: pytket-qir
+Version: 0.2.0rc5
+Summary: Extension for pytket, providing functions for conversion into to qir
+Author: TKET development team
+Author-email: tket-support@cambridgequantum.com
+License: Apache 2
+Project-URL: Documentation, https://cqcl.github.io/pytket-qir/api/index.html
+Project-URL: Source, https://github.com/CQCL/pytket-qir
+Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pytket (~=1.14)
+Requires-Dist: pyqir (==0.8.1)
+Requires-Dist: pyqir-generator (==0.7.0)
+Requires-Dist: pyqir-evaluator (==0.7.0)
+Requires-Dist: pyqir-parser (==0.7.0)
+
+# Pytket Extensions
+
+# this is currently work in progress
+
+This repository contains the pytket-qir extension, using Quantinuum's
+[pytket](https://cqcl.github.io/tket/pytket/api/index.html) quantum SDK.
+
+# pytket-qir
+
+[Pytket](https://cqcl.github.io/tket/pytket/api/index.html) is a python module for interfacing
+with tket, a quantum computing toolkit and optimisation compiler developed by Quantinuum.
+
+`pytket-qir` is an extension to `pytket` that allows `pytket` circuits to
+be converted to qir.
+
+## Getting started
+
+`pytket-qir` is available for Python 3.9, 3.10 and 3.11, on Linux, MacOS
+and Windows. To install, run:
+
+```pip install pytket-qir```
+
+This will install `pytket` if it isn't already installed, and add new classes
+and methods into the `pytket.extensions` namespace.
+
+The [example notebooks](https://github.com/CQCL/pytket-qir/tree/develop/examples) also demonstrate some of the key features of pytket-qir.
+
+## Bugs, support and feature requests
+
+Please file bugs and feature requests on the Github
+[issue tracker](https://github.com/CQCL/pytket-qir/issues).
+
+There is also a Slack channel for discussion and support. Click [here](https://tketusers.slack.com/join/shared_invite/zt-18qmsamj9-UqQFVdkRzxnXCcKtcarLRA#/shared-invite/email) to join.
+
+## Development
+
+To install this extension in editable mode, simply change to this directory, and run:
+
+```shell
+pip install -e .
+```
+
+## Contributing
+
+Pull requests are welcome. To make a PR, first fork the repo, make your proposed
+changes on the `develop` branch, and open a PR from your fork. If it passes
+tests and is accepted after review, it will be merged in.
+
+### Code style
+
+#### Formatting
+
+All code should be formatted using
+[black](https://black.readthedocs.io/en/stable/), with default options. This is
+checked on the CI. The CI is currently using version 20.8b1.
+
+#### Type annotation
+
+On the CI, [mypy](https://mypy.readthedocs.io/en/stable/) is used as a static
+type checker and all submissions must pass its checks. You should therefore run
+`mypy` locally on any changed files before submitting a PR. Because of the way
+extension modules embed themselves into the `pytket` namespace this is a little
+complicated, but it should be sufficient to run the script `modules/mypy-check`
+(passing as a single argument the root directory of the module to test). The
+script requires `mypy` 0.800 or above.
+
+#### Linting
+
+We use [pylint](https://pypi.org/project/pylint/) on the CI to check compliance
+with a set of style requirements (listed in `.pylintrc`). You should run
+`pylint` over any changed files before submitting a PR, to catch any issues.
+
+### Tests
+
+To run the tests:
+
+1. `cd` into the `tests` directory;
+2. ensure you have installed `pytest`, `hypothesis`, and any modules listed in
+the `test-requirements.txt` file (all via `pip`);
+3. run `pytest`.
+
+When adding a new feature, please add a test for it. When fixing a bug, please
+add a test that demonstrates the fix.
```

## Comparing `pytket_qir-0.2.0rc4.dist-info/RECORD` & `pytket_qir-0.2.0rc5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pytket/qir/__init__.py,sha256=gB96uST6dijUbtR6Pqbt3NouwaIZ9QIoDhu4AhjHzEk,882
-pytket/qir/_metadata.py,sha256=q2TM61cKIJ6M5wbxb3IsmokrXYqf28bSv7OnOx2qv44,71
-pytket/qir/conversion/__init__.py,sha256=fo1auCplBT-XWDMoIINsp9hG8z1u7sfkmTK3V57LYhs,733
-pytket/qir/conversion/api.py,sha256=84Z0_JoVLMy53map5oq1h0GAA0AHinjOHetafOk7U1s,1946
-pytket/qir/conversion/conversion.py,sha256=Rm1G9V7QID9UN8VEP7J-KZ1v2chf6HKc0eFocoZeh4E,28077
-pytket/qir/conversion/gatesets.py,sha256=-Hkz5mDNB6CT5ynevxCjhYmtYhQekAaO0D54lIFj8Zg,4237
-pytket/qir/conversion/module.py,sha256=T815C7xTzP2U3orcvdCASf8UXTnb_9i59EDXm4IZT2A,1529
-pytket_qir-0.2.0rc4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-pytket_qir-0.2.0rc4.dist-info/METADATA,sha256=46JT-E5CmsG6QLccvQzbWkKllZNwbQ1wQ7i1KoX9fjI,4296
-pytket_qir-0.2.0rc4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytket_qir-0.2.0rc4.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_qir-0.2.0rc4.dist-info/RECORD,,
+pytket/qir/__init__.py,sha256=bVQc7W5vFNKJ_hnMPYiFaYnU6NPJAMaYMY_m3rZ4Jgs,862
+pytket/qir/_metadata.py,sha256=KMtf0n2J0LqvXhMxyc7j3p16jqMBeVMhMAN09vlyZJk,69
+pytket/qir/conversion/__init__.py,sha256=FTpNgzkF_dlwlu67zaPKHX5y2_v_jGmTnViJ8IbiX8w,715
+pytket/qir/conversion/api.py,sha256=q1A4dphwvSCe0Yf0eUEPs-mGc9rR2lePhng7pIWHoMI,2519
+pytket/qir/conversion/conversion.py,sha256=UXT-fWtR_Jb3YUJn5n4k5uaQghogXzerfrngQvundAw,27522
+pytket/qir/conversion/gatesets.py,sha256=Ix1KkLlFoyE1LkoUs0J7wFikZXT9w5jYs8mnTQnZURM,4082
+pytket/qir/conversion/module.py,sha256=fj8iHNh27_-wbjKkO9JdnKkExiRAhMWXTzjVP9kCwtA,1481
+pytket_qir-0.2.0rc5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_qir-0.2.0rc5.dist-info/METADATA,sha256=YiSYOB5sqsH0LruIcRHXMbA_aHMJ8_GJz7jHUECd1e0,4183
+pytket_qir-0.2.0rc5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytket_qir-0.2.0rc5.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_qir-0.2.0rc5.dist-info/RECORD,,
```

