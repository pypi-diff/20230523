# Comparing `tmp/qtgql-0.117.0.tar.gz` & `tmp/qtgql-0.118.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.117.0.tar", max compression
+gzip compressed data, was "qtgql-0.118.0.tar", max compression
```

## Comparing `qtgql-0.117.0.tar` & `qtgql-0.118.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-05-22 06:43:00.978167 qtgql-0.117.0/LICENSE
--rw-r--r--   0        0        0     1901 2023-05-22 06:43:00.978167 qtgql-0.117.0/README.md
--rw-r--r--   0        0        0     4342 2023-05-22 06:43:28.758674 qtgql-0.117.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1587 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    11556 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3731 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2065 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      413 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17696 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    10999 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     4152 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0     5662 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/runtime/queryhandler.py
--rw-r--r--   0        0        0      467 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      541 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     2065 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     2397 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     2461 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-05-22 06:43:00.994167 qtgql-0.117.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 qtgql-0.117.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-23 13:48:24.651340 qtgql-0.118.0/LICENSE
+-rw-r--r--   0        0        0     1901 2023-05-23 13:48:24.651340 qtgql-0.118.0/README.md
+-rw-r--r--   0        0        0     4363 2023-05-23 13:48:43.635882 qtgql-0.118.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    11706 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3500 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2065 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      413 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17696 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    10618 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1506 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      541 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     2806 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     2377 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     2034 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-05-23 13:48:24.663341 qtgql-0.118.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 qtgql-0.118.0/PKG-INFO
```

### Comparing `qtgql-0.117.0/LICENSE` & `qtgql-0.118.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/README.md` & `qtgql-0.118.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/pyproject.toml` & `qtgql-0.118.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.117.0"
+version = "0.118.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
@@ -31,14 +31,15 @@
 aiohttp = {extras = ["speedups"], version = "^3.8.3"}
 faker = ">=15.3.4,<19.0.0"
 mypy = "^1.0.1"
 strawberry-graphql = ">=0.158.2,<0.180.0"
 aqtinstall = "^3.1.6"
 conan = "^2.0.4"
 cmake = "3.25.0"
+pygithub = "^1.58.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.5"
 mike = "^1.1.2"
 markdown-include = "^0.8.0"
 mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.22.0"}
 pygments = "^2.14.0"
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/cli.py` & `qtgql-0.118.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.118.0/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/qtgqlcodegen/compiler/operation.py` & `qtgql-0.118.0/qtgqlcodegen/compiler/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,21 @@
         )
 
     @cached_property
     def type(self) -> GqlTypeHinter:
         return self.definition.type
 
     @cached_property
-    def property_annotation(self) -> str:
+    def property_type(self) -> str:
         if self.definition.type.is_object_type:
             assert self.narrowed_type
             return self.narrowed_type.name
-        return self.type.annotation
+        if cs := self.definition.is_custom_scalar:
+            return cs.property_type
+        return self.type.member_type
 
     @property
     def proxy_of(self) -> GqlTypeHinter:
         ret = self.definition.type
         assert ret
         return ret
 
@@ -243,18 +245,18 @@
         )
 
 
 @define(slots=False)
 class QtGqlOperationDefinition:
     operation_def: gql_def.OperationDefinitionNode
     evaluator: SchemaEvaluator
-    directives: list[str] = []
-    fragments: list[str] = []
-    variables: list[QtGqlVariableDefinition] = []
-    narrowed_types_map: dict[str, QtGqlQueriedObjectType] = {}
+    directives: list[str] = attrs.Factory(list)
+    fragments: list[str] = attrs.Factory(list)
+    variables: list[QtGqlVariableDefinition] = attrs.Factory(list)
+    narrowed_types_map: dict[str, QtGqlQueriedObjectType] = attrs.Factory(dict)
 
     def __attrs_post_init__(self) -> None:
         # instantiating the queried fields here, they build the narrowed types.
         self.root_field  # noqa
 
     @property
     def operation_config(self) -> str:
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/compiler/template.py` & `qtgql-0.118.0/qtgqlcodegen/compiler/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-import inspect
-from typing import Any
 from typing import TYPE_CHECKING
 
 from attrs import define
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
 
@@ -49,25 +47,19 @@
     types: list[QtGqlObjectTypeDefinition]
     interfaces: list[QtGqlInterfaceDefinition]
     input_objects: list[QtGqlInputObjectTypeDefinition]
     config: QtGqlConfig
 
     @property
     def dependencies(self) -> list[str]:
