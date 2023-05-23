# Comparing `tmp/dbml-to-fides-1.0.0a4.tar.gz` & `tmp/dbml-to-fides-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbml-to-fides-1.0.0a4.tar", last modified: Mon May 22 19:44:28 2023, max compression
+gzip compressed data, was "dbml-to-fides-1.0.0a5.tar", last modified: Tue May 23 13:04:04 2023, max compression
```

## Comparing `dbml-to-fides-1.0.0a4.tar` & `dbml-to-fides-1.0.0a5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.368521 dbml-to-fides-1.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/dbml_to_fides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/dbml_to_fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/dbml_to_fides/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/dbml_to_fides/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:44:28.368521 dbml-to-fides-1.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:04.677630 dbml-to-fides-1.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 13:04:04.677630 dbml-to-fides-1.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:04.673630 dbml-to-fides-1.0.0a5/dbml_to_fides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/dbml_to_fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/dbml_to_fides/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/dbml_to_fides/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:04.677630 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 13:04:04.000000 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 13:04:04.000000 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:04:04.000000 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 13:04:04.000000 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 13:04:04.000000 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:04:04.000000 dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:04:04.677630 dbml-to-fides-1.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:04:04.677630 dbml-to-fides-1.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 13:03:51.000000 dbml-to-fides-1.0.0a5/tests/test_transforms.py
```

### Comparing `dbml-to-fides-1.0.0a4/LICENSE.txt` & `dbml-to-fides-1.0.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a4/PKG-INFO` & `dbml-to-fides-1.0.0a5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -37,14 +37,16 @@
 Fides dataset manifest.
 
 Combined, this can be used in automation to ensure that datasets are kept
 up-to-date with the latest schema changes in continuous integration.
 
 ## Usage
 
+### Basic
+
 Given a sample DBML in `sample.dbml`:
 
 ```dbml
 Table users {
   id integer [primary key]
   username varchar
   role varchar
@@ -74,39 +76,44 @@
 
 ```sh
 $ dbml-to-fides sample.dbml
 dataset:
 - name: public
   collections:
   - name: users
+    description: Users
     fields:
     - name: id
       fides_meta:
         primary_key: true
     - name: username
     - name: role
     - name: created_at
   - name: posts
+    description: All the content you crave
     fields:
     - name: id
       fides_meta:
         primary_key: true
     - name: title
     - name: body
+      description: Content of the post
     - name: user_id
       fides_meta:
         references:
         - dataset: public
           field: users.id
           direction: to
     - name: status
     - name: created_at
 
 ```
 
+### Merging with existing Fides dataset
+
 If you have an existing Fides dataset in `.fides/sample_dataset.yml`:
 
 ```yaml
 dataset:
 - fides_key: sample_dataset
   organization_fides_key: default_organization
   name: public
@@ -219,14 +226,16 @@
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
 
+### File output
+
 If we wanted to write the output to a file,
 we would add the `--output-file` flag:
 
 ```shell
 $ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml --output-file .fides/sample_dataset.yml
 $ git diff
 diff --git a/.fides/sample_dataset.yml b/.fides/sample_dataset.yml
@@ -238,7 +247,107 @@
        - system.operations
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
+
+### Initial generation
+
+If you do not have an existing Fides dataset, the `--include-fides-keys` flag will
+create a more "fleshed out" version of a
+[Fides dataset](https://ethyca.github.io/fideslang/resources/dataset/)
+including all keys. See the [docs](https://ethyca.github.io/fideslang/resources/dataset/)
+for what each field can/should be populated with.
+
+```shell
+$ dbml-to-fides sample.dbml --include-fides-keys
+dataset:
+- name: public
+  collections:
+  - description: Users
+    data_categories: []
+    data_qualifiers: []
+    retention: null
+    name: users
+    fields:
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: id
+      fides_meta:
+        primary_key: true
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: username
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: role
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: created_at
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: social
+  - description: All the content you crave
+    data_categories: []
+    data_qualifiers: []
+    retention: null
+    name: posts
+    fields:
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: id
+      fides_meta:
+        primary_key: true
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: title
+    - description: Content of the post
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: body
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: user_id
+      fides_meta:
+        references:
+        - dataset: public
+          field: users.id
+          direction: to
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: status
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: created_at
+  fides_key: null
+  description: null
+  organization_fides_key: null
+  meta: {}
+  third_country_transfers: []
+  joint_controller: []
+  retention: null
+  data_categories: []
+  data_qualifiers: []
+```
```

### Comparing `dbml-to-fides-1.0.0a4/dbml_to_fides/transform.py` & `dbml-to-fides-1.0.0a5/dbml_to_fides/transform.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 from collections import defaultdict
 from copy import deepcopy
 from typing import Dict
 
 from deepmerge import always_merger
 from pydbml.database import Database
 
+dataset_keys = {
+    "fides_key": None,
+    "description": None,
+    "organization_fides_key": None,
+    "meta": {},
+    "third_country_transfers": [],
+    "joint_controller": [],
+    "retention": None,
+    "data_categories": [],
+    "data_qualifiers": [],
+}
+
+collection_keys = {
+    "description": None,
+    "data_categories": [],
+    "data_qualifiers": [],
+    "retention": None,
+}
+
+field_keys = {
+    "description": None,
+    "data_categories": [],
+    "data_qualifier": None,
+    "retention": None,
+}
+
 
 def unlistify(manifest):
     unlistified = {"dataset": {}}
     for dataset in deepcopy(manifest["dataset"]):
         collections = {}
         for collection in dataset["collections"]:
             collections[collection["name"]] = collection
