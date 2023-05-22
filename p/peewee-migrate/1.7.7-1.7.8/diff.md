# Comparing `tmp/peewee_migrate-1.7.7.tar.gz` & `tmp/peewee_migrate-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.7.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.8.tar", max compression
```

## Comparing `peewee_migrate-1.7.7.tar` & `peewee_migrate-1.7.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4456 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/README.rst
--rw-r--r--   0        0        0      146 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11979 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/logs.py
--rw-r--r--   0        0        0    16468 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      461 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/router.py
--rw-r--r--   0        0        0     1709 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/types.py
--rw-r--r--   0        0        0     1589 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/README.rst
+-rw-r--r--   0        0        0      146 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    11862 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    16516 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1701 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1589 2023-05-22 21:38:45.437922 peewee_migrate-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.8/PKG-INFO
```

### Comparing `peewee_migrate-1.7.7/README.rst` & `peewee_migrate-1.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.7/peewee_migrate/auto.py` & `peewee_migrate-1.7.8/peewee_migrate/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,14 @@
             find_field_type(field),
             field.field_type,
             field.null,
             primary_key=field.primary_key,
             column_name=field.column_name,
             index=field.index,
             unique=field.unique,
-            default=field.default,
             **kwargs,
         )
 
         if self.field_class in FIELD_TO_PARAMS:
             if self.extra_parameters is None:  # type: ignore[has-type]
                 self.extra_parameters = {}
 
@@ -114,17 +113,14 @@
         return "{name}{space}={space}{module}.{field}".format(
             name=name, field=field, space=space, module=module
         )
 
     def get_field_parameters(self, *, change=False) -> TParams:
         """Generate parameters for self field."""
         params = super(Column, self).get_field_parameters()
-        if self.default is not None:
-            params.pop("constraints", None)
-
         params.pop("backref", None)
         if change:
             params["unique"] = bool(params.pop("unique", False))
             params["index"] = bool(params.pop("index", False)) or params["unique"]
             params.pop("on_delete", None)
             params.pop("on_update", None)
```

### Comparing `peewee_migrate-1.7.7/peewee_migrate/cli.py` & `peewee_migrate-1.7.8/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.7/peewee_migrate/migrator.py` & `peewee_migrate-1.7.8/peewee_migrate/migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,35 +60,33 @@
         operations: List[Union[Context, Operation]] = self.alter_change_column(
             table, column_name, field
         )
         if not field.null:
             operations.append(self.add_not_null(table, column_name))
         return operations
 
+    @operation
+    def add_default(self, table: str, column: str, field: pw.Field):
+        default = field.default
+        if callable(default):
+            default = default()
+        alter_column: pw.Context = self._alter_column(self.make_context(), table, column)
+        ctx: pw.Context = alter_column.literal(" SET DEFAULT ")
+        return ctx.sql(field.db_value(default))
+
     def alter_change_column(
         self, table: str, column: str, field: pw.Field
     ) -> List[Union[Context, Operation]]:
         """Support change columns."""
         ctx = self.make_context()
         field_null, field.null = field.null, True
         ctx = self._alter_table(ctx, table).literal(" ALTER COLUMN ").sql(field.ddl(ctx))
         field.null = field_null
         return [ctx]
 
-    @operation
-    def add_default(self, table, column, field):
-        default = field.default
-        if callable(default):
-            default = default()
-        return (
-            self._alter_column(self.make_context(), table, column)
-            .literal(" SET DEFAULT ")
-            .sql(field.db_value(default))
-        )
-
     def alter_add_column(
         self, table: str, column_name: str, field: pw.Field, **kwargs
     ) -> Operation:
         """Fix fieldname for ForeignKeys."""
         name = field.name
         op = super(SchemaMigrator, self).alter_add_column(table, column_name, field, **kwargs)
         if isinstance(field, pw.ForeignKeyField):
```

### Comparing `peewee_migrate-1.7.7/peewee_migrate/router.py` & `peewee_migrate-1.7.8/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.7/peewee_migrate/template.py` & `peewee_migrate-1.7.8/peewee_migrate/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     > migrator.drop_index(model, *col_names)
     > migrator.add_not_null(model, *field_names)
     > migrator.drop_not_null(model, *field_names)
     > migrator.add_default(model, field_name, default)
 
 \"\"\"
 
+from contextlib import suppress
+
 import peewee as pw
 from peewee_migrate import Migrator
-from decimal import ROUND_HALF_EVEN
 
-try:
+
+with suppress(ImportError):
     import playhouse.postgres_ext as pw_pext
-except ImportError:
-    pass
 
 
 def migrate(migrator: Migrator, database: pw.Database, *, fake=False):
     \"\"\"Write your migrations here.\"\"\"
     {migrate}
```

### Comparing `peewee_migrate-1.7.7/pyproject.toml` & `peewee_migrate-1.7.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.7"
+version = "1.7.8"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.7.7/PKG-INFO` & `peewee_migrate-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.7
+Version: 1.7.8
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

