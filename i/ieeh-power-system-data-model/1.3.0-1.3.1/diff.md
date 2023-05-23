# Comparing `tmp/ieeh-power-system-data-model-1.3.0.tar.gz` & `tmp/ieeh-power-system-data-model-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-power-system-data-model-1.3.0.tar", last modified: Fri May  5 11:06:33 2023, max compression
+gzip compressed data, was "ieeh-power-system-data-model-1.3.1.tar", last modified: Tue May 23 12:26:16 2023, max compression
```

## Comparing `ieeh-power-system-data-model-1.3.0.tar` & `ieeh-power-system-data-model-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      348 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/LICENSE
--rw-r--r--   0        0        0     2680 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/README.md
--rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/base.py
--rw-r--r--   0        0        0      579 2023-05-05 11:06:26.610995 ieeh-power-system-data-model-1.3.0/psdm/meta.py
--rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/__init__.py
--rw-r--r--   0        0        0     1047 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/active_power.py
--rw-r--r--   0        0        0     3880 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/case.py
--rw-r--r--   0        0        0     5062 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/controller.py
--rw-r--r--   0        0        0      432 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/external_grid.py
--rw-r--r--   0        0        0      539 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/load.py
--rw-r--r--   0        0        0     1091 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/reactive_power.py
--rw-r--r--   0        0        0      367 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/transformer.py
--rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/__init__.py
--rw-r--r--   0        0        0      491 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/active_power.py
--rw-r--r--   0        0        0     1931 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/branch.py
--rw-r--r--   0        0        0      337 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/characteristic.py
--rw-r--r--   0        0        0      364 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/coupler.py
--rw-r--r--   0        0        0      697 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/external_grid.py
--rw-r--r--   0        0        0     3739 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/load.py
--rw-r--r--   0        0        0     1694 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/load_model.py
--rw-r--r--   0        0        0      320 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/node.py
--rw-r--r--   0        0        0      486 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/reactive_power.py
--rw-r--r--   0        0        0      363 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/switch.py
--rw-r--r--   0        0        0     1011 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/topology.py
--rw-r--r--   0        0        0     2351 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/transformer.py
--rw-r--r--   0        0        0     1081 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/windings.py
--rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology_case/__init__.py
--rw-r--r--   0        0        0      501 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology_case/case.py
--rw-r--r--   0        0        0      399 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology_case/element_state.py
--rw-r--r--   0        0        0     2658 2023-05-05 11:06:26.634995 ieeh-power-system-data-model-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1441 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_active_power.py
--rw-r--r--   0        0        0      659 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_branch.py
--rw-r--r--   0        0        0     8953 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_controller.py
--rw-r--r--   0        0        0     1449 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_reactive_power.py
--rw-r--r--   0        0        0     1606 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_topology_load.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2680 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/README.md
+-rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/base.py
+-rw-r--r--   0        0        0      579 2023-05-23 12:26:07.077182 ieeh-power-system-data-model-1.3.1/psdm/meta.py
+-rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/__init__.py
+-rw-r--r--   0        0        0     1047 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/active_power.py
+-rw-r--r--   0        0        0     3880 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/case.py
+-rw-r--r--   0        0        0     5062 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/controller.py
+-rw-r--r--   0        0        0      432 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/external_grid.py
+-rw-r--r--   0        0        0      539 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/load.py
+-rw-r--r--   0        0        0     1091 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/reactive_power.py
+-rw-r--r--   0        0        0      367 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/transformer.py
+-rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/active_power.py
+-rw-r--r--   0        0        0     1931 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/branch.py
+-rw-r--r--   0        0        0      337 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/characteristic.py
+-rw-r--r--   0        0        0      364 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/coupler.py
+-rw-r--r--   0        0        0      697 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/external_grid.py
+-rw-r--r--   0        0        0     3739 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/load.py
+-rw-r--r--   0        0        0     1409 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/load_model.py
+-rw-r--r--   0        0        0      320 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/node.py
+-rw-r--r--   0        0        0      486 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/reactive_power.py
+-rw-r--r--   0        0        0      363 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/switch.py
+-rw-r--r--   0        0        0     1011 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/topology.py
+-rw-r--r--   0        0        0     2351 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/transformer.py
+-rw-r--r--   0        0        0     1081 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology/windings.py
+-rw-r--r--   0        0        0        1 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology_case/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology_case/case.py
+-rw-r--r--   0        0        0      399 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/psdm/topology_case/element_state.py
+-rw-r--r--   0        0        0     2686 2023-05-23 12:26:07.109185 ieeh-power-system-data-model-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1441 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_active_power.py
+-rw-r--r--   0        0        0      659 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_branch.py
+-rw-r--r--   0        0        0     8953 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_controller.py
+-rw-r--r--   0        0        0     1449 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_reactive_power.py
+-rw-r--r--   0        0        0     1606 2023-05-23 12:25:00.208428 ieeh-power-system-data-model-1.3.1/tests/test_topology_load.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.3.1/PKG-INFO
```

### Comparing `ieeh-power-system-data-model-1.3.0/LICENSE` & `ieeh-power-system-data-model-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/README.md` & `ieeh-power-system-data-model-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/base.py` & `ieeh-power-system-data-model-1.3.1/psdm/base.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/meta.py` & `ieeh-power-system-data-model-1.3.1/psdm/meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import datetime
 import uuid
 
 import pydantic
 
 from psdm.base import Base
 
