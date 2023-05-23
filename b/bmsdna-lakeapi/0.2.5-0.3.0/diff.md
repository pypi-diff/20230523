# Comparing `tmp/bmsdna_lakeapi-0.2.5.tar.gz` & `tmp/bmsdna_lakeapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.2.5.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.3.0.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.2.5.tar` & `bmsdna_lakeapi-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1081 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/LICENSE
--rw-r--r--   0        0        0     4722 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/README.md
--rw-r--r--   0        0        0      166 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5349 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     3699 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     8721 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6281 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12641 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12625 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15770 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6566 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     7822 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     3601 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2361 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-23 06:39:54.685208 bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     1842 2023-05-23 06:39:54.689208 bmsdna_lakeapi-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4722 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/README.md
+-rw-r--r--   0        0        0      166 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5349 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     3699 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8721 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6281 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12689 2023-05-23 12:38:31.631579 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    13366 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15906 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6589 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4450 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2361 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1842 2023-05-23 12:38:31.635580 bmsdna_lakeapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.3.0/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.2.5/LICENSE` & `bmsdna_lakeapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/README.md` & `bmsdna_lakeapi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     right_on: str
     file_type: FileTypes = "delta"
     how: JoinStrategy = "inner"
     suffix: str = "_right"
 
 
 @dataclass
-class DataframeConfig:
+class DatasourceConfig:
     uri: str
     file_type: FileTypes = "delta"
     select: Optional[List[Column]] = None
     exclude: Optional[List[str]] = None
     groupby: Optional[GroupByConfig] = None
     sortby: Optional[List[SortBy]] = None
     joins: Optional[List[Join]] = None
@@ -156,15 +156,15 @@
     ...
 
 
 @dataclass
 class Config:
     name: str
     tag: str
-    dataframe: DataframeConfig
+    datasource: DatasourceConfig
     version: Optional[int] = 1
     api_method: Union[Literal["get", "post"], List[Literal["get", "post"]]] = "get"
     params: Optional[List[Union[Param, str]]] = None
     engine: Engines = "duckdb"
     timestamp: Optional[datetime] = None
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
     options: Optional[Union[Option, None]] = None
@@ -182,35 +182,37 @@
         return "{}({})".format(type(self).__name__, ", ".join(kws))
 
     def __str__(self) -> str:
         kws = [f"{key}={value!r}" for key, value in self.__dict__.items()]
         return "{}({})".format(type(self).__name__, ", ".join(kws))
 
     @classmethod
-    def from_dict(cls, config: Dict, basic_config: BasicConfig, table_names: List[tuple[int, str, str]]) -> List["Config"]:
+    def from_dict(
+        cls, config: Dict, basic_config: BasicConfig, table_names: List[tuple[int, str, str]]
+    ) -> List["Config"]:
         name = config["name"]
         tag = config["tag"]
         version = config.get("version", 1)
         engine = config.get("engine", "duckdb")
         api_method = cast(Literal["post", "get"], config.get("api_method", "get"))
         params = config.get("params")
-        dataframe = config["dataframe"]
-        uri = dataframe["uri"]
+        datasource = config["datasource"]
+        uri = datasource["uri"]
         assert isinstance(uri, str)
-        file_type = cast(FileTypes, dataframe.get("file_type", "delta") if dataframe else "delta")
-        columns = dataframe.get("columns") if dataframe else None
-        select = dataframe.get("select") if dataframe else None
-        exclude = dataframe.get("exclude") if dataframe else None
-        groupby = dataframe.get("groupby") if dataframe else None
-        sortby = dataframe.get("sortby") if dataframe else None
+        file_type = cast(FileTypes, datasource.get("file_type", "delta") if datasource else "delta")
+        columns = datasource.get("columns") if datasource else None
+        select = datasource.get("select") if datasource else None
+        exclude = datasource.get("exclude") if datasource else None
+        groupby = datasource.get("groupby") if datasource else None
+        sortby = datasource.get("sortby") if datasource else None
         cache_expiration_time_seconds = (
-            dataframe.get("cache_expiration_time_seconds", CACHE_EXPIRATION_TIME_SECONDS) if dataframe else None
+            datasource.get("cache_expiration_time_seconds", CACHE_EXPIRATION_TIME_SECONDS) if datasource else None
         )
