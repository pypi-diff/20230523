# Comparing `tmp/pyapp-flow-0.8.0.tar.gz` & `tmp/pyapp-flow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapp-flow-0.8.0.tar", max compression
+gzip compressed data, was "pyapp-flow-0.9.0.tar", max compression
```

## Comparing `pyapp-flow-0.8.0.tar` & `pyapp-flow-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1321 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/HISTORY
--rw-r--r--   0        0        0     1514 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/LICENSE
--rw-r--r--   0        0        0     7117 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/README.md
--rw-r--r--   0        0        0     1202 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3083 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/__init__.py
--rw-r--r--   0        0        0       37 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/checks.py
--rw-r--r--   0        0        0     4940 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/datastructures.py
--rw-r--r--   0        0        0      473 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/exceptions.py
--rw-r--r--   0        0        0        0 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/ext/__init__.py
--rw-r--r--   0        0        0     6825 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/ext/sphinx/__init__.py
--rw-r--r--   0        0        0     2149 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/functions.py
--rw-r--r--   0        0        0    15801 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/nodes.py
--rw-r--r--   0        0        0      788 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/src/pyapp_flow/testing.py
--rw-r--r--   0        0        0        0 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/ext/__init__.py
--rw-r--r--   0        0        0     5919 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/ext/test_sphinx.py
--rw-r--r--   0        0        0       30 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/test_checks.py
--rw-r--r--   0        0        0     4081 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/test_datastructures.py
--rw-r--r--   0        0        0     2109 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/test_flow.py
--rw-r--r--   0        0        0     2847 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/test_functions.py
--rw-r--r--   0        0        0    12876 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/test_nodes.py
--rw-r--r--   0        0        0      881 2022-08-03 05:52:47.775470 pyapp-flow-0.8.0/tests/unit/test_testing.py
--rw-r--r--   0        0        0     8200 2022-08-03 05:52:56.367190 pyapp-flow-0.8.0/setup.py
--rw-r--r--   0        0        0     8152 2022-08-03 05:52:56.367887 pyapp-flow-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1592 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/HISTORY
+-rw-r--r--   0        0        0     1514 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7117 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/README.md
+-rw-r--r--   0        0        0     1202 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3081 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/__init__.py
+-rw-r--r--   0        0        0       37 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/checks.py
+-rw-r--r--   0        0        0     4940 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/datastructures.py
+-rw-r--r--   0        0        0      473 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/exceptions.py
+-rw-r--r--   0        0        0        0 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/ext/__init__.py
+-rw-r--r--   0        0        0     6825 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/ext/sphinx/__init__.py
+-rw-r--r--   0        0        0     3133 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/functions.py
+-rw-r--r--   0        0        0    16106 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/nodes.py
+-rw-r--r--   0        0        0     5244 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/parallel_nodes.py
+-rw-r--r--   0        0        0      788 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/src/pyapp_flow/testing.py
+-rw-r--r--   0        0        0        0 2022-09-27 03:25:40.785120 pyapp-flow-0.9.0/tests/unit/ext/__init__.py
+-rw-r--r--   0        0        0     6689 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/ext/test_sphinx.py
+-rw-r--r--   0        0        0       30 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_checks.py
+-rw-r--r--   0        0        0     4081 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_datastructures.py
+-rw-r--r--   0        0        0     2109 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_flow.py
+-rw-r--r--   0        0        0     3419 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_functions.py
+-rw-r--r--   0        0        0    13461 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_nodes.py
+-rw-r--r--   0        0        0      109 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_parallel_nodes.py
+-rw-r--r--   0        0        0      881 2022-09-27 03:25:40.789120 pyapp-flow-0.9.0/tests/unit/test_testing.py
+-rw-r--r--   0        0        0     8204 1970-01-01 00:00:00.000000 pyapp-flow-0.9.0/setup.py
+-rw-r--r--   0        0        0     8303 1970-01-01 00:00:00.000000 pyapp-flow-0.9.0/PKG-INFO
```

### Comparing `pyapp-flow-0.8.0/HISTORY` & `pyapp-flow-0.9.0/HISTORY`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+0.9.0
+=====
+
+Changes
+-------
+
+- Define a `Node` protocol
+- `CaptureErrors` node can now specify specific exception types
+- Early version of parallel nodes (using multiprocessing), this version has some
+  caveats relating to what can be passed into a parallel execution.
+
 0.8.0
 =====
 
 Changes
 -------
 
 - `WorkflowContext.state` variables can now be accessed as attributes
```

