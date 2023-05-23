# Comparing `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1553.tar.gz` & `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1567.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1553.tar", last modified: Fri May 19 00:30:26 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1567.tar", last modified: Tue May 23 16:52:48 2023, max compression
```

## Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553.tar` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-19 00:30:06.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 00:30:06.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-19 00:30:06.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-19 00:30:06.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/ext/workflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-19 00:30:26.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-19 00:30:06.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1553/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/dapr_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/dapr_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/workflow_activity_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/workflow_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/workflow_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-23 16:52:48.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-23 16:52:19.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1567/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/LICENSE` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1553
+Version: 0.0.1rc1.dev1567
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # Import your main classes here
-# from dapr.ext.workflow.creator import Creator, Workflow   # type:ignore
-
+from dapr.ext.workflow.workflow_runtime import WorkflowRuntime
+from dapr.ext.workflow.dapr_workflow_client import DaprWorkflowClient
+from dapr.ext.workflow.dapr_workflow_context import DaprWorkflowContext
+from dapr.ext.workflow.workflow_activity_context import WorkflowActivityContext
 
 __all__ = [
-    # 'Creator',
-    # 'Workflow',
+    'WorkflowRuntime',
+    'DaprWorkflowClient',
+    'DaprWorkflowContext',
+    'WorkflowActivityContext',
 ]
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr/ext/workflow/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1553
+Version: 0.0.1rc1.dev1567
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/setup.cfg` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 [options]
 python_requires = >=3.7
 packages = find_namespace:
 include_package_data = True
 install_requires = 
 	dapr-dev >= 1.9.0rc1.dev
+	durabletask >= 0.1.0a2
 
 [options.packages.find]
 include = 
 	dapr.*
 exclude = 
 	tests
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1553/setup.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1567/setup.py`

 * *Files identical despite different names*