-        def build_import_statement(t: type[Any]) -> str:
-            mod = inspect.getmodule(t)
-            assert mod
-            return f"from {mod.__name__} import {t.__name__}"
-
-        ret = [build_import_statement(scalar) for scalar in self.config.custom_scalars.values()]
-        return ret
+        return [f"#include {scalar.include_path}" for scalar in self.config.custom_scalars.values()]
 
     @property
     def custom_scalars(self) -> list[str]:
-        return [scalar.__name__ for scalar in self.config.custom_scalars.values()]
+        return [scalar.graphql_name for scalar in self.config.custom_scalars.values()]
 
 
 @define(slots=False)
 class OperationTemplateContext:
     operation: QtGqlOperationDefinition
     config: QtGqlConfig
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/config.py` & `qtgql-0.118.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/qtgqlcodegen/graphql_ref.py` & `qtgql-0.118.0/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/qtgqlcodegen/introspection.py` & `qtgql-0.118.0/qtgqlcodegen/introspection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/qtgqlcodegen/objecttype.py` & `qtgql-0.118.0/qtgqlcodegen/objecttype.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 import contextlib
 import enum
 from functools import cached_property
 from typing import Any
 from typing import Generic
 from typing import Optional
-from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attrs
 from attrs import define
 from typingref import TypeHinter
 from typingref import UNSET
 
 from qtgqlcodegen.compiler.builtin_scalars import BuiltinScalar
 from qtgqlcodegen.compiler.operation import QtGqlQueriedObjectType
 from qtgqlcodegen.cppref import QtGqlTypes
-from qtgqlcodegen.runtime.custom_scalars import BaseCustomScalar
-from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
 from qtgqlcodegen.utils import AntiForwardRef
 
+if TYPE_CHECKING:
+    from qtgqlcodegen.runtime.custom_scalars import CustomScalarDefinition
+    from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
+
 
 class Kinds(enum.Enum):
     SCALAR = "SCALAR"
     OBJECT = "OBJECT"
     ENUM = "ENUM"
     LIST = "LIST"
     UNION = "UNION"
@@ -38,25 +40,25 @@
     name: str
     type: GqlTypeHinter
     type_map: dict[str, QtGqlObjectTypeDefinition]
     enums: EnumMap
     scalars: CustomScalarMap
 
     @cached_property
-    def is_custom_scalar(self) -> Optional[Type[BaseCustomScalar]]:
+    def is_custom_scalar(self) -> Optional[CustomScalarDefinition]:
         return self.type.is_custom_scalar
 
     @cached_property
-    def annotation(self) -> str:
+    def member_type(self) -> str:
         """
         :returns: Annotation of the field based on the real type,
         meaning that the private attribute would be of that type.
         this goes for init and the property setter.
         """
-        return self.type.annotation
+        return self.type.member_type
 
 
 T = TypeVar("T")
 
 
 @define(slots=False)
 class QtGqlVariableDefinition(Generic[T], QtGqlBaseTypedNode):
@@ -68,15 +70,15 @@
         if self.type.is_input_object_type:
             return f"{attr_name}.asdict()"
         elif self.type.is_builtin_scalar:
             return attr_name
         elif self.type.is_enum:
             return f"{attr_name}.name"
         elif self.is_custom_scalar:
-            return f"{attr_name}.{BaseCustomScalar.parse_value.__name__}()"
+            raise NotImplementedError
 
         raise NotImplementedError(f"{self.type} is not supported as an input type ATM")
 
 
 @define(slots=False)
 class BaseQtGqlFieldDefinition(QtGqlBaseTypedNode):
     description: Optional[str] = ""
@@ -98,33 +100,33 @@
         if self.type.is_object_type:
             return "None"
 
         if self.type.is_model:
             # this would just generate the model without data.
             return "list()"
 
-        if custom_scalar := self.type.is_custom_scalar:
-            return f"SCALARS.{custom_scalar.__name__}()"
+        if self.type.is_custom_scalar:
+            return "{}"
 
         if enum_def := self.type.is_enum:
             return f"{enum_def.name}(1)"  # 1 is where auto() starts.
 
         return "None"  # Unions are not supported yet.
 
     @cached_property
     def fget_annotation(self) -> str:
         """This annotates the value that is QML-compatible."""
         if custom_scalar := self.type.is_custom_scalar:
             return TypeHinter.from_annotations(
-                custom_scalar.to_qt.__annotations__["return"],
+                custom_scalar.property_type,
             ).stringify()
         if self.type.is_enum:
             return "int"
 
