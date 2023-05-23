# Comparing `tmp/oarepo-model-builder-vocabularies-1.0.9.tar.gz` & `tmp/oarepo-model-builder-vocabularies-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-vocabularies-1.0.9.tar", last modified: Mon Apr 17 19:22:11 2023, max compression
+gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.0.tar", last modified: Tue May 23 08:21:20 2023, max compression
```

## Comparing `oarepo-model-builder-vocabularies-1.0.9.tar` & `oarepo-model-builder-vocabularies-4.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:19:42.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.429694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:18:39.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/setup.py
```

### Comparing `oarepo-model-builder-vocabularies-1.0.9/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 1.0.9
+Version: 4.0.0
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/datatypes.py` & `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-import munch
+import marshmallow as ma
 from marshmallow import fields
 from oarepo_model_builder.datatypes.datatypes import DataType
-from oarepo_model_builder.utils.hyphen_munch import HyphenMunch
 from oarepo_model_builder.validation import InvalidModelException
 from oarepo_model_builder_relations.datatypes import RelationDataType
 
 
 class VocabularyDataType(RelationDataType):
     model_type = "vocabulary"
     default_facet_class = "VocabularyFacet"
     default_facet_imports = [
         {"import": "oarepo_vocabularies.services.facets.VocabularyFacet"}
     ]
 
+    class ModelSchema(RelationDataType.ModelSchema):
+        vocabulary_type = ma.fields.String(
+            attribute="vocabulary-type", data_key="vocabulary-type"
+        )
+
     def prepare(self, context):
         vocabulary_type = self.definition.get("vocabulary-type", None)
         vocabulary_class = self.definition.pop("class", None)
 
         vocabulary_imports = self.definition.setdefault("imports", [])
         self.definition.setdefault("model", "vocabularies")
-        self.definition.setdefault(
-            "keys", ["id", "title", {"key": "type.id", "target": "type"}]
-        )
+        self.definition.setdefault("keys", ["id", "title"])
         self.definition.setdefault("marshmallow", {})
         self.definition.setdefault("ui", {}).setdefault("marshmallow", {})
         self.definition["ui"].setdefault("detail", "vocabulary_item")
         self.definition["ui"].setdefault("edit", "vocabulary_item")
         pid_field = self.definition.get("pid-field", None)
 
         if not pid_field:
@@ -107,41 +109,39 @@
                         return True
             return False
 
         if not has_key(keys, "id"):
             keys.append("id")
         if not has_key(keys, "title"):
             keys.append("title")
-        if not has_key(keys, "type.id"):
-            keys.append({"key": "type.id", "target": "type"})
         if not has_key(keys, "hierarchy"):
             keys.append(
                 {
                     "key": "hierarchy",
                     "model": {
                         "type": "object",
                         "marshmallow": {
-                            "schema-class": "oarepo_vocabularies.services.schemas.HierarchySchema",
+                            "class": "oarepo_vocabularies.services.schema.HierarchySchema",
                             "generate": False,
                             "imports": [
                                 {
-                                    "import": "oarepo_vocabularies.services.schemas.HierarchySchema"
+                                    "import": "oarepo_vocabularies.services.schema.HierarchySchema"
                                 }
                             ],
                         },
                         "ui": {
                             "marshmallow": {
-                                "schema-class": "oarepo_vocabularies.services.ui_schemas.HierarchyUISchema",
+                                "class": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema",
                                 "generate": False,
+                                "imports": [
+                                    {
+                                        "import": "oarepo_vocabularies.services.ui_schema.HierarchyUISchema"
+                                    }
+                                ],
                             },
-                            "imports": [
-                                {
-                                    "import": "oarepo_vocabularies.services.ui_schemas.HierarchyUISchema"
-                                }
-                            ],
                         },
                         "properties": {
                             "parent": {"type": "keyword"},
                             "level": {"type": "integer"},
                             "title": {
                                 "type": "array",
                                 "items": {
@@ -163,12 +163,12 @@
                                 "type": "array",
                                 "items": {"type": "keyword"},
                             },
                         },
                     },
                 }
             )
-        self.definition["keys"] = munch.munchify(list(keys), HyphenMunch)
+        self.definition["keys"] = list(keys)
         super().prepare(context)
 
 
 DATATYPES = [VocabularyDataType, TaxonomyDataType]
```

### Comparing `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.yaml` & `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 1.0.9
+Version: 4.0.0
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt` & `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder_vocabularies/__init__.py
 oarepo_model_builder_vocabularies/datatypes.py
-oarepo_model_builder_vocabularies/setup_cfg.py
 oarepo_model_builder_vocabularies.egg-info/PKG-INFO
 oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
 oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
 oarepo_model_builder_vocabularies.egg-info/entry_points.txt
 oarepo_model_builder_vocabularies.egg-info/not-zip-safe
 oarepo_model_builder_vocabularies.egg-info/requires.txt
 oarepo_model_builder_vocabularies.egg-info/top_level.txt
+oarepo_model_builder_vocabularies/builders/__init__.py
+oarepo_model_builder_vocabularies/builders/setup_cfg.py
 oarepo_model_builder_vocabularies/models/__init__.py
 oarepo_model_builder_vocabularies/models/vocabulary.json
 oarepo_model_builder_vocabularies/models/vocabulary.yaml
```

### Comparing `oarepo-model-builder-vocabularies-1.0.9/setup.cfg` & `oarepo-model-builder-vocabularies-4.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-vocabularies
-version = 1.0.9
+version = 4.0.0
 description = "A model builder plugin to reference vocabularies"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio vocabulary model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
@@ -14,32 +14,33 @@
 	Development Status :: 3 - Alpha
 
 [options]
 packages = find:
 python_requires = >=3.9
 zip_safe = False
 install_requires = 
-	oarepo-model-builder>=3.0.0
-	oarepo-model-builder-relations>=1.0.0
-	oarepo-model-builder-ui
+	oarepo-model-builder>=4.0.0
+	oarepo-model-builder-relations>=4.0.0
+	oarepo-model-builder-cf>=4.0.0
+	oarepo-model-builder-ui>=4.0.0
 
 [options.package_data]
 * = *.yaml, *.json, *.json5
 
 [options.extras_require]
 tests = 
 	pytest
 
 [options.entry_points]
 oarepo.models = 
 	vocabularies = oarepo_model_builder_vocabularies.models:vocabulary.json
 oarepo_model_builder.datatypes = 
 	vocabulary = oarepo_model_builder_vocabularies.datatypes:DATATYPES
-oarepo_model_builder.builders.model = 
-	2000-vocabularies  = oarepo_model_builder_vocabularies.setup_cfg:VocabulariesSetupCfgBuilder
+oarepo_model_builder.builders.record = 
+	2000-vocabularies  = oarepo_model_builder_vocabularies.builders.setup_cfg:VocabulariesSetupCfgBuilder
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
```

