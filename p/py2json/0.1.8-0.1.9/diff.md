# Comparing `tmp/py2json-0.1.8.tar.gz` & `tmp/py2json-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2json-0.1.8.tar", last modified: Wed Jan 25 23:48:20 2023, max compression
+gzip compressed data, was "py2json-0.1.9.tar", last modified: Thu Jan 26 01:16:55 2023, max compression
```

## Comparing `py2json-0.1.8.tar` & `py2json-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 23:48:20.287875 py2json-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-25 23:47:37.000000 py2json-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-25 23:48:20.287875 py2json-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-01-25 23:47:37.000000 py2json-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 23:48:20.287875 py2json-0.1.8/py2json/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/ctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/fakit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 23:48:20.287875 py2json-0.1.8/py2json/inspire/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/inspire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/inspire/attribute_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/inspire/example_fakit_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/inspire/func_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/inspire/serializing_sklearn_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/obj2dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-25 23:47:37.000000 py2json-0.1.8/py2json/w_glom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 23:48:20.287875 py2json-0.1.8/py2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-25 23:48:20.000000 py2json-0.1.8/py2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-25 23:48:20.000000 py2json-0.1.8/py2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 23:48:20.000000 py2json-0.1.8/py2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 23:48:20.000000 py2json-0.1.8/py2json.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-25 23:48:20.000000 py2json-0.1.8/py2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-25 23:48:20.000000 py2json-0.1.8/py2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-25 23:48:20.287875 py2json-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-25 23:47:37.000000 py2json-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:16:55.316588 py2json-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-26 01:16:18.000000 py2json-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-26 01:16:55.316588 py2json-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-01-26 01:16:18.000000 py2json-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:16:55.316588 py2json-0.1.9/py2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/ctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/fakit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:16:55.316588 py2json-0.1.9/py2json/inspire/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/inspire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/inspire/attribute_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/inspire/example_fakit_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/inspire/func_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/inspire/serializing_sklearn_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/obj2dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-26 01:16:18.000000 py2json-0.1.9/py2json/w_glom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 01:16:55.316588 py2json-0.1.9/py2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-01-26 01:16:55.000000 py2json-0.1.9/py2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-26 01:16:55.000000 py2json-0.1.9/py2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 01:16:55.000000 py2json-0.1.9/py2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 01:16:55.000000 py2json-0.1.9/py2json.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-26 01:16:55.000000 py2json-0.1.9/py2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-26 01:16:55.000000 py2json-0.1.9/py2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-26 01:16:55.316588 py2json-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-26 01:16:18.000000 py2json-0.1.9/setup.py
```

### Comparing `py2json-0.1.8/LICENSE` & `py2json-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/PKG-INFO` & `py2json-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2json
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for json serialization of python objects
 Home-page: UNKNOWN
 License: mit
 Description: Tools for json serialization of python objects
         
         # py2json
```

### Comparing `py2json-0.1.8/README.md` & `py2json-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/ctor.py` & `py2json-0.1.9/py2json/ctor.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,15 +275,15 @@
                     raise CtorException(
                         f'deconstruction spec not found for non-basic type at path={path}, key={key}'
                     )
             return key, value
 
         def enter(path, key, value):
             if not cls.is_python_to_json_basic_type(value) and key != Ctor.CONSTRUCTOR:
-                return path, False
+                return None, False
             else:
                 return default_enter(path, key, value)
 
         ctor_dict = remap(obj, visit, enter=enter)
         if output_type == Ctor.CTOR_DICT:
             return ctor_dict
         elif output_type == Ctor.JSON_DICT:
