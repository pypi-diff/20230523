# Comparing `tmp/adaptive-cards-py-0.0.6.tar.gz` & `tmp/adaptive-cards-py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive-cards-py-0.0.6.tar", last modified: Tue May 16 18:53:12 2023, max compression
+gzip compressed data, was "adaptive-cards-py-0.0.7.tar", last modified: Tue May 23 17:16:55 2023, max compression
```

## Comparing `adaptive-cards-py-0.0.6.tar` & `adaptive-cards-py-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.629420 adaptive-cards-py-0.0.6/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.6/LICENSE
--rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.6/MANIFEST.in
--rw-r--r--   0 dennis    (1000) dennis    (1000)    23576 2023-05-16 18:53:12.629420 adaptive-cards-py-0.0.6/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)    21841 2023-05-16 18:48:35.000000 adaptive-cards-py-0.0.6/README.md
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/adaptive_cards/
--rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.6/adaptive_cards/__init__.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/actions.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5615 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/card.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     4592 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/card_types.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/containers.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/elements.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/inputs.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/utils.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/validation.py
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/
--rw-r--r--   0 dennis    (1000) dennis    (1000)    23576 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)      563 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/SOURCES.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/dependency_links.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       25 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/requires.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/top_level.txt
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/examples/
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/examples/simple_card/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.6/examples/simple_card/simple_card.jpg
--rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.6/examples/simple_card/simple_card_2.jpg
--rw-r--r--   0 dennis    (1000) dennis    (1000)      711 2023-05-16 18:53:00.000000 adaptive-cards-py-0.0.6/pyproject.toml
--rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-05-16 18:53:12.629420 adaptive-cards-py-0.0.6/setup.cfg
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-23 17:16:55.032894 adaptive-cards-py-0.0.7/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.7/LICENSE
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.7/MANIFEST.in
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    23735 2023-05-23 17:16:55.032894 adaptive-cards-py-0.0.7/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    22000 2023-05-23 17:15:21.000000 adaptive-cards-py-0.0.7/README.md
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-23 17:16:55.022894 adaptive-cards-py-0.0.7/adaptive_cards/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.7/adaptive_cards/__init__.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     6092 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/actions.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    10893 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/card.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    10696 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/card_types.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    14372 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/containers.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     9687 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/elements.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     9638 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/inputs.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      521 2023-05-20 14:12:19.000000 adaptive-cards-py-0.0.7/adaptive_cards/utils.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3803 2023-05-23 17:14:34.000000 adaptive-cards-py-0.0.7/adaptive_cards/validation.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-23 17:16:55.032894 adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    23735 2023-05-23 17:16:55.000000 adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      563 2023-05-23 17:16:55.000000 adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-05-23 17:16:55.000000 adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       25 2023-05-23 17:16:55.000000 adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/requires.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-05-23 17:16:55.000000 adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/top_level.txt
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-23 17:16:55.022894 adaptive-cards-py-0.0.7/examples/
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-23 17:16:55.032894 adaptive-cards-py-0.0.7/examples/simple_card/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.7/examples/simple_card/simple_card.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.7/examples/simple_card/simple_card_2.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      711 2023-05-23 17:15:51.000000 adaptive-cards-py-0.0.7/pyproject.toml
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-05-23 17:16:55.032894 adaptive-cards-py-0.0.7/setup.cfg
```

### Comparing `adaptive-cards-py-0.0.6/LICENSE` & `adaptive-cards-py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.6/PKG-INFO` & `adaptive-cards-py-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-cards-py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python wrapper library for building beautiful adaptive cards
 License: MIT License
         
         Copyright (c) 2023 Dennis Eder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -115,15 +115,15 @@
 card: AdaptiveCard = AdaptiveCard.new(version) \
                                  .add_item(text_block) \
                                  .create()
 ```
 
 Find your final layout below.
 
-![simple card](examples/simple_card/simple_card.jpg)
+![simple card](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/simple_card/simple_card.jpg?raw=true)
 
 💡 **Please note**
 <br>After building the object is done, the `create(...)` method must be called in order to create the final object. In this case, the object will be of type `AdaptiveCard`.
 
 To directly export your result, make use of the 
 `to_json()` method provided by every card.
 
@@ -164,35 +164,35 @@
 
 with open("path/to/out/file.json", "w+") as f:
     f.write(card.to_json())
 ```
 
 This will result in a card like shown below.
 
-![simple card](examples/simple_card/simple_card_2.jpg)
+![simple card 2](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/simple_card/simple_card_2.jpg?raw=true)
 
 ### Finally, a more complex card
 
