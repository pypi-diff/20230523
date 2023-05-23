# Comparing `tmp/watchmen_storage-16.5.1.tar.gz` & `tmp/watchmen_storage-16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.1.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.2.tar", max compression
```

## Comparing `watchmen_storage-16.5.1.tar` & `watchmen_storage-16.5.2.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1061 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/LICENSE
--rw-r--r--   0        0        0      472 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/pyproject.toml
--rw-r--r--   0        0        0     2196 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1685 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0      988 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0     7259 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5884 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4645 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 watchmen_storage-16.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/LICENSE
+-rw-r--r--   0        0        0      492 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2196 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1819 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1096 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10150 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/ast_vister.py
+-rw-r--r--   0        0        0     2632 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0      890 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/query_performance_service.py
+-rw-r--r--   0        0        0     1441 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7259 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     5884 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4645 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-05-23 07:54:10.452673 watchmen_storage-16.5.2/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 watchmen_storage-16.5.2/PKG-INFO
```

### Comparing `watchmen_storage-16.5.1/LICENSE` & `watchmen_storage-16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.2/src/watchmen_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.2/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.2/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.2/src/watchmen_storage/free_storage_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from enum import Enum
-from typing import List, Optional
+from typing import List, Optional, Callable
 
 from watchmen_model.common import DataModel, Pageable
+from .sql_analysis.ast_vister import QueryPerformance
 from .storage_types import ColumnNameLiteral, EntityCriteria, EntitySortColumn, Literal
 
 
 class FreeAggregateArithmetic(str, Enum):
 	NONE = 'none'
 	DISTINCT_COUNT = 'distinct_count'
 	COUNT = 'count'
@@ -34,14 +35,15 @@
 	type: Optional[FreeJoinType] = None
 
 
 class FreeFinder(DataModel):
 	columns: List[FreeColumn] = None
 	joins: List[FreeJoin] = None
 	criteria: Optional[EntityCriteria] = None
+	preExecutor: Optional[Callable[[QueryPerformance,bool],None]] = None
 
 
 class FreeAggregateColumn(DataModel):
 	name: str  # name must match free column's index, such as column_1, column_2 (starts from 1)
 	arithmetic: Optional[FreeAggregateArithmetic] = None
 	alias: Optional[str] = None
```

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.2/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.2/src/watchmen_storage/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,31 @@
 
 
 class StorageSettings(BaseSettings):
 	DECIMAL_INTEGRAL_DIGITS: int = 24
 	DECIMAL_FRACTION_DIGITS: int = 8
 	DISABLE_COMPILED_CACHE: bool = False
 	OBJECT_STORAGE_NEED_DATE_DIRECTORY: bool = False
+
+	SQL_ANALYZER_ON: bool = True
 	
 	class Config:
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
 
 storage_settings = StorageSettings()
 logger.info(f'Storage settings[{storage_settings.dict()}].')
 
 
+def ask_sql_analyzer_on() -> bool:
+	return storage_settings.SQL_ANALYZER_ON
+
 def ask_decimal_integral_digits() -> int:
 	return storage_settings.DECIMAL_INTEGRAL_DIGITS
 
 
 def ask_decimal_fraction_digits() -> int:
 	return storage_settings.DECIMAL_FRACTION_DIGITS
```

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.2/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.2/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.2/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.2/src/watchmen_storage/storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.2/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.2/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.1/PKG-INFO` & `watchmen_storage-16.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage
-Version: 16.5.1
+Version: 16.5.2
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.24.20,<2.0.0)
-Requires-Dist: watchmen-model (==16.5.1)
+Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
+Requires-Dist: watchmen-model (==16.5.2)
```

