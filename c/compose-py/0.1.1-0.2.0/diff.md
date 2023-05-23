# Comparing `tmp/compose-py-0.1.1.tar.gz` & `tmp/compose-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-py-0.1.1.tar", last modified: Mon May 22 04:21:30 2023, max compression
+gzip compressed data, was "compose-py-0.2.0.tar", last modified: Tue May 23 15:49:17 2023, max compression
```

## Comparing `compose-py-0.1.1.tar` & `compose-py-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1070 2023-05-22 02:20:34.000000 compose-py-0.1.1/LICENSE
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3605 2023-05-22 04:21:30.623184 compose-py-0.1.1/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1760 2023-05-22 02:23:26.000000 compose-py-0.1.1/README.md
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      140 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       79 2023-05-22 03:42:37.000000 compose-py-0.1.1/compose_py/_types.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       22 2023-05-22 04:21:23.000000 compose-py-0.1.1/compose_py/_version.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      970 2023-05-22 02:37:15.000000 compose-py-0.1.1/compose_py/_yaml.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2671 2023-05-22 02:36:51.000000 compose-py-0.1.1/compose_py/dumper.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1869 2023-05-22 02:36:53.000000 compose-py-0.1.1/compose_py/loader.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       99 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/model_type.py
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py/models_dataclasses/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1054 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/models_dataclasses/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    12265 2023-05-22 04:17:18.000000 compose-py-0.1.1/compose_py/models_dataclasses/_generated.py
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py/models_pydantic/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      972 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/models_pydantic/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    15492 2023-05-22 04:17:18.000000 compose-py-0.1.1/compose_py/models_pydantic/_generated.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/py.typed
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py.egg-info/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3605 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      541 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        1 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      205 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       11 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1174 2023-05-22 04:19:03.000000 compose-py-0.1.1/pyproject.toml
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       38 2023-05-22 04:21:30.623184 compose-py-0.1.1/setup.cfg
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1070 2023-05-21 01:42:57.000000 compose-py-0.2.0/LICENSE
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3791 2023-05-23 15:49:17.957051 compose-py-0.2.0/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1946 2023-05-23 15:47:09.000000 compose-py-0.2.0/README.md
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      170 2023-05-23 15:47:09.000000 compose-py-0.2.0/compose_py/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       79 2023-05-23 15:13:52.000000 compose-py-0.2.0/compose_py/_types.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       22 2023-05-23 15:49:03.000000 compose-py-0.2.0/compose_py/_version.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      733 2023-05-23 15:46:51.000000 compose-py-0.2.0/compose_py/_yaml.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3713 2023-05-23 15:47:09.000000 compose-py-0.2.0/compose_py/dumper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2704 2023-05-23 15:47:09.000000 compose-py-0.2.0/compose_py/loader.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       99 2023-05-21 04:25:58.000000 compose-py-0.2.0/compose_py/model_type.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py/models_dataclasses/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1054 2023-05-21 08:33:20.000000 compose-py-0.2.0/compose_py/models_dataclasses/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    12265 2023-05-23 15:13:52.000000 compose-py-0.2.0/compose_py/models_dataclasses/_generated.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py/models_pydantic/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      972 2023-05-21 08:33:31.000000 compose-py-0.2.0/compose_py/models_pydantic/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    15492 2023-05-23 15:13:52.000000 compose-py-0.2.0/compose_py/models_pydantic/_generated.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-05-21 01:43:11.000000 compose-py-0.2.0/compose_py/py.typed
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3791 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      541 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      205 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       11 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1174 2023-05-23 15:13:52.000000 compose-py-0.2.0/pyproject.toml
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-05-23 15:49:17.957051 compose-py-0.2.0/setup.cfg
```

### Comparing `compose-py-0.1.1/LICENSE` & `compose-py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.1/PKG-INFO` & `compose-py-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-py
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library for parsing and loading Compose files
 Author-email: Yuki Igarashi <me@bonprosoft.com>
 License: MIT License
         
         Copyright (c) 2023 Yuki Igarashi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,40 +61,46 @@
 ## Tutorial: Load, modify, and save docker-compose.yml
 
 ### Pydantic.BaseModel (default)
 
 ```py
 import compose_py
 
-obj = compose_py.load_yaml("docker-compose.yml")
+with open("docker-compose.yml", "r") as f:
+    obj = compose_py.load_yaml(f)
 print(obj)  # Prints 'compose_py.models_pydantic.ComposeSpecification(...)'
 print(obj.services["web"])  # Prints 'compose_py.models_pydantic.Service(...)'
 
 # Copy and modify the existing service, then add it to the specification
 web2 = obj.services["web"].copy()
-web2.command = '--port 8081'
+web2.command = "--port 8081"
 obj.services["web2"] = web2
 
-compose_py.dump_yaml(obj, "docker-compose-modified.yml")
+print(compose_py.dump_yaml_str(obj))
+with open("docker-compose-modified.yml", "w") as f:
+    compose_py.dump_yaml(obj, f)
 ```
 
 You can find more APIs under `compose_py.models_pydantic` package.
 
 ### dataclasses.dataclass
 
 ```py
 import compose_py
 
-obj = compose_py.load_yaml("docker-compose.yml", model=compose_py.ModelType.DATACLASSES)
+with open("docker-compose.yml", "r") as f:
+    obj = compose_py.load_yaml(f, model=compose_py.ModelType.DATACLASSES)
 print(obj)  # Prints 'compose_py.models_dataclasses.ComposeSpecification(...)'
 print(obj.services["web"])  # Prints 'compose_py.models_dataclasses.Service(...)'
 
 # Copy and modify the existing service, then add it to the specification
 web2 = obj.services["web"].copy()
-web2.command = '--port 8081'
+web2.command = "--port 8081"
 obj.services["web2"] = web2
 
-compose_py.dump_yaml(obj, "docker-compose-modified.yml", model=compose_py.ModelType.DATACLASSES)
+print(compose_py.dump_yaml_str(obj))
+with open("docker-compose-modified.yml", "w") as f:
+    compose_py.dump_yaml(obj, f, model=compose_py.ModelType.DATACLASSES)
 ```
 
 You can find more APIs under `compose_py.models_dataclasses` package.