-You can have a look on the following sample for getting an idea of what's actually possible
+You can have a look on the following example for getting an idea of what's actually possible
 with adaptive cards. 
 
-![wrap up card](examples/wrap_up_card/wrap_up_card.jpg)
+![wrap up card](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/wrap_up_card/wrap_up_card.jpg?raw=true)
 
 <details>
 <summary>Code</summary>
 
 ```python
 import adaptive_cards.card_types as types
 from adaptive_cards.actions import ActionToggleVisibility, TargetElement
 from adaptive_cards.validation import SchemaValidator, Result
 from adaptive_cards.card import AdaptiveCard
 from adaptive_cards.elements import TextBlock, Image
-from adaptive_cards.containers import Container, ContainerT, ColumnSet, Column
+from adaptive_cards.containers import Container, ContainerTypes, ColumnSet, Column
 
-containers: list[ContainerT] = []
+containers: list[ContainerTypes] = []
 
 icon_source: str = "https://icons8.com/icon/vNXFqyQtOSbb/launch"
 icon_url: str = "https://img.icons8.com/3d-fluency/94/launched-rocket.png"
 
 header_column_set: ColumnSet = ColumnSet(
     columns=[
         Column(
@@ -623,20 +623,20 @@
 
 print(f"Validation was successful: {result == Result.SUCCESS}")
 
 ```
 
 ## Examples
 
-If you are interested in more comprehensive examples or the actual source code, have a look into the `examples` folder (coming soon!) or visit the samples page of the official documentation. 
+If you are interested in more comprehensive examples or the actual source code, have a look into the `examples` folder. 
 
 ## Contribution
 
 Feel free to create issues, fork the repository or even come up with a pull request. I am happy about any kind of contribution and would love
 to hear your feedback! 
 
 ## Roadmap
 
-+ 🔎 More complete valdidation
-+ 🚀 Better examples
-+ 📕 Comprehensive documentation on code level
-+ 🐍 Ready to use Python package
+- [x] 📕 Comprehensive documentation on code level
+- [x] 🐍 Ready to use Python package
+- [ ] 🚀 More and better examples
+- [ ] 🔎 Comprehensive validation
```

### Comparing `adaptive-cards-py-0.0.6/README.md` & `adaptive-cards-py-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 card: AdaptiveCard = AdaptiveCard.new(version) \
                                  .add_item(text_block) \
                                  .create()
 ```
 
 Find your final layout below.
 
-![simple card](examples/simple_card/simple_card.jpg)
+![simple card](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/simple_card/simple_card.jpg?raw=true)
 
 💡 **Please note**
 <br>After building the object is done, the `create(...)` method must be called in order to create the final object. In this case, the object will be of type `AdaptiveCard`.
 
 To directly export your result, make use of the 
 `to_json()` method provided by every card.
 
@@ -129,35 +129,35 @@
 
 with open("path/to/out/file.json", "w+") as f:
     f.write(card.to_json())
 ```
 
 This will result in a card like shown below.
 
-![simple card](examples/simple_card/simple_card_2.jpg)
+![simple card 2](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/simple_card/simple_card_2.jpg?raw=true)
 
 ### Finally, a more complex card
 
-You can have a look on the following sample for getting an idea of what's actually possible
+You can have a look on the following example for getting an idea of what's actually possible
 with adaptive cards. 
 
-![wrap up card](examples/wrap_up_card/wrap_up_card.jpg)
+![wrap up card](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/wrap_up_card/wrap_up_card.jpg?raw=true)
 
 <details>
 <summary>Code</summary>
 
 ```python
 import adaptive_cards.card_types as types
 from adaptive_cards.actions import ActionToggleVisibility, TargetElement
 from adaptive_cards.validation import SchemaValidator, Result
 from adaptive_cards.card import AdaptiveCard
 from adaptive_cards.elements import TextBlock, Image
-from adaptive_cards.containers import Container, ContainerT, ColumnSet, Column
+from adaptive_cards.containers import Container, ContainerTypes, ColumnSet, Column
 
-containers: list[ContainerT] = []
+containers: list[ContainerTypes] = []
 
 icon_source: str = "https://icons8.com/icon/vNXFqyQtOSbb/launch"
 icon_url: str = "https://img.icons8.com/3d-fluency/94/launched-rocket.png"
 
 header_column_set: ColumnSet = ColumnSet(
     columns=[
         Column(
@@ -588,20 +588,20 @@
 
 print(f"Validation was successful: {result == Result.SUCCESS}")
 
 ```
 
 ## Examples
 
