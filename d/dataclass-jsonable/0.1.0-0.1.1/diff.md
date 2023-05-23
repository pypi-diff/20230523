# Comparing `tmp/dataclass-jsonable-0.1.0.tar.gz` & `tmp/dataclass-jsonable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass-jsonable-0.1.0.tar", last modified: Mon Apr 24 08:26:35 2023, max compression
+gzip compressed data, was "dataclass-jsonable-0.1.1.tar", last modified: Tue May 23 02:42:10 2023, max compression
```

## Comparing `dataclass-jsonable-0.1.0.tar` & `dataclass-jsonable-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-04-24 08:26:35.959457 dataclass-jsonable-0.1.0/
--rw-r--r--   0 hit9       (501) staff       (20)     1539 2022-08-11 15:42:12.000000 dataclass-jsonable-0.1.0/LICENSE-BSD3
--rw-r--r--   0 hit9       (501) staff       (20)      600 2022-08-11 14:27:41.000000 dataclass-jsonable-0.1.0/MANIFEST.in
--rw-r--r--   0 hit9       (501) staff       (20)    10892 2023-04-24 08:26:35.956617 dataclass-jsonable-0.1.0/PKG-INFO
--rw-r--r--   0 hit9       (501) staff       (20)    10505 2023-04-24 08:16:51.000000 dataclass-jsonable-0.1.0/README.md
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-04-24 08:26:35.954930 dataclass-jsonable-0.1.0/dataclass_jsonable/
--rw-r--r--   0 hit9       (501) staff       (20)    22312 2023-04-24 08:16:51.000000 dataclass-jsonable-0.1.0/dataclass_jsonable/__init__.py
--rw-r--r--   0 hit9       (501) staff       (20)        0 2022-08-09 02:53:50.000000 dataclass-jsonable-0.1.0/dataclass_jsonable/py.typed
-drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-04-24 08:26:35.955177 dataclass-jsonable-0.1.0/dataclass_jsonable.egg-info/
--rw-r--r--   0 hit9       (501) staff       (20)      102 2023-04-24 08:26:35.000000 dataclass-jsonable-0.1.0/dataclass_jsonable.egg-info/SOURCES.txt
--rw-r--r--   0 hit9       (501) staff       (20)       38 2023-04-24 08:26:35.960235 dataclass-jsonable-0.1.0/setup.cfg
--rw-r--r--   0 hit9       (501) staff       (20)      590 2023-04-24 08:16:51.000000 dataclass-jsonable-0.1.0/setup.py
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-23 02:42:10.920745 dataclass-jsonable-0.1.1/
+-rw-r--r--   0 hit9       (501) staff       (20)     1539 2022-08-11 15:42:12.000000 dataclass-jsonable-0.1.1/LICENSE-BSD3
+-rw-r--r--   0 hit9       (501) staff       (20)      600 2022-08-11 14:27:41.000000 dataclass-jsonable-0.1.1/MANIFEST.in
+-rw-r--r--   0 hit9       (501) staff       (20)    11480 2023-05-23 02:42:10.920016 dataclass-jsonable-0.1.1/PKG-INFO
+-rw-r--r--   0 hit9       (501) staff       (20)    11093 2023-05-23 02:41:04.000000 dataclass-jsonable-0.1.1/README.md
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-23 02:42:10.919230 dataclass-jsonable-0.1.1/dataclass_jsonable/
+-rw-r--r--   0 hit9       (501) staff       (20)    22609 2023-05-23 02:41:04.000000 dataclass-jsonable-0.1.1/dataclass_jsonable/__init__.py
+-rw-r--r--   0 hit9       (501) staff       (20)        0 2022-08-09 02:53:50.000000 dataclass-jsonable-0.1.1/dataclass_jsonable/py.typed
+drwxr-xr-x   0 hit9       (501) staff       (20)        0 2023-05-23 02:42:10.919560 dataclass-jsonable-0.1.1/dataclass_jsonable.egg-info/
+-rw-r--r--   0 hit9       (501) staff       (20)      102 2023-05-23 02:42:10.000000 dataclass-jsonable-0.1.1/dataclass_jsonable.egg-info/SOURCES.txt
+-rw-r--r--   0 hit9       (501) staff       (20)       38 2023-05-23 02:42:10.921408 dataclass-jsonable-0.1.1/setup.cfg
+-rw-r--r--   0 hit9       (501) staff       (20)      590 2023-05-23 02:41:38.000000 dataclass-jsonable-0.1.1/setup.py
```

### Comparing `dataclass-jsonable-0.1.0/LICENSE-BSD3` & `dataclass-jsonable-0.1.1/LICENSE-BSD3`

 * *Files identical despite different names*

### Comparing `dataclass-jsonable-0.1.0/MANIFEST.in` & `dataclass-jsonable-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dataclass-jsonable-0.1.0/PKG-INFO` & `dataclass-jsonable-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-jsonable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple and flexible conversions between dataclasses and jsonable dictionaries.
 Home-page: https://github.com/hit9/dataclass-jsonable
 Author: hit9
 Author-email: hit9@icloud.com
 License: BSD
 Keywords: dataclasses,json,jsonable
 Requires-Python: >=3.7
