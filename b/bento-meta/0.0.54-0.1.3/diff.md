# Comparing `tmp/bento_meta-0.0.54.tar.gz` & `tmp/bento_meta-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_meta-0.0.54.tar", max compression
+gzip compressed data, was "bento_meta-0.1.3.tar", max compression
```

## Comparing `bento_meta-0.0.54.tar` & `bento_meta-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11446 2020-10-16 17:49:04.916483 bento_meta-0.0.54/LICENSE
--rw-r--r--   0        0        0      157 2020-10-16 17:49:04.917102 bento_meta-0.0.54/README.md
--rw-r--r--   0        0        0     2230 2023-02-13 01:45:22.041265 bento_meta-0.0.54/pyproject.toml
--rw-r--r--   0        0        0       70 2023-02-08 23:10:38.928433 bento_meta-0.0.54/src/bento_meta/__init__.py
--rw-r--r--   0        0        0    22569 2023-02-12 23:42:52.167649 bento_meta-0.0.54/src/bento_meta/entity.py
--rw-r--r--   0        0        0      502 2023-02-12 23:42:52.168386 bento_meta-0.0.54/src/bento_meta/logs/log.ini
--rw-r--r--   0        0        0      388 2023-02-08 23:10:38.930201 bento_meta-0.0.54/src/bento_meta/mdb/__init__.py
--rw-r--r--   0        0        0     8901 2023-02-08 23:10:38.930420 bento_meta-0.0.54/src/bento_meta/mdb/loaders.py
--rw-r--r--   0        0        0    13412 2023-02-08 23:10:38.931335 bento_meta-0.0.54/src/bento_meta/mdb/mdb.py
--rw-r--r--   0        0        0       89 2023-02-08 23:10:38.932332 bento_meta-0.0.54/src/bento_meta/mdb/mdb_tools/__init__.py
--rw-r--r--   0        0        0    28784 2023-02-08 23:10:38.933304 bento_meta-0.0.54/src/bento_meta/mdb/mdb_tools/mdb_tools.py
--rw-r--r--   0        0        0     3616 2023-02-08 23:10:38.933480 bento_meta-0.0.54/src/bento_meta/mdb/searchable.py
--rw-r--r--   0        0        0     2426 2023-02-08 23:10:38.934620 bento_meta-0.0.54/src/bento_meta/mdb/writeable.py
--rw-r--r--   0        0        0    19230 2023-02-08 23:10:38.935750 bento_meta-0.0.54/src/bento_meta/model.py
--rw-r--r--   0        0        0    25896 2023-02-08 23:10:38.936099 bento_meta-0.0.54/src/bento_meta/object_map.py
--rw-r--r--   0        0        0    10465 2023-02-12 23:30:19.090576 bento_meta-0.0.54/src/bento_meta/objects.py
--rw-r--r--   0        0        0      196 2023-02-08 23:10:38.940527 bento_meta-0.0.54/src/bento_meta/util/__init__.py
--rw-r--r--   0        0        0    15507 2023-02-08 23:10:38.941405 bento_meta-0.0.54/src/bento_meta/util/_engine.py
--rw-r--r--   0        0        0       87 2023-02-08 23:10:38.942242 bento_meta-0.0.54/src/bento_meta/util/cypher/__init__.py
--rw-r--r--   0        0        0     7427 2023-02-08 23:10:38.943782 bento_meta-0.0.54/src/bento_meta/util/cypher/clauses.py
--rw-r--r--   0        0        0    19302 2023-02-08 23:10:38.944679 bento_meta-0.0.54/src/bento_meta/util/cypher/entities.py
--rw-r--r--   0        0        0     2067 2023-02-08 23:10:38.945608 bento_meta-0.0.54/src/bento_meta/util/cypher/functions.py
--rw-r--r--   0        0        0    24424 2022-02-25 15:35:38.969950 bento_meta-0.0.54/src/bento_meta/util/cypher.py.old
--rw-r--r--   0        0        0     2532 2023-02-08 23:10:38.946393 bento_meta-0.0.54/src/bento_meta/util/makeq.py
--rw-r--r--   0        0        0     4910 2022-01-28 18:56:52.458052 bento_meta-0.0.54/src/bento_meta/util/query_paths.yml
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 bento_meta-0.0.54/setup.py
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 bento_meta-0.0.54/PKG-INFO
+-rw-r--r--   0        0        0    11446 2020-10-16 17:49:04.916483 bento_meta-0.1.3/LICENSE
+-rw-r--r--   0        0        0      157 2020-10-16 17:49:04.917102 bento_meta-0.1.3/README.md
+-rw-r--r--   0        0        0     2197 2023-05-23 18:53:13.654125 bento_meta-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-02-08 23:10:38.928433 bento_meta-0.1.3/src/bento_meta/__init__.py
+-rw-r--r--   0        0        0    22569 2023-02-12 23:42:52.167649 bento_meta-0.1.3/src/bento_meta/entity.py
+-rw-r--r--   0        0        0      502 2023-02-12 23:42:52.168386 bento_meta-0.1.3/src/bento_meta/logs/log.ini
+-rw-r--r--   0        0        0      388 2023-02-08 23:10:38.930201 bento_meta-0.1.3/src/bento_meta/mdb/__init__.py
+-rw-r--r--   0        0        0     8997 2023-05-23 18:53:13.655094 bento_meta-0.1.3/src/bento_meta/mdb/loaders.py
+-rw-r--r--   0        0        0    13412 2023-02-08 23:10:38.931335 bento_meta-0.1.3/src/bento_meta/mdb/mdb.py
+-rw-r--r--   0        0        0       89 2023-02-08 23:10:38.932332 bento_meta-0.1.3/src/bento_meta/mdb/mdb_tools/__init__.py
+-rw-r--r--   0        0        0    28784 2023-02-08 23:10:38.933304 bento_meta-0.1.3/src/bento_meta/mdb/mdb_tools/mdb_tools.py
+-rw-r--r--   0        0        0     3616 2023-02-08 23:10:38.933480 bento_meta-0.1.3/src/bento_meta/mdb/searchable.py
+-rw-r--r--   0        0        0     2426 2023-02-08 23:10:38.934620 bento_meta-0.1.3/src/bento_meta/mdb/writeable.py
+-rw-r--r--   0        0        0    19629 2023-05-23 18:53:13.656567 bento_meta-0.1.3/src/bento_meta/model.py
+-rw-r--r--   0        0        0    25896 2023-02-08 23:10:38.936099 bento_meta-0.1.3/src/bento_meta/object_map.py
+-rw-r--r--   0        0        0    10465 2023-02-12 23:30:19.090576 bento_meta-0.1.3/src/bento_meta/objects.py
+-rw-r--r--   0        0        0      196 2023-02-08 23:10:38.940527 bento_meta-0.1.3/src/bento_meta/util/__init__.py
+-rw-r--r--   0        0        0    15507 2023-02-08 23:10:38.941405 bento_meta-0.1.3/src/bento_meta/util/_engine.py
+-rw-r--r--   0        0        0       87 2023-02-08 23:10:38.942242 bento_meta-0.1.3/src/bento_meta/util/cypher/__init__.py
+-rw-r--r--   0        0        0     7427 2023-02-08 23:10:38.943782 bento_meta-0.1.3/src/bento_meta/util/cypher/clauses.py
+-rw-r--r--   0        0        0    19302 2023-02-08 23:10:38.944679 bento_meta-0.1.3/src/bento_meta/util/cypher/entities.py
+-rw-r--r--   0        0        0     2067 2023-02-08 23:10:38.945608 bento_meta-0.1.3/src/bento_meta/util/cypher/functions.py
+-rw-r--r--   0        0        0    24424 2022-02-25 15:35:38.969950 bento_meta-0.1.3/src/bento_meta/util/cypher.py.old
+-rw-r--r--   0        0        0     2532 2023-02-08 23:10:38.946393 bento_meta-0.1.3/src/bento_meta/util/makeq.py
+-rw-r--r--   0        0        0     4910 2022-01-28 18:56:52.458052 bento_meta-0.1.3/src/bento_meta/util/query_paths.yml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 bento_meta-0.1.3/setup.py
+-rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 bento_meta-0.1.3/PKG-INFO
```

### Comparing `bento_meta-0.0.54/LICENSE` & `bento_meta-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/pyproject.toml` & `bento_meta-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-meta"
-version = "0.0.54"
+version = "0.1.3"
 description = "Python drivers for Bento Metamodel Database"
 authors = [
   { name="Mark A. Jensen", email = "mark.jensen@nih.gov"},
   { name="Mark Benson", email = "mark.benson@nih.gov"},
   { name="Nelson Moore", email = "nelson.moore@essential-soft.com"}
 ]
 requires-python = ">=3.8"