### Comparing `pyapp-flow-0.8.0/LICENSE` & `pyapp-flow-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/README.md` & `pyapp-flow-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/pyproject.toml` & `pyapp-flow-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyapp-flow"
-version = "0.8.0"
+version = "0.9.0"
 description = "Application workflow framework"
 authors = ["Tim Savage <tim@savage.company>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/pyapp-org/pyapp-flow"
 keywords = ["framework", "application"]
 classifiers = [
@@ -26,15 +26,15 @@
 include = ["HISTORY"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^12.4.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 Cython = "^0.29.30"
 sphinx = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyapp-flow-0.8.0/src/pyapp_flow/__init__.py` & `pyapp-flow-0.9.0/src/pyapp_flow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Application Workflow
 """
-from typing import Callable, Optional
+from typing import Optional
 
 from . import exceptions
 from .datastructures import WorkflowContext, Navigable, Branches
 from .functions import extract_inputs
 from .nodes import (
+    Node,
     step,
     Step,
     SetVar,
     ForEach,
     CaptureErrors,
     Conditional,
     If,
@@ -23,15 +24,15 @@
 class Nodes(Navigable):
     """
     A series of nodes to be executed on call.
     """
 
     __slots__ = ("_nodes",)
 
-    def __init__(self, *nodes_):
+    def __init__(self, *nodes_: Node):
         self._nodes = list(nodes_)
 
     def __call__(self, context: WorkflowContext):
         with context:
             self._execute(context)
 
     @property
@@ -84,26 +85,26 @@
         """
         context = context or WorkflowContext()
         context.state.update(context_vars)
         context.logger.info("⏩ Workflow: `%s`", self._name)
         self._execute(context)
         return context
 
-    def nodes(self, *nodes_: Callable) -> "Workflow":
+    def nodes(self, *nodes_: Node) -> "Workflow":
         """
         Append additional node(s) into the node list
 
         :param nodes_: Nodes to append to the current block
         :return: Returns self; fluent interface
 
         """
         self._nodes.extend(nodes_)
         return self
 
-    def nested(self, *nodes_: Callable) -> "Workflow":
+    def nested(self, *nodes_: Node) -> "Workflow":
         """
         Add nested node(s), nested nodes have their own scope
 
         :param nodes_: Collection of nodes call from nested block.
         :return: Returns self; fluent interface
 
         """
```

### Comparing `pyapp-flow-0.8.0/src/pyapp_flow/datastructures.py` & `pyapp-flow-0.9.0/src/pyapp_flow/datastructures.py`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/src/pyapp_flow/ext/sphinx/__init__.py` & `pyapp-flow-0.9.0/src/pyapp_flow/ext/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/src/pyapp_flow/functions.py` & `pyapp-flow-0.9.0/src/pyapp_flow/functions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-from typing import Callable, Mapping, Tuple, Sequence, Union
+from typing import Callable, Mapping, Tuple, Sequence, Union, Iterable
 
 from .datastructures import WorkflowContext
 from .exceptions import WorkflowSetupError
 
 
+def var_list(var_names: Union[str, Sequence[str]]) -> Sequence[str]:
+    """
+    Split a comma separated list of var names into individual names.
+    """
+    if isinstance(var_names, str):
+        var_names = var_names.split(",")
+    return [name.strip() for name in var_names]
+
+
 def extract_inputs(func: Callable) -> Tuple[Mapping[str, type], str]:
     """
     Extract input variables from function
     """
     func_code = func.__code__
     annotations = func.__annotations__
 
@@ -46,24 +55,26 @@
 ) -> Sequence[Tuple[str, type]]:
     """
     Extract outputs from function
     """
     types = func.__annotations__.get("return")
 
     # Ensure names is a list
+    is_singular = False
     if names is None:
         names = ()
-    if isinstance(names, str):
-        names = (names,)
+    elif isinstance(names, str):
+        names = var_list(names)
+        is_singular = len(names) == 1
 
     # Ensure types is a list
     if types is None:
         types = ()
     elif getattr(types, "_name", None) == "Tuple":
-        types = types.__args__
+        types = (types,) if is_singular else types.__args__
     else:
         types = (types,)
 
     if len(names) != len(types):
         raise WorkflowSetupError("Name count does not match type count.")
 
     return tuple(zip(names, types))
@@ -71,7 +82,29 @@
 
 def call_nodes(context: WorkflowContext, nodes: Sequence[Callable]):
     """
     Call each node in a sequence
     """
     for node in nodes:
         node(context)
+
+
+def merge_nested_entries(
+    iterable: Iterable[list], merge_methods: Sequence[str]
+) -> Sequence[list]:
+    """
+    Rotate and combine rows of data
+
+    >>> merge_nested_entries([[1, 2, [3]], [4, 5, [6, 7]]], ("append", "append", "extend"))
+    ... [[1, 4], [2, 5], [3, 6, 7]]
+
+    """
+    results = tuple([] for _ in merge_methods)
+    merge_methods = tuple(
+        getattr(result, method) for result, method in zip(results, merge_methods)
+    )
+
+    for entry in iterable:
+        for value, merge_method in zip(entry, merge_methods):
+            merge_method(value)
+
+    return results
```

### Comparing `pyapp-flow-0.8.0/src/pyapp_flow/nodes.py` & `pyapp-flow-0.9.0/src/pyapp_flow/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,28 @@
     Callable,
     Sequence,
     Union,
     Iterable,
     Type,
     Hashable,
     Optional,
+    Any,
+    Protocol,
 )
 
 from .datastructures import WorkflowContext, Navigable, Branches
-from .functions import extract_inputs, extract_outputs, call_nodes
+from .functions import extract_inputs, extract_outputs, call_nodes, var_list
 from .exceptions import FatalError, WorkflowRuntimeError
 
 
+class Node(Protocol):
+    def __call__(self, context: WorkflowContext) -> Any:
+        ...
+
+
 class Step(Navigable):
     """
     Wrapper around a function that defines a workflow step
 
     Typically, this would be applied using the ``step`` decorator eg:
 
     >>> @step(outputs=(("var_b", str),))
@@ -88,15 +95,15 @@
                 context.error("  ⛔ Exception raised: %s", ex)
                 raise
 
         else:
             if self.outputs:
                 # Helper so a simple return can be used for a single result
                 values = (results,) if len(self.outputs) == 1 else results
-                for name, value in zip([name for name, _ in self.outputs], values):
+                for name, value in zip((output[0] for output in self.outputs), values):
                     context.state[name] = value
 
             return results
 
     @property
     def name(self) -> str:
         return self._name
@@ -136,15 +143,15 @@
 
     """
 
     __slots__ = ("values",)
 
     def __init__(
         self,
-        **values: Union[object, Callable[[WorkflowContext], object]],
+        **values: Union[Any, Callable[[WorkflowContext], Any]],
     ):
         self.values = values
 
     def __call__(self, context: WorkflowContext):
         context.info("📝 %s", self)
         values = (
             (key, value(context) if callable(value) else value)
@@ -212,44 +219,54 @@
             )
         )
 
     """
 
     __slots__ = ("target_var", "_nodes", "try_all")
 
-    def __init__(self, target_var: str, try_all: bool = True):
+    def __init__(
+        self,
+        target_var: str,
+        try_all: bool = True,
+        *,
+        except_types: Union[type, Sequence[type]] = None,
+    ):
         self.target_var = target_var
+        self.except_types = except_types
         self._nodes = []
         self.try_all = try_all
 
     def __call__(self, context: WorkflowContext):
         context.info("🥅 %s", self)
+        except_types = self.except_types
 
         try:
             var = context.state[self.target_var]
         except KeyError:
             var = context.state[self.target_var] = []
 
         with context:
             for node in self._nodes:
                 try:
                     node(context)
                 except Exception as ex:
+                    if except_types and not isinstance(ex, except_types):
+                        raise
                     var.append(ex)
                     if not self.try_all:
                         break
 
     @property
     def name(self):
         return f"Capture errors into `{self.target_var}`"
 
     def branches(self) -> Optional[Branches]:
         return {"": tuple(self._nodes)}
 
-    def nodes(self, *nodes):
+    def nodes(self, *nodes: Node):
         """
         Add additional nodes
         """
         self._nodes.extend(nodes)
         return self
 
 
@@ -303,22 +320,22 @@
     @property
     def name(self):
         return f"Conditional branch"
 
     def branches(self) -> Optional[Branches]:
         return {"true": self._true_nodes, "false": self._false_nodes}
 
-    def true(self, *nodes: Callable) -> "Conditional":
+    def true(self, *nodes: Node) -> "Conditional":
         """
         Nodes to use for the true branch
         """
         self._true_nodes = nodes
         return self
 
-    def false(self, *nodes: Callable) -> "Conditional":
+    def false(self, *nodes: Node) -> "Conditional":
         """
         Nodes to use for the false branch
         """
         self._false_nodes = nodes
         return self
 
 
@@ -380,22 +397,22 @@
 
     def branches(self) -> Optional[Branches]:
         branches = {str(case): nodes for case, nodes in self._options.items()}
         if self._default:
             branches["*DEFAULT*"] = self._default
         return branches
 
-    def case(self, key: Hashable, *nodes: Callable) -> "Switch":
+    def case(self, key: Hashable, *nodes: Node) -> "Switch":
         """
         Key used to match branch and the nodes that make up the branch
         """
         self._options[key] = nodes
         return self
 
-    def default(self, *nodes: Callable) -> "Switch":
+    def default(self, *nodes: Node) -> "Switch":
         """
         If a case key is not matched use these nodes as the default branch.
         """
         self._default = nodes
         return self
 
 
@@ -463,17 +480,15 @@
         )
 
     """
 
     __slots__ = ("target_vars", "in_var", "_nodes", "_update_context")
 
     def __init__(self, target_vars: Union[str, Sequence[str]], in_var: str):
-        if isinstance(target_vars, str):
-            target_vars = [var.strip() for var in target_vars.split(",")]
-        self.target_vars = target_vars
+        self.target_vars = target_vars = var_list(target_vars)
         self.in_var = in_var
         self._nodes = []
 
         if len(target_vars) == 1:
             self._update_context = self._single_value(target_vars[0])
         else:
             self._update_context = self._multiple_value(target_vars)
@@ -497,15 +512,15 @@
     def name(self):
         target_vars = ", ".join(f"`{var}`" for var in self.target_vars)
         return f"For ({target_vars}) in `{self.in_var}`"
 
     def branches(self) -> Optional[Branches]:
         return {"loop": self._nodes}
 
-    def loop(self, *nodes: Callable) -> "ForEach":
+    def loop(self, *nodes: Node) -> "ForEach":
         """
         Nodes to call on each iteration of the foreach block
         """
         self._nodes = nodes
         return self
 
     @staticmethod
```

### Comparing `pyapp-flow-0.8.0/src/pyapp_flow/testing.py` & `pyapp-flow-0.9.0/src/pyapp_flow/testing.py`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/tests/unit/ext/test_sphinx.py` & `pyapp-flow-0.9.0/tests/unit/ext/test_sphinx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,220 +1,219 @@
-from unittest.mock import Mock, call, ANY
+from unittest.mock import Mock
 
 import pytest
-from sphinx.ext.autodoc.directive import DocumenterBridge, Options
 
 import pyapp_flow as flow
-from pyapp_flow.ext import sphinx
-
-
-@flow.step(name="Sample Step", output="arg_d")
-def sample_step(arg_a: int, *, arg_b: str, arg_c) -> bool:
-    """
-    This is a sample step that just outputs false
-    """
-    return False
-
-
-@flow.step(name="Simple Step")
-def simple_step():
-    pass
 
+try:
+    from sphinx.ext.autodoc.directive import DocumenterBridge, Options
+    from pyapp_flow.ext import sphinx
+except ImportError:
+    pytest.skip("Sphinx not available for tests", allow_module_level=True)
+else:
+
+    @flow.step(name="Sample Step", output="arg_d")
+    def sample_step(arg_a: int, *, arg_b: str, arg_c) -> bool:
+        """
+        This is a sample step that just outputs false
+        """
+        return False
+
+    @flow.step(name="Simple Step")
+    def simple_step():
+        pass
+
+    def not_a_step():
+        """
+        This is not, and I repeat not a step
+        """
+
+    class TestStepDocumenter:
+        @pytest.fixture
+        def target(self):
+            directive = DocumenterBridge(
+                Mock(),
+                Mock(),
+                Options(),
+                15,
+                state=Mock(document=Mock(settings=Mock(tab_width=4))),
+            )
+            target = sphinx.StepDocumenter(directive, "Test")
+            target.object = sample_step
+            target.name = "ext.test_sphinx.sample_step"
+            return target
+
+        @pytest.mark.parametrize(
+            "step, expected",
+            (
+                (sample_step, True),
+                (not_a_step, False),
+            ),
+        )
+        def test_can_document_member(self, step, expected):
+            actual = sphinx.StepDocumenter.can_document_member(step)
 
-def not_a_step():
-    """
-    This is not, and I repeat not a step
-    """
+            assert actual is expected
 
+        def test_add_directive_header(self, target):
+            target.add_directive_header("")
 
-class TestStepDocumenter:
-    @pytest.fixture
-    def target(self):
-        directive = DocumenterBridge(
-            Mock(),
-            Mock(),
-            Options(),
-            15,
-            state=Mock(document=Mock(settings=Mock(tab_width=4))),
-        )
-        target = sphinx.StepDocumenter(directive, "Test")
-        target.object = sample_step
-        target.name = "ext.test_sphinx.sample_step"
-        return target
-
-    @pytest.mark.parametrize(
-        "step, expected",
-        (
-            (sample_step, True),
-            (not_a_step, False),
+            assert target.directive.result.data == [
+                ".. py:function:: ext.test_sphinx.sample_step",
+                "",
+                "**Sample Step**",
+            ]
+
+        def test_add_directive_header__with_no_name_option(self, target):
+            target.options["noname"] = True
+            target.add_directive_header("")
+
+            assert target.directive.result.data == [
+                ".. py:function:: ext.test_sphinx.sample_step",
+            ]
+
+        def test_get_doc(self, target):
+            actual = target.get_doc()
+
+            assert actual == [["This is a sample step that just outputs false", ""]]
+
+        def test_get_doc__where_method_has_no_docstring(self, target):
+            target.object = simple_step
+
+            actual = target.get_doc()
+
+            assert actual == []
+
+        def test_document_members(self, target):
+            target.document_members()
+
+            assert target.directive.result.data == [
+                "",
+                "**Input Variable(s)**",
+                "",
+                "* *arg_a*: *int*",
+                "* *arg_b*: *str*",
+                "* *arg_c*",
+                "",
+                "**Output Variable**",
+                "",
+                "* *arg_d*: *bool*",
+                "",
+            ]
+
+        def test_document_members__with_no_inputs_or_outputs(self, target):
+            target.object = simple_step
+            target.document_members()
+
+            assert target.directive.result.data == [""]
+
+    sample_workflow = flow.Workflow(
+        name="Sample workflow",
+        description="This is a sample workflow that just runs a simple operation",
+    ).nodes(
+        flow.SetVar(samples=["a", "b", "c"]),
+        flow.ForEach("sample", in_var="samples").loop(
+            flow.LogMessage("Reviewing sample {sample}")
         ),
+        sample_step,
     )
-    def test_can_document_member(self, step, expected):
-        actual = sphinx.StepDocumenter.can_document_member(step)
 
-        assert actual is expected
+    basic_workflow = flow.Workflow(name="Basic workflow").nodes(
+        flow.SetVar(samples=lambda ctx: ctx.state.a.title()),
+        (lambda ctx: ctx.info("Technically valid!")),
+        sample_step,
+    )
 
-    def test_add_directive_header(self, target):
-        target.add_directive_header("")
+    not_a_workflow = object()
 
-        assert target.directive.result.data == [
-            ".. py:function:: ext.test_sphinx.sample_step",
-            "",
-            "**Sample Step**",
-        ]
-
-    def test_add_directive_header__with_no_name_option(self, target):
-        target.options["noname"] = True
-        target.add_directive_header("")
-
-        assert target.directive.result.data == [
-            ".. py:function:: ext.test_sphinx.sample_step",
-        ]
-
-    def test_get_doc(self, target):
-        actual = target.get_doc()
-
-        assert actual == [["This is a sample step that just outputs false", ""]]
-
-    def test_get_doc__where_method_has_no_docstring(self, target):
-        target.object = simple_step
-
-        actual = target.get_doc()
-
-        assert actual == []
-
-    def test_document_members(self, target):
-        target.document_members()
-
-        assert target.directive.result.data == [
-            "",
-            "**Input Variable(s)**",
-            "",
-            "* *arg_a*: *int*",
-            "* *arg_b*: *str*",
-            "* *arg_c*",
-            "",
-            "**Output Variable**",
-            "",
-            "* *arg_d*: *bool*",
-            "",
-        ]
-
-    def test_document_members__with_no_inputs_or_outputs(self, target):
-        target.object = simple_step
-        target.document_members()
-
-        assert target.directive.result.data == [""]
-
-
-sample_workflow = flow.Workflow(
-    name="Sample workflow",
-    description="This is a sample workflow that just runs a simple operation",
-).nodes(
-    flow.SetVar(samples=["a", "b", "c"]),
-    flow.ForEach("sample", in_var="samples").loop(
-        flow.LogMessage("Reviewing sample {sample}")
-    ),
-    sample_step,
-)
-
-basic_workflow = flow.Workflow(name="Basic workflow").nodes(
-    flow.SetVar(samples=lambda ctx: ctx.state.a.title()),
-    (lambda ctx: ctx.info("Technically valid!")),
-    sample_step,
-)
-
-not_a_workflow = object()
-
-
-class TestWorkflowDocumenter:
-    @pytest.fixture
-    def target(self):
-        directive = DocumenterBridge(
-            Mock(),
-            Mock(),
-            Options(),
-            15,
-            state=Mock(document=Mock(settings=Mock(tab_width=4))),
+    class TestWorkflowDocumenter:
+        @pytest.fixture
+        def target(self):
+            directive = DocumenterBridge(
+                Mock(),
+                Mock(),
+                Options(),
+                15,
+                state=Mock(document=Mock(settings=Mock(tab_width=4))),
+            )
+            target = sphinx.WorkflowDocumenter(directive, "Test")
+            target.object = sample_workflow
+            target.name = "ext.test_sphinx.sample_workflow"
+            return target
+
+        @pytest.mark.parametrize(
+            "step, expected",
+            (
+                (sample_workflow, True),
+                (not_a_workflow, False),
+            ),
         )
-        target = sphinx.WorkflowDocumenter(directive, "Test")
-        target.object = sample_workflow
-        target.name = "ext.test_sphinx.sample_workflow"
-        return target
-
-    @pytest.mark.parametrize(
-        "step, expected",
-        (
-            (sample_workflow, True),
-            (not_a_workflow, False),
-        ),
-    )
-    def test_can_document_member(self, step, expected):
-        actual = sphinx.WorkflowDocumenter.can_document_member(step)
+        def test_can_document_member(self, step, expected):
+            actual = sphinx.WorkflowDocumenter.can_document_member(step)
 
-        assert actual is expected
+            assert actual is expected
 
-    def test_add_directive_header(self, target):
-        target.add_directive_header("")
+        def test_add_directive_header(self, target):
+            target.add_directive_header("")
 
-        assert target.directive.result.data == [
-            ".. py:function:: ext.test_sphinx.sample_workflow",
-            "",
-            "**Sample workflow**",
-        ]
-
-    def test_add_directive_header__with_no_name_option(self, target):
-        target.options["noname"] = True
-        target.add_directive_header("")
-
-        assert target.directive.result.data == [
-            ".. py:function:: ext.test_sphinx.sample_workflow",
-        ]
-
-    def test_get_doc(self, target):
-        actual = target.get_doc()
-
-        assert actual == [
-            ["This is a sample workflow that just runs a simple operation", ""]
-        ]
-
-    def test_get_doc__with_no_doc(self, target):
-        target.object = basic_workflow
-        actual = target.get_doc()
-
-        assert actual == []
-
-    def test_document_members(self, target):
-        target.document_members()
-
-        assert target.directive.result.data == []
-
-    def test_document_members__with_nodes_option(self, target):
-        target.options["nodes"] = True
-        target.document_members()
-
-        assert target.directive.result.data == [
-            "",
-            "- Set value(s) for samples",
-            "",
-            "- For (`sample`) in `samples`",
-            "",
-            "  - **loop**",
-            "",
-            "    - Log Message 'Reviewing sample {sample}'",
-            "",
-            "- Sample Step",
-        ]
-
-    def test_document_members__with_nodes_option_and_a_non_navigable(self, target):
-        target.object = basic_workflow
-        target.options["nodes"] = True
-        target.document_members()
-
-        assert target.directive.result.data == [
-            "",
-            "- Set value(s) for samples",
-            "",
-            "- *Unknown node*",
-            "",
-            "- Sample Step",
-        ]
+            assert target.directive.result.data == [
+                ".. py:function:: ext.test_sphinx.sample_workflow",
+                "",
+                "**Sample workflow**",
+            ]
+
+        def test_add_directive_header__with_no_name_option(self, target):
+            target.options["noname"] = True
+            target.add_directive_header("")
+
+            assert target.directive.result.data == [
+                ".. py:function:: ext.test_sphinx.sample_workflow",
+            ]
+
+        def test_get_doc(self, target):
+            actual = target.get_doc()
+
+            assert actual == [
+                ["This is a sample workflow that just runs a simple operation", ""]
+            ]
+
+        def test_get_doc__with_no_doc(self, target):
+            target.object = basic_workflow
+            actual = target.get_doc()
+
+            assert actual == []
+
+        def test_document_members(self, target):
+            target.document_members()
+
+            assert target.directive.result.data == []
+
+        def test_document_members__with_nodes_option(self, target):
+            target.options["nodes"] = True
+            target.document_members()
+
+            assert target.directive.result.data == [
+                "",
+                "- Set value(s) for samples",
+                "",
+                "- For (`sample`) in `samples`",
+                "",
+                "  - **loop**",
+                "",
+                "    - Log Message 'Reviewing sample {sample}'",
+                "",
+                "- Sample Step",
+            ]
+
+        def test_document_members__with_nodes_option_and_a_non_navigable(self, target):
+            target.object = basic_workflow
+            target.options["nodes"] = True
+            target.document_members()
+
+            assert target.directive.result.data == [
+                "",
+                "- Set value(s) for samples",
+                "",
+                "- *Unknown node*",
+                "",
+                "- Sample Step",
+            ]
```

### Comparing `pyapp-flow-0.8.0/tests/unit/test_datastructures.py` & `pyapp-flow-0.9.0/tests/unit/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/tests/unit/test_flow.py` & `pyapp-flow-0.9.0/tests/unit/test_flow.py`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/tests/unit/test_functions.py` & `pyapp-flow-0.9.0/tests/unit/test_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 import pytest
 
 from pyapp_flow import functions, WorkflowContext
 from pyapp_flow.exceptions import WorkflowSetupError
 
 
+@pytest.mark.parametrize(
+    "var_names, expected",
+    (
+        ("foo", ["foo"]),
+        ("foo,bar", ["foo", "bar"]),
+        ("foo , bar", ["foo", "bar"]),
+        (["foo", "bar"], ["foo", "bar"]),
+    ),
+)
+def test_var_list(var_names, expected):
+    actual = functions.var_list(var_names)
+
+    assert actual == expected
+
+
 def valid_a(context: WorkflowContext):
     pass
 
 
 def valid_b(context: WorkflowContext, var_a: str):
     pass
 
@@ -66,14 +81,15 @@
 @pytest.mark.parametrize(
     "func, names, expected",
     (
         (valid_e, "var_a", (("var_a", int),)),
         (valid_e, ("var_a",), (("var_a", int),)),
         (valid_f, "var_b", (("var_b", str),)),
         (valid_f, ("var_b",), (("var_b", str),)),
+        (valid_g, "var_a", (("var_a", Tuple[str, int]),)),
         (valid_g, ("var_a", "var_b"), (("var_a", str), ("var_b", int))),
     ),
 )
 def test_extract_outputs__where_args_are_valid(func, names, expected):
     actual = functions.extract_outputs(func, names)
 
     assert actual == expected
@@ -106,16 +122,23 @@
 
 @pytest.mark.parametrize(
     "func, names",
     (
         (valid_f, None),
         (valid_f, ("a", "b")),
         (valid_g, None),
-        (valid_g, "a"),
         (valid_g, ("a", "b", "c")),
     ),
 )
 def test_extract_outputs__where_args_are_invalid(func, names):
     with pytest.raises(
         WorkflowSetupError, match="Name count does not match type count."
     ):
         functions.extract_outputs(func, names)
+
+
+def test_merge_nested_entries():
+    data = [[1, 2, [3]], [4, 5, [6, 7]]]
+
+    actual = functions.merge_nested_entries(data, ["append", "append", "extend"])
+
+    assert actual == ([1, 4], [2, 5], [3, 6, 7])
```

### Comparing `pyapp-flow-0.8.0/tests/unit/test_nodes.py` & `pyapp-flow-0.9.0/tests/unit/test_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,31 @@
                 nodes.Step(valid_raise_exception),
                 nodes.Step(valid_raise_exception),
             ),
         )
 
         assert [str(e) for e in context.state["errors"]] == ["'Boom!'", "'Boom!'"]
 
