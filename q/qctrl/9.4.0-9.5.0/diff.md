# Comparing `tmp/qctrl-9.4.0.tar.gz` & `tmp/qctrl-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl-9.4.0.tar", last modified: Mon Mar 22 00:50:48 2021, max compression
+gzip compressed data, was "qctrl-9.5.0.tar", last modified: Mon Mar 22 22:52:01 2021, max compression
```

## Comparing `qctrl-9.4.0.tar` & `qctrl-9.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      277 2021-03-22 00:49:48.572430 qctrl-9.4.0/DESCRIPTION.md
--rw-r--r--   0        0        0    34692 2021-03-22 00:49:48.572430 qctrl-9.4.0/LICENSE
--rw-r--r--   0        0        0     2850 2021-03-22 00:50:08.725855 qctrl-9.4.0/pyproject.toml
--rw-r--r--   0        0        0      686 2021-03-22 00:50:08.753857 qctrl-9.4.0/qctrl/__init__.py
--rw-r--r--   0        0        0     3044 2021-03-22 00:50:08.753857 qctrl-9.4.0/qctrl/builders/__init__.py
--rw-r--r--   0        0        0     2808 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/async_result.py
--rw-r--r--   0        0        0     6887 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/client_builder.py
--rw-r--r--   0        0        0     6127 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_environment.py
--rw-r--r--   0        0        0     1155 2021-03-22 00:50:08.737856 qctrl-9.4.0/qctrl/builders/custom_handlers/__init__.py
--rw-r--r--   0        0        0      993 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_handlers/complex_array_entry_handler.py
--rw-r--r--   0        0        0     1859 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_handlers/complex_array_handler.py
--rw-r--r--   0        0        0     1346 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_handlers/complex_array_input_handler.py
--rw-r--r--   0        0        0     1129 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_handlers/complex_number_handler.py
--rw-r--r--   0        0        0     1666 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_handlers/complex_number_input_handler.py
--rw-r--r--   0        0        0     2951 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/custom_handlers/scalars.py
--rw-r--r--   0        0        0    13487 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/doc.py
--rw-r--r--   0        0        0     8452 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/functions.py
--rw-r--r--   0        0        0      741 2021-03-22 00:50:08.749857 qctrl-9.4.0/qctrl/builders/graphql_utils/__init__.py
--rw-r--r--   0        0        0     1191 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/base_type_registry.py
--rw-r--r--   0        0        0     6531 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/environment.py
--rw-r--r--   0        0        0     1100 2021-03-22 00:50:08.749857 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/__init__.py
--rw-r--r--   0        0        0     1380 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/base.py
--rw-r--r--   0        0        0     1624 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/enum_handler.py
--rw-r--r--   0        0        0     2594 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/input_object_handler.py
--rw-r--r--   0        0        0     1553 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/list_handler.py
--rw-r--r--   0        0        0     8190 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/mixins.py
--rw-r--r--   0        0        0     1591 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/non_null_handler.py
--rw-r--r--   0        0        0     5879 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/object_handler.py
--rw-r--r--   0        0        0     1598 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/scalar_handler.py
--rw-r--r--   0        0        0     2962 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/union_handler.py
--rw-r--r--   0        0        0     4760 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/http_transport.py
--rw-r--r--   0        0        0     6175 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/namespaces.py
--rw-r--r--   0        0        0     1766 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/result_mixin.py
--rw-r--r--   0        0        0    12442 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/type_registry.py
--rw-r--r--   0        0        0      288 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/utils.py
--rw-r--r--   0        0        0     2563 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/builders/wait.py
--rw-r--r--   0        0        0      659 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/constants.py
--rw-r--r--   0        0        0     1985 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/dynamic.py
--rw-r--r--   0        0        0     7333 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/qctrl.py
--rw-r--r--   0        0        0      849 2021-03-22 00:50:08.733856 qctrl-9.4.0/qctrl/queries/__init__.py
--rw-r--r--   0        0        0     3242 2021-03-22 00:49:48.572430 qctrl-9.4.0/qctrl/queries/action_export.py
--rw-r--r--   0        0        0     5531 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/activity_monitor.py
--rw-r--r--   0        0        0     2006 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/base.py
--rw-r--r--   0        0        0     2634 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/create_token.py
--rw-r--r--   0        0        0     5793 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/get_environment.py
--rw-r--r--   0        0        0     3903 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/get_result.py
--rw-r--r--   0        0        0     1930 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/me.py
--rw-r--r--   0        0        0     2680 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/queries/refresh_token.py
--rw-r--r--   0        0        0    11658 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/scripts.py
--rw-r--r--   0        0        0     5664 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/scripts_utils.py
--rw-r--r--   0        0        0     6682 2021-03-22 00:49:48.576430 qctrl-9.4.0/qctrl/utils.py
--rw-r--r--   0        0        0     1525 2021-03-22 00:50:48.779819 qctrl-9.4.0/setup.py
--rw-r--r--   0        0        0     2412 2021-03-22 00:50:48.780135 qctrl-9.4.0/PKG-INFO
+-rw-r--r--   0        0        0      277 2021-03-22 22:51:01.666052 qctrl-9.5.0/DESCRIPTION.md
+-rw-r--r--   0        0        0    34692 2021-03-22 22:51:01.670052 qctrl-9.5.0/LICENSE
+-rw-r--r--   0        0        0     2850 2021-03-22 22:51:21.515596 qctrl-9.5.0/pyproject.toml
+-rw-r--r--   0        0        0      686 2021-03-22 22:51:21.535598 qctrl-9.5.0/qctrl/__init__.py
+-rw-r--r--   0        0        0     3044 2021-03-22 22:51:21.535598 qctrl-9.5.0/qctrl/builders/__init__.py
+-rw-r--r--   0        0        0     2808 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/async_result.py
+-rw-r--r--   0        0        0     6887 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/client_builder.py
+-rw-r--r--   0        0        0     6127 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_environment.py
+-rw-r--r--   0        0        0     1155 2021-03-22 22:51:21.531597 qctrl-9.5.0/qctrl/builders/custom_handlers/__init__.py
+-rw-r--r--   0        0        0      993 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_handlers/complex_array_entry_handler.py
+-rw-r--r--   0        0        0     1859 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_handlers/complex_array_handler.py
+-rw-r--r--   0        0        0     1346 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_handlers/complex_array_input_handler.py
+-rw-r--r--   0        0        0     1129 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_handlers/complex_number_handler.py
+-rw-r--r--   0        0        0     1666 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_handlers/complex_number_input_handler.py
+-rw-r--r--   0        0        0     2951 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/custom_handlers/scalars.py
+-rw-r--r--   0        0        0    13487 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/doc.py
+-rw-r--r--   0        0        0     8452 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/functions.py
+-rw-r--r--   0        0        0      741 2021-03-22 22:51:21.535598 qctrl-9.5.0/qctrl/builders/graphql_utils/__init__.py
+-rw-r--r--   0        0        0     1191 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/base_type_registry.py
+-rw-r--r--   0        0        0     6531 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/environment.py
+-rw-r--r--   0        0        0     1100 2021-03-22 22:51:21.531597 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/__init__.py
+-rw-r--r--   0        0        0     1380 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/base.py
+-rw-r--r--   0        0        0     1624 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/enum_handler.py
+-rw-r--r--   0        0        0     2594 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/input_object_handler.py
+-rw-r--r--   0        0        0     1553 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/list_handler.py
+-rw-r--r--   0        0        0     8190 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/mixins.py
+-rw-r--r--   0        0        0     1591 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/non_null_handler.py
+-rw-r--r--   0        0        0     5879 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/object_handler.py
+-rw-r--r--   0        0        0     1598 2021-03-22 22:51:01.670052 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/scalar_handler.py
+-rw-r--r--   0        0        0     2962 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/union_handler.py
+-rw-r--r--   0        0        0     4760 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/http_transport.py
+-rw-r--r--   0        0        0     6175 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/namespaces.py
+-rw-r--r--   0        0        0     1766 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/result_mixin.py
+-rw-r--r--   0        0        0    12442 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/type_registry.py
+-rw-r--r--   0        0        0      288 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/utils.py
+-rw-r--r--   0        0        0     2563 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/builders/wait.py
+-rw-r--r--   0        0        0      659 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/constants.py
+-rw-r--r--   0        0        0     1985 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/dynamic.py
+-rw-r--r--   0        0        0     7333 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/qctrl.py
+-rw-r--r--   0        0        0      849 2021-03-22 22:51:21.531597 qctrl-9.5.0/qctrl/queries/__init__.py
+-rw-r--r--   0        0        0     3242 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/action_export.py
+-rw-r--r--   0        0        0     5531 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/activity_monitor.py
+-rw-r--r--   0        0        0     2006 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/base.py
+-rw-r--r--   0        0        0     2634 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/create_token.py
+-rw-r--r--   0        0        0     5793 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/get_environment.py
+-rw-r--r--   0        0        0     3903 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/get_result.py
+-rw-r--r--   0        0        0     1930 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/me.py
+-rw-r--r--   0        0        0     2680 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/queries/refresh_token.py
+-rw-r--r--   0        0        0    11658 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/scripts.py
+-rw-r--r--   0        0        0     5664 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/scripts_utils.py
+-rw-r--r--   0        0        0     6682 2021-03-22 22:51:01.674053 qctrl-9.5.0/qctrl/utils.py
+-rw-r--r--   0        0        0     1525 2021-03-22 22:52:01.708243 qctrl-9.5.0/setup.py
+-rw-r--r--   0        0        0     2412 2021-03-22 22:52:01.708678 qctrl-9.5.0/PKG-INFO
```

### Comparing `qctrl-9.4.0/LICENSE` & `qctrl-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/pyproject.toml` & `qctrl-9.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl"
-version = "9.4.0"
+version = "9.5.0"
 description = "Q-CTRL Python"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "DESCRIPTION.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -45,15 +45,15 @@
 gql = "3.0.0a4"
 requests = "^2.23.0"
 tenacity = "^6.0.0"
 attrs = "^19.3.0"
 cached-property = "^1.5.1"
 commonmark = "~0.9.1"
 pytz = "^2020.1"