@@ -12,14 +12,16 @@
 License-File: LICENSE-BSD3
 
 # dataclass-jsonable
 
 [![dataclass-jsonable ci](https://github.com/hit9/dataclass-jsonable/actions/workflows/ci.yml/badge.svg)](https://github.com/hit9/dataclass-jsonable/actions/workflows/ci.yml)
 ![](https://img.shields.io/badge/license-BSD3-brightgreen)
 
+[中文说明](README.zh.md)
+
 Simple and flexible conversions between dataclasses and jsonable dictionaries.
 
 It maps dataclasses to jsonable dictionaries but not json strings.
 
 
 ## Features
 
@@ -317,15 +319,15 @@
 
   Obj.from_json({})  # => Obj(updated_at=datetime.datetime(1970, 1, 1, 8, 0))
   ```
 
   dataclass-jsonable also introduces a class-level similar option `__default_factory__`.
   If a field has no `default` or `default_factory` declared, and has no `default_before_decoding` option used,
   this function will generate a default value according to its type, to prevent a
-  "missing positional arguments" TypeError from rasing.
+  "missing positional arguments" TypeError from raising.
 
   ```python
   from dataclass_jsonable import J, zero
 
   @dataclass
   class Obj(J):
       __default_factory__ = zero
@@ -372,14 +374,33 @@
               )
           },
       )
 
   Record().json()  # => {'created_at': '2022-08-09T23:23:02.543007'}
   ```
 
+  dataclass-jsonable gives `encoder` and `decoder` better alias names since 0.1.1:
+  `to_json` and `from_json`.
+
+  ```python
+  @dataclass
+  class Obj(J):
+      elems: List[str] = field(
+          metadata={
+              "j": json_options(
+                  to_json=lambda x: ",".join(x),  # Alias for encoder
+                  from_json=lambda x: x.split(","),  # Alias for decoder
+              )
+          }
+      )
+
+  Obj(elems=["a", "b", "c"]).json()  # => {'elems': 'a,b,c'}
+  Obj.from_json({"elems": "a,b,c"})  # => Obj(elems=['a', 'b', 'c'])
+  ```
+
 * For some very narrow scenarios, we may need to execute a hook function before decoding,
   for example, the data to be decoded is a serialized json string,
   and but we still want to use the built-in decoder functions instead of making a new decoder.
 
   ```python
   import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataclass-jsonable-0.1.0/README.md` & `dataclass-jsonable-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # dataclass-jsonable
 
 [![dataclass-jsonable ci](https://github.com/hit9/dataclass-jsonable/actions/workflows/ci.yml/badge.svg)](https://github.com/hit9/dataclass-jsonable/actions/workflows/ci.yml)
 ![](https://img.shields.io/badge/license-BSD3-brightgreen)
 
+[中文说明](README.zh.md)
+
 Simple and flexible conversions between dataclasses and jsonable dictionaries.
 
 It maps dataclasses to jsonable dictionaries but not json strings.
 
 
 ## Features
 
@@ -304,15 +306,15 @@
 
   Obj.from_json({})  # => Obj(updated_at=datetime.datetime(1970, 1, 1, 8, 0))
   ```
 
   dataclass-jsonable also introduces a class-level similar option `__default_factory__`.
   If a field has no `default` or `default_factory` declared, and has no `default_before_decoding` option used,
   this function will generate a default value according to its type, to prevent a
-  "missing positional arguments" TypeError from rasing.
+  "missing positional arguments" TypeError from raising.
 
   ```python
   from dataclass_jsonable import J, zero
 
   @dataclass
   class Obj(J):
       __default_factory__ = zero
@@ -359,14 +361,33 @@
               )
           },
       )
 
   Record().json()  # => {'created_at': '2022-08-09T23:23:02.543007'}
   ```
 
+  dataclass-jsonable gives `encoder` and `decoder` better alias names since 0.1.1:
+  `to_json` and `from_json`.
+
+  ```python
+  @dataclass
+  class Obj(J):
+      elems: List[str] = field(
+          metadata={
+              "j": json_options(
+                  to_json=lambda x: ",".join(x),  # Alias for encoder
+                  from_json=lambda x: x.split(","),  # Alias for decoder
+              )
+          }
+      )
+
+  Obj(elems=["a", "b", "c"]).json()  # => {'elems': 'a,b,c'}
+  Obj.from_json({"elems": "a,b,c"})  # => Obj(elems=['a', 'b', 'c'])
+  ```
+
 * For some very narrow scenarios, we may need to execute a hook function before decoding,
   for example, the data to be decoded is a serialized json string,
   and but we still want to use the built-in decoder functions instead of making a new decoder.
 
   ```python
   import json
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dataclass-jsonable-0.1.0/dataclass_jsonable/__init__.py` & `dataclass-jsonable-0.1.1/dataclass_jsonable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 
 class Action(enum.IntEnum):
     ENCODING = 1
     DECODING = 2
 
 