-If you are interested in more comprehensive examples or the actual source code, have a look into the `examples` folder (coming soon!) or visit the samples page of the official documentation. 
+If you are interested in more comprehensive examples or the actual source code, have a look into the `examples` folder. 
 
 ## Contribution
 
 Feel free to create issues, fork the repository or even come up with a pull request. I am happy about any kind of contribution and would love
 to hear your feedback! 
 
 ## Roadmap
 
-+ 🔎 More complete valdidation
-+ 🚀 Better examples
-+ 📕 Comprehensive documentation on code level
-+ 🐍 Ready to use Python package
+- [x] 📕 Comprehensive documentation on code level
+- [x] 🐍 Ready to use Python package
+- [ ] 🚀 More and better examples
+- [ ] 🔎 Comprehensive validation
```

### Comparing `adaptive-cards-py-0.0.6/adaptive_cards/validation.py` & `adaptive-cards-py-0.0.7/adaptive_cards/validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,134 @@
-from adaptive_cards.card import AdaptiveCard
-from dataclasses import dataclass, fields
+"""Validation class for evaluating a cards schema"""
+
 import dataclasses
-from adaptive_cards.elements import ElementT
-from adaptive_cards.containers import ContainerT
-from adaptive_cards.inputs import InputT
-from typing import Any
+from dataclasses import dataclass, fields
 from enum import Flag
+from typing import Any
+from adaptive_cards.card import AdaptiveCard
 
 MINIMUM_VERSION_KEY: str = "min_version"
 
+
 class Result(Flag):
+    """
+    Represents a result value as a combination of flags.
+
+    Arguments:
+    SUCCESS = 0: Represents a successful result.
+    EMPTY_CARD = 1: Represents an empty card result.
+    INVALID_FIELD_VERSION = 2: Represents an invalid field version result.
+    UNDEFINED = 3: Represents an undefined result.
+    """
+
     SUCCESS = 0
     EMPTY_CARD = 1
     INVALID_FIELD_VERSION = 2
     UNEDFINED = 3
 
+
 @dataclass
 class InvalidField:
+    """
+    Represents an invalid field within a parent type.
+
+    Attributes:
+        parent_type: The type of the parent object.
+        field_name: The name of the invalid field.
+        version: The version of the field.
+    """
     parent_type: str
     field_name: str
     version: str
 
+
+@dataclass
 class SchemaValidator:
+    """
+    Validator class for checking a cards schema w.r.t. to version numbers of individual fields.
+    """
     def __init__(self) -> None:
-        ...
-        
+        self.__card: AdaptiveCard
+        self.__item: Any
+        self.__invalid_fields: list[InvalidField]
+
     def validate(self, card: AdaptiveCard) -> Result:
+        """
+        Run validation on card.
+
+        Args:
+            card (AdaptiveCard): Card to be validated
+
+        Returns:
+            Result: Validation result
+        """
         self.__card = card
         self.__reset()
         result: Result = self.__validate_body()
         self.__debug()
-        
+
         return result
 
     def __reset(self) -> None:
-        self.__is_valid = True
-        self.__invalid_fields: list[InvalidField] = list()
-        
+        self.__invalid_fields: list[InvalidField] = []
+
     def __validate_body(self) -> Result:
         if self.__card.body is None:
             return Result.EMPTY_CARD
-    
+
         self.__validate_elements(self.__card.body)
-        
+
         if len(self.__invalid_fields) > 0:
             return Result.INVALID_FIELD_VERSION
-        
+
         return Result.SUCCESS
-        
 
     def __validate_elements(self, items: Any):
         if not isinstance(items, list):
             items = [items]
-        
+
         custom_types: list[Any] = []
         iterables: list[Any] = []
-        
+
         for item in items:
             self.__item = item
             for field in fields(item):
                 value: Any = getattr(item, field.name)
-                
+
                 if value is None:
                     continue
-                
+
                 if isinstance(value, list):
                     iterables.append(value)
                     # self.__validate_elements(value)
-                    
+
                 elif dataclasses.is_dataclass(value):
                     custom_types.append(value)
                     # self.__validate_elements(value)
-                    
+
                 else:
                     self.__validate_field_version(
-                        field.name, 
-                        field.metadata.get(MINIMUM_VERSION_KEY)
-                    ) 
+                        field.name, field.metadata.get(MINIMUM_VERSION_KEY)
+                    )
 
-        
         for iterable in iterables:
             self.__validate_elements(iterable)
 
         for custom_type in custom_types:
             self.__validate_elements(custom_type)
 
-            
     def __validate_field_version(self, field_name: str, minimum_version: Any) -> None:
