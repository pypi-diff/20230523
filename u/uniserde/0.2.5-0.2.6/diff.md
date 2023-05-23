# Comparing `tmp/uniserde-0.2.5.tar.gz` & `tmp/uniserde-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.2.5.tar", max compression
+gzip compressed data, was "uniserde-0.2.6.tar", max compression
```

## Comparing `uniserde-0.2.5.tar` & `uniserde-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5899 2023-03-16 11:39:14.649107 uniserde-0.2.5/README.md
--rw-r--r--   0        0        0      635 2023-03-16 11:39:27.431210 uniserde-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      170 2023-03-16 11:39:14.649107 uniserde-0.2.5/uniserde/__init__.py
--rw-r--r--   0        0        0     4851 2023-03-16 11:39:14.649107 uniserde-0.2.5/uniserde/common.py
--rw-r--r--   0        0        0     6986 2023-03-16 11:39:14.649107 uniserde-0.2.5/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     4263 2023-03-16 11:39:14.649107 uniserde-0.2.5/uniserde/serde_bson.py
--rw-r--r--   0        0        0     2652 2023-03-16 11:39:14.649107 uniserde-0.2.5/uniserde/serde_class.py
--rw-r--r--   0        0        0    12384 2023-03-16 11:39:14.650107 uniserde-0.2.5/uniserde/serde_json.py
--rw-r--r--   0        0        0     6615 1970-01-01 00:00:00.000000 uniserde-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     7615 2023-05-23 16:07:35.830016 uniserde-0.2.6/README.md
+-rw-r--r--   0        0        0      635 2023-05-23 16:08:14.020016 uniserde-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-01-22 22:04:26.958846 uniserde-0.2.6/uniserde/__init__.py
+-rw-r--r--   0        0        0     4908 2023-05-23 16:07:35.826683 uniserde-0.2.6/uniserde/common.py
+-rw-r--r--   0        0        0     6986 2023-01-24 22:17:19.618656 uniserde-0.2.6/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     4491 2023-05-23 16:07:35.826683 uniserde-0.2.6/uniserde/serde_bson.py
+-rw-r--r--   0        0        0     2716 2023-05-23 16:07:35.826683 uniserde-0.2.6/uniserde/serde_class.py
+-rw-r--r--   0        0        0    12655 2023-05-23 16:07:35.826683 uniserde-0.2.6/uniserde/serde_json.py
+-rw-r--r--   0        0        0     8331 1970-01-01 00:00:00.000000 uniserde-0.2.6/PKG-INFO
```

### Comparing `uniserde-0.2.5/README.md` & `uniserde-0.2.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     'birthDate': '1988-12-01T00:00:00+00:00'
 }
 ```
 
 You can easily convert this to a string using Python's built-in `json` module if
 that's what you need.
 
-# API
+## API
 
 The API is intentionally simple. Functions/Classes you might be interested in
 are:
 
 - `as_json`, `as_bson`
 
   Given a class with type annotations, these create a JSON/BSON like dictionary.
@@ -69,55 +69,55 @@
 - `as_mongodb_schema` automatically creates JSON schemas compatible with MongoDB
   from models
 
 - Custom serialization / deserialization can be achieved by inheriting from the
   `Serde` class and overriding the `as_json`, `as_bson`, `from_json`,
   `from_bson` and/or `as_mongodb_schema` methods.
 
-# Types & Conventions
+## Types & Conventions
 
 The library tries to stick to the naming conventions used by the target formats:
 
 - names in JSON are written in lowerCamelCase, as is commonly done in
   JavaScript
 - BSON uses the same conventions as JSON
 - Python class names are expected to be written in UpperCamelCase
 - Python enum values must be in ALL_UPPER_CASE
 
-## JSON
+### JSON
 
-| Python         | JSON            | Notes                                                                                                                |
-| -------------- | --------------- | -------------------------------------------------------------------------------------------------------------------- |
-| bool           | bool            |
-| int            | float           |
-| float          | float           |
-| str            | str             |
-| List           | list            |
-| Optional       | value or `None` |
-| Any            | as-is           |
-| Literal[str]   | str             |
-| enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                    |
-| custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.  |
-| bytes          | str             | base64 encoded                                                                                                       |
-| datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them.|
-| Dict[str, ...] | dict            |
-| bson.ObjectID  | str             |
+| Python         | JSON            | Notes                                                                                                                 |
+| -------------- | --------------- | --------------------------------------------------------------------------------------------------------------------  |
+| bool           | bool            |                                                                                                                       |
+| int            | float           |                                                                                                                       |
+| float          | float           |                                                                                                                       |
+| str            | str             |                                                                                                                       |
+| List           | list            |                                                                                                                       |
+| Optional       | value or `None` |                                                                                                                       |
+| Any            | as-is           |                                                                                                                       |
+| Literal[str]   | str             |                                                                                                                       |
+| enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                     |
+| custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
+| bytes          | str             | base64 encoded                                                                                                        |
+| datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| Dict[str, ...] | dict            |                                                                                                                       |
+| bson.ObjectId  | str             |                                                                                                                       |
 
-## BSON
+### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
 
-| Python        | BSON          | Notes                                                                                               |
-| ------------- | ------------- | -----------------------------------------------------------------------------                       |
-| custom class  | dict          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB                       |
-| bytes         | bytes         |
-| datetime      | datetime      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention. |
-| bson.ObjectID | bson.ObjectId |
+| Python        | BSON          | Notes                                                                                                                                                 |
+| ------------- | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| custom class  | dict          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
+| bytes         | bytes         |                                                                                                                                                       |
+| datetime      | datetime      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
+| bson.ObjectId | bson.ObjectId |                                                                                                                                                       |
 
-# Schema Generation
+## Schema Generation
 
 If you are working with MongoDB you will come to appreciate the automatic schema
 generation. Calling `uniserde.as_mongodb_schema` on any supported class will return
 a MongoDB compatible JSON schema without hassle.
 
 For example `uniserde.as_mongodb_schema(Person)` with the `Person` class from above:
 
@@ -140,15 +140,15 @@
         '_id',
         'name',
         'birthDate'
     ]
 }
 ```
 