-qctrl-commons = "~5.0.0"
+qctrl-commons = "~5.1.0"
 python-dateutil = "^2.8.1"
 jsonschema = "^3.2.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest-mock = "^1.4.0"
 pytest = "^5.0.1"
```

### Comparing `qctrl-9.4.0/qctrl/__init__.py` & `qctrl-9.5.0/qctrl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """The main qctrl namespace."""
 
-__version__ = "9.4.0"
+__version__ = "9.5.0"
 
 from .qctrl import Qctrl  # pylint:disable=cyclic-import
```

### Comparing `qctrl-9.4.0/qctrl/builders/__init__.py` & `qctrl-9.5.0/qctrl/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/async_result.py` & `qctrl-9.5.0/qctrl/builders/async_result.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/client_builder.py` & `qctrl-9.5.0/qctrl/builders/client_builder.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_environment.py` & `qctrl-9.5.0/qctrl/builders/custom_environment.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/__init__.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/complex_array_entry_handler.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/complex_array_entry_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/complex_array_handler.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/complex_array_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/complex_array_input_handler.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/complex_array_input_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/complex_number_handler.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/complex_number_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/complex_number_input_handler.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/complex_number_input_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/custom_handlers/scalars.py` & `qctrl-9.5.0/qctrl/builders/custom_handlers/scalars.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/doc.py` & `qctrl-9.5.0/qctrl/builders/doc.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/functions.py` & `qctrl-9.5.0/qctrl/builders/functions.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/__init__.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/base_type_registry.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/base_type_registry.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/environment.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/environment.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/__init__.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/base.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/base.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/enum_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/enum_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/input_object_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/input_object_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/list_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/list_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/mixins.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/mixins.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/non_null_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/non_null_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/object_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/object_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/scalar_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/scalar_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/graphql_utils/handlers/union_handler.py` & `qctrl-9.5.0/qctrl/builders/graphql_utils/handlers/union_handler.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/http_transport.py` & `qctrl-9.5.0/qctrl/builders/http_transport.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/namespaces.py` & `qctrl-9.5.0/qctrl/builders/namespaces.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/result_mixin.py` & `qctrl-9.5.0/qctrl/builders/result_mixin.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/type_registry.py` & `qctrl-9.5.0/qctrl/builders/type_registry.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/builders/wait.py` & `qctrl-9.5.0/qctrl/builders/wait.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/constants.py` & `qctrl-9.5.0/qctrl/constants.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/dynamic.py` & `qctrl-9.5.0/qctrl/dynamic.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/qctrl.py` & `qctrl-9.5.0/qctrl/qctrl.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/__init__.py` & `qctrl-9.5.0/qctrl/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/action_export.py` & `qctrl-9.5.0/qctrl/queries/action_export.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/activity_monitor.py` & `qctrl-9.5.0/qctrl/queries/activity_monitor.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/base.py` & `qctrl-9.5.0/qctrl/queries/base.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/create_token.py` & `qctrl-9.5.0/qctrl/queries/create_token.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/get_environment.py` & `qctrl-9.5.0/qctrl/queries/get_environment.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/get_result.py` & `qctrl-9.5.0/qctrl/queries/get_result.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/me.py` & `qctrl-9.5.0/qctrl/queries/me.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/queries/refresh_token.py` & `qctrl-9.5.0/qctrl/queries/refresh_token.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/scripts.py` & `qctrl-9.5.0/qctrl/scripts.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/scripts_utils.py` & `qctrl-9.5.0/qctrl/scripts_utils.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/qctrl/utils.py` & `qctrl-9.5.0/qctrl/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl-9.4.0/setup.py` & `qctrl-9.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,26 +19,26 @@
  'commonmark>=0.9.1,<0.10.0',
  'gql==3.0.0a4',
  'jsonschema>=3.2.0,<4.0.0',
  'numpy>=1.16.2',
  'python-dateutil>=2.8.1,<3.0.0',
  'python-forge>=18.6.0,<19.0.0',
  'pytz>=2020.1,<2021.0',