@@ -16,15 +16,15 @@
 
 [project.urls]
 "Homepage" = "https://cbiit.github.io/bento-meta/"
 "Bug Tracker" = "https://github.com/CBIIT/bento-meta/issues"
 
 [tool.poetry]
 name = "bento-meta"
-version = "0.0.54"
+version = "0.1.3"
 description = "Python drivers for Bento Metamodel Database"
 authors = [
     "Mark A. Jensen <mark.jensen@nih.gov>",
     "Mark Benson <mark.benson@nih.gov>",
     "Nelson Moore <nelson.moore@essential-soft.com>"
 ]
 license = "Apache 2.0"
@@ -48,15 +48,15 @@
 
 [tool.poetry.extras]
 Tools = ["click", "numpy", "pandas", "spacy"] #"scispacy",
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 # docker-compose = {version = "^1.29.2", optional = true}
-# pytest-docker = {version = "^1.0.1", optional = true}
+pytest-docker = "^1.0.1"
 requests = "^2.28.1"
 myst-nb = {version = "^0.17.1", python = "^3.8"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.1.1"
 python-semantic-release = "^7.33.0"
 pytest-cov = "^4.0.0"
```

### Comparing `bento_meta-0.0.54/src/bento_meta/entity.py` & `bento_meta-0.1.3/src/bento_meta/entity.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/mdb/loaders.py` & `bento_meta-0.1.3/src/bento_meta/mdb/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,24 @@
     )
 
 
 def load_mdf(mdf, mdb, _commit=None):
     """Load an MDF object into an MDB instance"""
     load_model(mdf.model, mdb, _commit)
 