-# TODO
+## TODO
 
 - Support for `Union` is currently very limited. Really only `Optional` is
   supported (which maps to `Union`)
 - `Literal` currently only supports strings
 - Make support for BSON optional, so the library doesn't depend on MongoDB
 - Extend `as_child`, to allow marking some classes as abstract. i.e. their
   parents/children can be serialized, but not those classes themselves
```

### Comparing `uniserde-0.2.5/pyproject.toml` & `uniserde-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.2.5"
+version = "0.2.6"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uniserde-0.2.5/uniserde/common.py` & `uniserde-0.2.6/uniserde/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import inspect
 import re
+from datetime import datetime
 from typing import Any, Callable, Dict, Iterable, Optional, Type, get_origin
 
+from bson import ObjectId
+
 Recur = Callable[[Any, Type], Any]
 Serializer = Callable[[Any, Type, Recur], Any]
 Deserializer = Callable[[Any, Type, Recur], Any]
 
 
 _SPLIT_CAMEL_CASE_PATTERN = re.compile(
     ".+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)"
```

### Comparing `uniserde-0.2.5/uniserde/schema_mongodb.py` & `uniserde-0.2.6/uniserde/schema_mongodb.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.2.5/uniserde/serde_bson.py` & `uniserde-0.2.6/uniserde/serde_bson.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 from datetime import datetime, timezone
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from bson import ObjectId
 
 from . import serde_class, serde_json
 from .common import *
 
 __all__ = [
     "as_bson",
     "from_bson",
+    "Bsonable",
+]
+
+
+Bsonable = Union[
+    None,
+    bool,
+    int,
+    float,
+    str,
+    Dict[str, "Bsonable"],
+    List["Bsonable"],
+    Tuple["Bsonable", ...],
+    bytes,
+    ObjectId,
+    datetime,
 ]
 
 
 def serialize_bytes_to_bytes(
     value: Any,
     value_type: Type,
     recur: Recur,
@@ -80,15 +96,15 @@
 
 
 def as_bson(
     value: Any,
     *,
     as_type: Optional[Type] = None,
     custom_serializers: Dict[Type, Callable[[Any], Any]] = {},
-) -> Any:
+) -> Bsonable:
     return common_serialize(
         value,
         type(value) if as_type is None else as_type,
         serialize_class,
         BSON_SERIALIZERS,
         custom_serializers,
     )
```

### Comparing `uniserde-0.2.5/uniserde/serde_class.py` & `uniserde-0.2.6/uniserde/serde_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 
 class Serde:
     def as_bson(
         self,
         *,
         as_type: Optional[Type] = None,
         custom_serializers: Dict[Type, Callable[[Any], Any]] = {},
-    ) -> Dict[str, Any]:
+    ) -> Dict[str, serde_bson.Bsonable]:
         """
         Serialize the entire instance to BSON, by applying the field serializer
         to each field. Field names are converted to camel case.
         """
         assert as_type is None or issubclass(self.__class__, as_type), as_type
         return serde_bson.as_bson(
             self,
             as_type=as_type,
             custom_serializers=custom_serializers,
-        )
+        )  # type: ignore
 
     def as_json(
         self,
         *,
         as_type: Optional[Type] = None,
         custom_serializers: Dict[Type, Callable[[Any], Any]] = {},
-    ) -> Dict[str, Any]:
+    ) -> Dict[str, serde_json.Jsonable]:
         """
         Serialize the entire instance to JSON, by applying the field serializer
         to each field. Field names are converted to camel case.
         """
         assert as_type is None or issubclass(self.__class__, as_type), as_type
         return serde_json.as_json(
             self,
             as_type=as_type,
             custom_serializers=custom_serializers,
-        )
+        )  # type: ignore
 
     @classmethod
     def from_bson(
         cls: Type[T],
         document: Dict[str, Any],
         custom_deserializers: Dict[Type, Callable[[Any], Any]] = {},
     ) -> T:
