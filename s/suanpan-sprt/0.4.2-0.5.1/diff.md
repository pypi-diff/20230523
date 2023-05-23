# Comparing `tmp/suanpan-sprt-0.4.2.tar.gz` & `tmp/suanpan-sprt-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.4.2.tar", last modified: Fri Apr  7 07:10:38 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.5.1.tar", last modified: Tue May 23 01:43:36 2023, max compression
```

## Comparing `suanpan-sprt-0.4.2.tar` & `suanpan-sprt-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-04-07 07:10:38.000000 suanpan-sprt-0.4.2/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      437 2023-04-07 07:10:38.000000 suanpan-sprt-0.4.2/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       84 2023-03-13 09:36:01.000000 suanpan-sprt-0.4.2/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-04-07 07:10:38.000000 suanpan-sprt-0.4.2/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1038 2023-03-13 09:36:01.000000 suanpan-sprt-0.4.2/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-04-07 07:10:38.000000 suanpan-sprt-0.4.2/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.4.2/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3136 2023-03-23 04:28:38.000000 suanpan-sprt-0.4.2/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8450 2023-04-06 01:54:57.000000 suanpan-sprt-0.4.2/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      190 2023-03-13 09:36:01.000000 suanpan-sprt-0.4.2/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3700 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3365 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      605 2023-04-04 09:18:04.000000 suanpan-sprt-0.4.2/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-04-07 07:10:38.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      437 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-04-07 07:10:38.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       44 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-04-07 07:10:37.000000 suanpan-sprt-0.4.2/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      437 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       84 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.1/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.1/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5072 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4853 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      605 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.1/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      437 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.1/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.4.2/setup.py` & `suanpan-sprt-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,10 +30,11 @@
 
     install_requires=requires,
     python_requires=">=3.7",
     classifiers=[],
     entry_points={
       "console_scripts": [
         "sprt=sprt.__main__:main",
+        "sprun=sprt.__main__:run",
       ]
     },
 )
```

### Comparing `suanpan-sprt-0.4.2/sprt/arguments.py` & `suanpan-sprt-0.5.1/sprt/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import json
 import pathlib
 import inspect
 import pydantic
-from typing import Union, Type, cast
 from dataclasses import is_dataclass, asdict
-from pydantic.dataclasses import dataclass as pydantic_dataclass
+from quart_schema import validation
 from .exceptions import ArgumentRequiredError, ArgumentError, RequestSchemaValidationError
 from .storage import Storage
 from . import envs
 
-PydanticModel = Union[Type[pydantic.BaseModel], Type["Dataclass"]]
-
 
 class BaseArgument(object):
     def __init__(self, key, alias=None, required=False, default=None, arg_spec: inspect.FullArgSpec = None, **kwargs):
         self.key = key
         self.alias = alias
         self.required = required
         self.default = default
@@ -123,30 +120,26 @@
         if value is None:
             return value
 
         return json.dumps(value)
 
 
 class Dataclass(Json):
-    def _to_pydantic_model(self) -> PydanticModel:
-        pydantic_model_class: PydanticModel
-        if is_dataclass(self.annotation):
-            pydantic_model_class = pydantic_dataclass(self.annotation)
-        else:
-            pydantic_model_class = cast(PydanticModel, self.annotation)
-        return pydantic_model_class
+    def __init__(self, key, **kwargs):
+        super().__init__(key, **kwargs)
+        self.model_class = None
 
     def load(self, value):
         value = super(Dataclass, self).load(value)
         if value is None:
             return value
-
-        model_class = self._to_pydantic_model()
+        if self.model_class is None:
+            self.model_class = validation._to_pydantic_model(self.annotation)
         try:
-            model = model_class(**value)
+            model = self.model_class(**value)
         except (TypeError, pydantic.ValidationError) as error:
             raise RequestSchemaValidationError(error)
 
         return model
 
     def save(self, value):
         value = self.get_value_or_default(value)