```

### Comparing `compose-py-0.1.1/README.md` & `compose-py-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -22,40 +22,46 @@
 ## Tutorial: Load, modify, and save docker-compose.yml
 
 ### Pydantic.BaseModel (default)
 
 ```py
 import compose_py
 
-obj = compose_py.load_yaml("docker-compose.yml")
+with open("docker-compose.yml", "r") as f:
+    obj = compose_py.load_yaml(f)
 print(obj)  # Prints 'compose_py.models_pydantic.ComposeSpecification(...)'
 print(obj.services["web"])  # Prints 'compose_py.models_pydantic.Service(...)'
 
 # Copy and modify the existing service, then add it to the specification
 web2 = obj.services["web"].copy()
-web2.command = '--port 8081'
+web2.command = "--port 8081"
 obj.services["web2"] = web2
 
-compose_py.dump_yaml(obj, "docker-compose-modified.yml")
+print(compose_py.dump_yaml_str(obj))
+with open("docker-compose-modified.yml", "w") as f:
+    compose_py.dump_yaml(obj, f)
 ```
 
 You can find more APIs under `compose_py.models_pydantic` package.
 
 ### dataclasses.dataclass
 
 ```py
 import compose_py
 
-obj = compose_py.load_yaml("docker-compose.yml", model=compose_py.ModelType.DATACLASSES)
+with open("docker-compose.yml", "r") as f:
+    obj = compose_py.load_yaml(f, model=compose_py.ModelType.DATACLASSES)
 print(obj)  # Prints 'compose_py.models_dataclasses.ComposeSpecification(...)'
 print(obj.services["web"])  # Prints 'compose_py.models_dataclasses.Service(...)'
 
 # Copy and modify the existing service, then add it to the specification
 web2 = obj.services["web"].copy()
-web2.command = '--port 8081'
+web2.command = "--port 8081"
 obj.services["web2"] = web2
 
-compose_py.dump_yaml(obj, "docker-compose-modified.yml", model=compose_py.ModelType.DATACLASSES)
+print(compose_py.dump_yaml_str(obj))
+with open("docker-compose-modified.yml", "w") as f:
+    compose_py.dump_yaml(obj, f, model=compose_py.ModelType.DATACLASSES)
 ```
 
 You can find more APIs under `compose_py.models_dataclasses` package.
```

### Comparing `compose-py-0.1.1/compose_py/dumper.py` & `compose-py-0.2.0/compose_py/dumper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
+import io
 import typing
-from typing import Any, Dict, Optional, TypeVar, cast, overload
+from typing import Any, Dict, Optional, TextIO, TypeVar, cast, overload
 
 from . import _yaml
-from ._types import Path
 from .model_type import ModelType
 
 ComposeSpecification = Any
 TObj = TypeVar("TObj")
 
 if typing.TYPE_CHECKING:
     from typing import Literal
