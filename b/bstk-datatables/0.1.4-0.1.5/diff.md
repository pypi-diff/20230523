# Comparing `tmp/bstk_datatables-0.1.4.tar.gz` & `tmp/bstk_datatables-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.1.4.tar", max compression
+gzip compressed data, was "bstk_datatables-0.1.5.tar", max compression
```

## Comparing `bstk_datatables-0.1.4.tar` & `bstk_datatables-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4244 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/README.md
--rw-r--r--   0        0        0     2319 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/bstk_datatables/__init__.py
--rw-r--r--   0        0        0      871 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3248 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/bstk_datatables/merge.py
--rw-r--r--   0        0        0     6737 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1521 2023-03-03 02:50:14.070531 bstk_datatables-0.1.4/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-03-03 02:50:42.682411 bstk_datatables-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/README.md
+-rw-r--r--   0        0        0     2319 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3248 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     6968 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-05-23 02:16:35.067516 bstk_datatables-0.1.5/bstk_datatables/table.py
+-rw-r--r--   0        0        0      669 2023-05-23 02:17:01.871551 bstk_datatables-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.5/PKG-INFO
```

### Comparing `bstk_datatables-0.1.4/README.md` & `bstk_datatables-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.4/bstk_datatables/__init__.py` & `bstk_datatables-0.1.5/bstk_datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.4/bstk_datatables/entry.py` & `bstk_datatables-0.1.5/bstk_datatables/enum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,22 @@
+import copy
 import typing
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from enum import Enum as PyEnum
 
 
 @dataclass
-class Entry:
+class Enum:
     uuid: typing.AnyStr
+    references: typing.Dict[typing.AnyStr, typing.Any]
+    code: typing.AnyStr
     name: typing.AnyStr
-    table_id: typing.AnyStr = field(default=None)
-    references: typing.Dict[typing.AnyStr, typing.Any] = field(default=None)
-    connector_references: typing.Dict[typing.AnyStr, typing.Any] = field(default=None)
-    schemata: typing.List[typing.AnyStr] = field(default=None)
-    values: typing.Dict[typing.AnyStr, typing.Any] = field(default=None)
+    values: PyEnum
 
     def __post_init__(self):
-        if not self.references:
-            self.references = {}
-        if not self.connector_references:
-            self.connector_references = {}
-        if not self.schemata:
-            self.schemata = []
-        if not self.values:
-            self.values = {}
+        vals = [val for val in self.values]
+        self.values = PyEnum(self.name, vals)
 
     def export(self) -> typing.Dict[typing.AnyStr, typing.Any]:
-        return self.__dict__
+        rtn = copy.copy(self.__dict__)
+        rtn["values"] = [v.name for v in self.values]
+        return rtn
```

### Comparing `bstk_datatables-0.1.4/bstk_datatables/merge.py` & `bstk_datatables-0.1.5/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.4/bstk_datatables/schema.py` & `bstk_datatables-0.1.5/bstk_datatables/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     def add_field(self, schema_field: SchemaField) -> None:
         if schema_field.code in self._field_list:
             raise ValueError(f"Duplicate field name `{schema_field.name}`")
         self._field_list.append(schema_field.code)
         self.fields.append(schema_field)
 
-    def set_fields(self, schema_fields: typing.List(SchemaField)):
+    def set_fields(self, schema_fields: typing.List[SchemaField]):
         self._field_list = []
         self.fields = []
         for schema_field in schema_fields:
             self.add_field(schema_field)
 
     def process_values(self, values: typing.Dict) -> None:
         _schema: MarshmallowSchema = self._schema()
@@ -138,28 +138,29 @@
 
 @dataclass
 class SchemaFieldFormat:
     type: typing.Optional[typing.AnyStr]
     values: typing.Optional[typing.Any] = None
     lookup: typing.Optional[typing.Any] = None
     required: typing.Optional[bool] = field(default=False)
+    many: typing.Optional[bool] = field(default=False)
     _field: marshmallow_fields.Field = field(init=False, default=None)
     _missing_lookup: bool = field(init=False, default=False)
 
     def __post_init__(self):
         self._generate_marshmallow_field()
 
     def attach_lookup(
         self, lookup_value: typing.Union[typing.List[typing.AnyStr], PyEnum]
     ):
         self.lookup = lookup_value
         self._generate_marshmallow_field()
 
     def export(self) -> typing.Dict[typing.AnyStr, typing.Any]:
-        _fields = ["type", "values", "lookup", "required"]
+        _fields = ["type", "values", "lookup", "required", "many"]
         rtn = {}
         for _exportfield in _fields:
             if _exportfield == "lookup" and isinstance(
                 self.__dict__[_exportfield], Enum
             ):
                 rtn[_exportfield] = self.__dict__[_exportfield].code
                 continue
@@ -193,8 +194,13 @@
         return {**_field_params, **SCHEMAFIELD_EXTATTR[self.type]}
 
     def _generate_marshmallow_field(self):
         _field_params = self._get_field_params()
         if _field_params is None:
             return
 
-        self._field = self._get_mapped_fieldclass()(**_field_params)
+        if self.many:
+            self._field = marshmallow_fields.List(
+                self._get_mapped_fieldclass()(**_field_params)
+            )
+        else:
+            self._field = self._get_mapped_fieldclass()(**_field_params)
```

### Comparing `bstk_datatables-0.1.4/bstk_datatables/table.py` & `bstk_datatables-0.1.5/bstk_datatables/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import typing
 from dataclasses import dataclass, field
 
+from . import name_to_code
 from .entry import Entry
 from .schema import Schema
 
-from . import name_to_code
-
 
 @dataclass
 class Table:
     uuid: typing.AnyStr
     name: typing.AnyStr
     code: typing.Optional[typing.AnyStr] = field(default=None)
     references: typing.Dict[typing.AnyStr, typing.Any] = field(default=None)
@@ -44,10 +43,12 @@
 
         if _schema in self.schemata:
             return
 
         self.schemata.append(_schema)
 
     def adopt_entry(self, entry: Entry) -> Entry:
-        entry.table_id = self.uuid
+        if entry.table_id != self.uuid:
+            entry.table_id = self.uuid
+
         entry.schemata = list(dict.fromkeys(self.schemata + entry.schemata))
         return entry
```

### Comparing `bstk_datatables-0.1.4/pyproject.toml` & `bstk_datatables-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.1.4"
+version = "0.1.5"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.1.4/PKG-INFO` & `bstk_datatables-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.1.4
+Version: 0.1.5
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

