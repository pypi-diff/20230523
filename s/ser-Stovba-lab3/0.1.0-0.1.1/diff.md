# Comparing `tmp/ser_Stovba_lab3-0.1.0.tar.gz` & `tmp/ser_Stovba_lab3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ser_Stovba_lab3-0.1.0.tar", last modified: Wed May 17 10:34:33 2023, max compression
+gzip compressed data, was "ser_Stovba_lab3-0.1.1.tar", last modified: Tue May 23 21:51:17 2023, max compression
```

## Comparing `ser_Stovba_lab3-0.1.0.tar` & `ser_Stovba_lab3-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:34:33.263337 ser_Stovba_lab3-0.1.0/
--rw-rw-rw-   0        0        0      407 2023-05-17 10:34:33.263337 ser_Stovba_lab3-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-17 10:33:56.000000 ser_Stovba_lab3-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 10:34:33.216604 ser_Stovba_lab3-0.1.0/ser_Stovba/
--rw-rw-rw-   0        0        0     1427 2023-05-17 09:26:02.000000 ser_Stovba_lab3-0.1.0/ser_Stovba/constants.py
--rw-rw-rw-   0        0        0      390 2023-05-17 05:43:59.000000 ser_Stovba_lab3-0.1.0/ser_Stovba/factory.py
--rw-rw-rw-   0        0        0     2974 2023-05-17 05:35:44.000000 ser_Stovba_lab3-0.1.0/ser_Stovba/json_serializer.py
--rw-rw-rw-   0        0        0     8766 2023-05-17 09:59:33.000000 ser_Stovba_lab3-0.1.0/ser_Stovba/serializersi.py
--rw-rw-rw-   0        0        0     2982 2023-05-17 05:39:58.000000 ser_Stovba_lab3-0.1.0/ser_Stovba/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-17 10:34:33.263337 ser_Stovba_lab3-0.1.0/ser_Stovba_lab3.egg-info/
--rw-rw-rw-   0        0        0      407 2023-05-17 10:34:33.000000 ser_Stovba_lab3-0.1.0/ser_Stovba_lab3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-17 10:34:33.000000 ser_Stovba_lab3-0.1.0/ser_Stovba_lab3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:34:33.000000 ser_Stovba_lab3-0.1.0/ser_Stovba_lab3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-17 10:34:33.000000 ser_Stovba_lab3-0.1.0/ser_Stovba_lab3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 10:34:33.000000 ser_Stovba_lab3-0.1.0/ser_Stovba_lab3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 10:34:33.263337 ser_Stovba_lab3-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-05-17 10:23:50.000000 ser_Stovba_lab3-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:51:17.347378 ser_Stovba_lab3-0.1.1/
+-rw-rw-rw-   0        0        0      407 2023-05-23 21:51:17.346381 ser_Stovba_lab3-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-17 10:33:56.000000 ser_Stovba_lab3-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 21:51:17.260217 ser_Stovba_lab3-0.1.1/ser_Stovba/
+-rw-rw-rw-   0        0        0     1432 2023-05-23 21:16:35.000000 ser_Stovba_lab3-0.1.1/ser_Stovba/constants.py
+-rw-rw-rw-   0        0        0      386 2023-05-17 14:14:32.000000 ser_Stovba_lab3-0.1.1/ser_Stovba/factory.py
+-rw-rw-rw-   0        0        0     2974 2023-05-17 11:39:27.000000 ser_Stovba_lab3-0.1.1/ser_Stovba/json_serializer.py
+-rw-rw-rw-   0        0        0     9327 2023-05-23 21:33:24.000000 ser_Stovba_lab3-0.1.1/ser_Stovba/serializersi.py
+-rw-rw-rw-   0        0        0     2982 2023-05-17 05:39:58.000000 ser_Stovba_lab3-0.1.1/ser_Stovba/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:51:17.344386 ser_Stovba_lab3-0.1.1/ser_Stovba_lab3.egg-info/
+-rw-rw-rw-   0        0        0      407 2023-05-23 21:51:16.000000 ser_Stovba_lab3-0.1.1/ser_Stovba_lab3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-05-23 21:51:16.000000 ser_Stovba_lab3-0.1.1/ser_Stovba_lab3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 21:51:16.000000 ser_Stovba_lab3-0.1.1/ser_Stovba_lab3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 21:51:16.000000 ser_Stovba_lab3-0.1.1/ser_Stovba_lab3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 21:51:16.000000 ser_Stovba_lab3-0.1.1/ser_Stovba_lab3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 21:51:17.347378 ser_Stovba_lab3-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1046 2023-05-23 21:44:53.000000 ser_Stovba_lab3-0.1.1/setup.py
```

### Comparing `ser_Stovba_lab3-0.1.0/ser_Stovba/constants.py` & `ser_Stovba_lab3-0.1.1/ser_Stovba/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import types
 
