# Comparing `tmp/arclet-letoderea-0.5.0.tar.gz` & `tmp/arclet-letoderea-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-letoderea-0.5.0.tar", last modified: Sun Apr 23 14:05:38 2023, max compression
+gzip compressed data, was "arclet-letoderea-0.6.0.tar", last modified: Tue May 23 11:48:12 2023, max compression
```

## Comparing `arclet-letoderea-0.5.0.tar` & `arclet-letoderea-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0      664 2023-04-23 09:37:34.234901 arclet-letoderea-0.5.0/arclet/letoderea/__init__.py
--rw-r--r--   0        0        0     5634 2023-04-23 12:57:29.709109 arclet-letoderea-0.5.0/arclet/letoderea/auxiliary.py
--rw-r--r--   0        0        0        0 2023-03-19 17:38:39.637869 arclet-letoderea-0.5.0/arclet/letoderea/builtin/__init__.py
--rw-r--r--   0        0        0     4126 2023-04-23 13:50:53.063424 arclet-letoderea-0.5.0/arclet/letoderea/builtin/breakpoint.py
--rw-r--r--   0        0        0      820 2023-04-07 06:45:50.811871 arclet-letoderea-0.5.0/arclet/letoderea/builtin/depend.py
--rw-r--r--   0        0        0      197 2023-03-31 18:59:49.623386 arclet-letoderea-0.5.0/arclet/letoderea/context.py
--rw-r--r--   0        0        0     5752 2023-04-23 13:49:49.822125 arclet-letoderea-0.5.0/arclet/letoderea/core.py
--rw-r--r--   0        0        0     1681 2023-04-23 09:37:34.338972 arclet-letoderea-0.5.0/arclet/letoderea/decorate.py
--rw-r--r--   0        0        0     1157 2023-03-23 05:47:21.240677 arclet-letoderea-0.5.0/arclet/letoderea/event.py
--rw-r--r--   0        0        0      304 2023-04-07 06:45:50.801739 arclet-letoderea-0.5.0/arclet/letoderea/exceptions.py
--rw-r--r--   0        0        0     6341 2023-04-07 07:32:34.326656 arclet-letoderea-0.5.0/arclet/letoderea/handler.py
--rw-r--r--   0        0        0     2689 2023-04-23 10:05:34.641270 arclet-letoderea-0.5.0/arclet/letoderea/provider.py
--rw-r--r--   0        0        0     5739 2023-04-23 13:09:19.611255 arclet-letoderea-0.5.0/arclet/letoderea/publisher.py
--rw-r--r--   0        0        0     3157 2023-04-05 12:57:09.191974 arclet-letoderea-0.5.0/arclet/letoderea/subscriber.py
--rw-r--r--   0        0        0      438 2023-04-23 12:57:29.695404 arclet-letoderea-0.5.0/arclet/letoderea/typing.py
--rw-r--r--   0        0        0     1091 2022-01-26 08:43:52.013649 arclet-letoderea-0.5.0/LICENSE
--rw-r--r--   0        0        0      983 2023-04-23 13:54:09.621159 arclet-letoderea-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1435 2023-04-23 14:03:37.949668 arclet-letoderea-0.5.0/README.md
--rw-r--r--   0        0        0     1527 2023-04-23 13:07:44.994194 arclet-letoderea-0.5.0/tests/breakpoint.py
--rw-r--r--   0        0        0     2013 2023-04-23 13:38:01.109308 arclet-letoderea-0.5.0/tests/breakpoint1.py
--rw-r--r--   0        0        0     2282 2023-04-07 06:47:47.105418 arclet-letoderea-0.5.0/tests/combine.py
--rw-r--r--   0        0        0     1894 2023-04-23 09:37:34.206903 arclet-letoderea-0.5.0/tests/condition.py
--rw-r--r--   0        0        0     1462 2023-04-23 09:37:34.153727 arclet-letoderea-0.5.0/tests/decorator.py
--rw-r--r--   0        0        0      751 2023-04-23 09:37:34.246904 arclet-letoderea-0.5.0/tests/depend.py
--rw-r--r--   0        0        0      574 2023-04-23 09:37:34.259901 arclet-letoderea-0.5.0/tests/except.py
--rw-r--r--   0        0        0      918 2023-04-23 09:37:34.217955 arclet-letoderea-0.5.0/tests/nest_except.py
--rw-r--r--   0        0        0      776 2023-03-23 05:47:21.277677 arclet-letoderea-0.5.0/tests/test_handler.py
--rw-r--r--   0        0        0      583 2023-04-05 13:13:59.929688 arclet-letoderea-0.5.0/tests/test_param_parser.py
--rw-r--r--   0        0        0     1892 2023-04-23 09:37:34.294207 arclet-letoderea-0.5.0/tests/test_provider.py
--rw-r--r--   0        0        0      886 2023-04-23 10:03:48.864079 arclet-letoderea-0.5.0/tests/test_provider_validate.py
--rw-r--r--   0        0        0      784 2023-04-23 13:11:33.978272 arclet-letoderea-0.5.0/tests/test_publisher.py
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 arclet-letoderea-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      699 2023-05-23 11:13:22.565530 arclet-letoderea-0.6.0/arclet/letoderea/__init__.py
+-rw-r--r--   0        0        0     5634 2023-04-23 12:57:29.709109 arclet-letoderea-0.6.0/arclet/letoderea/auxiliary.py
+-rw-r--r--   0        0        0        0 2023-03-19 17:38:39.637869 arclet-letoderea-0.6.0/arclet/letoderea/builtin/__init__.py
+-rw-r--r--   0        0        0     4126 2023-05-23 11:09:48.618672 arclet-letoderea-0.6.0/arclet/letoderea/builtin/breakpoint.py
+-rw-r--r--   0        0        0      820 2023-04-07 06:45:50.811871 arclet-letoderea-0.6.0/arclet/letoderea/builtin/depend.py
+-rw-r--r--   0        0        0      197 2023-03-31 18:59:49.623386 arclet-letoderea-0.6.0/arclet/letoderea/context.py
+-rw-r--r--   0        0        0     5729 2023-05-23 11:13:22.582428 arclet-letoderea-0.6.0/arclet/letoderea/core.py
+-rw-r--r--   0        0        0     2795 2023-05-23 11:13:22.596426 arclet-letoderea-0.6.0/arclet/letoderea/decorate.py
+-rw-r--r--   0        0        0     1157 2023-05-23 11:10:03.568928 arclet-letoderea-0.6.0/arclet/letoderea/event.py
+-rw-r--r--   0        0        0      304 2023-04-07 06:45:50.801739 arclet-letoderea-0.6.0/arclet/letoderea/exceptions.py
+-rw-r--r--   0        0        0     6547 2023-05-23 11:10:50.897248 arclet-letoderea-0.6.0/arclet/letoderea/handler.py
+-rw-r--r--   0        0        0     2777 2023-05-23 10:37:01.126215 arclet-letoderea-0.6.0/arclet/letoderea/provider.py
+-rw-r--r--   0        0        0     5739 2023-05-23 11:10:21.612761 arclet-letoderea-0.6.0/arclet/letoderea/publisher.py
+-rw-r--r--   0        0        0     2843 2023-05-23 10:42:21.102508 arclet-letoderea-0.6.0/arclet/letoderea/ref.py
+-rw-r--r--   0        0        0     3835 2023-05-23 10:07:54.108344 arclet-letoderea-0.6.0/arclet/letoderea/subscriber.py
+-rw-r--r--   0        0        0      438 2023-04-23 12:57:29.695404 arclet-letoderea-0.6.0/arclet/letoderea/typing.py
+-rw-r--r--   0        0        0     1091 2022-01-26 08:43:52.013649 arclet-letoderea-0.6.0/LICENSE
+-rw-r--r--   0        0        0      983 2023-05-23 10:51:39.907899 arclet-letoderea-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4039 2023-05-23 11:40:50.641876 arclet-letoderea-0.6.0/README.md
+-rw-r--r--   0        0        0      789 2023-05-23 10:08:12.767551 arclet-letoderea-0.6.0/tests/annotated.py
+-rw-r--r--   0        0        0     1527 2023-04-23 13:07:44.994194 arclet-letoderea-0.6.0/tests/breakpoint.py
+-rw-r--r--   0        0        0     2013 2023-04-23 13:38:01.109308 arclet-letoderea-0.6.0/tests/breakpoint1.py
+-rw-r--r--   0        0        0     2282 2023-04-07 06:47:47.105418 arclet-letoderea-0.6.0/tests/combine.py
+-rw-r--r--   0        0        0     1894 2023-04-23 09:37:34.206903 arclet-letoderea-0.6.0/tests/condition.py
+-rw-r--r--   0        0        0     1462 2023-04-23 09:37:34.153727 arclet-letoderea-0.6.0/tests/decorator.py
+-rw-r--r--   0        0        0      751 2023-04-23 09:37:34.246904 arclet-letoderea-0.6.0/tests/depend.py
+-rw-r--r--   0        0        0      556 2023-05-23 10:37:01.110216 arclet-letoderea-0.6.0/tests/except.py
+-rw-r--r--   0        0        0      918 2023-04-23 09:37:34.217955 arclet-letoderea-0.6.0/tests/nest_except.py
+-rw-r--r--   0        0        0     1114 2023-05-23 10:44:20.958987 arclet-letoderea-0.6.0/tests/shortcut.py
+-rw-r--r--   0        0        0      776 2023-03-23 05:47:21.277677 arclet-letoderea-0.6.0/tests/test_handler.py
+-rw-r--r--   0        0        0      583 2023-04-05 13:13:59.929688 arclet-letoderea-0.6.0/tests/test_param_parser.py
+-rw-r--r--   0        0        0     1892 2023-04-23 09:37:34.294207 arclet-letoderea-0.6.0/tests/test_provider.py
+-rw-r--r--   0        0        0      860 2023-05-23 10:38:49.060805 arclet-letoderea-0.6.0/tests/test_provider_validate.py
+-rw-r--r--   0        0        0      767 2023-05-23 10:38:49.047836 arclet-letoderea-0.6.0/tests/test_publisher.py
+-rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 arclet-letoderea-0.6.0/PKG-INFO
```

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/__init__.py` & `arclet-letoderea-0.6.0/arclet/letoderea/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,13 +14,14 @@
     SupplyAuxiliary,
     auxilia,
 )
 from .builtin.breakpoint import Breakpoint, StepOut
 from .builtin.depend import Depend, Depends
 from .context import system_ctx
 from .core import EventSystem
-from .decorate import bind, subscribe
+from .decorate import bind, subscribe, bypass_if
 from .event import BaseEvent
 from .exceptions import JudgementError, ParsingStop, PropagationCancelled
 from .provider import Param, Provider, provide
 from .publisher import Publisher
 from .typing import Contexts, Force
+from .ref import deref
```

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/auxiliary.py` & `arclet-letoderea-0.6.0/arclet/letoderea/auxiliary.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/builtin/breakpoint.py` & `arclet-letoderea-0.6.0/arclet/letoderea/builtin/breakpoint.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/builtin/depend.py` & `arclet-letoderea-0.6.0/arclet/letoderea/builtin/depend.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/core.py` & `arclet-letoderea-0.6.0/arclet/letoderea/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,26 +86,25 @@
                     continue
                 await self.publish(event, publisher)
 
     def add_publisher(self, publisher: Publisher):
         self.publishers[publisher.id] = publisher
 
     def publish(self, event: BaseEvent, publisher: str | Publisher | None = None):