-VERSION = "1.3.0"
+VERSION = "1.3.1"
 
 
 class Meta(Base):
     version = VERSION
     name: str
     date: datetime.date  # date of export
     id: uuid.UUID = pydantic.Field(default_factory=uuid.uuid4)  # noqa: A003
```

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/active_power.py` & `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/case.py` & `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/case.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/controller.py` & `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/load.py` & `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/reactive_power.py` & `ieeh-power-system-data-model-1.3.1/psdm/steadystate_case/reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/topology/branch.py` & `ieeh-power-system-data-model-1.3.1/psdm/topology/branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/topology/external_grid.py` & `ieeh-power-system-data-model-1.3.1/psdm/topology/external_grid.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/topology/load.py` & `ieeh-power-system-data-model-1.3.1/psdm/topology/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/topology/topology.py` & `ieeh-power-system-data-model-1.3.1/psdm/topology/topology.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/topology/transformer.py` & `ieeh-power-system-data-model-1.3.1/psdm/topology/transformer.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/psdm/topology/windings.py` & `ieeh-power-system-data-model-1.3.1/psdm/topology/windings.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/pyproject.toml` & `ieeh-power-system-data-model-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "loguru",
     "pydantic",
 ]
 description = "A data model for describing power systems"
 name = "ieeh-power-system-data-model"
 readme = "README.md"
 requires-python = ">=3.10,<3.11"
-version = "1.3.0"
+version = "1.3.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/power-system-data-model"
 
@@ -101,16 +101,17 @@
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.3.0"
+version = "1.3.1"
 version_files = [
+    ".zenodo.json:version",
     "CITATION.cff:cff-version",
     "psdm/meta.py:VERSION",
     "pyproject.toml:version",
 ]
 
 [tool.mypy]
 follow_imports = "normal"
```

### Comparing `ieeh-power-system-data-model-1.3.0/tests/test_active_power.py` & `ieeh-power-system-data-model-1.3.1/tests/test_active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/tests/test_branch.py` & `ieeh-power-system-data-model-1.3.1/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/tests/test_controller.py` & `ieeh-power-system-data-model-1.3.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/tests/test_reactive_power.py` & `ieeh-power-system-data-model-1.3.1/tests/test_reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/tests/test_topology_load.py` & `ieeh-power-system-data-model-1.3.1/tests/test_topology_load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.3.0/PKG-INFO` & `ieeh-power-system-data-model-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeh-power-system-data-model
-Version: 1.3.0
+Version: 1.3.1
 Summary: A data model for describing power systems
 Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Laura Fiedler <laura.fiedler1@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 Requires-Python: >=3.10,<3.11
 Project-URL: Source, https://github.com/ieeh-tu-dresden/power-system-data-model
 Description-Content-Type: text/markdown
 
 # IEEH Power System Data Model
```

