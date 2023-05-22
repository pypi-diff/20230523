# Comparing `tmp/pinotdb-0.4.9.tar.gz` & `tmp/pinotdb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinotdb-0.4.9.tar", max compression
+gzip compressed data, was "pinotdb-0.5.0.tar", max compression
```

## Comparing `pinotdb-0.4.9.tar` & `pinotdb-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1087 2022-08-11 17:52:15.356834 pinotdb-0.4.9/LICENSE
--rw-r--r--   0        0        0    14979 2022-12-12 00:22:53.478907 pinotdb-0.4.9/README.md
--rw-r--r--   0        0        0      682 2022-08-11 17:52:53.762874 pinotdb-0.4.9/pinotdb/__init__.py
--rw-r--r--   0        0        0    18193 2022-12-19 16:02:09.811804 pinotdb-0.4.9/pinotdb/db.py
--rw-r--r--   0        0        0      438 2022-08-11 17:52:53.763654 pinotdb-0.4.9/pinotdb/exceptions.py
--rw-r--r--   0        0        0    13171 2022-08-11 17:52:53.764110 pinotdb-0.4.9/pinotdb/keywords.py
--rw-r--r--   0        0        0    10309 2022-09-12 20:11:30.443642 pinotdb-0.4.9/pinotdb/sqlalchemy.py
--rw-r--r--   0        0        0     1040 2022-12-19 16:10:26.616966 pinotdb-0.4.9/pyproject.toml
--rw-r--r--   0        0        0    17024 1970-01-01 00:00:00.000000 pinotdb-0.4.9/setup.py
--rw-r--r--   0        0        0    15868 1970-01-01 00:00:00.000000 pinotdb-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-22 23:18:12.052278 pinotdb-0.5.0/LICENSE
+-rw-r--r--   0        0        0    15733 2023-05-22 23:18:12.052278 pinotdb-0.5.0/README.md
+-rw-r--r--   0        0        0      682 2023-05-22 23:18:12.056278 pinotdb-0.5.0/pinotdb/__init__.py
+-rw-r--r--   0        0        0    18742 2023-05-22 23:18:12.056278 pinotdb-0.5.0/pinotdb/db.py
+-rw-r--r--   0        0        0      438 2023-05-22 23:18:12.056278 pinotdb-0.5.0/pinotdb/exceptions.py
+-rw-r--r--   0        0        0    13171 2023-05-22 23:18:12.056278 pinotdb-0.5.0/pinotdb/keywords.py
+-rw-r--r--   0        0        0    10640 2023-05-22 23:18:12.056278 pinotdb-0.5.0/pinotdb/sqlalchemy.py
+-rw-r--r--   0        0        0     1240 2023-05-22 23:18:31.412436 pinotdb-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    16625 1970-01-01 00:00:00.000000 pinotdb-0.5.0/PKG-INFO
```

### Comparing `pinotdb-0.4.9/LICENSE` & `pinotdb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinotdb-0.4.9/README.md` & `pinotdb-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 ```python
 conn = connect(host="localhost", port=443, path="/query/sql", scheme="https", username="my-user", password="my-password", verify_ssl=True)
 ```
 
 To pass in additional query parameters (such as `useMultistageEngine=true`) you may pass
 them in as part of the `execute` method. For example:
+
 ```python
 curs.execute("select * from airlineStats air limit 10", queryOptions="useMultistageEngine=true")
 ```
 
 ### Using SQLAlchemy:
 
 Since db engine requires more information beyond Pinot Broker, you need to provide pinot controller for table and schema information.
@@ -229,16 +230,34 @@
 
 1. Run the Pinot QuickStart (for integration tests): `$ make run-pinot`
 2. On a separate shell, run: `$ make init`
 3. Then: `$ make test`
 
 ## Release
 
+### Prepare release credential
+
+First, configure your credentials for the release. You can simply attach your PyPI API token to the Poetry tool:
+
+```
+$ poetry config pypi-token.pypi <your_api_token_generated_from_pypi.org>
+```
+
+You should only need to do this once to set up your poetry config for the release.
+Alternatively, you can also use username and password:
+
+```
+$ poetry publish --username=<your_username> --password='<your_password>'
+```
+
+### Build and release a new Pinot DB-API to PyPI
+
 Bump the project to whichever next version is more suitable according to
-[SemVer](https://semver.org/). For example, to bump the patch version:
+[SemVer](https://semver.org/). For example, to bump the patch version automatically,
+simply ran the following command:
 
 ```
 $ poetry version patch
 ```
 
 Run to build the distribution:
 
@@ -247,7 +266,9 @@
 ```
 
 Then publish it to [pinotdb in PyPI](https://pypi.org/project/pinotdb/):
 
 ```
 $ poetry publish
 ```
+
+You can also go to Github Action: [Pinotdb Pypi Publisher](https://github.com/python-pinot-dbapi/pinot-dbapi/actions/workflows/pinotdb-pypi-publisher.yml) to click and run the workflow to publish to PYPI.
```

### Comparing `pinotdb-0.4.9/pinotdb/__init__.py` & `pinotdb-0.5.0/pinotdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pinotdb-0.4.9/pinotdb/db.py` & `pinotdb-0.5.0/pinotdb/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import asyncio
+from functools import wraps
+from typing import Any
+
 import ciso8601
 import json
 import logging
-from collections import namedtuple, OrderedDict
+from collections import namedtuple
 from enum import Enum
 from pprint import pformat
 
 import httpx
-from six import string_types
-from six.moves.urllib import parse
+from urllib import parse
 
 from pinotdb import exceptions
 
 logger = logging.getLogger(__name__)
 
 
 class Type(Enum):
     STRING = 1
     NUMBER = 2
     BOOLEAN = 3
     TIMESTAMP = 4
+    JSON = 5
 
 
 def connect(*args, **kwargs):
     """
     Constructor for creating a connection to the database.
 
         >>> conn = connect('localhost', 8099)
@@ -43,25 +46,27 @@
     """
     return AsyncConnection(*args, **kwargs)
 
 
 def check_closed(f):
     """Decorator that checks if connection/cursor is closed."""
 
+    @wraps(f)
     def g(self, *args, **kwargs):
         if self.closed:
             raise exceptions.Error(f"{self.__class__.__name__} already closed")
         return f(self, *args, **kwargs)
 
     return g
 
 
 def check_result(f):
     """Decorator that checks if the cursor has results from `execute`."""
 
+    @wraps(f)
     def g(self, *args, **kwargs):
         if self._results is None:
             raise exceptions.Error("Called before `execute`")
         return f(self, *args, **kwargs)
 
     return g
 
@@ -76,14 +81,15 @@
             None,  # [precision]
             None,  # [scale]
             None,  # [null_ok]
         )
         for name, tc in zip(column_names, types)
     ]
 
