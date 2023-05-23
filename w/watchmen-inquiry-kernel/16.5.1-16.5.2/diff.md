# Comparing `tmp/watchmen_inquiry_kernel-16.5.1.tar.gz` & `tmp/watchmen_inquiry_kernel-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_kernel-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_inquiry_kernel-16.5.2.tar", max compression
```

## Comparing `watchmen_inquiry_kernel-16.5.1.tar` & `watchmen_inquiry_kernel-16.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/LICENSE
--rw-r--r--   0        0        0     1274 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/__init__.py
--rw-r--r--   0        0        0      112 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/common/__init__.py
--rw-r--r--   0        0        0       47 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/common/exception.py
--rw-r--r--   0        0        0      620 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/common/settings.py
--rw-r--r--   0        0        0       86 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1847 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/enum_service.py
--rw-r--r--   0        0        0     1404 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/report_service.py
--rw-r--r--   0        0        0     2358 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/subject_service.py
--rw-r--r--   0        0        0       82 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/schema/__init__.py
--rw-r--r--   0        0        0     2178 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/schema/report_schema.py
--rw-r--r--   0        0        0    12544 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/schema/subject_schema.py
--rw-r--r--   0        0        0      104 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/report_data_service.py
--rw-r--r--   0        0        0     1228 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/subject_data_service.py
--rw-r--r--   0        0        0    53360 2023-04-25 10:52:45.984220 watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/subject_storage.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/LICENSE
+-rw-r--r--   0        0        0     1274 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/__init__.py
+-rw-r--r--   0        0        0      112 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/common/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/common/exception.py
+-rw-r--r--   0        0        0      620 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/common/settings.py
+-rw-r--r--   0        0        0       86 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/enum_service.py
+-rw-r--r--   0        0        0     1404 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/report_service.py
+-rw-r--r--   0        0        0     2358 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/subject_service.py
+-rw-r--r--   0        0        0       82 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/schema/__init__.py
+-rw-r--r--   0        0        0     2178 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/schema/report_schema.py
+-rw-r--r--   0        0        0    12544 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/schema/subject_schema.py
+-rw-r--r--   0        0        0      104 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1544 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/report_data_service.py
+-rw-r--r--   0        0        0     1228 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/subject_data_service.py
+-rw-r--r--   0        0        0    54334 2023-05-23 07:54:10.412670 watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/subject_storage.py
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.2/PKG-INFO
```

### Comparing `watchmen_inquiry_kernel-16.5.1/LICENSE` & `watchmen_inquiry_kernel-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/pyproject.toml` & `watchmen_inquiry_kernel-16.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-inquiry-kernel"
-version = "16.5.1"
+version = "16.5.2"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-kernel = "16.5.1"
-watchmen-inquiry-trino = { version = "16.5.1", optional = true }
-watchmen-storage-mysql = { version = "16.5.1", optional = true }
-watchmen-storage-oracle = { version = "16.5.1", optional = true }
-watchmen-storage-mongodb = { version = "16.5.1", optional = true }
-watchmen-storage-mssql = { version = "16.5.1", optional = true }
-watchmen-storage-postgresql = { version = "16.5.1", optional = true }
-watchmen-storage-oss = { version = "16.5.1", optional = true }
-watchmen-storage-s3 = { version = "16.5.1", optional = true }
+watchmen-data-kernel = "16.5.2"
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

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/common/settings.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/enum_service.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/enum_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/report_service.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/meta/subject_service.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/meta/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/schema/report_schema.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/schema/report_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/schema/subject_schema.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/schema/subject_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/report_data_service.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/report_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/subject_data_service.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/subject_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.1/src/watchmen_inquiry_kernel/storage/subject_storage.py` & `watchmen_inquiry_kernel-16.5.2/src/watchmen_inquiry_kernel/storage/subject_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from watchmen_model.common import ComputedParameter, ConstantParameter, DataModel, DataPage, FactorId, Pageable, \
 	Parameter, ParameterComputeType, ParameterCondition, ParameterExpression, ParameterExpressionOperator, \
 	ParameterJoint, ParameterJointType, SubjectDatasetColumnId, TopicFactorParameter, TopicId, \
 	VariablePredefineFunctions
 from watchmen_model.console import ConnectedSpace, ReportDimension, ReportFunnel, ReportFunnelType, ReportIndicator, \
 	ReportIndicatorArithmetic, SubjectDatasetColumn, SubjectDatasetJoin, SubjectJoinType
 from watchmen_model.console.subject import Subject, SubjectColumnArithmetic
+from watchmen_pipeline_kernel.pipeline.sql_performance_invoker import create_sql_performance_pipeline_invoker
 from watchmen_storage import ColumnNameLiteral, ComputedLiteral, ComputedLiteralOperator, EntityCriteria, \
 	EntityCriteriaExpression, EntityCriteriaJoint, EntityCriteriaJointConjunction, EntityCriteriaOperator, \
 	EntityCriteriaStatement, EntitySortColumn, EntitySortMethod, FreeAggregateArithmetic, FreeAggregateColumn, \
 	FreeAggregatePager, FreeAggregator, FreeColumn, FreeFinder, FreeJoin, FreeJoinType, FreePager, Literal, \
 	TopicDataStorageSPI
 from watchmen_utilities import ArrayHelper, date_might_with_prefix, get_current_time_in_seconds, is_blank, is_date, \
 	is_decimal, is_not_blank, is_time, month_diff, move_date, translate_date_format_to_memory, truncate_time, year_diff