@@ -55,58 +55,109 @@
 
         return models_dataclasses.dump_dict(obj, simplify=simplify)
 
 
 @overload
 def dump_yaml(
     obj: "models_pydantic.ComposeSpecification",
-    path: Path,
+    stream: TextIO,
     *,
     model: "Literal[ModelType.PYDANTIC]" = ...,
     simplify: bool = ...,
     dumper: Optional[_yaml.DumperType] = ...,
 ) -> None:
     ...
 
 
 @overload
 def dump_yaml(
     obj: "models_dataclasses.ComposeSpecification",
-    path: Path,
+    stream: TextIO,
     *,
     model: "Literal[ModelType.DATACLASSES]",
     simplify: bool = ...,
     dumper: Optional[_yaml.DumperType] = ...,
 ) -> None:
     ...
 
 
 @overload
 def dump_yaml(
     obj: ComposeSpecification,
-    path: Path,
+    stream: TextIO,
     *,
     model: ModelType,
     simplify: bool = ...,
     dumper: Optional[_yaml.DumperType] = ...,
 ) -> None:
     ...
 
 
 def dump_yaml(
     obj: ComposeSpecification,
-    path: Path,
+    stream: TextIO,
     *,
     model: ModelType = ModelType.PYDANTIC,
     simplify: bool = True,
     dumper: Optional[_yaml.DumperType] = None,
 ) -> None:
     data = dump_dict(obj, model=model, simplify=simplify)
     data = replace_enum_with_values(data)