-        return self.annotation
+        return self.member_type
 
     @cached_property
     def property_type(self) -> str:
         if self.type.is_builtin_scalar or self.type.is_custom_scalar:
             return self.fget_annotation
         else:
             if self.type.is_enum:
@@ -152,22 +154,14 @@
     def signal_name(self) -> str:
         return f"{self.name}Changed"
 
     @cached_property
     def private_name(self) -> str:
         return f"m_{self.name}"
 
-    @property
-    def fget(self) -> str:
-        if self.type.is_custom_scalar:
-            return f"return self.{self.private_name}.{BaseCustomScalar.to_qt.__name__}()"
-        if self.type.is_enum:
-            return f"return self.{self.private_name}.value"
-        return f"return self.{self.private_name}"
-
     @cached_property
     def can_select_id(self) -> Optional[QtGqlFieldDefinition]:
         object_type = self.type.is_object_type or self.type.is_interface
         if not object_type:
             if self.type.is_model:
                 object_type = self.type.is_model.is_object_type
         if object_type:
@@ -303,45 +297,45 @@
     @cached_property
     def is_builtin_scalar(self) -> Optional[BuiltinScalar]:
         t_self = self.optional_maybe.type
         if isinstance(t_self, BuiltinScalar):
             return t_self
 
     @cached_property
-    def is_custom_scalar(self) -> Optional[Type[BaseCustomScalar]]:
+    def is_custom_scalar(self) -> Optional[CustomScalarDefinition]:
         t_self = self.optional_maybe.type
         if t_self in self.scalars.values():
             return t_self
 
     @cached_property
-    def annotation(self) -> str:
+    def member_type(self) -> str:
         """
         :returns: Annotation of the field based on the real type,
         meaning that the private attribute would be of that type.
         this goes for init and the property setter. They are optional by default,
         (at the template) so unwrap optional first
         """
         t_self = self.optional_maybe
 
         # int, str, float etc...
         if builtin_scalar := t_self.is_builtin_scalar:
             return builtin_scalar.tp
 
         if scalar := t_self.is_custom_scalar:
-            return f"SCALARS.{scalar.__name__}"
+            return scalar.type_name
         if gql_enum := t_self.is_enum:
             return gql_enum.name
         if model_of := t_self.is_model:
-            return f"{QtGqlTypes.QGraphQLList.name}[{model_of.annotation}]"
+            return f"{QtGqlTypes.QGraphQLList.name}[{model_of.member_type}]"
         if object_def := t_self.is_object_type or t_self.is_interface:
             return f"{object_def.name}"
         if q_object_def := t_self.is_queried_object_type:
             return f"{q_object_def.name}"
         if t_self.is_union:
-            return "std::variant<" + ", ".join(th.annotation for th in t_self.of_type) + ">"
+            return "std::variant<" + ", ".join(th.member_type for th in t_self.of_type) + ">"
         if input_obj := t_self.is_input_object_type:
             return input_obj.name
 
         raise NotImplementedError  # pragma no cover
 
     def as_annotation(self, object_map=None):  # pragma: no cover
         raise NotImplementedError("not safe to call on this type")
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.118.0/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.118.0/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -17,44 +17,74 @@
         parent,
         field_data,
         inner_config,
         metadata,
     )
 {% elif f.type.is_model -%}
 {% if f.type.is_model.is_object_type -%}