-        orderby = dataframe.get("orderby") if dataframe else None
-        joins = dataframe.get("joins") if dataframe else None
+        orderby = datasource.get("orderby") if datasource else None
+        joins = datasource.get("joins") if datasource else None
         search_config = [SearchConfig(**c) for c in config["search"]] if "search" in config else None
         logger.debug(config)
 
         _params: list[Param] = []
         if params:
             logger.debug(f"Parameter: {name} -> {params}")
 
@@ -248,15 +250,15 @@
             else:
                 ls = []
                 for it in os.scandir(root_folder):
                     res_name = (version, tag, it.name)
                     if res_name not in table_names and (
                         (it.is_dir() and file_type == "delta") or (it.is_file() and file_type != "delta")
                     ):
-                        dataframe = DataframeConfig(
+                        datasource = DatasourceConfig(
                             uri=folder + "/" + it.name,
                             file_type=file_type,
                             select=select,
                             exclude=exclude,
                             groupby=groupby,
                             sortby=sortby,
                             joins=joins,
@@ -270,21 +272,21 @@
                                 tag=tag,
                                 engine=engine,  # type: ignore
                                 version=version,
                                 api_method=api_method,
                                 search=search_config,
                                 params=_params,  # type: ignore
                                 allow_get_all_pages=config.get("allow_get_all_pages", False),
-                                dataframe=dataframe,
+                                datasource=datasource,
                                 cache_expiration_time_seconds=cache_expiration_time_seconds,
                             )
                         )
             return ls
         else:
-            dataframe = DataframeConfig(
+            datasource = DatasourceConfig(
                 uri=uri,
                 file_type=file_type,
                 select=select,
                 exclude=exclude,
                 groupby=groupby,
                 sortby=sortby,
                 joins=joins,
@@ -298,15 +300,15 @@
                     tag=tag,
                     version=version,
                     search=search_config,
                     engine=engine,  # type: ignore
                     api_method=api_method,
                     params=_params,  # type: ignore
                     allow_get_all_pages=config.get("allow_get_all_pages", False),
-                    dataframe=dataframe,
+                    datasource=datasource,
                     cache_expiration_time_seconds=cache_expiration_time_seconds,
                 )
             ]
 
     async def to_dict(self) -> dict:
         return self.__dict__
```

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pyarrow.parquet
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
 
-from bmsdna.lakeapi.core.config import BasicConfig, DataframeConfig, GroupByConfig, GroupByExpConfig, Param
+from bmsdna.lakeapi.core.config import BasicConfig, DatasourceConfig, GroupByConfig, GroupByExpConfig, Param
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.model import get_param_def, should_hide_colname
 from bmsdna.lakeapi.core.types import DeltaOperatorTypes, FileTypes
 from bmsdna.lakeapi.context.df_base import ResultData, ExecutionContext
 import pypika
 from pypika.queries import QueryBuilder
@@ -47,21 +47,23 @@
     except IndexError:
         return uri
 
 
 class Dataframe:
     def __init__(
         self,
+        version: str,
         tag: str,
         name: str,
-        config: DataframeConfig,
+        config: DatasourceConfig,
         sql_context: ExecutionContext,
         basic_config: BasicConfig,
         df: Optional[ResultData] = None,
     ) -> None:
+        self.version = version
         self.config = config
         self.tag = tag
         self.name = name
         self.df = df
         self.sql_context = sql_context
         self.basic_config = basic_config
 
@@ -132,15 +134,15 @@
             df = self.select_df(df)
         if endpoint != "meta":
             df = self.sort_df(df)
         return df
 
     @property
     def tablename(self):
-        return self.tag + "_" + self.name + "_" + get_table_name_from_uri(self.config.uri)
+        return self.version + "_" + self.tag + "_" + self.name + "_" + get_table_name_from_uri(self.config.uri)
 
     def get_df(
         self,
         partitions: Optional[List[Tuple[str, str, Any]]],
         endpoint: endpoints = "request",
     ) -> ResultData:
         if self.df is None:
@@ -209,14 +211,26 @@
                 value_for_partitioning = [hvl[:prefix_len] for hvl in hashvl]
             else:
                 hashvl = hashlib.md5(value.encode("utf8")).hexdigest()
                 value_for_partitioning = hashvl[:prefix_len]
             if op not in operators:
                 col_for_partitioning = None
                 continue
+        elif partcol.startswith(colname + "_md5_mod_"):
+            col_for_partitioning = partcol
+            modulo_len = int(partcol[len(colname + "_md5_mod_") :])
+            if isinstance(value, (List, Tuple)):
+                hashvl = [int(hashlib.md5(v.encode("utf8")).hexdigest(), 16) for v in value]
+                value_for_partitioning = [hvl % modulo_len for hvl in hashvl]
+            else:
+                hashvl = int(hashlib.md5(value.encode("utf8")).hexdigest(), 16)
+                value_for_partitioning = hashvl % modulo_len
+            if op not in operators:
+                col_for_partitioning = None
+                continue
         elif partcol.startswith(colname + "_prefix_"):
             col_for_partitioning = partcol
             prefix_len = int(partcol[len(colname + "_prefix_") :])
             if isinstance(value, (List, Tuple)):
                 value_for_partitioning = [v[:prefix_len] for v in value]
             else:
                 value_for_partitioning = value[:prefix_len]
```

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,28 @@
 async def get_partitions(dataframe: Dataframe, params: BaseModel, config: Config) -> Optional[list]:
     parts = (
         await filter_partitions_based_on_params(
             DeltaTable(dataframe.uri).metadata(),
             params.dict(exclude_unset=True) if params else {},
             config.params or [],
         )
-        if config.dataframe.file_type == "delta"
+        if config.datasource.file_type == "delta"
         else None
     )
     return parts
 
 
 def remove_search(prm_dict: dict, config: Config):
     if not config.search or len(prm_dict) == 0:
         return prm_dict
     search_cols = [s.name.lower() for s in config.search]
     return {k: v for k, v in prm_dict.items() if k.lower() not in search_cols}
 
 