+    def test_call__match_specified_exception(self):
+        context = call_node(
+            nodes.CaptureErrors("errors", except_types=KeyError).nodes(
+                nodes.Step(valid_raise_exception),
+            )
+        )
+
+        assert [str(e) for e in context.state.errors] == ["'Boom!'"]
+
+    def test_call__not_match_specified_exception(self):
+        with pytest.raises(KeyError):
+            call_node(
+                nodes.CaptureErrors("errors", except_types=(ValueError,)).nodes(
+                    nodes.Step(valid_raise_exception),
+                )
+            )
+
     def test_str(self):
         target = nodes.CaptureErrors("errors").nodes(nodes.LogMessage("foo"))
 
         assert str(target) == "Capture errors into `errors`"
 
     def test_branches(self):
         target = nodes.CaptureErrors("errors", try_all=False).nodes(
```

### Comparing `pyapp-flow-0.8.0/tests/unit/test_testing.py` & `pyapp-flow-0.9.0/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `pyapp-flow-0.8.0/setup.py` & `pyapp-flow-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 {'': ['*']}
 
 install_requires = \
 ['rich>=12.4.4,<13.0.0']
 
 setup_kwargs = {
     'name': 'pyapp-flow',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Application workflow framework',
     'long_description': '# pyapp-flow\nA simple application level workflow library.\n\nAllows complex processes to be broken into smaller specific steps, greatly \nsimplifying testing and re-use.\n\n[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=pyapp-org_pyapp-flow&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=pyapp-org_pyapp-flow)\n[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=pyapp-org_pyapp-flow&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=pyapp-org_pyapp-flow)\n[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=pyapp-org_pyapp-flow&metric=coverage)](https://sonarcloud.io/summary/new_code?id=pyapp-org_pyapp-flow)\n[![Once you go Black...](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n\n## Installation\n\n```shell\npip install pyapp-flow\n```\n\n\n## Usage\n\n```python\nfrom pathlib import Path\nfrom typing import Sequence\nimport pyapp_flow as flow\n\n# Define steps:\n\n@flow.step(name="Load Names", output="names")\ndef load_names(root_path: Path) -> Sequence[str]:\n    """\n    Read a sequence of names from a file\n    """\n    with (root_path / "names.txt").open() as f_in:\n        return [name.strip() for name in f_in.readlines()]\n\n@flow.step(name="Say hello")\ndef say_hi(name: str):\n    print(f"Hello {name}")\n\n# Define a workflow:\n\ngreat_everybody = (\n    flow.Workflow(name="Great everybody in names file")\n    .nodes(\n      load_names,\n      flow.ForEach("name", in_var="names").loop(say_hi)\n    )\n)\n\n# Execute workflow:\n\ncontext = flow.WorkflowContext(root_path=Path())\ngreat_everybody(context)\n```\n\nAll nodes within the workflow follow a simple interface of:\n```python\ndef node_function(context: WorkflowContext):\n    ...\n```\nor using typing\n```python\nNodeFunction = Callable[[WorkflowContext], Any]\n```\n\nThe `step` decorator simplifies definition of a step by handling loading and saving \nof state variables from the `WorkflowContext`.\n\n\n## Reference\n\n### Workflow\n\nAt the basic level a workflow is an object that holds a series of nodes to be called \nin sequence. The workflow object also includes helper methods to generate and append\nthe nodes defined in the *Builtin Nodes* section of the documentation. \n\nJust like every node in pyApp-Flow a workflow is called with an `WorkflowContext` \nobject, this means workflows can be nested in workflows, or called from a for-each \nnode.\n\nThe one key aspect with a workflow object is related to context variable scope. \nWhen a workflow is triggered the context scope is copied and any changes made \nto the variables are discarded when the workflow ends. However, just like Python \nscoping only the reference to the variable is copied meaning mutable objects can \nbe modified (eg list/dicts).\n\n```python\nworkflow = (\n    Workflow(name="My Workflow")\n    .nodes(...)\n)\n```\n\n### WorkflowContext\n\nThe workflow context object holds the state of the workflow including handling \nvariable scoping and helper methods for logging progress.\n\n**Properties**\n\n- `state` \n\n  Direct access to state variables in the current scope.\n\n- `depth` \n \n  Current scope depth\n\n- `indent` \n\n  Helper that returns a string indent for use formatting messages\n\n**Methods**\n\n- `format`\n\n  Format a string using values from the context state. Most *name*\n  values for nodes/workflows use this method to allow values to be included\n  from scope eg:\n\n  ```python\n  context.format("Current path {working_path}")\n  ```\n\n- `push_state`/`pop_state`\n\n  Used to step into or out of a lower state scope. Typically these methods are\n  not called directly but are called via using a with block eg:\n  \n  ```python\n  with context:\n      pass  # Separate variable scope \n  ```\n\n- Logging wrappers\n\n  Wrappers around an internal workflow logger that handle indentation to make\n  reading the log easier.\n  \n  - log\n  - debug\n  - info\n  - warning\n  - error\n  - exception\n\n\n\n### Builtin Nodes\n\n**Modify context variables**\n\n- `SetVar`\n  \n    Set one or more variables into the context\n\n    ```python\n    SetVar(my_var="foo")\n    ```\n\n- `Append`\n\n    Append a value to a list in the context object (will create the list if it \n    does not exist).\n\n    ```python\n    Append("messages", "Operation failed to add {my_var}")\n    ```\n  \n- `CaptureErrors`\n\n    Capture and store any errors raised by node(s) within the capture block to a \n    variable within the context.\n\n    ```python\n    CaptureErrors("errors").nodes(my_flaky_step)\n    ```\n  \n    This node also has a `try_all` argument that controls the behaviour when an  \n    error is captured, if `True` every node is called even if they all raise errors,\n    this is useful for running a number of separate tests that may fail.\n\n    ```python\n    CaptureErrors(\n        "errors", \n        try_all=True\n    ).nodes(\n        my_first_check, \n        my_second_check, \n    )\n    ```\n\n**Provide feedback**\n\n- `LogMessage`\n    \n    Insert a message within optional values from the context into the runtime \n    log with an optional level.\n    \n    ```python\n    LogMessage("State of my_var is {my_var}", level=logging.INFO)\n    ```\n\n\n**Branching**\n\nBranching nodes utilise a fluent interface for defining the nodes within each \nbranch. \n\n- `Conditional` / `If`\n    \n    Analogous with an `if` statement, it can accept either a context variable \n    that can be interpreted as a `bool` or a function/lamba that accepts a \n    `WorkflowContext` object and returns a `bool`.\n\n    ```python \n    # With context variable\n    (\n        If("is_successful")\n        .true(log_message("Process successful :)"))\n        .false(log_message("Process failed :("))\n    )\n  \n    # With Lambda\n    (\n        If(lambda context: len(context.state.errors) == 0)\n        .true(log_message("Process successful :)"))\n        .false(log_message("Process failed :("))\n    )\n    ```\n  \n- `Switch`\n\n    Analogous with a `switch` statement found in many languages or with Python \n    a `dict` lookup with a default fallback.\n\n    Like the conditional node switch can accept a context variable or a \n    function/lambda that accepts a `WorkflowContext`, except returns any *hashable*\n    object.\n\n    ```python\n    # With context variable\n    (\n        Switch("my_var")\n        .case("foo", log_message("Found foo!"))\n        .case("bar", log_message("Found bar!"))\n        .default(log_message("Found neither."))\n    )\n  \n    # With Lambda\n    (\n        Switch(lambda context: context.state["my_var"])\n        .case("foo", log_message("Found foo!"))\n        .case("bar", log_message("Found bar!"))\n    )\n    ```\n  \n\n**Iteration**\n\n- `ForEach`\n    \n    Analogous with a `for` loop this node will iterate through a sequence and \n    call each of the child nodes.\n\n    All nodes within a for-each loop are in a nested context scope.\n    \n    ```python\n    # With a single target variable\n    (\n        ForEach("message", in_var="messages")\n        .loop(log_message("- {message}"))\n    )\n  \n    # With multiple target variables\n    (\n        ForEach("name, age", in_var="students")\n        .loop(log_message("- {name} is {age} years old."))\n    )\n    ```\n',
     'author': 'Tim Savage',
     'author_email': 'tim@savage.company',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/pyapp-org/pyapp-flow',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `pyapp-flow-0.8.0/PKG-INFO` & `pyapp-flow-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: pyapp-flow
-Version: 0.8.0
+Version: 0.9.0
 Summary: Application workflow framework
 Home-page: https://github.com/pyapp-org/pyapp-flow
 License: BSD-3-Clause
 Keywords: framework,application
 Author: Tim Savage
 Author-email: tim@savage.company
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: rich (>=12.4.4,<13.0.0)
```