-    _yaml.dump(data, path, dumper=dumper)
+    _yaml.dump(data, stream, dumper=dumper)
+
+
+@overload
+def dump_yaml_str(
+    obj: "models_pydantic.ComposeSpecification",
+    *,
+    model: "Literal[ModelType.PYDANTIC]" = ...,
+    simplify: bool = ...,
+    dumper: Optional[_yaml.DumperType] = ...,
+) -> str:
+    ...
+
+
+@overload
+def dump_yaml_str(
+    obj: "models_dataclasses.ComposeSpecification",
+    *,
+    model: "Literal[ModelType.DATACLASSES]",
+    simplify: bool = ...,
+    dumper: Optional[_yaml.DumperType] = ...,
+) -> str:
+    ...
+
+
+@overload
+def dump_yaml_str(
+    obj: ComposeSpecification,
+    *,
+    model: ModelType,
+    simplify: bool = ...,
+    dumper: Optional[_yaml.DumperType] = ...,
+) -> str:
+    ...
+
+
+def dump_yaml_str(
+    obj: ComposeSpecification,
+    *,
+    model: ModelType = ModelType.PYDANTIC,
+    simplify: bool = True,
+    dumper: Optional[_yaml.DumperType] = None,
+) -> str:
+    with io.StringIO() as buf:
+        dump_yaml(
+            obj,
+            stream=buf,
+            model=model,
+            simplify=simplify,
+            dumper=dumper,
+        )
+        return buf.getvalue()
 
 
 def replace_enum_with_values(obj: TObj) -> TObj:
     if isinstance(obj, enum.Enum):
         ret = obj.value
     elif isinstance(obj, dict):
         ret = {
```

### Comparing `compose-py-0.1.1/compose_py/loader.py` & `compose-py-0.2.0/compose_py/loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import io
 import typing
-from typing import Any, Dict, Optional, overload
+from typing import Any, Dict, Optional, TextIO, overload
 
 from . import _yaml
-from ._types import Path
 from .model_type import ModelType
 
 ComposeSpecification = Any
 
 if typing.TYPE_CHECKING:
     from typing import Literal
 
@@ -49,43 +49,83 @@
         from . import models_dataclasses
 
         return models_dataclasses.load_dict(data)
 
 
 @overload
 def load_yaml(
-    path: Path,
+    stream: TextIO,
     *,
     model: "Literal[ModelType.PYDANTIC]" = ...,
     loader: Optional[_yaml.LoaderType] = ...,
 ) -> "models_pydantic.ComposeSpecification":
     ...
 
 
 @overload
 def load_yaml(
-    path: Path,
+    stream: TextIO,
     *,
     model: "Literal[ModelType.DATACLASSES]",
     loader: Optional[_yaml.LoaderType] = ...,
 ) -> "models_dataclasses.ComposeSpecification":
     ...
 
 
 @overload
 def load_yaml(
-    path: Path,
+    stream: TextIO,
     *,
     model: ModelType,
     loader: Optional[_yaml.LoaderType] = ...,
 ) -> ComposeSpecification:
     ...
 
 
 def load_yaml(
-    path: Path,
+    stream: TextIO,
     *,
     model: ModelType = ModelType.PYDANTIC,
     loader: Optional[_yaml.LoaderType] = None,
 ) -> ComposeSpecification:
-    data = _yaml.load(path, loader=loader)
+    data = _yaml.load(stream, loader=loader)
     return load_dict(data, model=model)
+
+
+@overload
+def load_yaml_str(
+    content: str,
+    *,
+    model: "Literal[ModelType.PYDANTIC]" = ...,
+    loader: Optional[_yaml.LoaderType] = ...,
+) -> "models_pydantic.ComposeSpecification":
+    ...
+
+
+@overload
+def load_yaml_str(
+    content: str,
+    *,
+    model: "Literal[ModelType.DATACLASSES]",
+    loader: Optional[_yaml.LoaderType] = ...,
+) -> "models_dataclasses.ComposeSpecification":
+    ...
+
+
+@overload
+def load_yaml_str(
+    content: str,
+    *,
+    model: ModelType,
+    loader: Optional[_yaml.LoaderType] = ...,
+) -> ComposeSpecification:
+    ...
+
+
+def load_yaml_str(
+    content: str,
+    *,
+    model: ModelType = ModelType.PYDANTIC,
+    loader: Optional[_yaml.LoaderType] = None,
+) -> ComposeSpecification:
+    with io.StringIO(content) as buf:
+        return load_yaml(buf, model=model, loader=loader)
```

### Comparing `compose-py-0.1.1/compose_py/models_dataclasses/__init__.py` & `compose-py-0.2.0/compose_py/models_dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.1/compose_py/models_dataclasses/_generated.py` & `compose-py-0.2.0/compose_py/models_dataclasses/_generated.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.1/compose_py/models_pydantic/__init__.py` & `compose-py-0.2.0/compose_py/models_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.1/compose_py/models_pydantic/_generated.py` & `compose-py-0.2.0/compose_py/models_pydantic/_generated.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.1/compose_py.egg-info/PKG-INFO` & `compose-py-0.2.0/compose_py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-py
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python library for parsing and loading Compose files
 Author-email: Yuki Igarashi <me@bonprosoft.com>
 License: MIT License
         
         Copyright (c) 2023 Yuki Igarashi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,40 +61,46 @@
 ## Tutorial: Load, modify, and save docker-compose.yml
 
 ### Pydantic.BaseModel (default)
 
 ```py
 import compose_py
 
-obj = compose_py.load_yaml("docker-compose.yml")
+with open("docker-compose.yml", "r") as f:
+    obj = compose_py.load_yaml(f)
 print(obj)  # Prints 'compose_py.models_pydantic.ComposeSpecification(...)'
 print(obj.services["web"])  # Prints 'compose_py.models_pydantic.Service(...)'
 
 # Copy and modify the existing service, then add it to the specification
 web2 = obj.services["web"].copy()
-web2.command = '--port 8081'
+web2.command = "--port 8081"
 obj.services["web2"] = web2
 
-compose_py.dump_yaml(obj, "docker-compose-modified.yml")
+print(compose_py.dump_yaml_str(obj))
+with open("docker-compose-modified.yml", "w") as f:
+    compose_py.dump_yaml(obj, f)
 ```
 
 You can find more APIs under `compose_py.models_pydantic` package.
 
 ### dataclasses.dataclass
 
 ```py
 import compose_py
 
-obj = compose_py.load_yaml("docker-compose.yml", model=compose_py.ModelType.DATACLASSES)
+with open("docker-compose.yml", "r") as f:
+    obj = compose_py.load_yaml(f, model=compose_py.ModelType.DATACLASSES)
 print(obj)  # Prints 'compose_py.models_dataclasses.ComposeSpecification(...)'
 print(obj.services["web"])  # Prints 'compose_py.models_dataclasses.Service(...)'
 
 # Copy and modify the existing service, then add it to the specification
 web2 = obj.services["web"].copy()
-web2.command = '--port 8081'
+web2.command = "--port 8081"
 obj.services["web2"] = web2
 
-compose_py.dump_yaml(obj, "docker-compose-modified.yml", model=compose_py.ModelType.DATACLASSES)
+print(compose_py.dump_yaml_str(obj))
+with open("docker-compose-modified.yml", "w") as f:
+    compose_py.dump_yaml(obj, f, model=compose_py.ModelType.DATACLASSES)
 ```
 
 You can find more APIs under `compose_py.models_dataclasses` package.
```

### Comparing `compose-py-0.1.1/compose_py.egg-info/SOURCES.txt` & `compose-py-0.2.0/compose_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.1/pyproject.toml` & `compose-py-0.2.0/pyproject.toml`

 * *Files identical despite different names*