-@dataclass(frozen=True)
+@dataclass
 class json_options:
     """Field-level options to override the default conversion behavior.
     For each option, leaving `None` means not-set.
     """
 
     # Custom key to be mapping in the dictionary.
     # Uses the name of this field by default.
@@ -107,25 +107,38 @@
     default_before_decoding: Optional[V] = None
     # Backward compatiable, the same of default_before_decoding.
     default_on_missing: Optional[V] = None
 
     # Custom encoder function, to be called like: encoder(field_value).
     # Uses `get_encoder` to get the default encoder function by annotated type.
     encoder: Optional[F] = None
+    # Alias name for `encoder` option.
+    to_json: Optional[F] = None
 
-    # Custom encoder function, to be called like: decoder(dict_value).
+    # Custom decoder function, to be called like: decoder(dict_value).
     # Uses `get_decoder` to get the default decoder function by annotated type.
     decoder: Optional[F] = None
+    # Alias name for `decoder` option.
+    from_json: Optional[F] = None
 
     # Hook function to be executed before decoder's execution.
     # The decoding looks like `before_decoder(decoder(dict_value))` if this option is set.
     # Although this feature can be achieved by a new `decoder` function, but it's more
     # convenient to work with the builtin decoder functions.
     before_decoder: Optional[F] = None
 
+    def __post_init__(self):
+        # Handle alias options
+        if self.encoder is None:
+            self.encoder = self.to_json
+        if self.decoder is None:
+            self.decoder = self.from_json
+        if self.default_before_decoding is None:
+            self.default_before_decoding = self.default_on_missing
+
 
 _BASIC_TYPES = {  # Ensures callable
     int,
     float,
     str,
     bool,
     list,
@@ -472,19 +485,15 @@
                     k = _k
                     # record the key in dictionary `d` for this field.
                     _name_choice_map[name] = k
                     break
 
             if k is None:
                 # Key is missing in dictionary.
-                default = (
-                    options.default_before_decoding
-                    if options.default_before_decoding is not None
-                    else options.default_on_missing
-                )
+                default = options.default_before_decoding
                 if default is not None:
                     # Gives a default value before decoding.
                     v = default
                 else:
                     # Just continue going if the value is missing.
                     # An error like "missing 1 required positional argument" will be raised if this field doesn't
                     # have a default value declared.
```

### Comparing `dataclass-jsonable-0.1.0/setup.py` & `dataclass-jsonable-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup  # type: ignore
 
 setup(
     name="dataclass-jsonable",
-    version="0.1.0",
+    version="0.1.1",
     author="hit9",
     author_email="hit9@icloud.com",
     description="Simple and flexible conversions between dataclasses and jsonable dictionaries.",
     license="BSD",
     keywords="dataclasses,json,jsonable",
     url="https://github.com/hit9/dataclass-jsonable",
     packages=["dataclass_jsonable"],
```

