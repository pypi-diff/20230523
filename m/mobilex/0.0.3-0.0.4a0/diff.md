# Comparing `tmp/mobilex-0.0.3.tar.gz` & `tmp/mobilex-0.0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobilex-0.0.3.tar", max compression
+gzip compressed data, was "mobilex-0.0.4a0.tar", max compression
```

## Comparing `mobilex-0.0.3.tar` & `mobilex-0.0.4a0.tar`

### file list

```diff
@@ -1,31 +1,19 @@
--rw-r--r--   0        0        0     1067 2022-11-14 21:23:55.060421 mobilex-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1361 2022-11-14 21:24:15.572610 mobilex-0.0.3/README.md
--rw-r--r--   0        0        0      125 2022-11-14 21:23:55.060421 mobilex-0.0.3/mobilex/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/cache/__init__.py
--rw-r--r--   0        0        0     9429 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/cache/base.py
--rw-r--r--   0        0        0     2190 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/cache/dict.py
--rw-r--r--   0        0        0     2601 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/cache/redis.py
--rw-r--r--   0        0        0      327 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/const.py
--rw-r--r--   0        0        0     2184 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/core.py
--rw-r--r--   0        0        0      912 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/exc.py
--rw-r--r--   0        0        0     2692 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/namespaces.py
--rw-r--r--   0        0        0     2519 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/response.py
--rw-r--r--   0        0        0     6887 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/router.py
--rw-r--r--   0        0        0      132 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/screens/__init__.py
--rw-r--r--   0        0        0     9271 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/screens/base.py
--rw-r--r--   0        0        0      840 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/screens/core.py
--rw-r--r--   0        0        0     2372 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/screens/mixins.py
--rw-r--r--   0        0        0     1017 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/screens/registry.py
--rw-r--r--   0        0        0       43 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/sessions/__init__.py
--rw-r--r--   0        0        0     5199 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/sessions/core.py
--rw-r--r--   0        0        0     3508 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/sessions/managers.py
--rw-r--r--   0        0        0     5806 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/settings.py
--rw-r--r--   0        0        0     1691 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/utils/__init__.py
--rw-r--r--   0        0        0     3759 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/utils/enums.py
--rw-r--r--   0        0        0      984 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/utils/functools.py
--rw-r--r--   0        0        0    11553 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/utils/local.py
--rw-r--r--   0        0        0     3276 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/utils/types.py
--rw-r--r--   0        0        0     3797 2022-11-14 21:23:55.064421 mobilex-0.0.3/mobilex/utils/uri.py
--rw-r--r--   0        0        0     1569 2022-11-14 21:23:55.064421 mobilex-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 mobilex-0.0.3/setup.py
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 mobilex-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/LICENSE.txt
+-rw-r--r--   0        0        0     1365 2023-05-23 05:26:31.482713 mobilex-0.0.4a0/README.md
+-rw-r--r--   0        0        0      342 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/__init__.py
+-rw-r--r--   0        0        0     3594 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/base.py
+-rw-r--r--   0        0        0     1880 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/dict.py
+-rw-r--r--   0        0        0     1765 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/cache/redis.py
+-rw-r--r--   0        0        0      327 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/const.py
+-rw-r--r--   0        0        0     4935 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/core.py
+-rw-r--r--   0        0        0     1022 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/exc.py
+-rw-r--r--   0        0        0     2516 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/response.py
+-rw-r--r--   0        0        0     6057 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/router.py
+-rw-r--r--   0        0        0      267 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/screens/__init__.py
+-rw-r--r--   0        0        0    11671 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/screens/base.py
+-rw-r--r--   0        0        0     6932 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/sessions.py
+-rw-r--r--   0        0        0     1807 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/utils/__init__.py
+-rw-r--r--   0        0        0     1881 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/mobilex/utils/types.py
+-rw-r--r--   0        0        0     1828 2023-05-23 05:26:17.390648 mobilex-0.0.4a0/pyproject.toml
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 mobilex-0.0.4a0/PKG-INFO
```

### Comparing `mobilex-0.0.3/LICENSE.txt` & `mobilex-0.0.4a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mobilex-0.0.3/README.md` & `mobilex-0.0.4a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 [pyversions-link]: https://pypi.python.org/pypi/mobilex
 [ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
 [ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster
 [codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex
 
 
-See this release on GitHub: [v0.0.3](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.3)
+See this release on GitHub: [v0.0.4a0](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4a0)
```

### Comparing `mobilex-0.0.3/mobilex/cache/dict.py` & `mobilex-0.0.4a0/mobilex/cache/dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 import asyncio
+import re
 import typing as t
-
 from datetime import timedelta
 
 try:
-    from cachetools import TTLCache    
-except ImportError: # pragma: no cover
+    from cachetools import TTLCache
+except ImportError:  # pragma: no cover
     raise ImportError(
         f"{__name__!r} requires 'cachetools' installed. `pip install cachetools`"
     )
 
-
 from .base import BaseCache
 
-
-
-loop = asyncio.get_event_loop()
+if t.TYPE_CHECKING:
+    from mobilex import App
 
 
 class DictCache(BaseCache):
-    
     store: TTLCache
 
-    async def setup(self, app):
-        self.store = TTLCache(1024, self.default_timeout)
-
-    async def add(self, key, value, timeout=..., version=None) -> bool:
-        """
-        Set a value in the cache if the key does not already exist. If
-        timeout is given, use that timeout for the key; otherwise use the
-        default cache timeout.
+    def __init__(self, app: "App", location=None, **options):
+        super().__init__(app, **options)
+        self.store = TTLCache(1024, self.ttl.total_seconds())
 
-        Return True if the value was stored, False otherwise.
-        """
-        sk = self.make_key(key, version)
-        if rv := not sk in self.store:
-            self.store[sk] = self.dumps(value)
-        return rv
-
-    async def get(self, key, version=None) -> t.Any:
+    async def get(self, key) -> t.Any:
         """
         Fetch a given key from the cache. If the key does not exist, return
         default, which itself defaults to None.
         """
-        rv = self.store.get(self.make_key(key, version))
-        return rv if rv is None else self.loads(rv)
+        if (rv := self.store.get(self.make_key(key))) is not None:
+            rv = self.loads(rv)
+        return rv
 
-    async def set(self, key, value, timeout=..., version=None) -> bool:
+    async def set(self, key, value) -> bool:
         """
         Set a value in the cache. If timeout is given, use that timeout for the
         key; otherwise use the default cache timeout.
         """
-        self.store[self.make_key(key, version)] = self.dumps(value)
+        self.store[self.make_key(key)] = self.dumps(value)
         return True
 
-    async def delete(self, key, version=None) -> int:
+    async def delete(self, key) -> int:
         """
         Delete a key from the cache, failing silently.
         """
-        return +(not self.store.pop(self.make_key(key, version), None) is None)
+        return +(not self.store.pop(self.make_key(key), None) is None)
 
-    async def keys(self, pattern='*', version=None) -> int:
+    async def keys(self, key="*"):
         """
         Delete a key from the cache, failing silently.
         """
-        return self.store.keys()
-
-    async def clear(self):
-        """Remove *all* values from the cache at once."""
-        self.store.clear()
-
-    async def close(self, **kwargs):
-        """Close the cache connection"""
-        self.store.clear()
+        key = b".*".join(re.escape(p) for p in self.make_key(key).split(b"*") if p)
+        p_re = key and re.compile(key)
+        return [k for k in self.store.keys() if not p_re or p_re.search(k)]
+
+    # async def clear(self):
+    #     """Remove *all* values from the cache at once."""
+    #     self.store.clear()
+
+    # async def close(self, **kwargs):
+    #     """Close the cache connection"""
+    #     self.clear()
```

### Comparing `mobilex-0.0.3/mobilex/exc.py` & `mobilex-0.0.4a0/mobilex/exc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
+class UssdError(Exception):  # pragma: no cover
+    __slots__ = (
+        "messages",
+        "code",
+        "__weakref__",
+    )
 
-class UssdError(Exception):
-
-    __slots__ = ('messages', 'code', '__weakref__',)
-
-    default_code = 'error'
-    default_message = 'Error'
+    default_code = "error"
+    default_message = "Error"
 
     def __init__(self, *msgs, code=None):
-        self.messages = msgs and list(msgs) or [self.default_message,]
+        self.messages = (
+            msgs
+            and list(msgs)
+            or [
+                self.default_message,
+            ]
+        )
         self.code = self.default_code if code is None else code
 
     @property
     def message(self):
-        return '\n'.join(self)
-    
+        return "\n".join(self)
+
     def __iter__(self):
         return iter((str(m) for m in self.messages))
 
     def __str__(self):
         return self.message
 
     def __repr__(self):
         return f'{type(self).__name__}({", ".join(map(repr, self))})'
 
 
-
 class ValidationError(UssdError):
-    
-    default_code = 'invalid'
-    default_message = 'Error! Invalid input'
-
-
+    default_code = "invalid"
+    default_message = "Error! Invalid input"
 
 
 class InputError(ValidationError):
     pass
 
 
-
 class InvalidChoiceError(ValidationError):
-
-    default_code = 'invalid_choice'
-    default_message = 'Error! Invalid choice'
-
-
+    default_code = "invalid_choice"
+    default_message = "Error! Invalid choice"
```

### Comparing `mobilex-0.0.3/mobilex/response.py` & `mobilex-0.0.4a0/mobilex/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 import typing as t
 
 
 from collections import ChainMap
+from typing import Any
 
 from .const import ResponseType
 
 
 if t.TYPE_CHECKING:
     from . import Request
 
+
 class _ResponseMeta(type):
-    
     def __new__(mcls, name, bases, dct):
         super_new = super(_ResponseMeta, mcls).__new__
-
-        st = dct['__state_attrs__'] = set(dct.get('__state_attrs__', ()))
-        exclude = {n for n in st if n[0] == '-'}
+        st = dct["__state_attrs__"] = set(dct.get("__state_attrs__", ()))
+        exclude = {n for n in st if n[0] == "-"}
         st -= exclude
         st.update(*(b.__state_attrs__ for b in bases if isinstance(b, _ResponseMeta)))
         st -= {n[1:] for n in exclude}
         # Create class
         return super_new(mcls, name, bases, dct)
 
 
-
 class Response(metaclass=_ResponseMeta):
     """USSD response object"""
 
     type: ResponseType = None
-    request: 'Request' = None
+    request: "Request" = None
     content: t.Any
     ctx: t.Mapping
 
-    __state_attrs__ = 'type', 'content', 'ctx'
-
-    def __init__(self, content: t.Optional[t.Any] = None, 
-                ctx: t.Optional[t.Mapping] = None, 
-                /, type: t.Optional[ResponseType] = None):
+    __state_attrs__ = "type", "content", "ctx"
 
+    def __init__(
+        self,
+        content: t.Optional[t.Any] = None,
+        ctx: t.Optional[t.Mapping] = None,
+        /,
+        type: t.Optional[ResponseType] = None,
+    ):
         self.content = content
         self.type = type or self.__class__.type
         self.ctx = ChainMap() if ctx is None else ChainMap({}, ctx)
-    
+
     def get_context(self, request, ctx: t.Optional[t.Mapping] = None):
         return self.ctx.new(ctx)
 
     async def render_content(self, request, ctx: t.Optional[t.Mapping] = None):
-        return f'{self.type} {self.content}'
+        return f"{self.type} {self.content}"
 
     def __getstate__(self):
         return {n: getattr(self, n) for n in self.__state_attrs__}
-        
+
     def __setstate__(self, state):
-        for k,v in state.items():
+        for k, v in state.items():
             setattr(self, k, v)
 
     async def __call__(self, request, ctx: t.Optional[t.Mapping] = None):
         return await self.render_content(request, ctx)
 
 
+R_to = t.TypeVar("R_to", str, int)
 
-R_to = t.TypeVar('R_to', str, int)
-class RedirectResponse(t.Generic[R_to], Response):
 
-    __state_attrs__ = 'to',
+class RedirectResponse(t.Generic[R_to], Response):
+    __state_attrs__ = ("to",)
 
     type: ResponseType = ResponseType.PUSH
 
-    def __init__(self, to: R_to, 
-                inpt: t.Optional[t.Any] = None, 
-                ctx: t.Optional[t.Mapping] = None, /, 
-                type: t.Optional[ResponseType] = None):
+    def __init__(
+        self,
+        to: R_to,
+        inpt: t.Optional[t.Any] = None,
+        ctx: t.Optional[t.Mapping] = None,
+        /,
+        type: t.Optional[ResponseType] = None,
+    ):
         super().__init__(inpt, ctx, type=type)
         self.to = to if isinstance(to, (str, int)) else str(to)
 
 
-
-
 class RedirectBackResponse(RedirectResponse[int]):
-
     type: ResponseType = ResponseType.POP
 
 
-
-
-def redirect(to: R_to, inpt: t.Optional[t.Any] = None, /, **ctx) -> RedirectResponse[R_to]:
+def redirect(to: R_to, inpt=None, /, **ctx) -> RedirectResponse[R_to]:
     if isinstance(to, int):
         return RedirectBackResponse(to, inpt, ctx)
     else:
         return RedirectResponse(to, inpt, ctx)
-
```

### Comparing `mobilex-0.0.3/mobilex/router.py` & `mobilex-0.0.4a0/mobilex/router.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,126 @@
-import asyncio
 import logging
 import typing as t
 
-from collections import defaultdict
-
-
-from .utils import ArgumentVector
-from .screens import CON, END
 from .const import ResponseType
-
-from .response import Response, RedirectResponse
-from .screens.registry import ScreenRegistry
-
+from .response import RedirectResponse, Response
+from .screens import CON, END, Screen
+from .utils import ArgumentVector
 
 logger = logging.getLogger(__name__)
 
 if t.TYPE_CHECKING:
-    from . import FlexUssd, Response, Request
-
+    from . import App, Request, Response
 
 
-class UssdRouter:
-
-    parent: 'FlexUssd'
+class Router:
+    parent: "App"
 
     def __init__(self, name):
         self.name = name
-        self._registry = defaultdict(ScreenRegistry)
+        self._registry = {}
         self._start_screen = None
 
     @property
     def _home_screen(self):
         try:
-            return self.__dict__['_home_screen']
+            return self.__dict__["_home_screen"]
         except KeyError:
             return self._start_screen
-    
+
     @_home_screen.setter
     def _home_screen(self, value):
-        self.__dict__['_home_screen'] = value
-    
-    @property
-    def config(self):
-        return self.parent.config
-    
+        self.__dict__["_home_screen"] = value
+
     def run_embeded(self, parent):
         self.parent = parent
 
     def screen(self, name: str):
         def decorator(screen):
             nonlocal name, self
             self.register_screen(name, screen)
             return screen
+
         return decorator
-    
+
     def register_screen(self, name: str, screen: t.Any):
-        self._registry[''].set(name, screen)
+        self._registry[name] = screen
         return screen
 
     def start_screen(self, name: str):
         def decorator(screen):
             nonlocal name, self
             self.register_start_screen(name, screen)
             return screen
+
         return decorator
-    
+
     def register_start_screen(self, name: str, screen: t.Any):
         self._start_screen = name, screen
         return self.register_screen(name, screen)
 
     def home_screen(self, name: str):
         def decorator(screen):
             nonlocal name, self
             self.register_home_screen(name, screen)
             return screen
+
         return decorator
-    
+
     def register_home_screen(self, name: str, screen: t.Any):
         self._home_screen = name, screen
         return self.register_screen(name, screen)
 
     def get_screen(self, name: str, default=...):
-        rkey, key = name.split('.', 1)
-        if (reg := self._registry.get('' if rkey == self.name else rkey)):
-            return reg.get(key, default)
-        elif default is ...:
-            raise LookupError(f'UssdScreen {name!r} not found')
-        return default
+        nm, key = self.name, name
+        if name.startswith(f"/{nm}/"):
+            key = name[len(nm) + 2 :]
 
-    def get_all_screens(self, name: str, default=...):
-        rkey, key = name.split('.', 1)
-        if (reg := self._registry.get('' if rkey == self.name else rkey)):
-            return reg.getall(key, default)
+        if (rv := self._registry.get(key)) is not None:
+            return rv
         elif default is ...:
-            raise LookupError(f'UssdScreen {name!r} not found')
+            raise LookupError(f"UssdScreen {name!r} not found")
         return default
 
     def get_start_screen(self, *, withname=False):
         name, screen = self._start_screen
-        return (f'{self.name}.{name}', screen) if withname else screen
-    
+        return (f"/{self.name}/{name}", screen) if withname else screen
+
     def get_home_screen(self, *, withname=False):
         name, screen = self._home_screen
-        return (f'{self.name}.{name}', screen) if withname else screen
-    
+        return (f"/{self.name}/{name}", screen) if withname else screen
+
     def abs_screen_name(self, name: str):
-        return f'{self.name}{name}' if name[0] == 0 else name
+        return name if name[:1] == "/" else f"/{self.name}/{name}"
 
-    def _eval_argv(self, request: 'Request') -> 'Response':
+    def eval_argv(self, request: "Request") -> "Response":
         session = request.session
         argv = ArgumentVector(
             service_code=request.service_code,
             argstr=request.ussd_string,
-            base_code=request.initial_code
+            base_code=request.initial_code,
         )
-        
+
         if session.is_stale or not (oldargv := session.argv):
             request.args = argv.args
         else:
             request.args = argv - oldargv
 
         session.argv = argv
 
-    async def pre_request(self, request: 'Request') -> 'Response':
-        request.app = self
-        self._eval_argv(request)
-
-    async def post_request(self, request: 'Request', response: 'Response') -> 'Response':
-        return response
-
     def create_new_state(self, name, screen):
-        cls = screen.Meta.state_class
+        cls = screen._state_class
         return cls(name)
 
-    def create_screen(self, state, request: 'Request'):
+    def create_screen(self, state, request: "Request") -> "Screen":
         cls = self.get_screen(state.screen)
         rv = cls(state)
         return rv
 
-    async def dispatch_request(self, request):
-
+    async def dispatch_request(self, request: "Request"):
         session = request.session
         state = session.state
 
         if session.restored:
             screen = self.get_screen(state.screen)
             if request.args or not screen._meta.restore_sessions:
                 session.reset()
@@ -152,58 +129,58 @@
             name, screen = self.get_start_screen(withname=True)
             state = session.state = self.create_new_state(name, screen)
             inpt, args = None, request.args
         else:
             inpt, *args = request.args or (None,)
 
         if state is None:
-            raise RuntimeError('Screen state cannot be None.')
+            raise RuntimeError("Screen state cannot be None.")
 
         rv = await self.dispatch_to_screen(request, state, inpt, *args)
         return rv
 
-    async def dispatch_to_screen(self, request: 'Request', state, inpt=None, /, *args):
+    async def dispatch_to_screen(self, request: "Request", state, inpt=None, /, *args):
         screen = self.create_screen(state, request)
-        
+
         try:
+            if inpt is not None and not screen.state.get("__initialized__"):
+                await screen(request)
             res = await screen(request, inpt)
         except Exception as e:
             logger.exception(e)
             raise e
 
         if isinstance(res, RedirectResponse):
             if res.type == ResponseType.POP:
                 if res.to == 0 or not (ores := await request.history.pop(res.to)):
                     n, s = self.get_home_screen(withname=True)
                     state = request.session.state = self.create_new_state(n, s)
                     state.update(res.ctx)
                 else:
-                    n, s = ores.to, self.get_screen(ores.to) 
+                    n, s = ores.to, self.get_screen(ores.to)
                     state = request.session.state = self.create_new_state(n, s)
                     state.update(ores.ctx)
                     state.update(res.ctx)
                 return await self.dispatch_to_screen(request, state, *args)
             else:
                 n = res.to = self.abs_screen_name(res.to)
                 s = self.get_screen(n)
                 state = request.session.state = self.create_new_state(n, s)
                 state.update(res.ctx)
 
                 await request.history.push(res)
-                res.content is None or (args := (res.content,) + args) 
+                res.content is None or (args := (res.content,) + args)
                 return await self.dispatch_to_screen(request, state, *args)
-    
+
         request.session.state = screen.state
-        
+
         if res in (CON, END):
-            return f'{res} {screen.payload}'
+            return f"{res} {screen.payload}"
         elif isinstance(res, tuple):
-            return ' '.join(res)
+            return " ".join(res)
         elif isinstance(res, str):
             return res
-        print('*'*30, f'RESPONSE --> {res}')
-        raise RuntimeError('Screen must return Response object or string.')
+        raise RuntimeError("Screen must return Response object or string.")
 
     async def __call__(self, request, *args, **kwargs):
-        response = await self.pre_request(request)
-        response is None and (response := await self.dispatch_request(request))
-        return await self.post_request(request, response) or response
+        self.eval_argv(request)
+        return await self.dispatch_request(request)
```

### Comparing `mobilex-0.0.3/mobilex/sessions/core.py` & `mobilex-0.0.4a0/mobilex/sessions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,61 @@
-import time
 import asyncio
-import hashlib
+import dataclasses
 import logging
+import time
 import typing as t
-import dataclasses
-from collections import namedtuple
-
-from mobilex.utils.uri import Uri
-from mobilex.utils.types import AttributeMapping
+from collections import abc
+from hashlib import md5
 
+from mobilex.utils import to_bytes
+from mobilex.utils.types import NamespaceDict
 
 if t.TYPE_CHECKING:
-    from .managers import HistoryManager
+    from mobilex.cache.base import BaseCache
+
+    from . import Request, Response
+    from .screens import ScreenState
 
 logger = logging.getLogger(__package__)
 
+_T = t.TypeVar("_T", covariant=True)
+
+_object_new = object.__new__
+
 
 @dataclasses.dataclass()
 class SessionKey:
-
-    __slots__ = 'msisdn', 'ident', #'timestamp',
+    __slots__ = (
+        "msisdn",
+        "ident",
+    )  #'timestamp',
 
     msisdn: str
     ident: str
 
-    # timestamp: float = dataclasses.field(
-    # 		init=False, compare=False, 
-    # 		repr=False, default_factory=time.time
-    # 	)
-
-    # @property
-    # def age(self) -> float:
-    # 	return time.time() - self.timestamp
-    
     def __str__(self):
-        return f'{self.msisdn}/{self.ident}'
+        return f"{self.msisdn}/{self.ident}"
 
 
 class Session:
-
     restored = None
     _is_started = False
 
     @t.overload
-    def __init__(self, ttl: int, key: SessionKey): 
+    def __init__(self, ttl: int, key: SessionKey):
         ...
+
     @t.overload
-    def __init__(self, ttl: int, msisdn: str, id: t.Optional[str]=None): 
+    def __init__(self, ttl: int, msisdn: str, id: t.Optional[str] = None):
         ...
-    def __init__(self, ttl: int, key: SessionKey, id: t.Optional[str]=None):
-        isinstance(key, SessionKey) or (key := SessionKey(key, id or None))		
-        self.key = key
-        self.ttl = ttl
-        self.created_at = None
-        self.accessed_at = None
-        self.data = AttributeMapping()
-        self.argv = None
-        self.restored = None
+
+    def __init__(self, ttl: int, key: SessionKey, id: t.Optional[str] = None):
+        isinstance(key, SessionKey) or (key := SessionKey(key, id or None))
+        self.key, self.ttl, self.created_at, self.accessed_at = key, ttl, None, None
+        self.data, self.argv, self.restored = NamespaceDict(), None, None
 
     @property
     def pk(self):
         return self.key.msisdn
 
     @property
     def msisdn(self):
@@ -79,43 +74,40 @@
         return self.age >= self.ttl
 
     @property
     def is_new(self) -> bool:
         return self.accessed_at == self.created_at
 
     @property
-    def state(self):
-        return self.data.get('__state__')
+    def state(self) -> "ScreenState":
+        return self.data.get("__state__")
 
     @state.setter
     def state(self, value):
-        self.data['__state__'] = value
-    
-    async def start_request(self, request, *, session_id: t.Optional[str]=...) -> t.NoReturn:
-        if self._is_started:
-            return self
-        
-        session_id is ... and (session_id := request.session_id)
+        self.data["__state__"] = value
 
+    def start_request(self, request: "Request") -> t.NoReturn:
+        assert not self._is_started
+        session_id = request.session_id
         if int(self.id is None) + int(session_id is None) == 1:
             self.reset()
         elif session_id != self.id or (self.id is None and self.is_stale):
             self.restored = self.key
             self.key = SessionKey(self.msisdn, session_id)
             self.accessed_at = min(self.accessed_at, time.time() - self.ttl - 1)
         elif self.restored is None:
             self.accessed_at = time.time()
             self.created_at = self.created_at or self.accessed_at
         self._is_started = True
 
-    async def finish_request(self, request) -> t.NoReturn:
-        if self._is_started:
-            del self._is_started
-            self.accessed_at = time.time()
-    
+    def finalize(self, request: "Request") -> t.NoReturn:
+        assert self._is_started
+        del self._is_started
+        self.accessed_at = time.time()
+
     def reset(self):
         self.data.clear()
         self.reset_restored()
         self.created_at = self.accessed_at = time.time()
 
     def reset_restored(self):
         self.restored = None
@@ -139,74 +131,117 @@
         self.data[key] = value
 
     def pop(self, key, *default):
         return self.data.pop(key, *default)
 
     def setdefault(self, key, value):
         return self.data.setdefault(key, value)
-    
+
     def update(self, *arg, **kw):
         self.data.update(*arg, **kw)
 
-    # def __getstate__(self):
-    # 	state = self.__dict__.copy()
-    # 	# state.setdefault('restored', None)
-    # 	return state
-
     def __eq__(self, other):
         return isinstance(other, Session) and self.key == other.key
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
         return hash(self.key)
 
     def __str__(self):
         return f'{self.__class__.__name__}("{self.key}")'
 
 
+class NavId(t.NamedTuple):
+    """Unique"""
 
+    path: bytes
+    name: bytes
 
+    def digest(self):
+        return md5(bytes(self)).digest()
 
-class StateUri(Uri):
-    """Unique 
-    """
-    __slots__ = ()
-
-    @property
-    def stem(self):
-        return self[-1] if self else None
-
-    @property
-    def hash(self):
-        return hashlib.md5(str(self).encode()).hexdigest()
+    def __bool__(self):
+        return any(self)
 
+    def __bytes__(self):
+        return b"|".join(v for v in self if v)
 
+    def __truediv__(self, seg: bytes):
+        if isinstance(seg, bytes):
+            return self.__class__(self.digest() if self else None, seg)
+        return NotImplemented
 
 
 class History:
+    __slots__ = "stack", "key_prefix", "backend", "background", "__weakref__"
 
-    def __init__(self, manager: 'HistoryManager', stack: list=None):
-        self.manager = manager
-        self.stack = [] if stack is None else stack
+    stack: list[NavId]
+    backend: "BaseCache"
+    background: list[abc.Awaitable]
+
+    def __new__(cls, request: "Request", session: "Session"):
+        app, self = request.app, _object_new(cls)
+        self.backend, self.background = app.history_backend, []
+        self.stack = session.setdefault("__state_stack", [NavId(None, None)])
+        self.key_prefix = to_bytes(buri) + b"|" if (buri := request.base_uri) else b""
+        return self
+
+    async def finalize(self):
+        background = self.background
+        del self.stack, self.background
+        background and await asyncio.gather(*background)
 
     def __len__(self):
-        return len(self.stack) + 1
-    
+        return len(self.stack)
+
     async def pop(self, k: int = None):
-        k is None and (k := -1)
-        stack = self.stack		
+        # k is None and (k := -1)
+        k = -1 if k is None else k + 1 if k > -1 else k
+        stack = self.stack
         stack[k:] = []
-        if (path := stack and stack[-1] or None):
-            return await self.manager.load_state(path.hash)
-
-    async def push(self, res):
-        screen = res.to
-        prev = self.stack and self.stack[-1] or ''
-        if not prev or prev.stem != screen:
-            path = StateUri(prev, screen)
-            self.stack.append(path)
-            asyncio.create_task(self.manager.save_state(path.hash, res))
-
+        if id := stack[-1]:
+            return await self.backend.get(self.make_key(id))
 
+    async def push(self, res: "Response"):
+        screen = to_bytes(res.to)
+        head = self.stack[-1]
+        if head.name != screen:
+            self.stack.append(id := head / screen)
+            coro = self.backend.set(self.make_key(id), res)
+            self.background.append(asyncio.ensure_future(coro))
+
+    def make_key(self, id: NavId):
+        return self.key_prefix + id.digest()
+
+
+class SessionManager:
+    def create(self, req: "Request") -> Session:
+        con = req.app.config
+        return con.session_class(con.session_ttl, req.msisdn, req.session_id)
+
+    async def load(self, req: "Request") -> Session:
+        return await req.app.session_backend.get(self.make_key(req))
+
+    async def persist(self, req: "Request", session) -> None:
+        return await req.app.session_backend.set(self.make_key(req), session)
+
+    async def open(self, request: "Request"):
+        session = await self.load(request) or self.create(request)
+        if isinstance(rv := session.start_request(request), abc.Awaitable):
+            await rv
+        request.session = session
+        request.history = History(request, session)
+        return request
+
+    async def close(self, request: "Request", response):
+        session, history = request.session, request.history
+        tasks = (
+            history.finalize(),
+            session.finalize(request),
+            self.persist(request, session),
+        )
+        await asyncio.gather(*(x for x in tasks if isinstance(x, abc.Awaitable)))
 
+    def make_key(self, req: "Request"):
+        return f"{req.base_uri}|{req.msisdn}"
```

### Comparing `mobilex-0.0.3/mobilex/utils/__init__.py` & `mobilex-0.0.4a0/mobilex/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import re
 import typing as t
 from collections import abc
+from datetime import timedelta
 
 _ussd_split_re = r"\*(?=(?:[^\"]*\"[^\"]*\")*[^\"]*$)"
 
 
+def to_bytes(obj):
+    return obj if isinstance(obj, bytes) else str(obj).encode()
+
+
+def to_timedelta(
+    val: int | float | timedelta | None, *, resolution: timedelta = timedelta(seconds=1)
+):
+    return val if isinstance(val, timedelta) else (val or 0) * resolution
+
+
 def split_argstr(s):
     return re.split(_ussd_split_re, s) if s else ()
 
 
 class ArgumentVector(list[str]):
-
     __slots__ = ()
 
     def __init__(
         self,
         iterable: t.Optional[abc.Iterable[str]] = None,
         *,
         service_code=None,
@@ -33,34 +43,26 @@
 
     @property
     def service_code(self):
         return self[0].split("*", 1)[0]
 
     @property
     def base_code(self):
-        if "*" in self[0]:
-            return self[0].split("*", 1)[1]
-        else:
-            return ""
+        return self[0].split("*", 1)[1] if "*" in self[0] else ""
 
     @property
     def args(self):
         return self[1:]
 
     def __sub__(self, other):
-        if not isinstance(other, ArgumentVector):
+        if not isinstance(other, ArgumentVector):  # pragma: no cover
             return NotImplemented
 
         ld = len(self) - len(other)
 
         return self[-ld:] if ld > 0 and self[:-ld] == other else []
 
-    # def __getitem__(self, key):
-    # 	if isinstance(key, slice):
-    # 		return self.__class__(super().__getitem__(key))
-    # 	return super().__getitem__(key)
-
     def __str__(self):
         return "%s" % "*".join(self)
 
     def __repr__(self):
         return "<ArgumentVector: %s>" % (self,)
```

### Comparing `mobilex-0.0.3/mobilex/utils/types.py` & `mobilex-0.0.4a0/mobilex/utils/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,65 @@
 import typing as t
 from collections import abc
-from copy import deepcopy
-
-from typing_extensions import Self
+from typing import Any
 
 _T_Key = t.TypeVar("_T_Key", bound=abc.Hashable)
 _T_Val = t.TypeVar("_T_Val")
 
-_T_Pk = t.TypeVar("_T_Pk", bound=abc.Hashable)
-
-
-_object_new = object.__new__
-_object_setattr = object.__setattr__
-
-
-class FallbackDict(dict[_T_Key, _T_Val]):
-
-    __slots__ = ()
-
-    def __missing__(self, key):
-        return None
-
-
-
-class ReadonlyDict(dict[_T_Key, _T_Val]):
-    """A readonly `dict` subclass.
-
-    Raises:
-        TypeError: on any attempted modification
-    """
-
-    __slots__ = ()
-
-    def not_mutable(self, *a, **kw):
-        raise TypeError(f"readonly type: {self} ")
-
-    __delitem__ = __setitem__ = setdefault = not_mutable
-    clear = pop = popitem = update = __ior__ = not_mutable
-    del not_mutable
-
-    @classmethod
-    def fromkeys(cls, it: abc.Iterable[_T_Key], value: _T_Val = None):
-        return cls((k, value) for k in it)
-
-    def __reduce__(self):
-        return (
-            self.__class__,
-            (dict(self),),
-        )
-
-    def copy(self):
-        return self.__class__(self)
-
-    __copy__ = copy
-
-    def __deepcopy__(self, memo=None):
-        return self.__class__(deepcopy(dict(self), memo))
 
-    __or = dict[_T_Key, _T_Val].__or__
-
-    def __or__(self, o):
-        r = self.__or(o)
-        if r.__class__ is dict:
-            return self.__class__(r)
-        return r
-
-
-class FrozenDict(ReadonlyDict[_T_Key, _T_Val]):
-    """An hashable `ReadonlyDict`"""
-
-    __slots__ = ("_v_hash",)
-
-    def __hash__(self):
-        try:
-            ash = self._v_hash
-        except AttributeError:
-            ash = None
-            items = self._eval_hashable()
-            if items is not None:
-                try:
-                    ash = hash(items)
-                except TypeError:
-                    pass
-            _object_setattr(self, "_v_hash", ash)
-
-        if ash is None:
-            raise TypeError(f"un-hashable type: {self.__class__.__name__!r}")
-
-        return ash
-
-    def _eval_hashable(self) -> abc.Hashable:
-        return (*((k, self[k]) for k in sorted(self)),)
-
-
-
-
-class FrozenAttributeMapping(abc.Mapping[_T_Key, _T_Val]):
+class FrozenNamespaceDict(abc.Mapping[_T_Key, _T_Val]):
     """Provides mapping access to object attributes."""
 
-    __slots__ = '__dict__',
+    __slots__ = ("__dict__", "__weakref__")
+
+    def __init__(self, *args, **kwds) -> None:
+        self.__dict__.update(*args, **kwds)
 
     def __len__(self) -> int:
-        return len(getattr(self, "__dict__", "-"))
+        return len(self.__dict__)
 
     def __contains__(self, o: _T_Key) -> bool:
         return hasattr(self, o)
 
+    # def __dir__(self) -> abc.Iterable[str]:
+    #     return iter(self.__dict__)
+
     def __iter__(self):
         return iter(self.__dict__)
 
     def __json__(self):
-        return dict(self)
+        return vars(self)
 
     def __getitem__(self, k: _T_Key) -> _T_Val:
         try:
             return getattr(self, k)
         except AttributeError:
             return self.__missing__(k)
 
+    def __setattr__(self, name: str, value: Any) -> None:
+        cls = self.__class__
+        raise AttributeError(f"cannot set attribute {name!r} on {cls.__name__!r}")
+
+    def __delattr__(self, name: str) -> None:
+        cls = self.__class__
+        raise AttributeError(f"cannot delete attribute {name!r} on {cls.__name__!r}")
+
     def __missing__(self, key: _T_Key):
         raise KeyError(key)
 
 
-class AttributeMapping(FrozenAttributeMapping[_T_Key, _T_Val], abc.MutableMapping[_T_Key, _T_Val]):
-
+class NamespaceDict(
+    FrozenNamespaceDict[_T_Key, _T_Val], abc.MutableMapping[_T_Key, _T_Val]
+):
     __slots__ = ()
     _pos_args: t.ClassVar[tuple[str]] = ()
 
+    __setattr__ = object.__setattr__
+    __delattr__ = object.__delattr__
+
     def __init__(self, *args, **kwds) -> None:
         (args or kwds) and self.update(*args, **kwds)
 
     def __delitem__(self, k):
         try:
             return delattr(self, k)
         except AttributeError as e:
```

### Comparing `mobilex-0.0.3/pyproject.toml` & `mobilex-0.0.4a0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mobilex"
-version = "0.0.3"
+version = "0.0.4a0"
 description = "USSD and SMS exchange framework"
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/davidkyalo/python-mobilex"
 documentation = "https://davidkyalo.github.io/python-mobilex"
 keywords = [
@@ -20,48 +20,71 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<4.0"
 typing-extensions = "^4.1.1"
 phonenumbers = "^8.12.51"
-redis = "^4.3.4"
-cachetools = {version = "^5.2.0", optional = true}
+redis = "^4.5.5"
 
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.1"
-pytest-asyncio = "^0.18.3"
-pytest-cov = {extras = ["toml"], version = "^3.0.0"}
-pip = "^22.0.4"
-mkdocs = "^1.3.0"
-mkdocs-material = "^8.2.8"
-mike = "^1.1.2"
-black = {version = "^22.3.0", allow-prereleases = true}
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+ipython = "^8.10.0"
+tox = "^4.4.8"
+cachetools = "^5.2.0"
+black = "*"
+
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2.0"
+pytest-asyncio = "^0.20.3"
+pytest-cov = {version = "^4.0.0", extras = ["toml"]}
+tox = "^4.4.8"
+faker = "^18.6.1"
 cachetools = "^5.2.0"
+fakeredis = "^2.12.1"
+
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "*"
+mkdocs-material = "*"
+mike = "*"
+mkdocstrings = "*"
+
+[tool.mypy]
+python_version = "3.10"
+ignore_missing_imports = "True"
 
 
 [tool.pytest.ini_options]
-addopts = "--cov=mobilex --cov-report html --cov-config pyproject.toml"
+addopts = "--showlocals --cov=mobilex --cov-report html --cov-config pyproject.toml"
 asyncio_mode="auto"
+xfail_strict= "True"
 log_level = "DEBUG"
-python_files = "tests.py test_*.py *_test.py *_tests.py"
-python_classes = "*Test *Tests test_* *_test *_tests Test_* *_Test *_Tests"
-python_functions = "*_test test_*"
+python_files = "tests.py test.py test_*.py"
+python_classes = "test_* Test_*"
+python_functions = "test_* test"
+
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
+    "^\\s*pass\\s*$",
+    "^\\s*\\.\\.\\.\\s*$",
     "raise NotImplementedError",
-    "if\\s+([a-zA-Z0-9_]+\\.)?TYPE_CHECKING",
+    "if\\s+([a-zA-Z0-9_]+\\.)?TYPE_CHECKING\\s*:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
 ]
 
-[tool.coverage.run]
-omit = [
-    "*/tests/*",
-    "*/tests.py",
-]
```

### Comparing `mobilex-0.0.3/setup.py` & `mobilex-0.0.4a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,67 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mobilex
+Version: 0.0.4a0
+Summary: USSD and SMS exchange framework
+Home-page: https://github.com/davidkyalo/python-mobilex
+License: MIT
+Keywords: mobilex,mobile,USSD,SMS
+Author: David Kyalo
+Author-email: davidmkyalo@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: phonenumbers (>=8.12.51,<9.0.0)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
+Project-URL: Documentation, https://davidkyalo.github.io/python-mobilex
+Project-URL: Repository, https://github.com/davidkyalo/python-mobilex
+Description-Content-Type: text/markdown
 
-packages = \
-['mobilex',
- 'mobilex.cache',
- 'mobilex.screens',
- 'mobilex.sessions',
- 'mobilex.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['phonenumbers>=8.12.51,<9.0.0',
- 'redis>=4.3.4,<5.0.0',
- 'typing-extensions>=4.1.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'mobilex',
-    'version': '0.0.3',
-    'description': 'USSD and SMS exchange framework',
-    'long_description': '# Python Mobilex\n\n\n[![PyPi version][pypi-image]][pypi-link]\n[![Supported Python versions][pyversions-image]][pyversions-link]\n[![Build status][ci-image]][ci-link]\n[![Coverage status][codecov-image]][codecov-link]\n\n\nA USSD and SMS exchange framework for Python \n\n\n## Installation\n\nInstall from [PyPi](https://pypi.org/project/mobilex/)\n\n```\npip install mobilex\n```\n\n## Documentation\n\nFull documentation is available [here][docs-link].\n\n\n\n## Production\n\n__This package is still in active development and should not be used in production environment__\n\n\n\n\n[docs-link]: https://davidkyalo.github.io/python-mobilex/\n[pypi-image]: https://img.shields.io/pypi/v/mobilex.svg?color=%233d85c6\n[pypi-link]: https://pypi.python.org/pypi/mobilex\n[pyversions-image]: https://img.shields.io/pypi/pyversions/mobilex.svg\n[pyversions-link]: https://pypi.python.org/pypi/mobilex\n[ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main\n[ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster\n[codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg\n[codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex\n\n\nSee this release on GitHub: [v0.0.3](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.3)\n',
-    'author': 'David Kyalo',
-    'author_email': 'davidmkyalo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/davidkyalo/python-mobilex',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+# Python Mobilex
 
 
-setup(**setup_kwargs)
+[![PyPi version][pypi-image]][pypi-link]
+[![Supported Python versions][pyversions-image]][pyversions-link]
+[![Build status][ci-image]][ci-link]
+[![Coverage status][codecov-image]][codecov-link]
+
+
+A USSD and SMS exchange framework for Python 
+
+
+## Installation
+
+Install from [PyPi](https://pypi.org/project/mobilex/)
+
+```
+pip install mobilex
+```
+
+## Documentation
+
+Full documentation is available [here][docs-link].
+
+
+
+## Production
+
+__This package is still in active development and should not be used in production environment__
+
+
+
+
+[docs-link]: https://davidkyalo.github.io/python-mobilex/
+[pypi-image]: https://img.shields.io/pypi/v/mobilex.svg?color=%233d85c6
+[pypi-link]: https://pypi.python.org/pypi/mobilex
+[pyversions-image]: https://img.shields.io/pypi/pyversions/mobilex.svg
+[pyversions-link]: https://pypi.python.org/pypi/mobilex
+[ci-image]: https://github.com/davidkyalo/python-mobilex/actions/workflows/workflow.yaml/badge.svg?event=push&branch=main
+[ci-link]: https://github.com/davidkyalo/python-mobilex/actions?query=workflow%3ACI%2FCD+event%3Apush+branch%3Amaster
+[codecov-image]: https://codecov.io/gh/davidkyalo/python-mobilex/branch/main/graph/badge.svg
+[codecov-link]: https://codecov.io/gh/davidkyalo/python-mobilex
+
+
+See this release on GitHub: [v0.0.4a0](https://github.com/davidkyalo/python-mobilex/releases/tag/0.0.4a0)
+
```