@@ -52,26 +78,30 @@
     _new = unlistify(new)
 
     updated = always_merger.merge(_existing, _new)
 
     return relistify(updated)
 
 
-def dbml_to_fides_dataset_dict(dbml: Database) -> Dict:
+def dbml_to_fides_dataset_dict(dbml: Database, include_fides_keys: bool = False) -> Dict:
     collections = defaultdict(list)
     for table in dbml.tables:
-        collection = {}
+        collection = {**(deepcopy(collection_keys) if include_fides_keys else {})}
+
         collection["name"] = table.name
         if table.note:
             collection["description"] = str(table.note)
 
         fields = []
         for column in table.columns:
-            field = {}
+            field = {**(deepcopy(field_keys) if include_fides_keys else {})}
+
             field["name"] = column.name
+            if column.note:
+                field["description"] = str(column.note)
 
             fides_meta = {}
             if column.pk:
                 fides_meta["primary_key"] = True
 
             fides_meta_references = []
             for reference in column.get_refs():
@@ -101,11 +131,15 @@
         if fields:
             collection["fields"] = fields
 
         collections[table.schema].append(collection)
 
     return {
         "dataset": [
-            {"name": schema, "collections": _collections}
+            {
+                "name": schema,
+                "collections": _collections,
+                **(deepcopy(dataset_keys) if include_fides_keys else {}),
+            }
             for schema, _collections in collections.items()
         ]
     }
```

### Comparing `dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/PKG-INFO` & `dbml-to-fides-1.0.0a5/dbml_to_fides.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -37,14 +37,16 @@
 Fides dataset manifest.
 
 Combined, this can be used in automation to ensure that datasets are kept
 up-to-date with the latest schema changes in continuous integration.
 
 ## Usage
 
+### Basic
+
 Given a sample DBML in `sample.dbml`:
 
 ```dbml
 Table users {
   id integer [primary key]
   username varchar
   role varchar
@@ -74,39 +76,44 @@
 
 ```sh
 $ dbml-to-fides sample.dbml
 dataset:
 - name: public
   collections:
   - name: users
+    description: Users
     fields:
     - name: id
       fides_meta:
         primary_key: true
     - name: username
     - name: role
     - name: created_at
   - name: posts
+    description: All the content you crave
     fields:
     - name: id
       fides_meta:
         primary_key: true
     - name: title
     - name: body
+      description: Content of the post
     - name: user_id
       fides_meta:
         references:
         - dataset: public
           field: users.id
           direction: to
     - name: status
     - name: created_at
 
 ```
 
+### Merging with existing Fides dataset
+
 If you have an existing Fides dataset in `.fides/sample_dataset.yml`:
 
 ```yaml
 dataset:
 - fides_key: sample_dataset
   organization_fides_key: default_organization
   name: public
@@ -219,14 +226,16 @@
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
 
+### File output
+
 If we wanted to write the output to a file,
 we would add the `--output-file` flag:
 
 ```shell
 $ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml --output-file .fides/sample_dataset.yml
 $ git diff
 diff --git a/.fides/sample_dataset.yml b/.fides/sample_dataset.yml
@@ -238,7 +247,107 @@
        - system.operations
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
+
+### Initial generation
+
+If you do not have an existing Fides dataset, the `--include-fides-keys` flag will
+create a more "fleshed out" version of a
+[Fides dataset](https://ethyca.github.io/fideslang/resources/dataset/)
+including all keys. See the [docs](https://ethyca.github.io/fideslang/resources/dataset/)
+for what each field can/should be populated with.
+
+```shell
+$ dbml-to-fides sample.dbml --include-fides-keys
+dataset:
+- name: public
+  collections:
+  - description: Users
+    data_categories: []
+    data_qualifiers: []
+    retention: null
+    name: users
+    fields:
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: id
+      fides_meta:
+        primary_key: true
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: username
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: role
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: created_at
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: social
+  - description: All the content you crave
+    data_categories: []
+    data_qualifiers: []
+    retention: null
+    name: posts
+    fields:
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: id
+      fides_meta:
+        primary_key: true
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: title
+    - description: Content of the post
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: body
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: user_id
+      fides_meta:
+        references:
+        - dataset: public
+          field: users.id
+          direction: to
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: status
+    - description: null
+      data_categories: []
+      data_qualifier: null
+      retention: null
+      name: created_at
+  fides_key: null
+  description: null
+  organization_fides_key: null
+  meta: {}
+  third_country_transfers: []
+  joint_controller: []
+  retention: null
+  data_categories: []
+  data_qualifiers: []
+```
```

### Comparing `dbml-to-fides-1.0.0a4/pyproject.toml` & `dbml-to-fides-1.0.0a5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbml-to-fides"
-version = "1.0.0a4"
+version = "1.0.0a5"
 description = "Interoperatbility for DBML and Fides dataset manifests"
 
 readme = "README.md"
 requires-python = ">=3.8, <4"
 license = {file = "LICENSE.txt"}
 
 keywords = ["fides", "dbml"]
@@ -30,14 +30,15 @@
 
 dependencies = [ # Optional
   "click",
   "deepmerge",
   "fideslang",
   "pydbml",
   "pyaml",
+  "typing_extensions<4.6.0",
 ]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/ewdurbin/dbml-to-fides"
 "Source" = "https://github.com/ewdurbin/dbml-to-fides"
 
 [project.scripts]  # Optional
```

### Comparing `dbml-to-fides-1.0.0a4/tests/test_transforms.py` & `dbml-to-fides-1.0.0a5/tests/test_transforms.py`

 * *Files identical despite different names*