-        pubs = []
+        pubs = [self._backend_publisher]
         if isinstance(publisher, str) and (pub := self.publishers.get(publisher)):
             pubs.append(pub)
         elif not publisher:
             pubs.extend(
                 pub
                 for pub in self.publishers.values()
                 if pub.validate(event.__class__)  # type: ignore
             )
         else:
             pubs.append(publisher)
-        pubs.append(self._backend_publisher)
         subscribers = sum((pub.subscribers.get(event.__class__, []) for pub in pubs), [])
         task = self.loop.create_task(dispatch(subscribers, event))
         task.add_done_callback(self._ref_tasks.discard)
         return task
 
     def on(
         self,
```

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/event.py` & `arclet-letoderea-0.6.0/arclet/letoderea/event.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/handler.py` & `arclet-letoderea-0.6.0/arclet/letoderea/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,15 +176,19 @@
             continue
         if res.__class__ is Force:
             res = res.value
         return res
     if annotation:
         for key, value in context.items():
             if generic_isinstance(value, annotation):
-                providers.append(provide(annotation, target=key)())
+                providers.append(provide(annotation, key)())
                 return value
             if isinstance(annotation, str) and f"{type(value)}" == annotation:
-                providers.append(provide(type(value), target=key)())
+                providers.append(provide(type(value), key)())
                 return value
+        if hasattr(context["event"], name):
+            value = getattr(context["event"], name)
+            providers.append(provide(type(value), call=lambda x: getattr(x['event'], name))())
+            return value
     if default is not Empty:
         return default
     raise UndefinedRequirement(name, annotation, default, providers)
```

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/provider.py` & `arclet-letoderea-0.6.0/arclet/letoderea/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,18 +55,18 @@
         依据提供模式，从集合中提供一个对象
         """
         raise NotImplementedError
 
 
 def provide(
     origin: type[T],
-    name: str = "_Provider",
-    call: Callable[[Contexts], T | None | Awaitable[T | None]] | None = None,
-    validate: Callable[[Param], bool] | None = None,
     target: str | None = None,
+    call: Callable[[Contexts], T | None | Awaitable[T | None]] | str | None = None,
+    validate: Callable[[Param], bool] | None = None,
+    _id: str = "_Provider",
 ) -> type[Provider[T]]:
     """
     用于动态生成 Provider 的装饰器
     """
     if not call and not target:
         raise ValueError("Either `call` or `target` must be provided")
 
@@ -77,15 +77,17 @@
                 if validate
                 else param.name == target
                 if target
                 else super().validate(param)
             )
 
         async def __call__(self, context: Contexts):
-            return (
-                await run_always_await(call, context) if call else context.get(target)
-            )
+            if not call:
+                return context.get(target)
+            if isinstance(call, str):
+                return context.get(call)
+            return await run_always_await(call, context)
 
         def __repr__(self):
-            return f"Provider::{name}(origin={origin})"
+            return f"Provider::{_id}(origin={origin})"
 
     return _Provider
```

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/publisher.py` & `arclet-letoderea-0.6.0/arclet/letoderea/publisher.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/arclet/letoderea/subscriber.py` & `arclet-letoderea-0.6.0/arclet/letoderea/subscriber.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import partial
 from typing import Any, Callable, Generic, TypeVar
 from tarina import signatures, run_always_await
+from typing_extensions import Annotated, get_origin, get_args
 
 from .auxiliary import Scope, AuxType, BaseAuxiliary, Executor, combine
 from .provider import Param, Provider, provide
 from .typing import TTarget
+from .ref import Deref, generate
 
 
 @dataclass
 class CompileParam:
     name: str
     annotation: Any
     default: Any
@@ -26,14 +28,25 @@
     for name, anno, default in signatures(target):
         param = CompileParam(name, anno, default, [], None)
         for _provider in providers:
             if _provider.validate(
                 Param(name, anno, default, bool(len(param.providers)))
             ):
                 param.providers.append(_provider)
+        if get_origin(anno) is Annotated:
+            org, *meta = get_args(anno)
+            for m in reversed(meta):
+                if isinstance(m, Provider):
+                    param.providers.insert(0, m)
+                elif isinstance(m, str):
+                    param.providers.insert(0, provide(org, name, lambda x: x.get(m))())
+                elif isinstance(m, Deref):
+                    param.providers.insert(0, provide(org, name, generate(m))())
+                elif callable(m):
+                    param.providers.insert(0, provide(org, name, m)())
         if isinstance(default, Provider):
             param.providers.insert(0, default)
         if isinstance(default, BaseAuxiliary) and (default.type == AuxType.depend):
             param.depend = provide(anno, call=partial(default, "parsing"))()
         res.append(param)
     return res
```

### Comparing `arclet-letoderea-0.5.0/LICENSE` & `arclet-letoderea-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/pyproject.toml` & `arclet-letoderea-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-letoderea"
-version = "0.5.0"
+version = "0.6.0"
 description = "A high-performance, simple-structured event system, relies on asyncio"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "tarina>=0.3.0",
 ]
```

### Comparing `arclet-letoderea-0.5.0/tests/breakpoint.py` & `arclet-letoderea-0.6.0/tests/breakpoint.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/breakpoint1.py` & `arclet-letoderea-0.6.0/tests/breakpoint1.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/combine.py` & `arclet-letoderea-0.6.0/tests/combine.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/condition.py` & `arclet-letoderea-0.6.0/tests/condition.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/decorator.py` & `arclet-letoderea-0.6.0/tests/decorator.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/depend.py` & `arclet-letoderea-0.6.0/tests/depend.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/nest_except.py` & `arclet-letoderea-0.6.0/tests/nest_except.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/test_handler.py` & `arclet-letoderea-0.6.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/test_param_parser.py` & `arclet-letoderea-0.6.0/tests/test_param_parser.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/test_provider.py` & `arclet-letoderea-0.6.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `arclet-letoderea-0.5.0/tests/test_provider_validate.py` & `arclet-letoderea-0.6.0/tests/test_provider_validate.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     type: str = "TestEvent"
     msg: int = 0
 
     async def gather(self, context: dict):
         context['index'] = self.msg
 
 
-@es.on(TestEvent, providers=[provide(int, call=lambda x: x['index'])])
+@es.on(TestEvent, providers=[provide(int, call='index')])
 async def test(index: Union[str, int], a: str = "hello", ):
     print("test:", index, a)
     # test: 0 hello
     # provide, 'index' -> int -> index: Union[str, int]
     # no provide, a: str = "hello"
 
 
-@es.on(TestEvent, providers=[provide(Union[int, str], call=lambda x: x['index'])])
+@es.on(TestEvent, providers=[provide(Union[int, str], call='index')])
 async def test1(index: int, a: str = "hello", ):
     print("test1:", index, a)
     # test1: 0 0
     # provide, 'index' -> Union[int, str] -> index: int
     # provide, 'index' -> Union[int, str] -> a: str
```

### Comparing `arclet-letoderea-0.5.0/tests/test_publisher.py` & `arclet-letoderea-0.6.0/tests/test_publisher.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class MyPublisher(Publisher):
 
     def validate(self, event: type[BaseEvent]):
         return event == TestEvent
 
 
-test = provide(str, call=lambda x: x.get("name"))
+test = provide(str, call="name")
 my_publisher = MyPublisher("test")
 es.add_publisher(my_publisher)
 my_publisher.unsafe_push(TestEvent("hello world"))
 my_publisher[TestEvent] += test()
 
 
 @es.on(TestEvent)
```