-👉 assign_to 👈 = QGraphQListModel(
+👉 assign_to 👈 = qtgql::ListModel(
   parent=parent,
   data=[👉f.type.is_model.is_object_type.name👈.from_dict(parent, data=node, config=inner_config, metadata=metadata) for
         node in field_data],
 )
 {% elif f.type.is_model.is_interface -%}
-👉 assign_to 👈 = QGraphQListModel(
+👉 assign_to 👈 = qtgql::ListModel(
     parent=parent,
     data=[👉f.type.is_model.is_interface.name👈.from_dict(parent, data=node, config=inner_config, metadata=metadata) for
           node in field_data],
 )
 {% elif f.type.is_model.is_union -%}
 model_data = []
 for node in field_data:
     type_name = node['__typename']
     choice = inner_config.choices[type_name]
     model_data.append(
         __TYPE_MAP__[type_name].from_dict(self, node,
                                           choice, metadata)
     )
-👉 assign_to 👈 = QGraphQListModel(parent, data=model_data)
+👉 assign_to 👈 = qtgql::ListModel(parent, data=model_data)
 {% endif %}
 {% elif f.type.is_builtin_scalar -%}
 👉 assign_to 👈 = data.value("👉f.name👈").👉 f.type.type.from_json_convertor 👈;
 {% elif f.is_custom_scalar -%}
-👉 assign_to 👈 = SCALARS.👉f.is_custom_scalar.__name__👈.deserialize(field_data);
+👉 assign_to 👈 = 👉 f.is_custom_scalar.type_name 👈();
+👉 assign_to 👈.deserialize(data.value("👉f.name👈"));
 {% elif f.type.is_enum -%}
 👉 assign_to 👈 = 👉f.type.is_enum.name👈[field_data];
 {% elif f.type.is_union -%}
 type_name = field_data['__typename']
 choice = inner_config.choices[type_name]
 👉 assign_to 👈 = __TYPE_MAP__[type_name].from_dict(parent, field_data, choice, metadata);
 {% endif -%}
 };
 {%- endmacro %}
 
 
+
+{% macro props(type) -%}
+protected:
+{% for f in type.fields -%}
+👉 f.member_type 👈 👉 f.private_name 👈 = 👉 f.default_value 👈;
+{% endfor %}
+signals:
+{%for f in type.fields -%}
+void 👉 f.signal_name 👈();
+{% endfor %}
+
+public:
+{%for f in type.fields %}
+{% if f.is_custom_scalar %}
+const 👉 f.is_custom_scalar.property_type 👈 & 👉 f.getter_name 👈() {
+return 👉 f.private_name 👈.to_qt();
+}
+{% else %}
+const 👉 f.member_type 👈 & 👉 f.getter_name 👈() const {
+return 👉 f.private_name 👈;
+}
+{% endif %}
+void 👉 f.setter_name 👈(const 👉 f.member_type 👈 &v)
+{
+👉 f.private_name 👈 = v;
+emit 👉 f.signal_name 👈();
+};
+{% endfor %}
+{% endmacro -%}
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.118.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% import "macros.jinja.hpp" as macros -%}
 #pragma once
 #include "./schema.hpp"