@@ -275,14 +276,16 @@
 		def to_free_column(column: SubjectDatasetColumn) -> Tuple[FreeColumn, List[PossibleParameterType]]:
 			parsed_parameter = parse_parameter_for_storage(
 				column.parameter, available_schemas_for_columns, self.principalService, False)
 			literal = parsed_parameter.run(empty_variables, self.principalService)
 			arithmetic = column.arithmetic
 			if arithmetic is None or arithmetic == SubjectColumnArithmetic.NONE:
 				column_arithmetic = FreeAggregateArithmetic.NONE
+			elif arithmetic == SubjectColumnArithmetic.DISTINCT_COUNT:
+				column_arithmetic = FreeAggregateArithmetic.DISTINCT_COUNT
 			elif arithmetic == SubjectColumnArithmetic.COUNT:
 				column_arithmetic = FreeAggregateArithmetic.COUNT
 			elif arithmetic == SubjectColumnArithmetic.SUMMARY:
 				column_arithmetic = FreeAggregateArithmetic.SUMMARY
 			elif arithmetic == SubjectColumnArithmetic.AVERAGE:
 				column_arithmetic = FreeAggregateArithmetic.AVERAGE
 			elif arithmetic == SubjectColumnArithmetic.MAXIMUM:
@@ -311,27 +314,31 @@
 			)]
 		else:
 			joins = ArrayHelper(dataset.joins).map(lambda x: self.build_join(x, available_schemas)).to_list()
 
 		storage = ask_topic_storage(self.schema.get_primary_topic_schema(), self.principalService)
 		# register topic, in case of it is not registered yet
 		ArrayHelper(available_schemas).each(lambda x: storage.register_topic(x.get_topic()))
-		return FreeFinder(columns=columns, joins=joins, criteria=criteria), possible_types_list
+		return FreeFinder(columns=columns, joins=joins, criteria=criteria,
+		                  preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
+		                                                                      self.principalService)), possible_types_list
 
 	def find(self) -> List[Dict[str, Any]]:
 		finder, _ = self.ask_storage_finder()
 		return self.find_data(lambda agent: agent.free_find(finder))
 
 	def ask_storage_pager(self, pageable: Pageable) -> FreePager:
 		finder, _ = self.ask_storage_finder()
 		return FreePager(
 			columns=finder.columns,
 			joins=finder.joins,
 			criteria=finder.criteria,
-			pageable=pageable
+			pageable=pageable,
+			preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
+			                                                    self.principalService)
 		)
 
 	def page(self, pageable: Pageable) -> DataPage:
 		return self.find_data(
 			lambda agent: agent.free_page(self.ask_storage_pager(pageable)))
 
 	# noinspection PyMethodMayBeStatic
@@ -455,15 +462,15 @@
 
 		def to_integer(
 				a_start_value: Optional[str], an_end_value: Optional[str]
 		) -> Tuple[Optional[int], Optional[int]]:
 			a_start_value, an_end_value = to_decimal(a_start_value, an_end_value)
 			return \
 				None if a_start_value is None else a_start_value.to_integral(), \
-				None if an_end_value is None else an_end_value.to_integral()
+					None if an_end_value is None else an_end_value.to_integral()
 
 		if funnel_type == ReportFunnelType.NUMERIC:
 			return to_decimal(start_value, end_value)
 		elif funnel_type == ReportFunnelType.DATE:
 			# if given value cannot be parsed to a date, let it be None
 			_, start_value = is_date(start_value, ask_all_date_formats())
 			_, end_value = is_date(end_value, ask_all_date_formats())
@@ -1147,15 +1154,17 @@
 		return FreeAggregator(
 			columns=finder.columns,
 			joins=finder.joins,
 			criteria=finder.criteria,
 			highOrderAggregateColumns=self.build_aggregate_columns(report_schema),
 			highOrderCriteria=self.build_high_order_criteria(report_schema, possible_types_list),
 			highOrderSortColumns=self.build_sort_columns(report_schema),
-			highOrderTruncation=report_schema.get_truncation_count()
+			highOrderTruncation=report_schema.get_truncation_count(),
+			preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
+			                                                    self.principalService)
 		)
 
 	def aggregate_find(self, report_schema: ReportSchema) -> List[Dict[str, Any]]:
 		return self.find_data(lambda agent: agent.free_aggregate_find(self.ask_storage_aggregator(report_schema)))
 
 	def ask_storage_aggregate_pager(
 			self, report_schema: ReportSchema, pageable: Pageable) -> FreeAggregatePager:
@@ -1164,15 +1173,17 @@
 			columns=aggregator.columns,
 			joins=aggregator.joins,
 			criteria=aggregator.criteria,
 			highOrderAggregateColumns=aggregator.highOrderAggregateColumns,
 			highOrderCriteria=aggregator.highOrderCriteria,
 			highOrderSortColumns=aggregator.highOrderSortColumns,
 			highOrderTruncation=aggregator.highOrderTruncation,
-			pageable=pageable
+			pageable=pageable,
+			preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
+			                                                    self.principalService)
 		)
 
 	def aggregate_page(self, report_schema: ReportSchema, pageable: Pageable) -> DataPage:
 		return self.find_data(
 			lambda agent: agent.free_aggregate_page(self.ask_storage_aggregate_pager(report_schema, pageable)))
 
 	# noinspection PyMethodMayBeStatic
```

### Comparing `watchmen_inquiry_kernel-16.5.1/PKG-INFO` & `watchmen_inquiry_kernel-16.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-kernel
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
-Requires-Dist: watchmen-data-kernel (==16.5.1)
-Requires-Dist: watchmen-inquiry-trino (==16.5.1) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.2)
+Requires-Dist: watchmen-inquiry-trino (==16.5.2) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.5.2) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.2) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.2) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.2) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.2) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.2) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.2) ; extra == "s3"
```

