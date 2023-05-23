# Comparing `tmp/watchmen_indicator_kernel-16.5.1.tar.gz` & `tmp/watchmen_indicator_kernel-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_kernel-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_indicator_kernel-16.5.2.tar", max compression
```

## Comparing `watchmen_indicator_kernel-16.5.1.tar` & `watchmen_indicator_kernel-16.5.2.tar`

### file list

```diff
@@ -1,39 +1,34 @@
--rw-r--r--   0        0        0     1281 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/__init__.py
--rw-r--r--   0        0        0       86 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/common/__init__.py
--rw-r--r--   0        0        0       49 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/common/exception.py
--rw-r--r--   0        0        0      329 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/common/settings.py
--rw-r--r--   0        0        0      286 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/__init__.py
--rw-r--r--   0        0        0       53 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/data_helper.py
--rw-r--r--   0        0        0     4327 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/inspection_data_service.py
--rw-r--r--   0        0        0    11588 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/subject_base_service.py
--rw-r--r--   0        0        0    19385 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/topic_base_service.py
--rw-r--r--   0        0        0      140 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/__init__.py
--rw-r--r--   0        0        0      313 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/data_helper.py
--rw-r--r--   0        0        0    27145 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/data_service.py
--rw-r--r--   0        0        0       59 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
--rw-r--r--   0        0        0    11941 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
--rw-r--r--   0        0        0    21400 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
--rw-r--r--   0        0        0    10799 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
--rw-r--r--   0        0        0     8341 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
--rw-r--r--   0        0        0      397 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/bucket.py
--rw-r--r--   0        0        0      979 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/derived_objective.py
--rw-r--r--   0        0        0     1051 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/enum.py
--rw-r--r--   0        0        0      284 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/factor.py
--rw-r--r--   0        0        0     1330 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/indicator.py
--rw-r--r--   0        0        0     3110 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/parameter.py
--rw-r--r--   0        0        0      786 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/subject.py
--rw-r--r--   0        0        0    12305 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/time_frame.py
--rw-r--r--   0        0        0     1074 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/topic.py
--rw-r--r--   0        0        0      268 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1762 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/achievement_task_service.py
--rw-r--r--   0        0        0     8647 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/bucket_service.py
--rw-r--r--   0        0        0     4960 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/derived_objective_service.py
--rw-r--r--   0        0        0     6695 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/indicator_service.py
--rw-r--r--   0        0        0     5783 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/objective_service.py
--rw-r--r--   0        0        0       46 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/plugin/__init__.py
--rw-r--r--   0        0        0      678 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/plugin/connector.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1281 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/__init__.py
+-rw-r--r--   0        0        0       86 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/common/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/common/exception.py
+-rw-r--r--   0        0        0      329 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/common/settings.py
+-rw-r--r--   0        0        0      286 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective/data_helper.py
+-rw-r--r--   0        0        0    27145 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective/data_service.py
+-rw-r--r--   0        0        0       59 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
+-rw-r--r--   0        0        0    11941 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
+-rw-r--r--   0        0        0    21400 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
+-rw-r--r--   0        0        0    10799 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
+-rw-r--r--   0        0        0     8341 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
+-rw-r--r--   0        0        0      397 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/bucket.py
+-rw-r--r--   0        0        0      979 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/derived_objective.py
+-rw-r--r--   0        0        0     1051 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/enum.py
+-rw-r--r--   0        0        0      284 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/factor.py
+-rw-r--r--   0        0        0     1330 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/indicator.py
+-rw-r--r--   0        0        0     3110 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/parameter.py
+-rw-r--r--   0        0        0      786 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/subject.py
+-rw-r--r--   0        0        0    12305 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/time_frame.py
+-rw-r--r--   0        0        0     1074 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/topic.py
+-rw-r--r--   0        0        0      268 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1762 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/achievement_task_service.py
+-rw-r--r--   0        0        0     8647 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/bucket_service.py
+-rw-r--r--   0        0        0     4960 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/derived_objective_service.py
+-rw-r--r--   0        0        0     6695 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/indicator_service.py
+-rw-r--r--   0        0        0     5783 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/objective_service.py
+-rw-r--r--   0        0        0       46 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/plugin/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-23 07:54:10.408670 watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/plugin/connector.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.5.2/PKG-INFO
```

### Comparing `watchmen_indicator_kernel-16.5.1/pyproject.toml` & `watchmen_indicator_kernel-16.5.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-indicator-kernel"
-version = "16.5.1"
+version = "16.5.2"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.1"
-watchmen-inquiry-trino = { version = "16.5.1", optional = true }
-watchmen-storage-mysql = { version = "16.5.1", optional = true }
-watchmen-storage-oracle = { version = "16.5.1", optional = true }
-watchmen-storage-mongodb = { version = "16.5.1", optional = true }
-watchmen-storage-mssql = { version = "16.5.1", optional = true }
-watchmen-storage-postgresql = { version = "16.5.1", optional = true }
-watchmen-storage-oss = { version = "16.5.1", optional = true }
-watchmen-storage-s3 = { version = "16.5.1", optional = true }
+watchmen-inquiry-kernel = "16.5.2"
+watchmen-inquiry-trino = { version = "16.5.2", optional = true }
+watchmen-storage-mysql = { version = "16.5.2", optional = true }
+watchmen-storage-oracle = { version = "16.5.2", optional = true }
+watchmen-storage-mongodb = { version = "16.5.2", optional = true }
+watchmen-storage-mssql = { version = "16.5.2", optional = true }
+watchmen-storage-postgresql = { version = "16.5.2", optional = true }
+watchmen-storage-oss = { version = "16.5.2", optional = true }
+watchmen-storage-s3 = { version = "16.5.2", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/data_helper.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,56 @@
-from datetime import datetime
-
 from watchmen_auth import PrincipalService
-from .inspection_data_service import InspectionDataService
+from watchmen_indicator_kernel.common import IndicatorKernelException
+from watchmen_model.common import SubjectId, TopicId
+from watchmen_model.indicator import Indicator, IndicatorBaseOn, Objective, ObjectiveFactorOnIndicator
+from watchmen_utilities import is_blank, is_not_blank
+from .data_service import ObjectiveFactorDataService
+from .subject_base_service import SubjectBaseObjectiveFactorDataService
+from .topic_base_service import TopicBaseObjectiveFactorDataService
+from ..utils import ask_indicator, ask_subject, ask_topic
+
+
+def get_topic_base_service(
+		objective: Objective, objective_factor: ObjectiveFactorOnIndicator, indicator: Indicator, topic_id: TopicId,
+		principal_service: PrincipalService
+) -> TopicBaseObjectiveFactorDataService:
+	topic = ask_topic(topic_id, principal_service)
+	return TopicBaseObjectiveFactorDataService(objective, objective_factor, indicator, topic, principal_service)
+
+
+def get_subject_base_service(
+		objective: Objective, objective_factor: ObjectiveFactorOnIndicator, indicator: Indicator, subject_id: SubjectId,
+		principal_service: PrincipalService
+) -> SubjectBaseObjectiveFactorDataService:
+	subject = ask_subject(subject_id, principal_service)
+	return SubjectBaseObjectiveFactorDataService(objective, objective_factor, indicator, subject, principal_service)
 
 
-# def get_topic_base_service(
-# 		inspection: Inspection, indicator: Indicator, topic_id: TopicId,
-# 		dt: datetime,
-# 		principal_service: PrincipalService
-# ) -> TopicBaseInspectionDataService:
-# 	topic = ask_topic(topic_id, principal_service)
-# 	clone_inspection = redress_inspection(inspection, topic, dt, principal_service)
-# 	return TopicBaseInspectionDataService(clone_inspection, indicator, topic, principal_service)
-#
-#
-# def get_subject_base_service(
-# 		inspection: Inspection, indicator: Indicator, subject_id: SubjectId,
-# 		dt: datetime,
-# 		principal_service: PrincipalService
-# ) -> SubjectBaseInspectionDataService:
-# 	subject = ask_subject(subject_id, principal_service)
-# 	clone_inspection = redress_inspection(inspection, subject, dt, principal_service)
-# 	return SubjectBaseInspectionDataService(clone_inspection, indicator, subject, principal_service)
 
-# TODO REFACTOR-OBJECTIVE ACHIEVEMENT BREAK DOWN DATA SERVICE, ENTRYPOINT
-def get_inspection_data_service(dt: datetime, principal_service: PrincipalService) -> InspectionDataService:
+
+
+def get_objective_factor_data_service(
+		objective: Objective, objective_factor: ObjectiveFactorOnIndicator, principal_service: PrincipalService
+) -> ObjectiveFactorDataService:
 	"""
-	to identify that given inspection is based on topic or subject
+	to identify that given objective_factor is based on topic or subject
 	"""
-	# indicator = ask_indicator(inspection.indicatorId, principal_service)
-	# topic_or_subject_id = indicator.topicOrSubjectId
-	# base_on = indicator.baseOn
-	# if base_on == IndicatorBaseOn.TOPIC and is_not_blank(topic_or_subject_id):
-	# 	return get_topic_base_service(inspection, indicator, topic_or_subject_id, dt, principal_service)
-	# elif base_on == IndicatorBaseOn.SUBJECT and is_not_blank(topic_or_subject_id):
-	# 	return get_subject_base_service(inspection, indicator, topic_or_subject_id, dt, principal_service)
-	# else:
-	# 	raise IndicatorKernelException('Indicator is not based on topic or subject, not supported yet.')
-	pass
+	indicator_id = objective_factor.indicatorId
+	if is_blank(indicator_id):
+		raise IndicatorKernelException(
+			f'Indicator not declared on objective factor'
+			f'[objectiveId={objective.objectiveId}, factorId={objective_factor.uuid}].')
+	indicator = ask_indicator(indicator_id, principal_service)
+	if indicator is None:
+		raise IndicatorKernelException(
+			f'Indicator[indicatorId={indicator_id}] not found for objective factor'
+			f'[objectiveId={objective.objectiveId}, factorId={objective_factor.uuid}].')
+
+
+	topic_or_subject_id = indicator.topicOrSubjectId
+	base_on = indicator.baseOn
+	if base_on == IndicatorBaseOn.TOPIC and is_not_blank(topic_or_subject_id):
+		return get_topic_base_service(objective, objective_factor, indicator, topic_or_subject_id, principal_service)
+	elif base_on == IndicatorBaseOn.SUBJECT and is_not_blank(topic_or_subject_id):
+		return get_subject_base_service(objective, objective_factor, indicator, topic_or_subject_id, principal_service)
+	else:
+		raise IndicatorKernelException('Indicator is not based on topic, not supported yet.')
```

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/data_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/bucket.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/bucket.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/derived_objective.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/derived_objective.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/enum.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/enum.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/indicator.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/indicator.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/parameter.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/subject.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/subject.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/time_frame.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/time_frame.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/topic.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/data/utils/topic.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/achievement_task_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/achievement_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/bucket_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/bucket_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/derived_objective_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/derived_objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/indicator_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/indicator_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/objective_service.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/meta/objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/plugin/connector.py` & `watchmen_indicator_kernel-16.5.2/src/watchmen_indicator_kernel/plugin/connector.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.1/PKG-INFO` & `watchmen_indicator_kernel-16.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-kernel
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,16 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.1)
-Requires-Dist: watchmen-inquiry-trino (==16.5.1) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.2)
+Requires-Dist: watchmen-inquiry-trino (==16.5.2) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
```