+
 def load_model(model, mdb, _commit=None):
     """Load a model object into an MDB instance."""
     if not isinstance(mdb, WriteableMDB):
         raise RuntimeError("mdb object must be a WriteableMDB")
     cstmts = load_model_statements(model, _commit)
     for stmt in tqdm(cstmts):
         mdb.put_with_statement(str(stmt), stmt.params)
 
+
 def load_model_statements(model, _commit=None):
     """
     Create Cypher statements from a model to load it de novo into an
     MDB instance.
 
     :param :class:`mdb.Model` model: Model instance for loading
     :param str _commit: 'Commit string' for marking entities in DB. If set, this will override
@@ -122,29 +124,31 @@
         cProp = _cEntity(pr, model, _commit)
         cStatements.extend([
             Statement(
                 Merge(cValueSet),
                 use_params=True
                 ),
             Statement(
-                Match(cProp),
-                Merge(R(Type="has_value_set").relate(_plain_var(cProp), cValueSet)),
+                Match(cProp, cValueSet),
+                Merge(R(Type="has_value_set").
+                      relate(_plain_var(cProp),
+                             _plain_var(cValueSet))),
                 use_params=True
                 )
             ])
         if pr.concept:
             cStatements.extend(
                 _annotate_statements(pr, cProp, _commit)
                 )
         for tm in pr.terms.values():
             cTerm = _cEntity(tm, model, _commit)
             cStatements.extend([
                 Statement(
                     Merge(cTerm),
-                    use_params = True
+                    use_params=True
                     ),
                 Statement(
                     Match(cValueSet, cTerm),
                     Merge(R(Type="has_term").relate(_plain_var(cValueSet),
                                                     _plain_var(cTerm))),
                     use_params=True
                     )
@@ -171,26 +175,26 @@
         if ent.origin_id:
             cEnt._add_props({"origin_id": ent.origin_id})
         if ent.origin_version:
             cEnt._add_props({"origin_version": ent.origin_version})
         if ent.origin_definition:
             cEnt._add_props({"origin_defintion": ent.origin_definition})
         if ent.handle:
-            cEnt._add_props({"handle":ent.handle})
+            cEnt._add_props({"handle": ent.handle})
     elif label == 'value_set':
         cEnt = N(label='value_set',
                  props={"handle": ent.handle})
         if ent.url:
             cEnt._add_props({"url": ent.url})
     elif label == 'concept':
-        cEnt = N(label='concept')    
+        cEnt = N(label='concept')
     elif label == 'tag':
         cEnt = N(label="tag",
-                 props={"key": t.key,
-                        "value": t.value})
+                 props={"key": ent.key,
+                        "value": ent.value})
         
     else:
         cEnt = N(label=label,
                  props={"handle": ent.handle,
                         "model": model.handle})
     # all ents
     if _commit:
@@ -242,14 +246,15 @@
             ])
         if p.tags:
             stmts.extend(
                 _tag_statements(p, cProp, _commit)
                 )
     return stmts
 
+
 def _annotate_statements(ent, cEnt, _commit):
     stmts = []
     if not ent.concept:
         return []
     cConcept = _cEntity(ent.concept, None, _commit)
     stmts = []
     for tm in ent.concept.terms.values():
@@ -263,14 +268,14 @@
                 Match(cEnt),
                 Merge(R(Type="has_concept").relate(
                     _plain_var(cEnt), cConcept)),
                 use_params=True
             ),
             Statement(
                 Match(R(Type="has_concept").relate(
-                    cEnt, cConcept)),
+                    cEnt, cConcept), cTerm),
                 Merge(R(Type="represents").relate(
-                    cTerm, _plain_var(cConcept))),
+                    _plain_var(cTerm), _plain_var(cConcept))),
                 use_params=True
             ),
         ])
     return stmts
```

### Comparing `bento_meta-0.0.54/src/bento_meta/mdb/mdb.py` & `bento_meta-0.1.3/src/bento_meta/mdb/mdb.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/mdb/mdb_tools/mdb_tools.py` & `bento_meta-0.1.3/src/bento_meta/mdb/mdb_tools/mdb_tools.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/mdb/searchable.py` & `bento_meta-0.1.3/src/bento_meta/mdb/searchable.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/mdb/writeable.py` & `bento_meta-0.1.3/src/bento_meta/mdb/writeable.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/model.py` & `bento_meta-0.1.3/src/bento_meta/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         if not handle:
             raise ArgError("model requires arg 'handle' set")
         self.handle = handle
         self._mdb = None
         self.nodes = {}
         self.edges = {}  # keys are (edge.handle, src.handle, dst.handle) tuples
         self.props = {}  # keys are ({edge|node}.handle, prop.handle) tuples
-        self.terms = {}
+        self.terms = {}  # keys are (term.handle, term.origin) tuples
         self.removed_entities = []
 
         if mdb:
             self.mdb = mdb
 
     @classmethod
     def versioning(cls, on=None):
@@ -180,26 +180,29 @@
         """
         if not isinstance(ent, Entity):
             raise ArgError("arg1 must be Entity")
         if not isinstance(term, Term):
             raise ArgError("arg2 must be Term")
         if not ent.concept:
             ent.concept = Concept({"nanoid":make_nanoid()})