-BASE_TYPES = {"str": str, "int": int, "bool": bool, "float": float, "complex": complex}
+PRIMITIVES = {"str": str, "int": int, "bool": bool, "float": float, "complex": complex}
 
-SIMILAR_COLLECTIONS = {"list": list, "tuple": tuple, "frozenset": frozenset, "set": set, "bytes": bytes,
+COLLECTIONS_PRIMITIVES = {"list": list, "tuple": tuple, "frozenset": frozenset, "set": set, "bytes": bytes,
                        "bytearray": bytearray}
 
 BASE_COLLECTIONS = {"list": list, "tuple": tuple, "frozenset": frozenset, "set": set, "bytes": bytes,
                     "bytearray": bytearray, "dict": dict}
 
 METHODS = {"staticmethod": staticmethod, "classmethod": classmethod}
 
@@ -23,14 +23,15 @@
                    "co_filename",
                    "co_name",
                    "co_firstlineno",
                    "co_lnotab",
                    "co_freevars",
                    "co_cellvars")
 
+
 CLASS_PROPERTIES = ("__name__", "__base__",
                           "__basicsize__", "__dictoffset__", "__class__")
 
 TYPESES = (
                 types.WrapperDescriptorType,
                 types.MethodDescriptorType,
                 types.BuiltinFunctionType,
```

### Comparing `ser_Stovba_lab3-0.1.0/ser_Stovba/json_serializer.py` & `ser_Stovba_lab3-0.1.1/ser_Stovba/json_serializer.py`

 * *Files identical despite different names*

### Comparing `ser_Stovba_lab3-0.1.0/ser_Stovba/serializersi.py` & `ser_Stovba_lab3-0.1.1/ser_Stovba/serializersi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import inspect
-import re
-import types
 
+import types
+import sys
 
-from ser_Stovba.constants import BASE_TYPES, SIMILAR_COLLECTIONS, CODE_PROPERTIES, BASE_COLLECTIONS, CLASS_PROPERTIES, TYPESES, \
-    METHODS
+from ser_Stovba.constants import PRIMITIVES, COLLECTIONS_PRIMITIVES, CODE_PROPERTIES, BASE_COLLECTIONS, \
+    CLASS_PROPERTIES, TYPESES, METHODS
 
 
 def serialize(obj):
-    if isinstance(obj, tuple(BASE_TYPES.values())):
+    if isinstance(obj, tuple(PRIMITIVES.values())):
         return serialize_single_var(obj)
     elif isinstance(obj, types.NoneType):
         return serialize_none_type()
-    elif isinstance(obj, tuple(SIMILAR_COLLECTIONS.values())):
+    elif isinstance(obj, tuple(COLLECTIONS_PRIMITIVES.values())):
         return serialize_collections(obj)
     elif isinstance(obj, dict):
         return serialize_dict(obj)
     elif inspect.isfunction(obj):
         return serialize_function(obj)
     elif inspect.iscode(obj):
         return serialize_code(obj)
     elif isinstance(obj, types.CellType):
         return serialize_cell(obj)
     elif inspect.isclass(obj):
         return serialize_class(obj)
+    elif iteration_check(obj):
+        return serialize_iter_objects(obj)
     else:
         return serialize_object(obj)
 
 
+def iteration_check(obj):
+    return hasattr(obj, "__next__") and hasattr(obj, "__iter__") and callable(obj.__iter__)
+
+
 def get_obj_type(obj):
     obj_type = str(type(obj))
     return obj_type[8:-2]
 
 
 def serialize_single_var(obj):
     data = {"type": get_obj_type(obj), "value": obj}
     return data
 
 
 def serialize_collections(obj):
-    data = {"type": get_obj_type(obj), "value": list(map(serialize,obj))}
+    data = {"type": get_obj_type(obj), "value": list(map(serialize, obj))}
     return data
 
 
 def serialize_none_type():
     data = {"type": "NoneType", "value": "none"}
     return data
 
@@ -54,14 +60,20 @@
 
 
 def serialize_function(obj):
     data = {"type": "function", "value": get_function_values(obj)}
     return data
 
 
+def serialize_iter_objects(obj):
+    data = list(map(serialize, obj))
+    iter_data = {"type": "iterator", "value": data}
+    return iter_data
+
+
 def get_function_values(obj, cls=None):
     value = dict()
 
     value["__name__"] = obj.__name__
     value["__globals__"] = get_globals(obj, cls)
 
     value["__closure__"] = serialize(obj.__closure__)
@@ -83,29 +95,29 @@
 
             if isinstance(obj.__globals__[global_variable], types.ModuleType):
                 globs[" ".join(["module", global_variable])] = serialize(
                     obj.__globals__[global_variable].__name__)
 
             elif inspect.isclass(obj.__globals__[global_variable]):
 
-                if cls and obj.__globals__[global_variable] != cls or not cls:
+                if (cls and obj.__globals__[global_variable] != cls) or (not cls):
                     globs[global_variable] = serialize(obj.__globals__[global_variable])
 
             elif global_variable != obj.__code__.co_name:
                 globs[global_variable] = serialize(obj.__globals__[global_variable])
 
             else:
                 globs[global_variable] = serialize(obj.__name__)
 
     return globs
 
 
 def serialize_code(obj):
     value = {key: serialize(value) for key, value in inspect.getmembers(obj)
-                    if key in CODE_PROPERTIES}
+             if key in CODE_PROPERTIES}
     data = {"type": "code", "value": value}
     return data
 
 
 def serialize_cell(obj):
     data = {"type": "cell", "value": serialize(obj.cell_contents)}
     return data