-async def get_expr(columns: List[str], config: Config, params: BaseModel) -> Optional[pypika.Criterion]:
+async def get_params_filter_expr(columns: List[str], config: Config, params: BaseModel) -> Optional[pypika.Criterion]:
     expr = await filter_df_based_on_params(
         remove_search(params.dict(exclude_unset=True) if params else {}, config),
         config.params if config.params else [],
         columns,
     )
     return expr
 
@@ -124,20 +124,22 @@
     def get_detailed_metadata(req: Request):
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
         with DuckDbExecutionContext() as context:
-            realdataframe = Dataframe(config.tag, config.name, config.dataframe, context, basic_config=basic_config)
+            realdataframe = Dataframe(
+                config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
+            )
             partition_columns = []
             partition_values = None
             delta_tbl = None
             df = realdataframe.get_df(None)
-            if config.dataframe.file_type == "delta":
+            if config.datasource.file_type == "delta":
                 delta_tbl = DeltaTable(realdataframe.uri)
                 partition_columns = delta_tbl.metadata().partition_columns
                 if len(partition_columns) > 0:
                     qb: QueryBuilder = (
                         df.query_builder().select(*[pypika.Field(c) for c in partition_columns]).distinct()
                     )
                     partition_values = context.execute_sql(qb).to_arrow_table().to_pylist()
@@ -250,20 +252,22 @@
         engine = engine or config.engine
 
         logger.info(f"Engine: {engine}")
 
         ExecutionContext = get_context_by_engine(engine)
 
         with ExecutionContext() as context:
-            realdataframe = Dataframe(config.tag, config.name, config.dataframe, context, basic_config=basic_config)
+            realdataframe = Dataframe(
+                config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
+            )
 
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
-            expr = await get_expr(df.columns(), config, params)
+            expr = await get_params_filter_expr(df.columns(), config, params)
 
             new_query = df.query_builder()
             new_query = new_query.where(expr) if expr is not None else new_query
 
             columns = exclude_cols(df.columns())
 
             if columns:
```

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 class TypeBaseModel(BaseModel):
     class Config:
         orm_mode = True
 
 
 def should_hide_colname(name: str):
-    return name.startswith("_") or "_md5_prefix_" in name or "_xxhash64_prefix_" in name
+    return name.startswith("_") or "_md5_prefix_" in name or "_xxhash64_prefix_" in name or "_md5_mod_" in name
 
 
 def create_response_model(name: str, frame: ResultData) -> type[BaseModel]:
     schema = frame.arrow_schema()
     props = {k: get_schema_for(name, schema.field(k)) for k in schema.names if not should_hide_colname(k)}
 
     return create_model(name, **props, __base__=TypeBaseModel)
```

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.3.0/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.2.5/pyproject.toml` & `bmsdna_lakeapi-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.2.5"
+version = "0.3.0"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.2.5/PKG-INFO` & `bmsdna_lakeapi-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