```

### Comparing `uniserde-0.2.5/uniserde/serde_json.py` & `uniserde-0.2.6/uniserde/serde_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 import base64
 import inspect
+import typing
 from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, List, Literal, Type, Union, get_args, get_type_hints
+from typing import Any, Dict, List, Literal, Tuple, Type, Union
 
 import dateutil.parser
 from bson import ObjectId
 
 from . import serde_class
 from .common import *
 
 __all__ = [
     "as_json",
     "from_json",
+    "Jsonable",
+]
+
+
+Jsonable = Union[
+    None,
+    bool,
+    int,
+    float,
+    str,
+    Dict[str, "Jsonable"],
+    List["Jsonable"],
+    Tuple["Jsonable", ...],
 ]
 
 
 def serialize_bool_to_bool(
     value: Any,
     value_type: Type,
     recur: Recur,
@@ -75,23 +89,23 @@
 
 def serialize_list_to_list(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> List[Any]:
     assert isinstance(value, list), value
-    return [recur(v, get_args(value_type)[0]) for v in value]
+    return [recur(v, typing.get_args(value_type)[0]) for v in value]
 
 
 def serialize_dict_to_dict(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Dict[Any, Any]:
-    subtypes = get_args(value_type)
+    subtypes = typing.get_args(value_type)
     assert isinstance(value, dict), value
     return {recur(k, subtypes[0]): recur(v, subtypes[1]) for k, v in value.items()}
 
 
 def serialize_object_id_to_str(
     value: Any,
     value_type: Type,
@@ -105,15 +119,15 @@
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
     if value is None:
         return None
 
-    return recur(value, get_args(value_type)[0])
+    return recur(value, typing.get_args(value_type)[0])
 
 
 def serialize_any(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
@@ -131,27 +145,27 @@
 
 def serialize_tuple_as_list(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> List[Any]:
     assert isinstance(value, tuple), value
-    subtypes = get_args(value_type)
+    subtypes = typing.get_args(value_type)
     assert len(subtypes) == len(value), (subtypes, value)
 
     return [recur(v, subtype) for v, subtype in zip(value, subtypes)]
 
 
 def serialize_set_as_list(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> List[Any]:
     assert isinstance(value, set), value
-    subtype = get_args(value_type)[0]
+    subtype = typing.get_args(value_type)[0]
     return [recur(v, subtype) for v in value]
 
 
 def serialize_class(
     value: Any,
     value_type: Type,
     recur: Recur,
@@ -175,15 +189,15 @@
     # Case: Anything else
     # Make sure to serialize as the correct class
     if should_serialize_as_child(value_type):
         assert issubclass(type(value), value_type), (type(value), value_type)
         value_type = type(value)
 
     result = {}
-    for field_py_name, field_type in get_type_hints(value_type).items():
+    for field_py_name, field_type in typing.get_type_hints(value_type).items():
         field_doc_name = all_lower_to_camel_case(field_py_name)
         result[field_doc_name] = recur(getattr(value, field_py_name), field_type)
 
     # Add a type tag?
     if should_serialize_as_child(value_type):
         result["type"] = upper_camel_case_to_camel_case(value.__class__.__name__)
 
@@ -209,15 +223,15 @@
 
 
 def as_json(
     value: Any,
     *,
     as_type: Optional[Type] = None,
     custom_serializers: Dict[Type, Callable[[Any], Any]] = {},
-) -> Any:
+) -> Jsonable:
     return common_serialize(
         value,
         type(value) if as_type is None else as_type,
         serialize_class,
         JSON_SERIALIZERS,
         custom_serializers,
     )
@@ -263,15 +277,15 @@
 ) -> bytes:
     if not isinstance(value, str):
         raise SerdeError(f"Expected bytes encoded as string, got {value}")
 
     try:
         return base64.b64decode(value.encode("utf-8"))
     except ValueError:
-        raise SerdeError("Received inavlid base64 encoded string.")
+        raise SerdeError("Received invalid base64 encoded string.")
 
 
 def deserialize_str_from_str(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> str:
@@ -304,28 +318,28 @@
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> List[Any]:
     if not isinstance(value, list):
         raise SerdeError(f"Expected list, got {value}")
 
-    subtype = get_args(value_type)[0]
+    subtype = typing.get_args(value_type)[0]
 
     return [recur(v, subtype) for v in value]
 
 
 def deserialize_dict_from_dict(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Dict[Any, Any]:
     if not isinstance(value, dict):
         raise SerdeError(f"Expected dict, got {value}")
 
-    subtypes = get_args(value_type)
+    subtypes = typing.get_args(value_type)
 
     return {recur(k, subtypes[0]): recur(v, subtypes[1]) for k, v in value.items()}
 
 
 def deserialize_object_id_from_str(
     value: Any,
     value_type: Type,
@@ -346,15 +360,15 @@
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
     if value is None:
         return None
 
-    return recur(value, get_args(value_type)[0])
+    return recur(value, typing.get_args(value_type)[0])
 
 
 def deserialize_any(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
@@ -362,30 +376,30 @@
 
 
 def deserialize_literal_as_is(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
-    options = get_args(value_type)
+    options = typing.get_args(value_type)
     if value not in options:
         raise SerdeError(f"Expected {value_type}, got {value}")
 
     return value
 
 
 def deserialize_tuple_from_list(
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
     if not isinstance(value, list):
         raise SerdeError(f"Expected list, got {value}")
 
-    subtypes = get_args(value_type)
+    subtypes = typing.get_args(value_type)
 
     if len(value) != len(subtypes):
         raise SerdeError(
             f"Expected list of size {len(subtypes)}, but received one of size {len(value)}"
         )
 
     return tuple(recur(v, subtype) for v, subtype in zip(value, subtypes))
@@ -395,15 +409,15 @@
     value: Any,
     value_type: Type,
     recur: Recur,
 ) -> Any:
     if not isinstance(value, list):
         raise SerdeError(f"Expected list, got {value}")
 
-    subtype = get_args(value_type)[0]
+    subtype = typing.get_args(value_type)[0]
 
     return set(recur(v, subtype) for v in value)
 
 
 def deserialize_class(
     value: Any,
     value_type: Type,
@@ -453,16 +467,16 @@
     del value_type
 
     # Case: Anything else
     if not isinstance(value, dict):
         raise SerdeError(f"Expected Object, got {value}")
 
     # Deserialize each field
-    result = object.__new__(actual_type)
-    for field_name, field_type in get_type_hints(actual_type).items():
+    result = object.__new__(actual_type)  # type: ignore
+    for field_name, field_type in typing.get_type_hints(actual_type).items():
         doc_name = all_lower_to_camel_case(field_name)
 
         try:
             field_value = recur(value.pop(doc_name), field_type)
         except KeyError:
             raise SerdeError(f'Object is missing the "{doc_name}" field') from None
```

### Comparing `uniserde-0.2.5/PKG-INFO` & `uniserde-0.2.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.2.5
+Version: 0.2.6
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -57,15 +57,15 @@
     'birthDate': '1988-12-01T00:00:00+00:00'
 }
 ```
 
 You can easily convert this to a string using Python's built-in `json` module if
 that's what you need.
 
-# API
+## API
 
 The API is intentionally simple. Functions/Classes you might be interested in
 are:
 
 - `as_json`, `as_bson`
 
   Given a class with type annotations, these create a JSON/BSON like dictionary.
@@ -88,55 +88,55 @@
 - `as_mongodb_schema` automatically creates JSON schemas compatible with MongoDB
   from models
 
 - Custom serialization / deserialization can be achieved by inheriting from the
   `Serde` class and overriding the `as_json`, `as_bson`, `from_json`,
   `from_bson` and/or `as_mongodb_schema` methods.
 
-# Types & Conventions
+## Types & Conventions
 
 The library tries to stick to the naming conventions used by the target formats:
 
 - names in JSON are written in lowerCamelCase, as is commonly done in
   JavaScript
 - BSON uses the same conventions as JSON
 - Python class names are expected to be written in UpperCamelCase
 - Python enum values must be in ALL_UPPER_CASE
 
-## JSON
+### JSON
 
-| Python         | JSON            | Notes                                                                                                                |
-| -------------- | --------------- | -------------------------------------------------------------------------------------------------------------------- |
-| bool           | bool            |
-| int            | float           |
-| float          | float           |
-| str            | str             |
-| List           | list            |
-| Optional       | value or `None` |
-| Any            | as-is           |
-| Literal[str]   | str             |
-| enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                    |
-| custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.  |
-| bytes          | str             | base64 encoded                                                                                                       |
-| datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them.|
-| Dict[str, ...] | dict            |
-| bson.ObjectID  | str             |
+| Python         | JSON            | Notes                                                                                                                 |
+| -------------- | --------------- | --------------------------------------------------------------------------------------------------------------------  |
+| bool           | bool            |                                                                                                                       |
+| int            | float           |                                                                                                                       |
+| float          | float           |                                                                                                                       |
+| str            | str             |                                                                                                                       |
+| List           | list            |                                                                                                                       |
+| Optional       | value or `None` |                                                                                                                       |
+| Any            | as-is           |                                                                                                                       |
+| Literal[str]   | str             |                                                                                                                       |
+| enum.Enum      | str             | Enum values are mapped to their name (NOT value!)                                                                     |
+| custom class   | dict            | Each attribute is stored as key, in lowerCamelCase. If marked with `as_child`, an additional `type` field is added.   |
+| bytes          | str             | base64 encoded                                                                                                        |
+| datetime       | str             | as ISO 8601 - with timezone. Naïve datetimes are intentionally not supported. Do yourself a favor and don't use them. |
+| Dict[str, ...] | dict            |                                                                                                                       |
+| bson.ObjectId  | str             |                                                                                                                       |
 
-## BSON
+### BSON
 
 BSON uses the same conventions as JSON, with just a few changes
 
-| Python        | BSON          | Notes                                                                                               |
-| ------------- | ------------- | -----------------------------------------------------------------------------                       |
-| custom class  | dict          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB                       |
-| bytes         | bytes         |
-| datetime      | datetime      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention. |
-| bson.ObjectID | bson.ObjectId |
+| Python        | BSON          | Notes                                                                                                                                                 |
+| ------------- | ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| custom class  | dict          | Same as JSON, but any fields named `id` are renamed to `_id` to match MongoDB. (Exception: if an `_id` field is already present, `id` is not renamed) |
+| bytes         | bytes         |                                                                                                                                                       |
+| datetime      | datetime      | Serialization requires a timezone be set. Deserialization imputes UTC, to match MongoDB convention.                                                   |
+| bson.ObjectId | bson.ObjectId |                                                                                                                                                       |
 
-# Schema Generation
+## Schema Generation
 
 If you are working with MongoDB you will come to appreciate the automatic schema
 generation. Calling `uniserde.as_mongodb_schema` on any supported class will return
 a MongoDB compatible JSON schema without hassle.
 
 For example `uniserde.as_mongodb_schema(Person)` with the `Person` class from above:
 
@@ -159,15 +159,15 @@
         '_id',
         'name',
         'birthDate'
     ]
 }
 ```
 
-# TODO
+## TODO
 
 - Support for `Union` is currently very limited. Really only `Optional` is
   supported (which maps to `Union`)
 - `Literal` currently only supports strings
 - Make support for BSON optional, so the library doesn't depend on MongoDB
 - Extend `as_child`, to allow marking some classes as abstract. i.e. their
   parents/children can be serialized, but not those classes themselves
```