-        assert(minimum_version is not None)
-            
+        assert minimum_version is not None
+
         if float(self.__card.version) < float(minimum_version):
             self.__invalid_fields.append(
                 InvalidField(type(self.__item).__name__, field_name, minimum_version)
             )
-    
+
     def __debug(self):
         for invalid_field in self.__invalid_fields:
-            print(f"Wrong version for field <{invalid_field.field_name}> " \
-                f"in type <{invalid_field.parent_type}> | " \
-                f"selected card version {self.__card.version} < minimum field version {invalid_field.version}")
-                
+            print(
+                f"Wrong version for field <{invalid_field.field_name}> "
+                f"in type <{invalid_field.parent_type}> | "
+                f"selected card version {self.__card.version} < minimum field version "
+                f"{invalid_field.version}"
+            )
```

### Comparing `adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/PKG-INFO` & `adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-cards-py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python wrapper library for building beautiful adaptive cards
 License: MIT License
         
         Copyright (c) 2023 Dennis Eder
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -115,15 +115,15 @@
 card: AdaptiveCard = AdaptiveCard.new(version) \
                                  .add_item(text_block) \
                                  .create()
 ```
 
 Find your final layout below.
 
-![simple card](examples/simple_card/simple_card.jpg)
+![simple card](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/simple_card/simple_card.jpg?raw=true)
 
 💡 **Please note**
 <br>After building the object is done, the `create(...)` method must be called in order to create the final object. In this case, the object will be of type `AdaptiveCard`.
 
 To directly export your result, make use of the 
 `to_json()` method provided by every card.
 
@@ -164,35 +164,35 @@
 
 with open("path/to/out/file.json", "w+") as f:
     f.write(card.to_json())
 ```
 
 This will result in a card like shown below.
 
-![simple card](examples/simple_card/simple_card_2.jpg)
+![simple card 2](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/simple_card/simple_card_2.jpg?raw=true)
 
 ### Finally, a more complex card
 
-You can have a look on the following sample for getting an idea of what's actually possible
+You can have a look on the following example for getting an idea of what's actually possible
 with adaptive cards. 
 
-![wrap up card](examples/wrap_up_card/wrap_up_card.jpg)
+![wrap up card](https://github.com/dennis6p/adaptive-cards-py/blob/main/examples/wrap_up_card/wrap_up_card.jpg?raw=true)
 
 <details>
 <summary>Code</summary>
 
 ```python
 import adaptive_cards.card_types as types
 from adaptive_cards.actions import ActionToggleVisibility, TargetElement
 from adaptive_cards.validation import SchemaValidator, Result
 from adaptive_cards.card import AdaptiveCard
 from adaptive_cards.elements import TextBlock, Image
-from adaptive_cards.containers import Container, ContainerT, ColumnSet, Column
+from adaptive_cards.containers import Container, ContainerTypes, ColumnSet, Column
 
-containers: list[ContainerT] = []
+containers: list[ContainerTypes] = []
 
 icon_source: str = "https://icons8.com/icon/vNXFqyQtOSbb/launch"
 icon_url: str = "https://img.icons8.com/3d-fluency/94/launched-rocket.png"
 
 header_column_set: ColumnSet = ColumnSet(
     columns=[
         Column(
@@ -623,20 +623,20 @@
 
 print(f"Validation was successful: {result == Result.SUCCESS}")
 
 ```
 
 ## Examples
 
-If you are interested in more comprehensive examples or the actual source code, have a look into the `examples` folder (coming soon!) or visit the samples page of the official documentation. 
+If you are interested in more comprehensive examples or the actual source code, have a look into the `examples` folder. 
 
 ## Contribution
 
 Feel free to create issues, fork the repository or even come up with a pull request. I am happy about any kind of contribution and would love
 to hear your feedback! 
 
 ## Roadmap
 
-+ 🔎 More complete valdidation
-+ 🚀 Better examples
-+ 📕 Comprehensive documentation on code level
-+ 🐍 Ready to use Python package
+- [x] 📕 Comprehensive documentation on code level
+- [x] 🐍 Ready to use Python package
+- [ ] 🚀 More and better examples
+- [ ] 🔎 Comprehensive validation
```

### Comparing `adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/SOURCES.txt` & `adaptive-cards-py-0.0.7/adaptive_cards_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.6/examples/simple_card/simple_card.jpg` & `adaptive-cards-py-0.0.7/examples/simple_card/simple_card.jpg`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.6/examples/simple_card/simple_card_2.jpg` & `adaptive-cards-py-0.0.7/examples/simple_card/simple_card_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.6/pyproject.toml` & `adaptive-cards-py-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaptive-cards-py"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python wrapper library for building beautiful adaptive cards"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 readme = "README.md"
```