-#include "qtgqloperationhandler.hpp"
+#include <qtgql/gqlwstransport/operationhandler.hpp>
 namespace 👉 context.config.env_name 👈{
 namespace 👉context.ns👈{
 
 inline const qtgql::OperationMetadata OPERATION_METADATA = qtgql::OperationMetadata{
         "👉 context.operation.name 👈",
         {
                 👉 context.operation.root_field.as_conf_string() 👈
@@ -25,51 +25,51 @@
 
 👉 t.name 👈(const QJsonObject& data,
 const qtgql::SelectionsConfig& config){
     m_inst = 👉context.schema_ns👈::👉 t.definition.name 👈::from_json(data, config, OPERATION_METADATA);
 
 }
 {%- for f in t.fields.values() %}
-inline const 👉 f.type.annotation 👈 & 👉 f.definition.getter_name 👈() const {
+inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
     return m_inst->👉 f.definition.getter_name 👈();
 };
 {% endfor -%}
 };
 {% endfor %}
 
-class 👉 context.operation.name 👈: public qtgql::QtGqlOperationHandlerABC {
+class 👉 context.operation.name 👈: public qtgql::OperationHandlerABC {
     Q_OBJECT
-Q_PROPERTY(const 👉 context.operation.root_field.property_annotation 👈* data READ get_data NOTIFY dataChanged);
+Q_PROPERTY(const 👉 context.operation.root_field.property_type 👈* data READ get_data NOTIFY dataChanged);
 
-std::unique_ptr<👉 context.operation.root_field.property_annotation 👈> m_data;
+std::unique_ptr<👉 context.operation.root_field.property_type 👈> m_data;
 
 inline const QString &ENV_NAME() override{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
 public:
 
-👉 context.operation.name 👈(): qtgql::QtGqlOperationHandlerABC(qtgql::GqlWsTrnsMsgWithID(qtgql::OperationPayload(
+👉 context.operation.name 👈(): qtgql::OperationHandlerABC(qtgql::GqlWsTrnsMsgWithID(qtgql::OperationPayload(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
         ))){};
 
 inline const QUuid &operation_id() const override{
 return m_message_template.op_id;
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data && message.contains("data")){
         auto data = message.value("data").toObject();
         if (data.contains("👉 context.operation.root_field.name 👈")){
-            m_data = std::make_unique<👉 context.operation.root_field.property_annotation 👈>(data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA.selections);
+            m_data = std::make_unique<👉 context.operation.root_field.property_type 👈>(data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA.selections);
         }
     }
 }
-inline const 👉 context.operation.root_field.property_annotation 👈* get_data(){
+inline const 👉 context.operation.root_field.property_type 👈* get_data(){
     return m_data.get();
 }
 
 signals:
     void dataChanged();
 };
 };
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.118.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,44 @@
 {% import "macros.jinja.hpp" as macros -%}
 #pragma once
 #include <QObject>
 #include <QJsonObject>
 #include <memory>
-#include <qtgqlobjecttype.hpp>
-#include <qtgqlmetadata.hpp>
-#include <qtgqlconstants.hpp>
-
-namespace 👉context.config.env_name👈{
-{% macro props(type) %}
-protected:
-
-{% for f in type.fields -%}
-👉f.annotation👈 👉f.private_name👈 = 👉f.default_value👈;
-{% endfor %}
-signals:
-{%for f in type.fields -%}
-void 👉f.signal_name👈();
+#include <qtgql/bases/objecttype.hpp>
+#include <qtgql/bases/metadata.hpp>
+#include <qtgql/bases/constants.hpp>
+{% for dep in context.dependencies %}
+👉 dep 👈
 {% endfor %}
 
-public:
-{%for f in type.fields %}
-const 👉f.annotation👈 & 👉f.getter_name👈() const {
-    return 👉f.private_name👈;
-}
-void 👉f.setter_name👈(const 👉f.annotation👈 &v)
-{
-  👉f.private_name👈 = v;
-  emit 👉f.signal_name👈();
-};
-{% endfor %}
-{% endmacro %}
+namespace 👉 context.config.env_name 👈{
+
 // ----------- Object Types -----------
 {% for type in context.types %}
-{%- set base_class -%}{% if type.has_id_field %}QtGqlObjectTypeABCWithID{% else %}QtGqlObjectTypeABC{% endif %}{%- endset -%}
+{%- set base_class -%}{% if type.has_id_field %}ObjectTypeABCWithID{% else %}ObjectTypeABC{% endif %}{%- endset -%}
 class 👉 type.name 👈 : public qtgql::👉 base_class 👈{
 protected:
 static auto & INST_STORE() {
-    static qtgql::QGraphQLObjectStore<👉 type.name 👈> _store;
+    static qtgql::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
 
-👉 props(type) 👈
+👉 macros.props(type) 👈
 public:
 inline static const QString TYPE_NAME = "👉 type.name 👈";
-👉type.name👈 (QObject* parent = nullptr)
+👉 type.name 👈 (QObject* parent = nullptr)
 : qtgql::👉 base_class 👈::👉 base_class 👈(parent) {};
 
 
-static std::shared_ptr<👉type.name👈> from_json(const QJsonObject& data,
+static std::shared_ptr<👉 type.name 👈> from_json(const QJsonObject& data,
                                  const qtgql::SelectionsConfig& config,
                                  const qtgql::OperationMetadata& metadata){
-auto inst = std::make_shared<👉type.name👈>();
+auto inst = std::make_shared<👉 type.name 👈>();
 {% for f in type.fields -%}
-{% set assign_to %} inst->👉f.private_name👈 {% endset %}
+{% set assign_to %} inst->👉 f.private_name 👈 {% endset %}
 👉macros.deserialize_field(f, assign_to)👈
 {% endfor %}
 
 {% if type.id_is_optional %}
 if (inst->id) {
   auto record = NodeRecord(node = inst, retainers = set())
                     .retain(metadata.operation_name)
```

### Comparing `qtgql-0.117.0/qtgqlcodegen/utils.py` & `qtgql-0.118.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.117.0/PKG-INFO` & `qtgql-0.118.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.117.0
+Version: 0.118.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

