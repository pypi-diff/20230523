# Comparing `tmp/forestadmin_agent_toolkit-0.1.0b8.tar.gz` & `tmp/forestadmin_agent_toolkit-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-0.1.0b8.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-0.1.0b9.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-0.1.0b8.tar` & `forestadmin_agent_toolkit-0.1.0b9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/README.md
--rw-r--r--   0        0        0      190 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     3917 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0       57 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0      564 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2249 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     5919 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      427 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0      891 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0    13948 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    16998 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     2838 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0     9841 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5466 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0     9227 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      144 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     3928 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0     8382 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0      264 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     1660 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0     9301 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3289 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     1826 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3040 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     2942 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2236 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     4543 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0     1975 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     7732 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      485 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     2670 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1282 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     3329 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1685 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0      541 2022-12-07 16:06:23.356099 forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1625 2022-12-07 16:06:40.300316 forestadmin_agent_toolkit-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-0.1.0b8/setup.py
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/README.md
+-rw-r--r--   0        0        0      190 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     3917 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0       57 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0      564 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2249 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     5919 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      427 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0      891 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0    13948 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    16998 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     2838 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0     9841 2022-12-07 16:21:48.623912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5466 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0     9227 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      144 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     3928 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0     8382 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0      264 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     1660 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0     9301 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3289 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     1826 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3040 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     2942 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2236 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     4543 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0     1975 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     7732 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      485 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     2670 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1282 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     3329 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1685 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0      541 2022-12-07 16:21:48.627912 forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1625 2022-12-07 16:22:08.667917 forestadmin_agent_toolkit-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-0.1.0b9/setup.py
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-0.1.0b9/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/__init__.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/permissions/__init__.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-0.1.0b9/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-0.1.0b8/pyproject.toml` & `forestadmin_agent_toolkit-0.1.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
-version = "0.1.0-beta.8"
+version = "0.1.0-beta.9"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 tzdata = "~2022.6"
 aiohttp = "~=3.8"
 oic = "~=1.4"
 python-jose = ">=3.3, <4.0"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
-forestadmin-datasource-toolkit = "^0.1.0-beta.8"
+forestadmin-datasource-toolkit = "^0.1.0-beta.9"
 [[tool.poetry.dependencies.pandas]]
 version = "==1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
 version = "==1.3.5"
 python = ">=3.7.1,<3.8"
```

### Comparing `forestadmin_agent_toolkit-0.1.0b8/setup.py` & `forestadmin_agent_toolkit-0.1.0b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8,<4.0',
  'cachetools>=5.2,<6.0',
- 'forestadmin-datasource-toolkit>=0.1.0-beta.8,<0.2.0',
+ 'forestadmin-datasource-toolkit>=0.1.0-beta.9,<0.2.0',
  'marshmallow-jsonapi>=0.24.0,<1.0',
  'oic>=1.4,<2.0',
  'python-jose>=3.3,<4.0',
  'typing-extensions>=4.2.0,<5.0',
  'tzdata>=2022.6,<2022.7']
 
 extras_require = \
 {':python_full_version < "3.7.1"': ['pandas==1.1.5'],
  ':python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas==1.3.5'],
  ':python_version < "3.9"': ['backports.zoneinfo[tzdata]>=0.2.1,<0.3.0'],
  ':python_version >= "3.8"': ['pandas>=1.4.2,<1.5.0']}
 
 setup_kwargs = {
     'name': 'forestadmin-agent-toolkit',
-    'version': '0.1.0b8',
+    'version': '0.1.0b9',
     'description': '',
     'long_description': '',
     'author': 'Valentin Monté',
     'author_email': 'valentinm@forestadmin.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `forestadmin_agent_toolkit-0.1.0b8/PKG-INFO` & `forestadmin_agent_toolkit-0.1.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0); python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=0.1.0-beta.8,<0.2.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=0.1.0-beta.9,<0.2.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (==1.1.5); python_full_version < "3.7.1"
 Requires-Dist: pandas (==1.3.5); python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.2,<1.5.0); python_version >= "3.8"
 Requires-Dist: python-jose (>=3.3,<4.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
```