-        if (term.value, term.origin_name) in ent.concept.terms:
-            raise ValueError("Concept already represented by a Term with value '{}'"
-                             "and origin_name '{}'".format(term.value, term.origin_name))
-        ent.concept.terms[(term.value, term.origin_name)] = term
+        term_key = term.handle if term.handle else term.value;
+        if (term_key, term.origin_name) in ent.concept.terms:
+            raise ValueError("Concept already represented by a Term with handle or value '{}'"
+                             "and origin_name '{}'".format(term_key, term.origin_name))
+        ent.concept.terms[(term_key, term.origin_name)] = term
+        self.terms[(term_key, term.origin_name)] = term
         
     def add_terms(self, prop, *terms):
         """Add a list of :class:`Term` and/or strings to a :class:`Property` with a value domain of ``value_set``
 
         :param Property prop: :class:`Property` to modify
         :param list terms: A list of :class:`Term` instances and/or str
 
-        :class:`Term` instances are created for strings; `Term.value` is set to the string.
+        :class:`Term` instances are created for strings; 
+        `Term.value` and `Term.handle` is set to the string.
         """
         if not isinstance(prop, Property):
             raise ArgError("arg1 must be Property")
         if not re.match("value_set|enum", prop.value_domain):
             raise AttributeError(
                 "Property value domain is not value_set or enum, can't add terms"
             )