+
 def get_columns_and_types(column_names, types):
     return [
         {
             'name': name,
             'type': type
         }
         for name, type in zip(column_names, types)
@@ -102,57 +108,43 @@
         is_iterable = "_ARRAY" in column_data_type
         if (
             data_type == "INT"
             or data_type == "LONG"
             or data_type == "FLOAT"
             or data_type == "DOUBLE"
         ):
-            types[column_index] = TypeCodeAndValue(Type.NUMBER, is_iterable, False)
+            types[column_index] = TypeCodeAndValue(
+                Type.NUMBER, is_iterable, False)
         elif data_type == "STRING" or data_type == "BYTES":
-            types[column_index] = TypeCodeAndValue(Type.STRING, is_iterable, False)
+            types[column_index] = TypeCodeAndValue(
+                Type.STRING, is_iterable, False)
         elif data_type == "BOOLEAN":
-            types[column_index] = TypeCodeAndValue(Type.BOOLEAN, is_iterable, False)
+            types[column_index] = TypeCodeAndValue(
+                Type.BOOLEAN, is_iterable, False)
         elif data_type == "TIMESTAMP":
-            types[column_index] = TypeCodeAndValue(Type.TIMESTAMP, is_iterable, True)
+            types[column_index] = TypeCodeAndValue(
+                Type.TIMESTAMP, is_iterable, True)
+        elif data_type == "JSON":
+            types[column_index] = TypeCodeAndValue(
+                Type.JSON, is_iterable, True)
         else:
-            types[column_index] = TypeCodeAndValue(Type.STRING, is_iterable, True)
+            types[column_index] = TypeCodeAndValue(
+                Type.STRING, is_iterable, True)
     return types
 
 
-def get_group_by_column_names(aggregation_results):
-    group_by_cols = []
-    for metric in aggregation_results:
-        metric_name = metric.get("function", "noname")
-        gby_cols_for_metric = metric.get("groupByColumns", [])
-        if group_by_cols and group_by_cols != gby_cols_for_metric:
-            raise exceptions.DatabaseError(
-                f"Cols for metric {metric_name}: {gby_cols_for_metric} differ from other columns {group_by_cols}"
-            )
-        elif not group_by_cols:
-            group_by_cols = gby_cols_for_metric[:]
-    return group_by_cols
-
-
-def is_iterable(value):
-    try:
-        _ = iter(value)
-        return True
-    except TypeError:
-        return False
-
-
-class Connection(object):
-
+class Connection:
     """Connection to a Pinot database."""
 
     def __init__(self, *args, **kwargs):
         self._debug = kwargs.get("debug", False)
         self._args = args
         self._kwargs = kwargs
         self.closed = False
+        self.use_multistage_engine = kwargs.get('use_multistage_engine', False)
         self.cursors = []
         self.session = kwargs.get('session')
         self.is_session_external = False
         if self.session:
             self.verify_session()
             self.is_session_external = True
 
@@ -167,18 +159,15 @@
         for cursor in self.cursors:
             try:
                 cursor.close()
             except exceptions.Error:
                 pass  # already closed
         # if we're managing the httpx session, attempt to close it
         if not self.is_session_external:
-            try:
-                self.session.close()
-            except exceptions.Error:
-                pass  # already closed
+            self.session.close()
 
     @check_closed
     def commit(self):
         """
         Commit any pending transaction to the database.
 
         Not supported.
@@ -239,18 +228,15 @@
                 close_reqs.append(cursor.close())
             except exceptions.Error:
                 pass  # already closed
 
         await asyncio.gather(*close_reqs)
         # if we're managing the httpx session, attempt to close it
         if not self.is_session_external:
-            try:
-                await self.session.aclose()
-            except exceptions.Error:
-                pass  # already closed
+            await self.session.aclose()
 
     @check_closed
     async def execute(self, operation, parameters=None):
         cursor = self.cursor()
         return await cursor.execute(operation, parameters)
 
     async def __aenter__(self):
@@ -264,48 +250,58 @@
     needs_conversion = any(t.needs_conversion for t in data_types)
     if not needs_conversion:
         return rows
     for i, t in enumerate(data_types):
         if t.needs_conversion:
             for row in rows:
                 if row[i] is not None:
-                    row[i] = convert_result(t, json.dumps(row[i]))
+                    row[i] = convert_result(t, row[i])
     return rows
 
 
 def convert_result(data_type, raw_row):
     if data_type.code == Type.TIMESTAMP:
-        # Pinot returns TIMESTAMP as STRING with double quote.
-        return ciso8601.parse_datetime(raw_row.strip('"'))
+        # Pinot returns TIMESTAMP as STRING
+        return ciso8601.parse_datetime(raw_row)
+    elif data_type.code == Type.JSON:
+        # Pinot returns JSON as STRING
+        return json.loads(raw_row) if raw_row != '' else None
     else:
-        return raw_row
+        return json.dumps(raw_row)
 
-class Cursor(object):
+
+class Cursor:
     """Connection cursor."""
 
     def __init__(
         self,
         host,
         port=8099,
         scheme="http",
         path="/query/sql",
         username=None,
         password=None,
+        # TODO: Remove this unused parameter when we can afford to break the
+        #  interface (e.g. new minor version).
         verify_ssl=True,
         extra_request_headers="",
         debug=False,
         preserve_types=False,
         ignore_exception_error_codes="",
         acceptable_respond_fraction=-1,
+        # TODO: Move this parameter when we can afford to break the
+        #  interface (e.g. new minor version).
         session=None,
+        use_multistage_engine=False,
         **kwargs
     ):
         if path == "query":
             path = "query/sql"
-        self.url = parse.urlunparse((scheme, f"{host}:{port}", path, None, None, None))
+        self.url = parse.urlunparse(
+            (scheme, f"{host}:{port}", path, None, None, None))
         self.session = session
 
         # This read/write attribute specifies the number of rows to fetch at a
         # time with .fetchmany(). It defaults to 1 meaning to fetch a single
         # row at a time.
         self.arraysize = 1
 
@@ -314,28 +310,23 @@
         # these are updated only after a query
         self.description = None
         self.schema = None
         self.rowcount = -1
         self._results = None
         self._debug = debug
         self._preserve_types = preserve_types
+        self._use_multistage_engine = use_multistage_engine
         self.acceptable_respond_fraction = acceptable_respond_fraction
         if ignore_exception_error_codes:
             self._ignore_exception_error_codes = set(
                 [int(x) for x in ignore_exception_error_codes.split(",")]
             )
         else:
             self._ignore_exception_error_codes = []
 
-        if not self.session:
-            if self.use_async:
-                self.session = httpx.AsyncClient(verify=verify_ssl, **kwargs)
-            else:
-                self.session = httpx.Client(verify=verify_ssl, **kwargs)
-
         self.auth = None
         if username and password:
             self.auth = httpx.DigestAuth(username, password)
 
         self.session.headers.update({"Content-Type": "application/json"})
 
         extra_headers = {}
@@ -345,15 +336,16 @@
                 extra_headers[k] = v
 
         self.session.headers.update(extra_headers)
 
     @check_closed
     def close(self):
         """Close the cursor."""
-        self.session.close()
+        if self.session is not None and not self.session.is_closed:
+            self.session.close()
         self.closed = True
 
     def is_valid_exception(self, e):
         if "errorCode" not in e:
             return True
         else:
             return e["errorCode"] not in self._ignore_exception_error_codes
@@ -363,102 +355,131 @@
         if fraction == 0:
             return
         if queried < 0 or responded < 0:
             responded = -1
             needed = -1
         elif fraction <= -1:
             needed = queried
-        elif fraction > 0 and fraction < 1:
+        elif 0 < fraction < 1:
             needed = int(fraction * queried)
         else:
             needed = fraction
         if responded < 0 or responded < needed:
             raise exceptions.DatabaseError(
                 f"Query\n\n{query} timed out: Out of {queried}, only"
                 f" {responded} responded, while needed was {needed}"
             )
 
-    def finalize_query_payload(self, operation, parameters=None, queryOptions=None):
+    def finalize_query_payload(
+            self, operation, parameters=None, queryOptions=None
+    ):
         query = apply_parameters(operation, parameters or {})
 
         if self._preserve_types:
             query += " OPTION(preserveType='true')"
 
+        if self._use_multistage_engine:
+            if queryOptions:
+                queryOptions += ";useMultistageEngine=true"
+            else:
+                queryOptions = "useMultistageEngine=true"
         if queryOptions:
             return {"sql": query, "queryOptions": queryOptions}
         else:
             return {"sql": query}
 
     def normalize_query_response(self, input_query, query_response):
         try:
             payload = query_response.json()
         except Exception as e:
             raise exceptions.DatabaseError(
-                f"Error when querying {input_query} from {self.url}, raw response is:\n{query_response.text}"
+                f"Error when querying {input_query} from {self.url}, "
+                f"raw response is:\n{query_response.text}"
             ) from e
 
         if self._debug:
+            status_code = (
+                0 if not query_response else query_response.status_code)
             logger.info(
-                f"Got the payload of type {type(payload)} with the status code {0 if not query_response else query_response.status_code}:\n{payload}"
+                f"Got the payload of type {type(payload)} "
+                f"with the status code {status_code}:\n{payload}"
             )
 
         num_servers_responded = payload.get("numServersResponded", -1)
         num_servers_queried = payload.get("numServersQueried", -1)
 
         self.check_sufficient_responded(
             input_query, num_servers_queried, num_servers_responded
         )
 
         # raise any error messages
         if query_response.status_code != 200:
-            msg = f"Query\n\n{input_query}\n\nreturned an error: {query_response.status_code}\nFull response is {pformat(payload)}"
+            msg = (
+                f"Query\n\n{input_query}\n\nreturned an error: "
+                f"{query_response.status_code}\n"
+                f"Full response is {pformat(payload)}")
             raise exceptions.ProgrammingError(msg)
 
         query_exceptions = [
-            e for e in payload.get("exceptions", []) if self.is_valid_exception(e)
+            e for e in payload.get("exceptions", [])
+            if self.is_valid_exception(e)
         ]
         if query_exceptions:
-            msg = "\n".join(pformat(exception) for exception in query_exceptions)
+            msg = "\n".join(
+                pformat(exception) for exception in query_exceptions)
             raise exceptions.DatabaseError(msg)
 
-        rows = []  # array of array, where inner array is array of column values
-        column_names = []  # column names, such that len(column_names) == len(rows[0])
-        column_data_types = []  # column data types 1:1 mapping to column_names
+        # array of array, where inner array is array of column values
+        rows = []
+        # column names, such that len(column_names) == len(rows[0])
+        column_names = []
+        # column data types 1:1 mapping to column_names
+        column_data_types = []
         if "resultTable" in payload:
             results = payload["resultTable"]
-            column_names = results.get("dataSchema").get("columnNames")
-            column_data_types = results.get("dataSchema").get("columnDataTypes")
+            data_schema = results.get("dataSchema")
+            column_names = data_schema.get("columnNames")
+            column_data_types = data_schema.get("columnDataTypes")
             values = results.get("rows")
             if column_names:
                 rows = values
             else:
                 raise exceptions.DatabaseError(
-                    f"Expected columns and results in resultTable, but got {pformat(results)} instead"
+                    "Expected columns and results in resultTable, "
+                    f"but got {pformat(results)} instead"
                 )
 
-        logger.debug(f"Got the rows as a type {type(rows)} of size {len(rows)}")
-        if logger.isEnabledFor(logging.DEBUG):
+        logger.debug(
+            f"Got the rows as a type {type(rows)} of size {len(rows)}")
+        if logger.isEnabledFor(logging.DEBUG):  # pragma: no cover
             logger.debug(pformat(rows))
         self.description = None
         self._results = []
         if column_data_types:
             types = get_types_from_column_data_types(column_data_types)
             if self._debug:
                 logger.info(
-                    f"Column_names are {pformat(column_names)}, Column_data_types are {pformat(column_data_types)}, Types are {pformat(types)}"
+                    f"Column_names are {pformat(column_names)}, "
+                    f"Column_data_types are {pformat(column_data_types)}, "
+                    f"Types are {pformat(types)}"
                 )
             self._results = convert_result_if_required(types, rows)
             self.description = get_description_from_types(column_names, types)
-            self.schema = get_columns_and_types(column_names, column_data_types)
+            self.schema = get_columns_and_types(
+                column_names, column_data_types)
         return self
 
-
     @check_closed
+    # TODO: Rename queryOptions to query_options when releasing a breaking
+    #  version - even though Pinot understands "queryOptions", we don't need
+    #  to follow the same camel casing convention, but rather should stick
+    #  to PEP-8 instead.
     def execute(self, operation, parameters=None, queryOptions=None, **kwargs):
-        query = self.finalize_query_payload(operation, parameters, queryOptions)
+        query = self.finalize_query_payload(
+            operation, parameters, queryOptions)
 
         if self.auth and self.auth._username and self.auth._password:
             r = self.session.post(
                 self.url,
                 json=query,
                 auth=(self.auth._username, self.auth._password),
                 **kwargs)
@@ -505,15 +526,15 @@
     def fetchall(self):
         """
         Fetch all (remaining) rows of a query result, returning them as a
         sequence of sequences (e.g. a list of tuples). Note that the cursor's
         arraysize attribute can affect the performance of this operation.
         """
         return list(self)
-    
+
     @check_result
     @check_closed
     def fetchwithschema(self):
         """
         Fetch results with schema. Schema includs column names and type
         """
         return {'schema': self.schema,
@@ -542,16 +563,19 @@
         return output
 
     next = __next__
 
 
 class AsyncCursor(Cursor):
     @check_closed
-    async def execute(self, operation, parameters=None, queryOptions=None, **kwargs):
-        query = self.finalize_query_payload(operation, parameters, queryOptions)
+    async def execute(
+            self, operation, parameters=None, queryOptions=None, **kwargs
+    ):
+        query = self.finalize_query_payload(
+            operation, parameters, queryOptions)
 
         if self.auth and self.auth._username and self.auth._password:
             r = await self.session.post(
                 self.url,
                 json=query,
                 auth=(self.auth._username, self.auth._password),
                 **kwargs)
@@ -567,22 +591,22 @@
     async def close(self):
         """Close the cursor."""
         await self.session.aclose()
         self.closed = True
 
 
 def apply_parameters(operation, parameters):
-    escaped_parameters = {key: escape(value) for key, value in parameters.items()}
+    escaped_parameters = {
+        key: escape(value) for key, value in parameters.items()}
     return operation % escaped_parameters
 
 
-def escape(value):
+def escape(value: Any) -> Any:
     if value == "*":
         return value
-    elif isinstance(value, string_types):
+    elif isinstance(value, str):
         return "'{}'".format(value.replace("'", "''"))
-    elif isinstance(value, (int, float)):
-        return value
     elif isinstance(value, bool):
         return "TRUE" if value else "FALSE"
     elif isinstance(value, (list, tuple)):
-        return ", ".join(escape(element) for element in value)
+        return ", ".join(str(escape(element)) for element in value)
+    return value
```

### Comparing `pinotdb-0.4.9/pinotdb/keywords.py` & `pinotdb-0.5.0/pinotdb/keywords.py`

 * *Files identical despite different names*

### Comparing `pinotdb-0.4.9/pinotdb/sqlalchemy.py` & `pinotdb-0.5.0/pinotdb/sqlalchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from six.moves.urllib import parse
+from urllib import parse
 
 import requests
 from requests.auth import HTTPBasicAuth
 from sqlalchemy.engine import default
 from sqlalchemy.sql import compiler
 from sqlalchemy import types
 
@@ -39,23 +39,21 @@
         label,
         add_to_result_map=None,
         within_label_clause=False,
         within_columns_clause=False,
         render_label_as_label=None,
         **kw,
     ):
-        if kw:
-            render_label_as_label = kw.pop("render_label_as_label", None)
-        render_label_as_label = None
         return super().visit_label(
             label,
             add_to_result_map,
             within_label_clause,
             within_columns_clause,
-            render_label_as_label,
+            # Note: We force not to render labels in non-select clauses
+            render_label_as_label=None,
             **kw,
         )
 
 
 class PinotTypeCompiler(compiler.GenericTypeCompiler):
     def visit_REAL(self, type_, **kwargs):
         return "DOUBLE"
@@ -98,15 +96,16 @@
 
     def visit_NCLOB(self, type_, **kwargs):
         raise exceptions.NotSupportedError("Type NCBLOB is not supported")
 
 
 class PinotIdentifierPareparer(compiler.IdentifierPreparer):
     reserved_words = set(
-        [e.lower() for e in (keywords.CALCITE_KEYWORDS ^ keywords.SUPERSET_KEYWORDS)]
+        [e.lower()
+         for e in (keywords.CALCITE_KEYWORDS ^ keywords.SUPERSET_KEYWORDS)]
     )
 
     def __init__(
         self,
         dialect,
         initial_quote='"',
         final_quote=None,
@@ -123,14 +122,15 @@
 
 
 class PinotDialect(default.DefaultDialect):
 
     name = "pinot"
     scheme = "http"
     driver = "rest"
+    engine_type = "v1"
     preparer = PinotIdentifierPareparer
     statement_compiler = PinotCompiler
     type_compiler = PinotTypeCompiler
     supports_statement_cache = False
     supports_alter = False
     supports_pk_autoincrement = False
     supports_default_values = False
@@ -144,14 +144,16 @@
     broker_http_port = 8000
     broker_https_port = 443
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._controller = None
+        self._username = None
+        self._password = None
         self._debug = False
         self._verify_ssl = True
         self.update_from_kwargs(kwargs)
 
     def update_from_kwargs(self, givenkw):
         kwargs = givenkw.copy() if givenkw else {}
         # For backward compatible
@@ -188,14 +190,16 @@
             "port": url.port or self.get_default_broker_port(),
             "path": url.database,
             "scheme": self.scheme,
             "username": url.username,
             "password": url.password,
             "verify_ssl": self._verify_ssl or True,
         }
+        if self.engine_type == "multi_stage":
+            kwargs.update({"use_multistage_engine": True})
         if url.query:
             kwargs.update(url.query)
 
         kwargs = self.update_from_kwargs(kwargs)
         return ([], kwargs)
 
     def get_metadata_from_controller(self, path):
@@ -294,29 +298,40 @@
 PinotHTTPDialect = PinotDialect
 
 
 class PinotHTTPSDialect(PinotDialect):
     scheme = "https"
 
 
+class PinotMultiStageDialect(PinotDialect):
+    engine_type = "multi_stage"
+
+
+class PinotHTTPSMultiStageDialect(PinotDialect):
+    engine_type = "multi_stage"
+    scheme = "https"
+
+
 def get_default(pinot_column_default):
     if pinot_column_default == "null":
         return None
     else:
         return str(pinot_column_default)
 
 
-## Ref to supported Pinot data types: https://docs.pinot.apache.org/basics/components/schema#data-types
+# Ref to supported Pinot data types:
+# https://docs.pinot.apache.org/basics/components/schema#data-types
 def get_type(data_type, field_size):
     type_map = {
         "int": types.BigInteger,
         "long": types.BigInteger,
         "float": types.Float,
         "double": types.Numeric,
-        # BOOLEAN, is added after release 0.7.1. In release 0.7.1 and older releases, BOOLEAN is equivalent to STRING.
+        # BOOLEAN, is added after release 0.7.1.
+        # In release 0.7.1 and older releases, BOOLEAN is equivalent to STRING.
         "boolean": types.Boolean,
         "timestamp": types.TIMESTAMP,
         "string": types.String,
         "json": types.JSON,
         "bytes": types.LargeBinary,
         # Complex types
         "struct": types.BLOB,
```

### Comparing `pinotdb-0.4.9/setup.py` & `pinotdb-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,298 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pinotdb
+Version: 0.5.0
+Summary: Python DB-API and SQLAlchemy dialect for Pinot.
+Home-page: https://github.com/python-pinot-dbapi/pinot-dbapi
+License: MIT
+Author: Beto Dealmeida
+Author-email: beto@dealmeida.net
+Requires-Python: >=3.7,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: sqlalchemy
+Requires-Dist: ciso8601 (>=2.1.3,<3.0.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: requests (>=2.25.0,<3.0.0) ; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy (>=1.4,<2) ; extra == "sqlalchemy"
+Description-Content-Type: text/markdown
 
-packages = \
-['pinotdb']
+# Python DB-API and SQLAlchemy dialect for Pinot
 
-package_data = \
-{'': ['*']}
+This module allows accessing Pinot via its [SQL API](https://docs.pinot.apache.org/users/user-guide-query/pinot-query-language).
 
-install_requires = \
-['ciso8601>=2.2.0,<3.0.0', 'httpx>=0.23.0,<0.24.0']
-
-extras_require = \
-{':extra == "sqlalchemy"': ['requests>=2.28.1,<3.0.0'],
- 'sqlalchemy': ['sqlalchemy>=1.4']}
-
-entry_points = \
-{'sqlalchemy.dialects': ['pinot = pinotdb.sqlalchemy:PinotHTTPDialect',
-                         'pinot.http = pinotdb.sqlalchemy:PinotHTTPDialect',
-                         'pinot.https = pinotdb.sqlalchemy:PinotHTTPSDialect']}
-
-setup_kwargs = {
-    'name': 'pinotdb',
-    'version': '0.4.9',
-    'description': 'Python DB-API and SQLAlchemy dialect for Pinot.',
-    'long_description': '# Python DB-API and SQLAlchemy dialect for Pinot\n\nThis module allows accessing Pinot via its [SQL API](https://docs.pinot.apache.org/users/user-guide-query/pinot-query-language).\n\nCurrent supported Pinot version: 0.9.3.\n\n## Usage\n\n### Using the DB API to query Pinot Broker directly:\n\n```python\nfrom pinotdb import connect\n\n# this assumes 9000 is the controller port\nconn = connect(host=\'localhost\', port=9000, path=\'/sql\', scheme=\'http\')\ncurs = conn.cursor()\ncurs.execute("""\n    SELECT place,\n           CAST(REGEXP_EXTRACT(place, \'(.*),\', 1) AS FLOAT) AS lat,\n \xa0 \xa0 \xa0     CAST(REGEXP_EXTRACT(place, \',(.*)\', 1) AS FLOAT) AS lon\n      FROM places\n     LIMIT 10\n""")\nfor row in curs:\n    print(row)\n```\n\nFor HTTPS:\n\n```python\nfrom pinotdb import connect\n\n# this assumes that 443 is the controller port\nconn = connect(host=\'localhost\', port=443, path=\'/sql\', scheme=\'https\')\ncurs = conn.cursor()\ncurs.execute("""\n    SELECT place,\n           CAST(REGEXP_EXTRACT(place, \'(.*),\', 1) AS FLOAT) AS lat,\n \xa0 \xa0 \xa0     CAST(REGEXP_EXTRACT(place, \',(.*)\', 1) AS FLOAT) AS lon\n      FROM places\n     LIMIT 10\n""")\nfor row in curs:\n    print(row)\n```\n\nPinot also supports basic auth, e.g.\n\n```python\nconn = connect(host="localhost", port=443, path="/query/sql", scheme="https", username="my-user", password="my-password", verify_ssl=True)\n```\n\nTo pass in additional query parameters (such as `useMultistageEngine=true`) you may pass\nthem in as part of the `execute` method. For example:\n```python\ncurs.execute("select * from airlineStats air limit 10", queryOptions="useMultistageEngine=true")\n```\n\n### Using SQLAlchemy:\n\nSince db engine requires more information beyond Pinot Broker, you need to provide pinot controller for table and schema information.\n\nThe db engine connection string is format as:\n\n```\npinot+<pinot-broker-protocol>://<pinot-broker-host>:<pinot-broker-port><pinot-broker-path>?controller=<pinot-controller-protocol>://<pinot-controller-host>:<pinot-controller-port>/\n```\n\nDefault scheme is HTTP so you can ignore it. e.g. `pinot+http://localhost:8099/query/sql?controller=http://localhost:9000/` and `pinot://localhost:8099/query/sql?controller=localhost:9000/` work in same way.\n\nFor HTTPS, you have to specify the `https` scheme explicitly along with the port.\n\n```\npinot+https://<pinot-broker-host>:<pinot-broker-port><pinot-broker-path>?controller=https://<pinot-controller-host>:<pinot-controller-port>/\n```\n\nE.g. `pinot+https://pinot-broker.pinot.live:443/query/sql?controller=https://pinot-controller.pinot.live/`.\n\nPlease note that the broker port 443 has to be explicitly put there.\n\nThis can be used as Superset to Pinot connection:\n\n<img title="Superset Pinot Connection" src="assets/images/screenshots/superset-connection.png"/>\n\nIf you have basic auth:\n\n```\npinot+https://<my-user>:<my-password>@<pinot-broker-host>:<pinot-broker-port><pinot-broker-path>?controller=https://<pinot-controller-host>:<pinot-controller-port>/[&&verify_ssl=<true/false>]\n```\n\nE.g.\n`pinot+https://my-user:my-password@my-secure-pinot-broker:443/query/sql?controller=https://my-secure-pinot-controller/&&verify_ssl=true`.\n\nBelow are some sample scripts to query pinot using sqlalchemy:\n\n```python\nfrom sqlalchemy import *\nfrom sqlalchemy.engine import create_engine\nfrom sqlalchemy.schema import *\n\nengine = create_engine(\'pinot://localhost:8099/query/sql?controller=http://localhost:9000/\')  # uses HTTP by default :(\n# engine = create_engine(\'pinot+http://localhost:8099/query/sql?controller=http://localhost:9000/\')\n# engine = create_engine(\'pinot+https://localhost:8099/query/sql?controller=https://localhost:9000/\')\n\nplaces = Table(\'places\', MetaData(bind=engine), autoload=True)\nprint(select([func.count(\'*\')], from_obj=places).scalar())\n```\n\n## Examples with Pinot Quickstart\n\nStart Pinot Batch Quickstart\n\n```bash\ndocker run --name pinot-quickstart -p 2123:2123 -p 9000:9000 -p 8000:8000 -d apachepinot/pinot:latest QuickStart -type batch\n```\n\nOnce pinot batch quickstart is up, you can run below sample code snippet to query Pinot:\n\n```bash\npython3 examples/pinot_quickstart_batch.py\n```\n\nSample Output:\n\n```\nSending SQL to Pinot: SELECT * FROM baseballStats LIMIT 5\n[0, 11, 0, 0, 0, 0, 0, 0, 0, 0, \'NL\', 11, 11, \'aardsda01\', \'David Allan\', 1, 0, 0, 0, 0, 0, 0, \'SFN\', 0, 2004]\n[2, 45, 0, 0, 0, 0, 0, 0, 0, 0, \'NL\', 45, 43, \'aardsda01\', \'David Allan\', 1, 0, 0, 0, 1, 0, 0, \'CHN\', 0, 2006]\n[0, 2, 0, 0, 0, 0, 0, 0, 0, 0, \'AL\', 25, 2, \'aardsda01\', \'David Allan\', 1, 0, 0, 0, 0, 0, 0, \'CHA\', 0, 2007]\n[1, 5, 0, 0, 0, 0, 0, 0, 0, 0, \'AL\', 47, 5, \'aardsda01\', \'David Allan\', 1, 0, 0, 0, 0, 0, 1, \'BOS\', 0, 2008]\n[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, \'AL\', 73, 3, \'aardsda01\', \'David Allan\', 1, 0, 0, 0, 0, 0, 0, \'SEA\', 0, 2009]\n\nSending SQL to Pinot: SELECT playerName, sum(runs) FROM baseballStats WHERE yearID>=2000 GROUP BY playerName LIMIT 5\n[\'Scott Michael\', 26.0]\n[\'Justin Morgan\', 0.0]\n[\'Jason Andre\', 0.0]\n[\'Jeffrey Ellis\', 0.0]\n[\'Maximiliano R.\', 16.0]\n\nSending SQL to Pinot: SELECT playerName,sum(runs) AS sum_runs FROM baseballStats WHERE yearID>=2000 GROUP BY playerName ORDER BY sum_runs DESC LIMIT 5\n[\'Adrian\', 1820.0]\n[\'Jose Antonio\', 1692.0]\n[\'Rafael\', 1565.0]\n[\'Brian Michael\', 1500.0]\n[\'Alexander Emmanuel\', 1426.0]\n```\n\nStart Pinot Hybrid Quickstart\n\n```bash\ndocker run --name pinot-quickstart -p 2123:2123 -p 9000:9000 -p 8000:8000 -d apachepinot/pinot:latest QuickStart -type hybrid\n```\n\nBelow is an example against Pinot Quickstart Hybrid:\n\n```bash\npython3 examples/pinot_quickstart_hybrid.py\n```\n\n```bash\nSending SQL to Pinot: SELECT * FROM airlineStats LIMIT 5\n[171, 153, 19393, 0, 8, 8, 1433, \'1400-1459\', 0, 1425, 1240, 165, \'null\', 0, \'WN\', -2147483648, 1, 27, 17540, 0, 2, 2, 1242, \'1200-1259\', 0, \'MDW\', 13232, 1323202, 30977, \'Chicago, IL\', \'IL\', 17, \'Illinois\', 41, 861, 4, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-27\', 402, 1, -2147483648, -2147483648, 1, -2147483648, \'BOS\', 10721, 1072102, 30721, \'Boston, MA\', \'MA\', 25, \'Massachusetts\', 13, 1, [\'null\'], -2147483648, \'N556WN\', 6, 12, -2147483648, \'WN\', -2147483648, 1254, 1427, 2014]\n[183, 141, 20398, 1, 17, 17, 1302, \'1200-1259\', 1, 1245, 1005, 160, \'null\', 0, \'MQ\', 0, 1, 27, 17540, 0, -6, 0, 959, \'1000-1059\', -1, \'CMH\', 11066, 1106603, 31066, \'Columbus, OH\', \'OH\', 39, \'Ohio\', 44, 990, 4, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-27\', 3574, 1, 0, -2147483648, 1, 17, \'MIA\', 13303, 1330303, 32467, \'Miami, FL\', \'FL\', 12, \'Florida\', 33, 1, [\'null\'], 0, \'N605MQ\', 13, 29, -2147483648, \'MQ\', 0, 1028, 1249, 2014]\n[-2147483648, -2147483648, 20304, -2147483648, -2147483648, -2147483648, -2147483648, \'2100-2159\', -2147483648, 2131, 2005, 146, \'null\', 0, \'OO\', -2147483648, 1, 27, 17541, 1, 52, 52, 2057, \'2000-2059\', 3, \'COS\', 11109, 1110902, 30189, \'Colorado Springs, CO\', \'CO\', 8, \'Colorado\', 82, 809, 4, -2147483648, [11292], 1, [1129202], [\'DEN\'], -2147483648, 73, [9], 0, [\'null\'], [9], [-2147483648], [2304], 1, -2147483648, \'2014-01-27\', 5554, 1, -2147483648, -2147483648, 1, -2147483648, \'IAH\', 12266, 1226603, 31453, \'Houston, TX\', \'TX\', 48, \'Texas\', 74, 1, [\'SEA\', \'PSC\', \'PHX\', \'MSY\', \'ATL\', \'TYS\', \'DEN\', \'CHS\', \'PDX\', \'LAX\', \'EWR\', \'SFO\', \'PIT\', \'RDU\', \'RAP\', \'LSE\', \'SAN\', \'SBN\', \'IAH\', \'OAK\', \'BRO\', \'JFK\', \'SAT\', \'ORD\', \'ACY\', \'DFW\', \'BWI\'], -2147483648, \'N795SK\', -2147483648, 19, -2147483648, \'OO\', -2147483648, 2116, -2147483648, 2014]\n[153, 125, 20436, 1, 41, 41, 1442, \'1400-1459\', 2, 1401, 1035, 146, \'null\', 0, \'F9\', 2, 1, 27, 17541, 1, 34, 34, 1109, \'1000-1059\', 2, \'DEN\', 11292, 1129202, 30325, \'Denver, CO\', \'CO\', 8, \'Colorado\', 82, 967, 4, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-27\', 658, 1, 8, -2147483648, 1, 31, \'SFO\', 14771, 1477101, 32457, \'San Francisco, CA\', \'CA\', 6, \'California\', 91, 1, [\'null\'], 0, \'N923FR\', 11, 17, -2147483648, \'F9\', 0, 1126, 1431, 2014]\n[-2147483648, -2147483648, 20304, -2147483648, -2147483648, -2147483648, -2147483648, \'1400-1459\', -2147483648, 1432, 1314, 78, \'B\', 1, \'OO\', -2147483648, 1, 27, 17541, -2147483648, -2147483648, -2147483648, -2147483648, \'1300-1359\', -2147483648, \'EAU\', 11471, 1147103, 31471, \'Eau Claire, WI\', \'WI\', 55, \'Wisconsin\', 45, 268, 2, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-27\', 5455, 1, -2147483648, -2147483648, 1, -2147483648, \'ORD\', 13930, 1393003, 30977, \'Chicago, IL\', \'IL\', 17, \'Illinois\', 41, 1, [\'null\'], -2147483648, \'N903SW\', -2147483648, -2147483648, -2147483648, \'OO\', -2147483648, -2147483648, -2147483648, 2014]\n\nSending SQL to Pinot: SELECT count(*) FROM airlineStats LIMIT 5\n[17772]\n\nSending SQL to Pinot: SELECT AirlineID, sum(Cancelled) FROM airlineStats WHERE Year > 2010 GROUP BY AirlineID LIMIT 5\n[20409, 40.0]\n[19930, 16.0]\n[19805, 60.0]\n[19790, 115.0]\n[20366, 172.0]\n\nSending SQL to Pinot: select OriginCityName, max(Flights) from airlineStats group by OriginCityName ORDER BY max(Flights) DESC LIMIT 5\n[\'Casper, WY\', 1.0]\n[\'Deadhorse, AK\', 1.0]\n[\'Austin, TX\', 1.0]\n[\'Chicago, IL\', 1.0]\n[\'Monterey, CA\', 1.0]\n\nSending SQL to Pinot: SELECT OriginCityName, sum(Cancelled) AS sum_cancelled FROM airlineStats WHERE Year>2010 GROUP BY OriginCityName ORDER BY sum_cancelled DESC LIMIT 5\n[\'Chicago, IL\', 178.0]\n[\'Atlanta, GA\', 111.0]\n[\'New York, NY\', 65.0]\n[\'Houston, TX\', 62.0]\n[\'Denver, CO\', 49.0]\n\nSending Count(*) SQL to Pinot\n17773\n\nSending SQL: "SELECT OriginCityName, sum(Cancelled) AS sum_cancelled FROM "airlineStats" WHERE Year>2010 GROUP BY OriginCityName ORDER BY sum_cancelled DESC LIMIT 5" to Pinot\n[(\'Chicago, IL\', 178.0), (\'Atlanta, GA\', 111.0), (\'New York, NY\', 65.0), (\'Houston, TX\', 62.0), (\'Denver, CO\', 49.0)]\n```\n\n## Examples with existing pinot.live demo cluster\n\nJust run below script to query `pinot.live` demo cluster in two ways using pinotdb connect and sqlalchemy.\n\n```bash\npython3 examples/pinot_live.py\n```\n\nAnd response:\n\n```bash\nSending SQL to Pinot: SELECT * FROM airlineStats LIMIT 5\n[384, 359, 19805, 0, 13, 13, 1238, \'1200-1259\', 0, 1225, 900, 385, \'null\', 0, \'AA\', -2147483648, 3, 1, 16071, 0, 14, 14, 914, \'0900-0959\', 0, \'LAX\', 12892, 1289203, 32575, \'Los Angeles, CA\', \'CA\', 6, \'California\', 91, 2475, 10, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-01\', 1, 1, -2147483648, -2147483648, 1, -2147483648, \'JFK\', 12478, 1247802, 31703, \'New York, NY\', \'NY\', 36, \'New York\', 22, 1, [\'SEA\', \'PSC\', \'PHX\', \'MSY\', \'ATL\', \'TYS\', \'DEN\', \'CHS\', \'PDX\', \'LAX\', \'EWR\', \'SFO\', \'PIT\', \'RDU\', \'RAP\', \'LSE\', \'SAN\', \'SBN\', \'IAH\', \'OAK\', \'BRO\', \'JFK\', \'SAT\', \'ORD\', \'ACY\', \'DFW\', \'BWI\', \'TPA\', \'BFL\', \'BOS\', \'SNA\', \'ISN\'], -2147483648, \'N338AA\', 5, 20, -2147483648, \'AA\', -2147483648, 934, 1233, 2014]\n[269, 251, 19805, 0, -36, 0, 1549, \'1600-1659\', -2, 1625, 825, 300, \'null\', 0, \'AA\', -2147483648, 3, 1, 16071, 0, -5, 0, 820, \'0800-0859\', -1, \'JFK\', 12478, 1247802, 31703, \'New York, NY\', \'NY\', 36, \'New York\', 22, 2248, 9, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-01\', 44, 1, -2147483648, -2147483648, 1, -2147483648, \'LAS\', 12889, 1288903, 32211, \'Las Vegas, NV\', \'NV\', 32, \'Nevada\', 85, 1, [\'SEA\', \'PSC\', \'PHX\', \'MSY\', \'ATL\', \'TYS\', \'DEN\', \'CHS\', \'PDX\', \'LAX\', \'EWR\', \'SFO\', \'PIT\', \'RDU\', \'RAP\', \'LSE\', \'SAN\', \'SBN\', \'IAH\', \'OAK\'], -2147483648, \'N3DVAA\', 6, 12, -2147483648, \'AA\', -2147483648, 832, 1543, 2014]\n[307, 288, 19805, 0, -26, 0, 2039, \'2100-2159\', -2, 2105, 1340, 325, \'null\', 0, \'AA\', -2147483648, 3, 1, 16071, 0, -8, 0, 1332, \'1300-1359\', -1, \'LAX\', 12892, 1289203, 32575, \'Los Angeles, CA\', \'CA\', 6, \'California\', 91, 2556, 11, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-01\', 162, 1, -2147483648, -2147483648, 1, -2147483648, \'HNL\', 12173, 1217301, 32134, \'Honolulu, HI\', \'HI\', 15, \'Hawaii\', 2, 1, [\'SEA\', \'PSC\', \'PHX\', \'MSY\', \'ATL\', \'TYS\', \'DEN\'], -2147483648, \'N5FCAA\', 8, 11, -2147483648, \'AA\', -2147483648, 1343, 2031, 2014]\n[141, 126, 19805, 0, -19, 0, 1456, \'1500-1559\', -2, 1515, 1135, 160, \'null\', 0, \'AA\', -2147483648, 3, 1, 16071, 0, 0, 0, 1135, \'1100-1159\', 0, \'DCA\', 11278, 1127802, 30852, \'Washington, DC\', \'VA\', 51, \'Virginia\', 38, 1192, 5, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-01\', 130, 1, -2147483648, -2147483648, 1, -2147483648, \'DFW\', 11298, 1129803, 30194, \'Dallas/Fort Worth, TX\', \'TX\', 48, \'Texas\', 74, 1, [\'null\'], -2147483648, \'N3EGAA\', 4, 11, -2147483648, \'AA\', -2147483648, 1146, 1452, 2014]\n[300, 277, 19805, 0, -8, 0, 32, \'0001-0559\', -1, 40, 1625, 315, \'null\', 0, \'AA\', -2147483648, 3, 1, 16071, 0, 7, 7, 1632, \'1600-1659\', 0, \'JFK\', 12478, 1247802, 31703, \'New York, NY\', \'NY\', 36, \'New York\', 22, 2475, 10, -2147483648, [-2147483648], 0, [-2147483648], [\'null\'], -2147483648, -2147483648, [-2147483648], -2147483648, [\'null\'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, \'2014-01-01\', 180, 1, -2147483648, -2147483648, 1, -2147483648, \'LAX\', 12892, 1289203, 32575, \'Los Angeles, CA\', \'CA\', 6, \'California\', 91, 1, [\'null\'], -2147483648, \'N335AA\', 10, 13, -2147483648, \'AA\', -2147483648, 1645, 22, 2014]\n\nSending Count(*) SQL to Pinot\n9746\n\nSending SQL: "SELECT playerName, sum(runs) AS sum_runs FROM "baseballStats" WHERE yearID>=2000 GROUP BY playerName ORDER BY sum_runs DESC LIMIT 5" to Pinot\n[(19790, 581.0), (19977, 522.0), (19690, 520.0), (19805, 481.0), (20409, 410.0), (21171, 385.0), (19930, 378.0), (20355, 377.0), (19393, 326.0), (20437, 268.0)]\n```\n\n## Development\n\nIn order to develop this library, you need to have installed Poetry and tox.\n\nAfter you make sure you have them installed, test the library:\n\n1. Run the Pinot QuickStart (for integration tests): `$ make run-pinot`\n2. On a separate shell, run: `$ make init`\n3. Then: `$ make test`\n\n## Release\n\nBump the project to whichever next version is more suitable according to\n[SemVer](https://semver.org/). For example, to bump the patch version:\n\n```\n$ poetry version patch\n```\n\nRun to build the distribution:\n\n```\n$ poetry build\n```\n\nThen publish it to [pinotdb in PyPI](https://pypi.org/project/pinotdb/):\n\n```\n$ poetry publish\n```\n',
-    'author': 'Beto Dealmeida',
-    'author_email': 'beto@dealmeida.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/python-pinot-dbapi/pinot-dbapi',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4',
-}
+Current supported Pinot version: 0.9.3.
 
+## Usage
+
+### Using the DB API to query Pinot Broker directly:
+
+```python
+from pinotdb import connect
+
+# this assumes 9000 is the controller port
+conn = connect(host='localhost', port=9000, path='/sql', scheme='http')
+curs = conn.cursor()
+curs.execute("""
+    SELECT place,
+           CAST(REGEXP_EXTRACT(place, '(.*),', 1) AS FLOAT) AS lat,
+           CAST(REGEXP_EXTRACT(place, ',(.*)', 1) AS FLOAT) AS lon
+      FROM places
+     LIMIT 10
+""")
+for row in curs:
+    print(row)
+```
+
+For HTTPS:
+
+```python
+from pinotdb import connect
+
+# this assumes that 443 is the controller port
+conn = connect(host='localhost', port=443, path='/sql', scheme='https')
+curs = conn.cursor()
+curs.execute("""
+    SELECT place,
+           CAST(REGEXP_EXTRACT(place, '(.*),', 1) AS FLOAT) AS lat,
+           CAST(REGEXP_EXTRACT(place, ',(.*)', 1) AS FLOAT) AS lon
+      FROM places
+     LIMIT 10
+""")
+for row in curs:
+    print(row)
+```
+
+Pinot also supports basic auth, e.g.
+
+```python
+conn = connect(host="localhost", port=443, path="/query/sql", scheme="https", username="my-user", password="my-password", verify_ssl=True)
+```
+
+To pass in additional query parameters (such as `useMultistageEngine=true`) you may pass
+them in as part of the `execute` method. For example:
+
+```python
+curs.execute("select * from airlineStats air limit 10", queryOptions="useMultistageEngine=true")
+```
+
+### Using SQLAlchemy:
+
+Since db engine requires more information beyond Pinot Broker, you need to provide pinot controller for table and schema information.
+
+The db engine connection string is format as:
+
+```
+pinot+<pinot-broker-protocol>://<pinot-broker-host>:<pinot-broker-port><pinot-broker-path>?controller=<pinot-controller-protocol>://<pinot-controller-host>:<pinot-controller-port>/
+```
+
+Default scheme is HTTP so you can ignore it. e.g. `pinot+http://localhost:8099/query/sql?controller=http://localhost:9000/` and `pinot://localhost:8099/query/sql?controller=localhost:9000/` work in same way.
+
+For HTTPS, you have to specify the `https` scheme explicitly along with the port.
+
+```
+pinot+https://<pinot-broker-host>:<pinot-broker-port><pinot-broker-path>?controller=https://<pinot-controller-host>:<pinot-controller-port>/
+```
+
+E.g. `pinot+https://pinot-broker.pinot.live:443/query/sql?controller=https://pinot-controller.pinot.live/`.
+
+Please note that the broker port 443 has to be explicitly put there.
+
+This can be used as Superset to Pinot connection:
+
+<img title="Superset Pinot Connection" src="assets/images/screenshots/superset-connection.png"/>
+
+If you have basic auth:
+
+```
+pinot+https://<my-user>:<my-password>@<pinot-broker-host>:<pinot-broker-port><pinot-broker-path>?controller=https://<pinot-controller-host>:<pinot-controller-port>/[&&verify_ssl=<true/false>]
+```
+
+E.g.
+`pinot+https://my-user:my-password@my-secure-pinot-broker:443/query/sql?controller=https://my-secure-pinot-controller/&&verify_ssl=true`.
+
+Below are some sample scripts to query pinot using sqlalchemy:
+
+```python
+from sqlalchemy import *
+from sqlalchemy.engine import create_engine
+from sqlalchemy.schema import *
+
+engine = create_engine('pinot://localhost:8099/query/sql?controller=http://localhost:9000/')  # uses HTTP by default :(
+# engine = create_engine('pinot+http://localhost:8099/query/sql?controller=http://localhost:9000/')
+# engine = create_engine('pinot+https://localhost:8099/query/sql?controller=https://localhost:9000/')
+
+places = Table('places', MetaData(bind=engine), autoload=True)
+print(select([func.count('*')], from_obj=places).scalar())
+```
+
+## Examples with Pinot Quickstart
+
+Start Pinot Batch Quickstart
+
+```bash
+docker run --name pinot-quickstart -p 2123:2123 -p 9000:9000 -p 8000:8000 -d apachepinot/pinot:latest QuickStart -type batch
+```
+
+Once pinot batch quickstart is up, you can run below sample code snippet to query Pinot:
+
+```bash
+python3 examples/pinot_quickstart_batch.py
+```
+
+Sample Output:
+
+```
+Sending SQL to Pinot: SELECT * FROM baseballStats LIMIT 5
+[0, 11, 0, 0, 0, 0, 0, 0, 0, 0, 'NL', 11, 11, 'aardsda01', 'David Allan', 1, 0, 0, 0, 0, 0, 0, 'SFN', 0, 2004]
+[2, 45, 0, 0, 0, 0, 0, 0, 0, 0, 'NL', 45, 43, 'aardsda01', 'David Allan', 1, 0, 0, 0, 1, 0, 0, 'CHN', 0, 2006]
+[0, 2, 0, 0, 0, 0, 0, 0, 0, 0, 'AL', 25, 2, 'aardsda01', 'David Allan', 1, 0, 0, 0, 0, 0, 0, 'CHA', 0, 2007]
+[1, 5, 0, 0, 0, 0, 0, 0, 0, 0, 'AL', 47, 5, 'aardsda01', 'David Allan', 1, 0, 0, 0, 0, 0, 1, 'BOS', 0, 2008]
+[0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 'AL', 73, 3, 'aardsda01', 'David Allan', 1, 0, 0, 0, 0, 0, 0, 'SEA', 0, 2009]
+
+Sending SQL to Pinot: SELECT playerName, sum(runs) FROM baseballStats WHERE yearID>=2000 GROUP BY playerName LIMIT 5
+['Scott Michael', 26.0]
+['Justin Morgan', 0.0]
+['Jason Andre', 0.0]
+['Jeffrey Ellis', 0.0]
+['Maximiliano R.', 16.0]
+
+Sending SQL to Pinot: SELECT playerName,sum(runs) AS sum_runs FROM baseballStats WHERE yearID>=2000 GROUP BY playerName ORDER BY sum_runs DESC LIMIT 5
+['Adrian', 1820.0]
+['Jose Antonio', 1692.0]
+['Rafael', 1565.0]
+['Brian Michael', 1500.0]
+['Alexander Emmanuel', 1426.0]
+```
+
+Start Pinot Hybrid Quickstart
+
+```bash
+docker run --name pinot-quickstart -p 2123:2123 -p 9000:9000 -p 8000:8000 -d apachepinot/pinot:latest QuickStart -type hybrid
+```
+
+Below is an example against Pinot Quickstart Hybrid:
+
+```bash
+python3 examples/pinot_quickstart_hybrid.py
+```
+
+```bash
+Sending SQL to Pinot: SELECT * FROM airlineStats LIMIT 5
+[171, 153, 19393, 0, 8, 8, 1433, '1400-1459', 0, 1425, 1240, 165, 'null', 0, 'WN', -2147483648, 1, 27, 17540, 0, 2, 2, 1242, '1200-1259', 0, 'MDW', 13232, 1323202, 30977, 'Chicago, IL', 'IL', 17, 'Illinois', 41, 861, 4, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-27', 402, 1, -2147483648, -2147483648, 1, -2147483648, 'BOS', 10721, 1072102, 30721, 'Boston, MA', 'MA', 25, 'Massachusetts', 13, 1, ['null'], -2147483648, 'N556WN', 6, 12, -2147483648, 'WN', -2147483648, 1254, 1427, 2014]
+[183, 141, 20398, 1, 17, 17, 1302, '1200-1259', 1, 1245, 1005, 160, 'null', 0, 'MQ', 0, 1, 27, 17540, 0, -6, 0, 959, '1000-1059', -1, 'CMH', 11066, 1106603, 31066, 'Columbus, OH', 'OH', 39, 'Ohio', 44, 990, 4, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-27', 3574, 1, 0, -2147483648, 1, 17, 'MIA', 13303, 1330303, 32467, 'Miami, FL', 'FL', 12, 'Florida', 33, 1, ['null'], 0, 'N605MQ', 13, 29, -2147483648, 'MQ', 0, 1028, 1249, 2014]
+[-2147483648, -2147483648, 20304, -2147483648, -2147483648, -2147483648, -2147483648, '2100-2159', -2147483648, 2131, 2005, 146, 'null', 0, 'OO', -2147483648, 1, 27, 17541, 1, 52, 52, 2057, '2000-2059', 3, 'COS', 11109, 1110902, 30189, 'Colorado Springs, CO', 'CO', 8, 'Colorado', 82, 809, 4, -2147483648, [11292], 1, [1129202], ['DEN'], -2147483648, 73, [9], 0, ['null'], [9], [-2147483648], [2304], 1, -2147483648, '2014-01-27', 5554, 1, -2147483648, -2147483648, 1, -2147483648, 'IAH', 12266, 1226603, 31453, 'Houston, TX', 'TX', 48, 'Texas', 74, 1, ['SEA', 'PSC', 'PHX', 'MSY', 'ATL', 'TYS', 'DEN', 'CHS', 'PDX', 'LAX', 'EWR', 'SFO', 'PIT', 'RDU', 'RAP', 'LSE', 'SAN', 'SBN', 'IAH', 'OAK', 'BRO', 'JFK', 'SAT', 'ORD', 'ACY', 'DFW', 'BWI'], -2147483648, 'N795SK', -2147483648, 19, -2147483648, 'OO', -2147483648, 2116, -2147483648, 2014]
+[153, 125, 20436, 1, 41, 41, 1442, '1400-1459', 2, 1401, 1035, 146, 'null', 0, 'F9', 2, 1, 27, 17541, 1, 34, 34, 1109, '1000-1059', 2, 'DEN', 11292, 1129202, 30325, 'Denver, CO', 'CO', 8, 'Colorado', 82, 967, 4, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-27', 658, 1, 8, -2147483648, 1, 31, 'SFO', 14771, 1477101, 32457, 'San Francisco, CA', 'CA', 6, 'California', 91, 1, ['null'], 0, 'N923FR', 11, 17, -2147483648, 'F9', 0, 1126, 1431, 2014]
+[-2147483648, -2147483648, 20304, -2147483648, -2147483648, -2147483648, -2147483648, '1400-1459', -2147483648, 1432, 1314, 78, 'B', 1, 'OO', -2147483648, 1, 27, 17541, -2147483648, -2147483648, -2147483648, -2147483648, '1300-1359', -2147483648, 'EAU', 11471, 1147103, 31471, 'Eau Claire, WI', 'WI', 55, 'Wisconsin', 45, 268, 2, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-27', 5455, 1, -2147483648, -2147483648, 1, -2147483648, 'ORD', 13930, 1393003, 30977, 'Chicago, IL', 'IL', 17, 'Illinois', 41, 1, ['null'], -2147483648, 'N903SW', -2147483648, -2147483648, -2147483648, 'OO', -2147483648, -2147483648, -2147483648, 2014]
+
+Sending SQL to Pinot: SELECT count(*) FROM airlineStats LIMIT 5
+[17772]
+
+Sending SQL to Pinot: SELECT AirlineID, sum(Cancelled) FROM airlineStats WHERE Year > 2010 GROUP BY AirlineID LIMIT 5
+[20409, 40.0]
+[19930, 16.0]
+[19805, 60.0]
+[19790, 115.0]
+[20366, 172.0]
+
+Sending SQL to Pinot: select OriginCityName, max(Flights) from airlineStats group by OriginCityName ORDER BY max(Flights) DESC LIMIT 5
+['Casper, WY', 1.0]
+['Deadhorse, AK', 1.0]
+['Austin, TX', 1.0]
+['Chicago, IL', 1.0]
+['Monterey, CA', 1.0]
+
+Sending SQL to Pinot: SELECT OriginCityName, sum(Cancelled) AS sum_cancelled FROM airlineStats WHERE Year>2010 GROUP BY OriginCityName ORDER BY sum_cancelled DESC LIMIT 5
+['Chicago, IL', 178.0]
+['Atlanta, GA', 111.0]
+['New York, NY', 65.0]
+['Houston, TX', 62.0]
+['Denver, CO', 49.0]
+
+Sending Count(*) SQL to Pinot
+17773
+
+Sending SQL: "SELECT OriginCityName, sum(Cancelled) AS sum_cancelled FROM "airlineStats" WHERE Year>2010 GROUP BY OriginCityName ORDER BY sum_cancelled DESC LIMIT 5" to Pinot
+[('Chicago, IL', 178.0), ('Atlanta, GA', 111.0), ('New York, NY', 65.0), ('Houston, TX', 62.0), ('Denver, CO', 49.0)]
+```
+
+## Examples with existing pinot.live demo cluster
+
+Just run below script to query `pinot.live` demo cluster in two ways using pinotdb connect and sqlalchemy.
+
+```bash
+python3 examples/pinot_live.py
+```
+
+And response:
+
+```bash
+Sending SQL to Pinot: SELECT * FROM airlineStats LIMIT 5
+[384, 359, 19805, 0, 13, 13, 1238, '1200-1259', 0, 1225, 900, 385, 'null', 0, 'AA', -2147483648, 3, 1, 16071, 0, 14, 14, 914, '0900-0959', 0, 'LAX', 12892, 1289203, 32575, 'Los Angeles, CA', 'CA', 6, 'California', 91, 2475, 10, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-01', 1, 1, -2147483648, -2147483648, 1, -2147483648, 'JFK', 12478, 1247802, 31703, 'New York, NY', 'NY', 36, 'New York', 22, 1, ['SEA', 'PSC', 'PHX', 'MSY', 'ATL', 'TYS', 'DEN', 'CHS', 'PDX', 'LAX', 'EWR', 'SFO', 'PIT', 'RDU', 'RAP', 'LSE', 'SAN', 'SBN', 'IAH', 'OAK', 'BRO', 'JFK', 'SAT', 'ORD', 'ACY', 'DFW', 'BWI', 'TPA', 'BFL', 'BOS', 'SNA', 'ISN'], -2147483648, 'N338AA', 5, 20, -2147483648, 'AA', -2147483648, 934, 1233, 2014]
+[269, 251, 19805, 0, -36, 0, 1549, '1600-1659', -2, 1625, 825, 300, 'null', 0, 'AA', -2147483648, 3, 1, 16071, 0, -5, 0, 820, '0800-0859', -1, 'JFK', 12478, 1247802, 31703, 'New York, NY', 'NY', 36, 'New York', 22, 2248, 9, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-01', 44, 1, -2147483648, -2147483648, 1, -2147483648, 'LAS', 12889, 1288903, 32211, 'Las Vegas, NV', 'NV', 32, 'Nevada', 85, 1, ['SEA', 'PSC', 'PHX', 'MSY', 'ATL', 'TYS', 'DEN', 'CHS', 'PDX', 'LAX', 'EWR', 'SFO', 'PIT', 'RDU', 'RAP', 'LSE', 'SAN', 'SBN', 'IAH', 'OAK'], -2147483648, 'N3DVAA', 6, 12, -2147483648, 'AA', -2147483648, 832, 1543, 2014]
+[307, 288, 19805, 0, -26, 0, 2039, '2100-2159', -2, 2105, 1340, 325, 'null', 0, 'AA', -2147483648, 3, 1, 16071, 0, -8, 0, 1332, '1300-1359', -1, 'LAX', 12892, 1289203, 32575, 'Los Angeles, CA', 'CA', 6, 'California', 91, 2556, 11, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-01', 162, 1, -2147483648, -2147483648, 1, -2147483648, 'HNL', 12173, 1217301, 32134, 'Honolulu, HI', 'HI', 15, 'Hawaii', 2, 1, ['SEA', 'PSC', 'PHX', 'MSY', 'ATL', 'TYS', 'DEN'], -2147483648, 'N5FCAA', 8, 11, -2147483648, 'AA', -2147483648, 1343, 2031, 2014]
+[141, 126, 19805, 0, -19, 0, 1456, '1500-1559', -2, 1515, 1135, 160, 'null', 0, 'AA', -2147483648, 3, 1, 16071, 0, 0, 0, 1135, '1100-1159', 0, 'DCA', 11278, 1127802, 30852, 'Washington, DC', 'VA', 51, 'Virginia', 38, 1192, 5, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-01', 130, 1, -2147483648, -2147483648, 1, -2147483648, 'DFW', 11298, 1129803, 30194, 'Dallas/Fort Worth, TX', 'TX', 48, 'Texas', 74, 1, ['null'], -2147483648, 'N3EGAA', 4, 11, -2147483648, 'AA', -2147483648, 1146, 1452, 2014]
+[300, 277, 19805, 0, -8, 0, 32, '0001-0559', -1, 40, 1625, 315, 'null', 0, 'AA', -2147483648, 3, 1, 16071, 0, 7, 7, 1632, '1600-1659', 0, 'JFK', 12478, 1247802, 31703, 'New York, NY', 'NY', 36, 'New York', 22, 2475, 10, -2147483648, [-2147483648], 0, [-2147483648], ['null'], -2147483648, -2147483648, [-2147483648], -2147483648, ['null'], [-2147483648], [-2147483648], [-2147483648], 0, -2147483648, '2014-01-01', 180, 1, -2147483648, -2147483648, 1, -2147483648, 'LAX', 12892, 1289203, 32575, 'Los Angeles, CA', 'CA', 6, 'California', 91, 1, ['null'], -2147483648, 'N335AA', 10, 13, -2147483648, 'AA', -2147483648, 1645, 22, 2014]
+
+Sending Count(*) SQL to Pinot
+9746
+
+Sending SQL: "SELECT playerName, sum(runs) AS sum_runs FROM "baseballStats" WHERE yearID>=2000 GROUP BY playerName ORDER BY sum_runs DESC LIMIT 5" to Pinot
+[(19790, 581.0), (19977, 522.0), (19690, 520.0), (19805, 481.0), (20409, 410.0), (21171, 385.0), (19930, 378.0), (20355, 377.0), (19393, 326.0), (20437, 268.0)]
+```
+
+## Development
+
+In order to develop this library, you need to have installed Poetry and tox.
+
+After you make sure you have them installed, test the library:
+
+1. Run the Pinot QuickStart (for integration tests): `$ make run-pinot`
+2. On a separate shell, run: `$ make init`
+3. Then: `$ make test`
+
+## Release
+
+### Prepare release credential
+
+First, configure your credentials for the release. You can simply attach your PyPI API token to the Poetry tool:
+
+```
+$ poetry config pypi-token.pypi <your_api_token_generated_from_pypi.org>
+```
+
+You should only need to do this once to set up your poetry config for the release.
+Alternatively, you can also use username and password:
+
+```
+$ poetry publish --username=<your_username> --password='<your_password>'
+```
+
+### Build and release a new Pinot DB-API to PyPI
+
+Bump the project to whichever next version is more suitable according to
+[SemVer](https://semver.org/). For example, to bump the patch version automatically,
+simply ran the following command:
+
+```
+$ poetry version patch
+```
+
+Run to build the distribution:
+
+```
+$ poetry build
+```
+
+Then publish it to [pinotdb in PyPI](https://pypi.org/project/pinotdb/):
+
+```
+$ poetry publish
+```
+
+You can also go to Github Action: [Pinotdb Pypi Publisher](https://github.com/python-pinot-dbapi/pinot-dbapi/actions/workflows/pinotdb-pypi-publisher.yml) to click and run the workflow to publish to PYPI.
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