@@ -371,44 +371,53 @@
         Calls the Ctor.CONSTRUCTOR with given Ctor.ARGS and Ctor.KWARGS.
         Checks if ARGS or KWARGS are ctor_dicts and constructs those first
 
         :param ctor_dict: {Ctor.CONSTRUCTOR: Callable, Ctor.ARGS: List[Any], Ctor.KWARGS: Dict[str, Any]}
         :return: ctor_dict[Ctor.CONSTRUCTOR](*ctor_dict[Ctor.ARGS], **ctor_dict[Ctor.KWARGS])
         """
         if cls.is_ctor_dict(ctor_dict):
-            args = [
-                cls._construct_obj(_a) if cls.is_ctor_dict(_a) else _a
-                for _a in cls._get_value(ctor_dict, cls.ARGS, [])
-            ]
-            kwargs = {
-                _k: cls._construct_obj(_v) if cls.is_ctor_dict(_v) else _v
-                for _k, _v in cls._get_value(ctor_dict, cls.KWARGS, {}).items()
-            }
+            if args := cls._get_value(ctor_dict, cls.ARGS, []):
+                args = cls.construct(args)
+            if kwargs := cls._get_value(ctor_dict, cls.KWARGS, {}):
+                kwargs = cls.construct(kwargs)
+
             return ctor_dict[cls.CONSTRUCTOR](*args, **kwargs)
         else:
             raise CtorException(
                 f"ctor_dict must have a '{cls.CONSTRUCTOR}' key and optionally '{cls.ARGS}' and '{cls.KWARGS}' but got '{ctor_dict}'"
             )
 
     @classmethod
     def _deconstruct_obj(cls, obj, validate_conversion: bool = False):
         """
-        Breakdown an obj into a ctor_dict as described by deconstruction_specs
+        Breakdown an obj into a ctor_dict as described by deconstruction_specs.
+        Further breakdowns on deconstructed ARGS and KWARGS if necessary.
+
         :param obj: any object satisfying one of the deconstruction_specs
         :param validate_conversion: [boolean] True to compare obj to reconstructed ctor_dict. False to skip validation
         :return: ctor_dict: {Ctor.CONSTRUCTOR: Callable, Ctor.ARGS: List[Any], Ctor.KWARGS: Dict[str, Any]}
         """
         try:
             s = next(s for s in cls.deconstruction_specs if s['check_type'](obj))
             try:
                 serializer = s['serializer']
             except KeyError:
                 s['serializer'] = mk_serializer_and_deserializer(s['spec'])
                 serializer = s['serializer']
             ctor_dict = serializer(obj)
+
+            if ctor_dict[Ctor.ARGS] is not None:
+                ctor_dict[Ctor.ARGS] = cls.deconstruct(
+                    ctor_dict[Ctor.ARGS], validate_conversion=validate_conversion
+                )
+            if ctor_dict[Ctor.KWARGS] is not None:
+                ctor_dict[Ctor.KWARGS] = cls.deconstruct(
+                    ctor_dict[Ctor.KWARGS], validate_conversion=validate_conversion
+                )
+
             if validate_conversion is True:
                 try:
                     validator = s['validate_conversion']
                 except KeyError:
                     s['validate_conversion'] = cls._default_conversion_validation
                     validator = s['validate_conversion']
                 if validator(obj, ctor_dict) is False:
```

### Comparing `py2json-0.1.8/py2json/encoders.py` & `py2json-0.1.9/py2json/encoders.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/fakit.py` & `py2json-0.1.9/py2json/fakit.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/inspire/attribute_tree.py` & `py2json-0.1.9/py2json/inspire/attribute_tree.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/inspire/example_fakit_use.py` & `py2json-0.1.9/py2json/inspire/example_fakit_use.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/inspire/func_serialization.py` & `py2json-0.1.9/py2json/inspire/func_serialization.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/inspire/serializing_sklearn_estimators.py` & `py2json-0.1.9/py2json/inspire/serializing_sklearn_estimators.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/obj2dict.py` & `py2json-0.1.9/py2json/obj2dict.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/util.py` & `py2json-0.1.9/py2json/util.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json/w_glom.py` & `py2json-0.1.9/py2json/w_glom.py`

 * *Files identical despite different names*

### Comparing `py2json-0.1.8/py2json.egg-info/PKG-INFO` & `py2json-0.1.9/py2json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2json
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for json serialization of python objects
 Home-page: UNKNOWN
 License: mit
 Description: Tools for json serialization of python objects
         
         # py2json
```

### Comparing `py2json-0.1.8/py2json.egg-info/SOURCES.txt` & `py2json-0.1.9/py2json.egg-info/SOURCES.txt`

 * *Files identical despite different names*

