# Comparing `tmp/cognite_transformations_cli-2.3.6.tar.gz` & `tmp/cognite_transformations_cli-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_transformations_cli-2.3.6.tar", max compression
+gzip compressed data, was "cognite_transformations_cli-2.3.7.tar", max compression
```

## Comparing `cognite_transformations_cli-2.3.6.tar` & `cognite_transformations_cli-2.3.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10172 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/LICENSE
--rw-r--r--   0        0        0     4288 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/README.md
--rw-r--r--   0        0        0       22 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/__init__.py
--rw-r--r--   0        0        0      270 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/__main__.py
--rw-r--r--   0        0        0     1489 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/clients.py
--rw-r--r--   0        0        0        0 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/base.py
--rw-r--r--   0        0        0     1491 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/delete.py
--rw-r--r--   0        0        0        0 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/__init__.py
--rw-r--r--   0        0        0     6459 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/deploy.py
--rw-r--r--   0        0        0     6754 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/load_yaml.py
--rw-r--r--   0        0        0     4998 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_config.py
--rw-r--r--   0        0        0     4005 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types.py
--rw-r--r--   0        0        0     4705 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
--rw-r--r--   0        0        0    12780 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformations_api.py
--rw-r--r--   0        0        0     2166 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/jobs.py
--rw-r--r--   0        0        0     2438 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/list.py
--rw-r--r--   0        0        0     1242 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/query.py
--rw-r--r--   0        0        0     3639 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/run.py
--rw-r--r--   0        0        0     2787 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/show.py
--rw-r--r--   0        0        0     5792 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/utils.py
--rw-r--r--   0        0        0     1616 2023-05-12 09:48:30.489539 cognite_transformations_cli-2.3.6/pyproject.toml
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.6/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-05-23 12:19:49.876630 cognite_transformations_cli-2.3.7/LICENSE
+-rw-r--r--   0        0        0     4288 2023-05-23 12:19:49.876630 cognite_transformations_cli-2.3.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/__main__.py
+-rw-r--r--   0        0        0     1489 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/clients.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/base.py
+-rw-r--r--   0        0        0     1491 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/delete.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/__init__.py
+-rw-r--r--   0        0        0     6459 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/deploy.py
+-rw-r--r--   0        0        0     6754 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/load_yaml.py
+-rw-r--r--   0        0        0     4998 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformation_config.py
+-rw-r--r--   0        0        0     4005 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformation_types.py
+-rw-r--r--   0        0        0     4705 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
+-rw-r--r--   0        0        0    12723 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformations_api.py
+-rw-r--r--   0        0        0     2166 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/jobs.py
+-rw-r--r--   0        0        0     2438 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/list.py
+-rw-r--r--   0        0        0     1242 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/query.py
+-rw-r--r--   0        0        0     3639 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/run.py
+-rw-r--r--   0        0        0     2787 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/show.py
+-rw-r--r--   0        0        0     5792 2023-05-23 12:19:49.880630 cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/utils.py
+-rw-r--r--   0        0        0     1617 2023-05-23 12:19:49.884630 cognite_transformations_cli-2.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5475 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.7/PKG-INFO
```

### Comparing `cognite_transformations_cli-2.3.6/LICENSE` & `cognite_transformations_cli-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/README.md` & `cognite_transformations_cli-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/clients.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/clients.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/base.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/delete.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/deploy.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/load_yaml.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/load_yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_config.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformation_config.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformation_types.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformations_api.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/deploy/transformations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,15 @@
     OidcCredentials,
     Transformation,
     TransformationDestination,
     TransformationNotification,
     TransformationSchedule,
     TransformationUpdate,
 )
-from cognite.client.data_classes.transformations.common import (
-    EdgeType,
-    InstanceEdges,
-    InstanceNodes,
-    SequenceRows,
-    ViewInfo,
-)
+from cognite.client.data_classes.transformations.common import Edges, EdgeType, Nodes, SequenceRows, ViewInfo
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError, CogniteNotFoundError
 
 from cognite.transformations_cli.commands.deploy.transformation_types import (
     ActionType,
     AuthConfig,
     DestinationConfig,
     DestinationConfigType,
@@ -101,28 +95,28 @@
         view = None
         if destination.view:
             view = ViewInfo(
                 destination.view.space,
                 destination.view.external_id,
                 destination.view.version,
             )
-        return InstanceNodes(view, destination.instance_space)
+        return Nodes(view, destination.instance_space)
 
     elif isinstance(destination, InstanceEdgesDestinationConfig):
         view = None
         if destination.view:
             view = ViewInfo(
                 destination.view.space,
                 destination.view.external_id,
                 destination.view.version,
             )
         edge_type = None
         if destination.edge_type:
             edge_type = EdgeType(destination.edge_type.space, destination.edge_type.external_id)
-        return InstanceEdges(view, destination.instance_space, edge_type)
+        return Edges(view, destination.instance_space, edge_type)
 
     else:
         return TransformationDestination(destination.value)
 
 
 def to_query(conf_path: str, query: Union[str, QueryConfig]) -> str:
     try:
```

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/jobs.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/list.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/query.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/run.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/show.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/utils.py` & `cognite_transformations_cli-2.3.7/cognite/transformations_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.6/pyproject.toml` & `cognite_transformations_cli-2.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-transformations-cli"
-version = "2.3.6"
+version = "2.3.7"
 description = "A CLI for the Transformations service in CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>", "Emel Varol <emel.varol@cognite.com>", "Einar Marstrander Omang <einar.omang@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/transformations-cli"
 
 packages = [
@@ -26,15 +26,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.2"
 types-retry = "^0.1.5"
 tabulate = "^0.8.9"
 types-tabulate = "^0.8.3"
 sqlparse = "^0.4.2"
-cognite-sdk = "6.1.7"
+cognite-sdk = "6.1.10"
 regex = "^2021.11.10"
 dacite = "^1.6.0"
 python-dotenv = "^0.21.0"
 pyparsing = "^3.0.9"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `cognite_transformations_cli-2.3.6/PKG-INFO` & `cognite_transformations_cli-2.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cognite-transformations-cli
-Version: 2.3.6
+Version: 2.3.7
 Summary: A CLI for the Transformations service in CDF
 Home-page: https://github.com/cognitedata/transformations-cli
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0.2,<9.0.0)
-Requires-Dist: cognite-sdk (==6.1.7)
+Requires-Dist: cognite-sdk (==6.1.10)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: regex (>=2021.11.10,<2022.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: types-retry (>=0.1.5,<0.2.0)
```