```

### Comparing `suanpan-sprt-0.4.2/sprt/envs.py` & `suanpan-sprt-0.5.1/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.4.2/sprt/loader.py` & `suanpan-sprt-0.5.1/sprt/loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,76 +2,95 @@
 import logging
 import inspect
 import pathlib
 import importlib
 import importlib.util
 from .arguments import init_arg_from_arg_spec, init_return_from_value, DEFAULT_DATA_SUBTYPE_ARGS_MAP
 from .storage import Storage
-from .exceptions import ParamsArgError
+from .exceptions import ParamsArgError, InvocationFunctionError
 from . import envs
 
 
 class NodeFunction(object):
     def __init__(self, node_id, working_dir, filename, function='main'):
         file = pathlib.Path(filename)
         self.name = file.stem
         self.location = pathlib.Path(working_dir) / filename
         self.function = function
         self.module = self.load_module()
         self.context = RuntimeContext(envs.userId, envs.appId, node_id)
+        self.input_arguments = []
+        self.has_context = False
+        self.load_validator()
 
     def load_module(self):
         if not self.location.is_file():
             raise Exception(f'invalid component file: {self.location}')
 
         spec = importlib.util.spec_from_file_location(self.name, self.location)
         if spec is None:
             raise Exception(f'invalid component spec: {self.location}')
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         return module
 
-    async def call_func(self, request_id, args, params):
-        in_slot = []
+    def load_validator(self):
         has_context = False
 
         func = getattr(self.module, self.function)
         arg_spec = inspect.getfullargspec(func)
         for index, a in enumerate(arg_spec.args):
             if a == 'context':
                 if index != len(arg_spec.args) - 1:
                     raise ParamsArgError('context MUST be the last argument of function')
 
                 has_context = True
                 continue
 
             arg_class = init_arg_from_arg_spec(a, arg_spec)
             arg = arg_class(a, arg_spec=arg_spec)
+            self.input_arguments.append(arg)
+
+        if has_context or arg_spec.varkw is not None:
+            self.has_context = True
+        else:
+            raise ParamsArgError('function MUST have a "context" argument')
+
+    async def call_func(self, request_id, args, params):
+        in_slot = []
+
+        func = getattr(self.module, self.function)
+        arg_spec = inspect.getfullargspec(func)
+        for index, a in enumerate(arg_spec.args):
+            if a == 'context':
+                continue
+
+            arg = self.input_arguments[index]
 
             inx = f'in{index + 1}'
             value = args.get(inx)
             value = arg.load(value)
 
             in_slot.append(value)
 
         self.context.reset(request_id, params)
-        if has_context or arg_spec.varkw is not None:
+        try:
             if inspect.iscoroutinefunction(func):
                 ret = await func(*in_slot, context=self.context)
             else:
                 ret = func(*in_slot, context=self.context)
-        else:
-            raise ParamsArgError('function MUST have a "context" argument')
 
-        if isinstance(ret, tuple):
-            return {f'out{index + 1}': init_return_from_value(r, arg_spec, index)(
-                f'out{index + 1}', request_id=request_id).save(r)
-                    for index, r in enumerate(ret)}
-        else:
-            return {'out1': init_return_from_value(ret, arg_spec, 0)(f'out{1}', request_id=request_id).save(ret)}
+            if isinstance(ret, tuple):
+                return {f'out{index + 1}': init_return_from_value(r, arg_spec, index)(
+                    f'out{index + 1}', request_id=request_id).save(r)
+                        for index, r in enumerate(ret)}
+            else:
+                return {'out1': init_return_from_value(ret, arg_spec, 0)(f'out{1}', request_id=request_id).save(ret)}
+        except Exception as e:
+            raise InvocationFunctionError(f'call function: {e}')
 
 
 class RuntimeContext(object):
     def __init__(self, user_id, app_id, node_id):
         self.request_id = None
         self.user_id = user_id
         self.app_id = app_id
```

### Comparing `suanpan-sprt-0.4.2/sprt/log.py` & `suanpan-sprt-0.5.1/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.4.2/sprt/master.py` & `suanpan-sprt-0.5.1/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.4.2/sprt/storage.py` & `suanpan-sprt-0.5.1/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.4.2/sprt/testing.py` & `suanpan-sprt-0.5.1/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.4.2/sprt/utils.py` & `suanpan-sprt-0.5.1/sprt/utils.py`

 * *Files identical despite different names*

