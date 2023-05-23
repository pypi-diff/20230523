# Comparing `tmp/watchmen_indicator_surface-16.5.1.tar.gz` & `tmp/watchmen_indicator_surface-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_surface-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_indicator_surface-16.5.2.tar", max compression
```

## Comparing `watchmen_indicator_surface-16.5.1.tar` & `watchmen_indicator_surface-16.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1025 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/data/__init__.py
--rw-r--r--   0        0        0     8930 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/data/objective_data_router.py
--rw-r--r--   0        0        0      541 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/main.py
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/__init__.py
--rw-r--r--   0        0        0     6015 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
--rw-r--r--   0        0        0     7181 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/bucket_router.py
--rw-r--r--   0        0        0     9217 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/derived_objective_router.py
--rw-r--r--   0        0        0     7904 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/indicator_router.py
--rw-r--r--   0        0        0    12699 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/objective_router.py
--rw-r--r--   0        0        0     5673 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/subject_router.py
--rw-r--r--   0        0        0      471 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/settings.py
--rw-r--r--   0        0        0       80 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/util/__init__.py
--rw-r--r--   0        0        0     2038 2023-04-25 10:52:45.984220 watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/util/trans.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-05-23 07:54:10.408670 watchmen_indicator_surface-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-05-23 07:54:10.408670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.408670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/data/__init__.py
+-rw-r--r--   0        0        0     8936 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/data/objective_data_router.py
+-rw-r--r--   0        0        0      541 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/main.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/__init__.py
+-rw-r--r--   0        0        0     6015 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
+-rw-r--r--   0        0        0     7181 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/bucket_router.py
+-rw-r--r--   0        0        0     9156 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/derived_objective_router.py
+-rw-r--r--   0        0        0     7904 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/indicator_router.py
+-rw-r--r--   0        0        0    12699 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/objective_router.py
+-rw-r--r--   0        0        0     5673 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/subject_router.py
+-rw-r--r--   0        0        0      471 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/settings.py
+-rw-r--r--   0        0        0       80 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/util/__init__.py
+-rw-r--r--   0        0        0     2038 2023-05-23 07:54:10.412670 watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/util/trans.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.2/PKG-INFO
```

### Comparing `watchmen_indicator_surface-16.5.1/pyproject.toml` & `watchmen_indicator_surface-16.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "watchmen-indicator-surface"
-version = "16.5.1"
+version = "16.5.2"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-indicator-kernel = "16.5.1"
-watchmen-rest = "16.5.1"
-watchmen-storage-mysql = { version = "16.5.1", optional = true }
-watchmen-storage-oracle = { version = "16.5.1", optional = true }
-watchmen-storage-mongodb = { version = "16.5.1", optional = true }
-watchmen-storage-mssql = { version = "16.5.1", optional = true }
-watchmen-storage-postgresql = { version = "16.5.1", optional = true }
+watchmen-indicator-kernel = "16.5.2"
+watchmen-rest = "16.5.2"
+watchmen-storage-mysql = { version = "16.5.2", optional = true }
+watchmen-storage-oracle = { version = "16.5.2", optional = true }
+watchmen-storage-mongodb = { version = "16.5.2", optional = true }
+watchmen-storage-mssql = { version = "16.5.2", optional = true }
+watchmen-storage-postgresql = { version = "16.5.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/data/objective_data_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/data/objective_data_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 	for objective_factor in objective.factors:
 		if objective_factor.uuid == objective_factor_id:
 			return objective_factor
 
 
 @router.post("/indicator/derived-objective/breakdown/data", tags=[UserRole.ADMIN],
              response_model=ObjectiveTargetBreakdownValues)
-def load_objective_target_breakdown_values(breakdown_request: ObjectiveBreakdownRequest,
+async def load_objective_target_breakdown_values(breakdown_request: ObjectiveBreakdownRequest,
                                            principal_service: PrincipalService = Depends(
 	                                           get_admin_principal)) -> ObjectiveTargetBreakdownValues:
 	objective_target = breakdown_request.target
 	objective = breakdown_request.objective
 	breakdown_target = breakdown_request.breakdown
 
 	if objective.tenantId != principal_service.get_tenant_id():
```

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/main.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/bucket_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/bucket_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/derived_objective_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/derived_objective_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,14 @@
 		raise_404('Not Found')
 
 	if is_blank(derived_objective_id):
 		raise_400('Derived objective id is required.')
 
 	derived_objective_service = get_derived_objective_service(principal_service)
 
-	# noinspection DuplicatedCode
 	def action() -> DerivedObjective:
 		# noinspection PyTypeChecker
 		existing_derived_objective: Optional[DerivedObjective] = \
 			derived_objective_service.find_by_id(derived_objective_id)
 		if existing_derived_objective is None:
 			raise_404()
 		derived_objective_service.delete(derived_objective_id)
@@ -199,15 +198,15 @@
 def load_share_derived_objective_by_id_and_token(derived_objective_id:DerivedObjectiveId,token:str)->DerivedObjective:
 
 	principal_service: PrincipalService = get_principal_by_jwt(
 		retrieve_authentication_manager(), token, [UserRole.CONSOLE, UserRole.ADMIN])
 
 	derived_objective_service = get_derived_objective_service(principal_service)
 	def action() -> DerivedObjective:
-		# noinspection PyTypeChecker
+
 		existing_derived_objective: Optional[DerivedObjective] = \
 			derived_objective_service.find_by_id(derived_objective_id)
 		if existing_derived_objective is None:
 			raise_404()
 		return existing_derived_objective
 
 	return trans_readonly(derived_objective_service, action)
```

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/indicator_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/indicator_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/objective_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/meta/subject_router.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/meta/subject_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/src/watchmen_indicator_surface/util/trans.py` & `watchmen_indicator_surface-16.5.2/src/watchmen_indicator_surface/util/trans.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.1/PKG-INFO` & `watchmen_indicator_surface-16.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-surface
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
-Requires-Dist: watchmen-indicator-kernel (==16.5.1)
-Requires-Dist: watchmen-rest (==16.5.1)
-Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
+Requires-Dist: watchmen-indicator-kernel (==16.5.2)
+Requires-Dist: watchmen-rest (==16.5.2)
+Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
```