@@ -207,18 +210,20 @@
             warn("Creating ValueSet object for Property " + prop.handle)
             prop.value_set = ValueSet({"prop": prop, "_id": str(uuid4())})
             prop.value_set.handle = self.handle + prop.value_set._id[0:8]
 
         for t in terms:
             if isinstance(t, str):
                 warn("Creating Term object for string '{term}'".format(term=t))
-                t = Term({"value": t})
+                t = Term({"handle":t, "value": t})
             elif not isinstance(t, Term):
                 raise ArgError("encountered arg that was not a str or Term object")
-            prop.value_set.terms[t.value] = t
+            tm_key = t.handle if t.handle else t.value
+            prop.value_set.terms[tm_key] = t
+            self.terms[(tm_key, t.origin_name)] = t
 
     def rm_node(self, node):
         """Remove a :class:`Node` from the Model instance.
 
         :param Node node: Node to be removed
 
         Note: A node can't be removed if it is participating in an edge (i.e.,
@@ -350,14 +355,16 @@
             return
         if isinstance(ent, Node):
             return ent in set(self.nodes.values())
         if isinstance(ent, Edge):
             return ent in set(self.edges.values())
         if isinstance(ent, Property):
             return ent in set(self.props.values())
+        if isinstance(ent, Term):
+            return ent in set(self.terms.values())
         pass
 
     def edges_in(self, node):
         """Get all :class:`Edge` that have a given :class:`Node` as their dst attribute
 
         :param Node node: The node
         :return: list of :class:`Edge`
```

### Comparing `bento_meta-0.0.54/src/bento_meta/object_map.py` & `bento_meta-0.1.3/src/bento_meta/object_map.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/objects.py` & `bento_meta-0.1.3/src/bento_meta/objects.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/_engine.py` & `bento_meta-0.1.3/src/bento_meta/util/_engine.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/cypher/clauses.py` & `bento_meta-0.1.3/src/bento_meta/util/cypher/clauses.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/cypher/entities.py` & `bento_meta-0.1.3/src/bento_meta/util/cypher/entities.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/cypher/functions.py` & `bento_meta-0.1.3/src/bento_meta/util/cypher/functions.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/cypher.py.old` & `bento_meta-0.1.3/src/bento_meta/util/cypher.py.old`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/makeq.py` & `bento_meta-0.1.3/src/bento_meta/util/makeq.py`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/src/bento_meta/util/query_paths.yml` & `bento_meta-0.1.3/src/bento_meta/util/query_paths.yml`

 * *Files identical despite different names*

### Comparing `bento_meta-0.0.54/setup.py` & `bento_meta-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 {'tools': ['numpy>=1.23.5,<2.0.0',
            'pandas>=1.5.2,<2.0.0',
            'spacy>=3.4.3,<4.0.0',
            'click>=8.1.3,<9.0.0']}
 
 setup_kwargs = {
     'name': 'bento-meta',
-    'version': '0.0.54',
+    'version': '0.1.3',
     'description': 'Python drivers for Bento Metamodel Database',
     'long_description': '# bento_meta - Object Model for the Bento Metamodel Database\n\nRead the docs at\n[https://cbiit.github.io/bento-meta/](https://cbiit.github.io/bento-meta/).\n\n\n',
     'author': 'Mark A. Jensen',
     'author_email': 'mark.jensen@nih.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bento_meta-0.0.54/PKG-INFO` & `bento_meta-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-meta
-Version: 0.0.54
+Version: 0.1.3
 Summary: Python drivers for Bento Metamodel Database
 License: Apache 2.0
 Author: Mark A. Jensen
 Author-email: mark.jensen@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