- 'qctrl-commons>=5.0.0,<5.1.0',
+ 'qctrl-commons>=5.1.0,<5.2.0',
  'requests>=2.23.0,<3.0.0',
  'tenacity>=6.0.0,<7.0.0',
  'toml>=0.10.0,<0.11.0',
  'tqdm>=4.30.0']
 
 entry_points = \
 {'console_scripts': ['qctrl = qctrl.scripts:main']}
 
 setup_kwargs = {
     'name': 'qctrl',
-    'version': '9.4.0',
+    'version': '9.5.0',
     'description': 'Q-CTRL Python',
     'long_description': "# Q-CTRL Python\n\nThe Q-CTRL Python Package provides an intuitive and convenient Python interface\nto Q-CTRL's quantum control solutions for customers of Q-CTRL. To use the Q-CTRL\nPython Package, you will need a\n[BOULDER OPAL](https://q-ctrl.com/products/boulder-opal/) account.\n",
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
```

### Comparing `qctrl-9.4.0/PKG-INFO` & `qctrl-9.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl
-Version: 9.4.0
+Version: 9.5.0
 Summary: Q-CTRL Python
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: q-ctrl,qctrl,quantum control
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -33,15 +33,15 @@
 Requires-Dist: commonmark (>=0.9.1,<0.10.0)
 Requires-Dist: gql (==3.0.0a4)
 Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
 Requires-Dist: numpy (>=1.16.2)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: python-forge (>=18.6.0,<19.0.0)
 Requires-Dist: pytz (>=2020.1,<2021.0)
-Requires-Dist: qctrl-commons (>=5.0.0,<5.1.0)
+Requires-Dist: qctrl-commons (>=5.1.0,<5.2.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tenacity (>=6.0.0,<7.0.0)
 Requires-Dist: toml (>=0.10.0,<0.11.0)
 Requires-Dist: tqdm (>=4.30.0)
 Project-URL: Documentation, https://docs.q-ctrl.com/references/python/qctrl
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
```

