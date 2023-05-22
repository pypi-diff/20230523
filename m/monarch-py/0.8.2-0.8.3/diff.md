# Comparing `tmp/monarch_py-0.8.2.tar.gz` & `tmp/monarch_py-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.8.2.tar", max compression
+gzip compressed data, was "monarch_py-0.8.3.tar", max compression
```

## Comparing `monarch_py-0.8.2.tar` & `monarch_py-0.8.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-18 00:50:32.211882 monarch_py-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-18 00:50:32.211882 monarch_py-0.8.2/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1630 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7377 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11736 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     9463 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20498 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4697 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9031 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4145 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-05-18 00:50:32.215882 monarch_py-0.8.2/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-22 23:39:41.965812 monarch_py-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1630 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7461 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11736 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     9463 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3321 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20534 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4752 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9129 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4145 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-05-22 23:39:41.965812 monarch_py-0.8.3/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.8.3/PKG-INFO
```

### Comparing `monarch_py-0.8.2/pyproject.toml` & `monarch_py-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.8.2"
+version = "0.8.3"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.8.2/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.8.3/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/cli.py` & `monarch_py-0.8.3/src/monarch_py/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib
 from pathlib import Path
-from typing import Optional
+from typing import List, Optional
 
 import typer
 
 from monarch_py import solr_cli, sql_cli
 from monarch_py.datamodels.model import AssociationTypeEnum
 
 app = typer.Typer()
@@ -105,27 +105,28 @@
     """
     solr_cli.associations(**locals())
 
 
 @app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
-    category: str = typer.Option(None, "--category"),
-    taxon: str = typer.Option(None, "--taxon"),
-    limit: int = typer.Option(20, "--limit"),
+    category: List[str] = typer.Option(None, "--category", "-c"),
+    taxon: str = typer.Option(None, "--taxon", "-t"),
+    limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
+    # sort: str = typer.Option(None, "--sort", "-s"),
 ):
     """
     Search for entities
 
     Args:
         q: The query string to search for
         category: The category of the entity
```

### Comparing `monarch_py-0.8.2/src/monarch_py/datamodels/model.py` & `monarch_py-0.8.3/src/monarch_py/datamodels/model.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.8.3/src/monarch_py/datamodels/model.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/datamodels/solr.py` & `monarch_py-0.8.3/src/monarch_py/datamodels/solr.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     facet_fields: Optional[List[str]] = Field(default_factory=list)
     facet_queries: Optional[List[str]] = Field(default_factory=list)
     filter_queries: Optional[List[str]] = Field(default_factory=list)
     query_fields: str = None
     def_type: str = "edismax"
     mm: str = "100%"  # All tokens in the query must be found in the doc, equivalent to q.op="AND"
     boost: str = None
+    sort: str = None
 
     def add_field_filter_query(self, field, value):
         if field is not None and value is not None:
             self.filter_queries.append(f"{field}:{escape(value)}")
         else:
             raise ValueError("Can't add a field filter query without a field and value")
         return self
```

### Comparing `monarch_py-0.8.2/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.8.3/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,43 +215,42 @@
     ###############################
     # Implements: SearchInterface #
     ###############################
 
     def search(
         self,
         q: str = "*:*",
-        category: str = None,
-        taxon: str = None,
         offset: int = 0,
         limit: int = 20,
-        # add a facet_fields params defaulting to an empty list
+        category: List[str] = None,
+        in_taxon: List[str] = None,
         facet_fields: List[str] = None,
-        filter_queries: List[str] = None,
         facet_queries: List[str] = None,
+        filter_queries: List[str] = None,
+        sort: str = None,
     ) -> SearchResults:
         """Search for entities by label, with optional filters"""
 
         solr = SolrService(base_url=self.base_url, core=core.ENTITY)
-        query = SolrQuery(start=offset, rows=limit)
+        query = SolrQuery(start=offset, rows=limit, sort=sort)
 
         query.q = q
 
         query.def_type = "edismax"
         query.query_fields = self._entity_query_fields()
         query.boost = self._entity_boost()
 
+        if category:
+            query.add_filter_query(" OR ".join(f"category:{cat}" for cat in category))
+        if in_taxon:
+            query.add_filter_query(" OR ".join([f"in_taxon:{t}" for t in taxon]))
         if facet_fields:
             query.facet_fields = facet_fields
         if facet_queries:
             query.facet_queries = facet_queries
-
-        if category:
-            query.add_field_filter_query("category", category)
-        if taxon:
-            query.add_field_filter_query("in_taxon", taxon)
         if filter_queries:
             query.filter_queries.extend(filter_queries)
 
         query_result = solr.query(query)
         total = query_result.response.num_found
 
         items = []
```

### Comparing `monarch_py-0.8.2/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.8.3/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.8.3/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.8.3/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.8.3/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.8.3/src/monarch_py/interfaces/search_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 class SearchInterface(ABC):
     """Abstract interface for searching the Monarch KG in a Lucene way"""
 
     @abstractmethod
     def search(
         self,
         q: str,
-        category: str,
-        taxon: str,
         offset: int = 0,
         limit: int = 20,
+        category: List[str] = None,
+        in_taxon: List[str] = None,
         facet_fields: List[str] = None,
         filter_queries: List[str] = None,
         facet_queries: List[str] = None,
+        sort: str = None,
     ) -> SearchResults:
         """
 
         Args:
             q (str): Query string to match against
             category (str): Limit results to only this category
             taxon (str): Limit results to only this taxon
```

### Comparing `monarch_py-0.8.2/src/monarch_py/service/solr_service.py` & `monarch_py-0.8.3/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/solr_cli.py` & `monarch_py-0.8.3/src/monarch_py/solr_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 import pystow
 import typer
 
 from monarch_py.datamodels.model import AssociationCountList, AssociationTypeEnum
 from monarch_py.utils.solr_cli_utils import (
     check_solr_permissions,
     get_solr,
@@ -133,44 +135,47 @@
     response = data.get_associations(**args)
     format_output(fmt, response, output)
 
 
 @solr_app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
-    category: str = typer.Option(None, "--category", "-c"),
+    category: List[str] = typer.Option(None, "--category", "-c"),
     taxon: str = typer.Option(None, "--taxon", "-t"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
+    # sort: str = typer.Option(None, "--sort", "-s"),
 ):
     """
     Search for entities
 
     Optional Args:
         q: The query string to search for
         category: The category of the entity
         taxon: The taxon of the entity
         limit: The number of entities to return
         offset: The offset of the first entity to be retrieved
         fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
+    params = locals()
+    params.pop("fmt", None)
+    params.pop("output", None)
+
     data = get_solr(update=False)
-    response = data.search(
-        q=q, category=category, taxon=taxon, limit=limit, offset=offset
-    )
+    response = data.search(**params)
     format_output(fmt, response, output)
 
 
 @solr_app.command("autocomplete")
 def autocomplete(
     q: str = typer.Argument(None, help="Query string to autocomplete against"),
     fmt: str = typer.Option(
```

### Comparing `monarch_py-0.8.2/src/monarch_py/sql_cli.py` & `monarch_py-0.8.3/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.8.3/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.8.3/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/src/monarch_py/utils/utils.py` & `monarch_py-0.8.3/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.8.2/PKG-INFO` & `monarch_py-0.8.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.8.2
+Version: 0.8.3
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