@@ -182,16 +194,15 @@
     value["__members__"] = {key: serialize(value) for key, value in inspect.getmembers(obj)
                             if not (key.startswith("__") or inspect.isfunction(value) or inspect.ismethod(value))}
 
     return value
 
 
 def deserialize(obj):
-
-    if obj["type"] in BASE_TYPES:
+    if obj["type"] in PRIMITIVES:
         return deserialize_base_type(obj)
 
     elif obj["type"] in BASE_COLLECTIONS:
         return deserialize_base_collections(obj)
 
     elif obj["type"] == "code":
         return deserialize_code(obj["value"])
@@ -207,17 +218,20 @@
 
     elif obj["type"] in METHODS:
         return METHODS[obj["type"]](deserialize(obj["value"]))
 
     elif obj["type"] == "object":
         return deserialize_object(obj["value"])
 
+    elif obj["type"] == "iterator":
+        return deserialize_iter_objects(obj)
+
 
 def deserialize_base_type(obj):
-    return BASE_TYPES[obj["type"]](obj["value"])
+    return PRIMITIVES[obj["type"]](obj["value"])
 
 
 def deserialize_base_collections(obj):
     if obj["type"] == "list":
         return list(map(deserialize, obj["value"]))
     elif obj["type"] == "tuple":
         return tuple(map(deserialize, obj["value"]))
@@ -234,14 +248,19 @@
         return data
 
 
 def deserialize_code(code):
     return types.CodeType(*(deserialize(code[prop]) for prop in CODE_PROPERTIES))
 
 
+def deserialize_iter_objects(obj):
+    data = obj["value"]
+    return iter(deserialize(val) for val in data)
+
+
 def deserialize_function(func):
     code = func["__code__"]
     globs = func["__globals__"]
     func_closure = func["__closure__"]
 
     des_globals = deserialize_globals(globs, func)
 
@@ -295,7 +314,10 @@
 def deserialize_object(obj):
     cls = deserialize(obj["__class__"])
 
     des = object.__new__(cls)
     des.__dict__ = {key: deserialize(value) for key, value in obj["__members__"].items()}
 
     return des
+
+
+
```

### Comparing `ser_Stovba_lab3-0.1.0/ser_Stovba/xml_serializer.py` & `ser_Stovba_lab3-0.1.1/ser_Stovba/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `ser_Stovba_lab3-0.1.0/setup.py` & `ser_Stovba_lab3-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ser_Stovba_lab3",
-    version="0.1.0",
+    version="0.1.1",
     description="somme serialization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Stovba Vladislav",
     author_email="vlasstovbaboy@mail.ru",
     license="MIT",
     classifiers=[
```

