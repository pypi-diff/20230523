# Comparing `tmp/mocksafe-0.4.0a0.tar.gz` & `tmp/mocksafe-0.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocksafe-0.4.0a0.tar", last modified: Tue May 16 18:35:00 2023, max compression
+gzip compressed data, was "mocksafe-0.4.1a0.tar", last modified: Tue May 23 16:01:24 2023, max compression
```

## Comparing `mocksafe-0.4.0a0.tar` & `mocksafe-0.4.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.295553 mocksafe-0.4.0a0/
--rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.4.0a0/LICENSE
--rw-r--r--   0 danielmayo   (501) staff       (20)     3474 2023-05-16 18:35:00.295278 mocksafe-0.4.0a0/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)      820 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/README.rst
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.285380 mocksafe-0.4.0a0/mocksafe/
--rw-r--r--   0 danielmayo   (501) staff       (20)      400 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/__init__.py
--rw-r--r--   0 danielmayo   (501) staff       (20)      987 2023-05-08 16:37:20.000000 mocksafe-0.4.0a0/mocksafe/call_matchers.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     4198 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/call_type_validator.py
--rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.4.0a0/mocksafe/custom_types.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     5316 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/mock.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     1583 2023-05-14 14:52:32.000000 mocksafe-0.4.0a0/mocksafe/spy.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3162 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/stub.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3981 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/that.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     5504 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/when_then.py
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.294577 mocksafe-0.4.0a0/mocksafe.egg-info/
--rw-r--r--   0 danielmayo   (501) staff       (20)     3474 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/SOURCES.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/dependency_links.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/top_level.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)     1869 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/pyproject.toml
--rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-16 18:35:00.295623 mocksafe-0.4.0a0/setup.cfg
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.294929 mocksafe-0.4.0a0/tests/
--rw-r--r--   0 danielmayo   (501) staff       (20)     6117 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/tests/test_mocksafe.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.440817 mocksafe-0.4.1a0/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.4.1a0/LICENSE
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4777 2023-05-23 16:01:24.440563 mocksafe-0.4.1a0/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)     2123 2023-05-23 15:56:21.000000 mocksafe-0.4.1a0/README.rst
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.430740 mocksafe-0.4.1a0/mocksafe/
+-rw-r--r--   0 danielmayo   (501) staff       (20)      400 2023-05-23 15:56:21.000000 mocksafe-0.4.1a0/mocksafe/__init__.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1165 2023-05-18 16:23:02.000000 mocksafe-0.4.1a0/mocksafe/call_matchers.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6661 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/call_type_validator.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.4.1a0/mocksafe/custom_types.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     5464 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/mock.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1802 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/spy.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3294 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/stub.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4058 2023-05-18 16:23:02.000000 mocksafe-0.4.1a0/mocksafe/that.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6464 2023-05-23 15:54:53.000000 mocksafe-0.4.1a0/mocksafe/when_then.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.439831 mocksafe-0.4.1a0/mocksafe.egg-info/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4777 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/SOURCES.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/dependency_links.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-23 16:01:24.000000 mocksafe-0.4.1a0/mocksafe.egg-info/top_level.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1869 2023-05-23 15:56:21.000000 mocksafe-0.4.1a0/pyproject.toml
+-rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-23 16:01:24.440875 mocksafe-0.4.1a0/setup.cfg
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-23 16:01:24.440194 mocksafe-0.4.1a0/tests/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6118 2023-05-23 10:53:25.000000 mocksafe-0.4.1a0/tests/test_mocksafe.py
```

### Comparing `mocksafe-0.4.0a0/LICENSE` & `mocksafe-0.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mocksafe-0.4.0a0/mocksafe/mock.py` & `mocksafe-0.4.1a0/mocksafe/mock.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 import inspect
 from itertools import count
 from typing import Generic, TypeVar, Optional, Union, Any, cast
-from collections.abc import Callable
 from mocksafe.custom_types import MethodName, CallMatcher, Call
 from mocksafe.spy import MethodSpy
 from mocksafe.stub import MethodStub, ResultsProvider
 from mocksafe.call_matchers import ExactCallMatcher
 
 
 T = TypeVar("T")
@@ -47,119 +46,134 @@
     :meth:`mocksafe.spy`
     """
 
     # Is there a more type safe / proper way to do this?
     return cast(T, SafeMock(class_type, name))
 
 
-def mock_reset(mock_object) -> None:
+def mock_reset(mock_object: Any) -> None:
     if not isinstance(mock_object, SafeMock):
         raise ValueError(f"Not a SafeMocked object: {mock_object}")
     mock_object.reset()
 
 
 def call_equal_to(exact: Call) -> CallMatcher:
     return ExactCallMatcher(exact)
 
 
 class SafeMock(Generic[T]):
-    def __init__(self, class_type: type[T], name: Optional[str] = None):
+    def __init__(self: SafeMock, class_type: type[T], name: Optional[str] = None):
         self._class_type = class_type
         self._mocks: dict[MethodName, MethodMock] = {}
         self._name = name or next(MOCK_NUMBER)
 
     @property
-    def mocked_methods(self) -> dict[MethodName, MethodMock]:
+    def mocked_methods(self: SafeMock) -> dict[MethodName, MethodMock]:
         return self._mocks.copy()
 
+    def reset(self: SafeMock) -> None:
+        for mocked_method in self._mocks.values():
+            mocked_method.reset()
+
     # This is a bit of a hack to fool isinstance checks.
     # Is there a better way?
     @property  # type: ignore
-    def __class__(self):
+    def __class__(self: SafeMock):
         return self._class_type
 
-    def __repr__(self) -> str:
+    def __repr__(self: SafeMock) -> str:
         return f"SafeMock[{self._class_type.__name__}#{self._name}]"
 
-    def __getattr__(self, attr_name: str) -> Union[MethodMock, Any]:
-        if attr_mock := self._mocks.get(attr_name):
-            return attr_mock
-
+    def __getattr__(self: SafeMock, attr_name: str) -> MethodMock:
         if attr_name in getattr(self._class_type, "__attrs__", []):
             # Field attribute defined on the original class
             raise AttributeError(f"{self}.{attr_name} attribute value not set.")
 
+        original_attr = self.get_original_attr(attr_name)
+
+        if isinstance(original_attr, property):
+            raise ValueError(
+                (
+                    "MockSafe doesn't currently support properties, "
+                    f"so {self}.{attr_name} could not be mocked."
+                ),
+            )
+
+        if attr_name not in self._mocks:
+            signature = inspect.signature(original_attr)
+            self._mocks[attr_name] = MethodMock(self._class_type, attr_name, signature)
+
+        return self._mocks[attr_name]
+
+    def get_original_attr(self: SafeMock, attr_name: str) -> Any:
         try:
-            original_method: Callable = getattr(self._class_type, attr_name)
+            return getattr(self._class_type, attr_name)
         except AttributeError as err:
             raise AttributeError(
-                f"{self}.{attr_name} attribute doesn't exist on the "
-                f"original mocked type {self._class_type}."
+                (
+                    f"{self}.{attr_name} attribute doesn't exist on the "
+                    f"original mocked type {self._class_type}."
+                ),
             ) from err
 
-        try:
-            # Try treating it as a property
-            prop = cast(property, original_method)
-            # If it is a property, check it's read-only
-            if prop.fget and not prop.fset and not prop.fdel:
-                # Actually mock the fget (property getter) method
-                # instead of trying to mock the property attribute
-                original_method = cast(MethodMock, prop.fget)
-            else:
-                raise ValueError(
-                    f"MockSafe currently only supports read-only properties, "
-                    f"so the {self}.{attr_name} property could not be mocked."
-                )
-        except AttributeError:
-            # Not actually a property
-            pass
-
-        signature = inspect.signature(original_method)
-        attr_mock = MethodMock(self._class_type, attr_name, signature)
-        self._mocks[attr_name] = attr_mock
-        return attr_mock
-
 
 class MethodMock(Generic[T]):
     def __init__(
-        self, class_type: type[T], name: MethodName, signature: inspect.Signature
+        self: MethodMock,
+        class_type: type[T],
+        name: MethodName,
+        signature: inspect.Signature,
     ):
+        self._stub: MethodStub
+        self._spy: MethodSpy
+
         self._class_type = class_type
-        self._stub: MethodStub = MethodStub(name, signature.return_annotation)
-        self._spy: MethodSpy = MethodSpy(name, self._stub, signature)
+        self._name = name
+        self._signature = signature
+        self.reset()
+
+    def reset(self: MethodMock) -> None:
+        self._stub = MethodStub(self._name, self._signature.return_annotation)
+        self._spy = MethodSpy(self._name, self._stub, self._signature)
 
-    def __call__(self, *args, **kwargs) -> T:
+    def __call__(self: MethodMock, *args, **kwargs) -> T:
         return self._spy(*args, **kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self: MethodMock) -> str:
         return f"MethodMock[{self._stub}]"
 
     @property
-    def full_name(self) -> str:
+    def full_name(self: MethodMock) -> str:
         return f"{self._class_type.__name__}.{self.name}"
 
     @property
-    def name(self) -> MethodName:
+    def name(self: MethodMock) -> MethodName:
         return self._stub.name
 
     def add_stub(
-        self, matcher: CallMatcher, effects: list[Union[T, BaseException]]
+        self: MethodMock,
+        matcher: CallMatcher,
+        effects: list[Union[T, BaseException]],
     ) -> None:
         self._stub.add(matcher, effects)
 
-    def stub_last_call(self, effects: list[Union[T, BaseException]]) -> None:
+    def stub_last_call(
+        self: MethodMock, effects: list[Union[T, BaseException]]
+    ) -> None:
         matcher = call_equal_to(self._spy.pop_call())
         self._stub.add(matcher, effects)
 
-    def custom_result_for_last_call(self, custom: ResultsProvider) -> None:
+    def custom_result_for_last_call(self: MethodMock, custom: ResultsProvider) -> None:
         matcher = call_equal_to(self._spy.pop_call())
         self.custom_result(matcher, custom)
 
-    def custom_result(self, matcher: CallMatcher, custom: ResultsProvider) -> None:
+    def custom_result(
+        self: MethodMock, matcher: CallMatcher, custom: ResultsProvider
+    ) -> None:
         self._stub.add_effect(matcher, custom)
 
     @property
-    def calls(self) -> list[Call]:
+    def calls(self: MethodMock) -> list[Call]:
         return self._spy._calls
 
-    def nth_call(self, n: int) -> Call:
+    def nth_call(self: MethodMock, n: int) -> Call:
         return self._spy.nth_call(n)
```

### Comparing `mocksafe-0.4.0a0/mocksafe/spy.py` & `mocksafe-0.4.1a0/mocksafe/spy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,64 @@
+from __future__ import annotations
 from inspect import Signature
 from typing import Generic, TypeVar
 from collections.abc import Callable
 from mocksafe.custom_types import MethodName, Call
 from mocksafe.call_type_validator import CallTypeValidator
 
 
 T = TypeVar("T")
 
 
 class MethodSpy(Generic[T]):
     def __init__(
-        self, name: MethodName, delegate: Callable[..., T], signature: Signature
+        self: MethodSpy,
+        name: MethodName,
+        delegate: Callable[..., T],
+        signature: Signature,
     ):
         self._name = name
         self._delegate = delegate
         self._calls: list[Call] = []
         self._signature = signature
 
-    def __call__(self, *args, **kwargs) -> T:
+    def __call__(self: MethodSpy, *args, **kwargs) -> T:
         validator = CallTypeValidator(
-            self._name, self._signature.parameters, args, kwargs
+            self._name,
+            self._signature.parameters,
+            args,
+            kwargs,
         )
         validator.validate()
 
         self._calls.append((tuple(args), kwargs.copy()))
 
         return self._delegate(*args, **kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self: MethodSpy) -> str:
         return f"MethodSpy[{self._name}:{len(self.calls)} call(s)]"
 
     @property
-    def name(self) -> MethodName:
+    def name(self: MethodSpy) -> MethodName:
         return self._name
 
     @property
-    def calls(self) -> list[Call]:
+    def calls(self: MethodSpy) -> list[Call]:
         return self._calls
 
-    def pop_call(self) -> Call:
+    def pop_call(self: MethodSpy) -> Call:
         return self._calls.pop()
 
     # pylint: disable=raise-missing-from
-    def nth_call(self, n: int) -> Call:
+    def nth_call(self: MethodSpy, n: int) -> Call:
         try:
             return self._calls[n]
         except IndexError:
             if not self._calls:
                 raise ValueError(f"The mocked method {self._name}() was not called.")
 
             raise ValueError(
-                f"Mocked method {self._name}() was not called {n+1} time(s). "
-                f"The actual number of calls was {len(self.calls)}."
+                (
+                    f"Mocked method {self._name}() was not called {n+1} time(s). "
+                    f"The actual number of calls was {len(self.calls)}."
+                ),
             )
```

### Comparing `mocksafe-0.4.0a0/mocksafe/stub.py` & `mocksafe-0.4.1a0/mocksafe/stub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from inspect import Signature, isclass
 from typing import Generic, TypeVar, Optional, Union
 from collections.abc import Callable
 from mocksafe.custom_types import MethodName, CallMatcher
 from mocksafe.call_type_validator import type_match
 
 
@@ -10,85 +11,93 @@
 
 
 # Stub default values for these simple built-in types
 PRIMITIVES = [str, int, bool, float, dict, list, tuple, set]
 
 
 class MethodStub(Generic[T]):
-    def __init__(self, name: MethodName, result_type: type):
+    def __init__(self: MethodStub, name: MethodName, result_type: type):
         self._name = name
         self._stubs: list[tuple[CallMatcher, ResultsProvider]] = []
         self._result_type = result_type
 
-    def __call__(self, *args, **kwargs) -> Optional[T]:
+    def __call__(self: MethodStub, *args, **kwargs) -> Optional[T]:
         call = (tuple(args), kwargs)
         for matcher, results in self._stubs:
             if matcher(call):
                 return results(*args, **kwargs)
 
         # No default return value has been stubbed, try to determine
         # something sensible to return
 
         default_value: Optional[T]
         result_type: type = self._result_type
 
-        if result_type == type(None):
-            default_value = None  # type: ignore
-        elif result_type == Signature.empty:
-            # There are no type annotations to infer type from.
-            # Fall back to None.
-            default_value = None
-        elif not isclass(result_type):
-            default_value = None
-        elif any(issubclass(result_type, p) for p in PRIMITIVES):
+        primitive_result_type = isclass(result_type) and any(
+            issubclass(result_type, p) for p in PRIMITIVES
+        )
+
+        if primitive_result_type:
             default_value = result_type()
+        else:
+            default_value = None
 
         return default_value
 
-    def __repr__(self) -> str:
+    def __repr__(self: MethodStub) -> str:
         reps = []
         for matcher, results in self._stubs:
             reps.append(f"{matcher} -> {results}")
         return "; ".join(reps)
 
     @property
-    def name(self) -> MethodName:
+    def name(self: MethodStub) -> MethodName:
         return self._name
 
-    def add(self, matcher: CallMatcher, effects: list[Union[T, BaseException]]) -> None:
+    def add(
+        self: MethodStub, matcher: CallMatcher, effects: list[Union[T, BaseException]]
+    ) -> None:
         self._validate_effects(effects)
         self.add_effect(matcher, CannedEffects(effects))
 
-    def add_effect(self, matcher: CallMatcher, effect: ResultsProvider) -> None:
+    def add_effect(
+        self: MethodStub, matcher: CallMatcher, effect: ResultsProvider
+    ) -> None:
         self._stubs.insert(0, (matcher, effect))
 
-    def _validate_effects(self, effects: list[Union[T, BaseException]]):
+    def _validate_effects(
+        self: MethodStub, effects: list[Union[T, BaseException]]
+    ) -> None:
         # Runtime check in case static type checking allows an incompatible type
         # to slip through
         if self._result_type == Signature.empty:
             return  # Nothing we can check
 
         for e in effects:
             if isinstance(e, BaseException):
                 continue
             if not type_match(e, self._result_type):
                 raise TypeError(
-                    f"Cannot use stub result {e} ({type(e)}) with the mocked method {self._name}(), the expected return type is: {self._result_type}."
+                    (
+                        f"Cannot use stub result {e} ({type(e)}) with the mocked method"
+                        f" {self._name}(), the expected return type is:"
+                        f" {self._result_type}."
+                    ),
                 )
 
 
 class CannedEffects(Generic[T]):
-    def __init__(self, effects: list[T]):
+    def __init__(self: CannedEffects, effects: list[T]):
         self._effects = effects
 
-    def __call__(self, *args, **kwargs) -> T:
+    def __call__(self: CannedEffects, *args, **kwargs) -> T:
         if len(self._effects) == 1:
             effect = self._effects[0]
         else:
             effect = self._effects.pop(0)
 
         if isinstance(effect, BaseException):
             raise effect
         return effect
 
-    def __repr__(self) -> str:
+    def __repr__(self: CannedEffects) -> str:
         return str(self._effects[0])
```

### Comparing `mocksafe-0.4.0a0/mocksafe/that.py` & `mocksafe-0.4.1a0/mocksafe/that.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,41 +100,41 @@
         5
         >>> mock_random.randint(10, 20)
         13
         >>> assert that(mock_random.randint).last_call == (10, 20)
         >>> assert that(mock_random.randint).nth_call(0) == ((), {"a":1, "b":10})
     """
 
-    def __init__(self, method_mock: MethodMock):
+    def __init__(self: MockCalls, method_mock: MethodMock):
         self._method_mock = method_mock
 
-    def __repr__(self) -> str:
+    def __repr__(self: MockCalls) -> str:
         return f"MockCalls[{self._method_mock.name}();num_calls={self.num_calls}]"
 
     @property
-    def was_called(self) -> bool:
+    def was_called(self: MockCalls) -> bool:
         """Return whether the mocked method was called at least once."""
         return self.num_calls > 0
 
     @property
-    def was_not_called(self) -> bool:
+    def was_not_called(self: MockCalls) -> bool:
         """Return whether the mocked method was not called."""
         return not self.was_called
 
     @property
-    def num_calls(self) -> int:
+    def num_calls(self: MockCalls) -> int:
         """Returns the number of calls made to the mocked method."""
         return len(self._method_mock.calls)
 
     @property
-    def last_call(self) -> Union[Args, Call]:
+    def last_call(self: MockCalls) -> Union[Args, Call]:
         """Returns details of the last call made to the mocked method."""
         return self.nth_call(-1)
 
-    def nth_call(self, n: int) -> Union[Args, Call]:
+    def nth_call(self: MockCalls, n: int) -> Union[Args, Call]:
         """Returns details of the Nth call made to the mocked method."""
         call = self._method_mock.nth_call(n)
 
         args, kwargs = call
 
         if kwargs:
             return call
```

### Comparing `mocksafe-0.4.0a0/mocksafe/when_then.py` & `mocksafe-0.4.1a0/mocksafe/when_then.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,62 +21,76 @@
         >>> when(mock_random.random)
         <mocksafe.when_then.WhenStubber object at 0x...>
 
     :Example:
         >>> when(mock_random.random).any_call().then_return(0.31)
     """
     if not isinstance(mock_method, MethodMock):
-        raise ValueError("Not a SafeMocked method: mock_method")
+        raise ValueError(
+            f"Not a SafeMocked method: {mock_method} ({type(mock_method)})"
+        )
     return WhenStubber(mock_method)
 
 
 class WhenStubber(Generic[T]):
     """
     Set up conditions for when a stub is to be used.
 
     :Example:
         >>> when(mock_random.random).any_call().then_return(0.31)
 
     See: :class:`mocksafe.MatchCallStubber`
 
     :Example:
-        >>> when(mock_random.randint).called_with(mock_random.randint(1, 10)).then_return(7)
+        >>> when(
+        ...     mock_random.randint
+        ... ).called_with(
+        ...     mock_random.randint(1, 10)
+        ... ).then_return(7)
+
         >>> mock_random.randint(1, 10)
         7
 
     See: :class:`mocksafe.LastCallStubber`
 
     :Example:
-        >>> when(mock_random.randint).call_matching(lambda a, b: a <= 3 and b > 3).then_return(3)
+        >>> when(
+        ...     mock_random.randint
+        ... ).call_matching(
+        ...     lambda a, b: a <= 3 and b > 3
+        ... ).then_return(3)
+
         >>> mock_random.randint(2, 6)
         3
 
     See: :class:`mocksafe.MatchCallStubber`
     """
 
-    def __init__(self, method_mock: MethodMock[T]):
+    def __init__(self: WhenStubber, method_mock: MethodMock[T]):
         self._method_mock = method_mock
 
-    def any_call(self) -> MatchCallStubber[T]:
+    def any_call(self: WhenStubber) -> MatchCallStubber[T]:
         """
         Matches any calls made to the mocked method.
 
         :rtype: MatchCallStubber[T]
         """
         return MatchCallStubber(self._method_mock, matcher=ANY_CALL)
 
-    def called_with(self, _: T) -> LastCallStubber[T]:
+    def called_with(self: WhenStubber, _: T) -> LastCallStubber[T]:
         """
         Matches specific calls made to the mocked method.
 
         :rtype: LastCallStubber[T]
         """
         return LastCallStubber(self._method_mock)
 
-    def call_matching(self, call_lambda: Callable[..., bool]) -> MatchCallStubber[T]:
+    def call_matching(
+        self: WhenStubber, call_lambda: Callable[..., bool]
+    ) -> MatchCallStubber[T]:
         """
         Use a lambda to determine whether to match a call.
 
         :rtype: MatchCallStubber[T]
         """
         return MatchCallStubber(self._method_mock, CustomCallMatcher(call_lambda))
 
@@ -95,79 +109,118 @@
     :Example:
         >>> when(mock_random.random).any_call().then_raise(ValueError("..."))
 
     :Example:
         >>> when(mock_random.randint).any_call().then(lambda a, b: int((b - a) / 2))
 
     :Example:
-        >>> when(mock_random.randint).any_call().use_side_effects(1, 2, 3, ValueError("..."), 4)
+        >>> when(
+        ...     mock_random.randint
+        ... ).any_call().use_side_effects(
+        ...     1, 2, 3, ValueError("..."), 4
+        ... )
+
     """
 
-    def __init__(self, method_mock: MethodMock[T], matcher: CallMatcher):
+    def __init__(
+        self: MatchCallStubber, method_mock: MethodMock[T], matcher: CallMatcher
+    ):
         self._method_mock = method_mock
         self._matcher = matcher
 
-    def then_return(self, result: T, *consecutive_results: T) -> None:
+    def then_return(self: MatchCallStubber, result: T, *consecutive_results: T) -> None:
         """
         Set one or more results to be returned by the method stub.
         """
         self.use_side_effects(result, *consecutive_results)
 
-    def then_raise(self, error: BaseException) -> None:
+    def then_raise(self: MatchCallStubber, error: BaseException) -> None:
         """
         Raise an exception.
         """
         self.use_side_effects(error)
 
-    def then(self, result: ResultsProvider) -> None:
+    def then(self: MatchCallStubber, result: ResultsProvider) -> None:
         """
         Use a custom lambda to produce stubbed results.
         """
         self._method_mock.custom_result(self._matcher, result)
 
-    def use_side_effects(self, *side_effects: Union[T, BaseException]) -> None:
+    def use_side_effects(
+        self: MatchCallStubber, *side_effects: Union[T, BaseException]
+    ) -> None:
         """
         Specify an ordered sequence of results and/or exceptions to be returned/raised.
         """
         self._method_mock.add_stub(self._matcher, list(side_effects))
 
 
 class LastCallStubber(Generic[T]):
     """
     Set up results or side effects to be used when for the stub the
     condition matches.
 
     :Example:
-        >>> when(mock_random.randint).called_with(mock_random.randint(1, 2)).then_return(0.31)
-
-    :Example:
-        >>> when(mock_random.randint).called_with(mock_random.randint(3, 4)).then_return(0.1, 0.3, 0.2)
-
-    :Example:
-        >>> when(mock_random.randint).called_with(mock_random.randint(5, 6)).then_raise(ValueError("..."))
-
-    :Example:
-        >>> when(mock_random.randint).called_with(mock_random.randint(7, 8)).then(lambda a, b: int((b - a) / 2))
-
-    :Example:
-        >>> when(mock_random.randint).called_with(mock_random.randint(9, 10)).use_side_effects(1, 2, 3, ValueError("..."), 4)
+        >>> when(
+        ...     mock_random.randint
+        ... ).called_with(
+        ...     mock_random.randint(1, 2)
+        ... ).then_return(0.31)
+
+    :Example:
+        >>> when(
+        ...     mock_random.randint
+        ... ).called_with(
+        ...     mock_random.randint(3, 4)
+        ... ).then_return(0.1, 0.3, 0.2)
+
+    :Example:
+        >>> when(
+        ...     mock_random.randint
+        ... ).called_with(
+        ...     mock_random.randint(5, 6)
+        ... ).then_raise(ValueError("..."))
+
+    :Example:
+        >>> when(
+        ...     mock_random.randint
+        ... ).called_with(
+        ...     mock_random.randint(7, 8)
+        ... ).then(
+        ...     lambda a, b: int((b - a) / 2)
+        ... )
+
+    :Example:
+        >>> when(
+        ...     mock_random.randint
+        ... ).called_with(
+        ...     mock_random.randint(9, 10)
+        ... ).use_side_effects(
+        ...     1, 2, 3, ValueError("..."), 4
+        ... )
     """
 
-    def __init__(self, method_mock: MethodMock[T]):
+    def __init__(self: LastCallStubber, method_mock: MethodMock[T]):
         self._method_mock = method_mock
 
-    def then_return(self, result: T, *consecutive_results: T) -> None:
+    def then_return(self: LastCallStubber, result: T, *consecutive_results: T) -> None:
         self.use_side_effects(result, *consecutive_results)
 
-    def then_raise(self, error: BaseException) -> None:
+    def then_raise(self: LastCallStubber, error: BaseException) -> None:
         self.use_side_effects(error)
 
-    def then(self, result: ResultsProvider) -> None:
+    def then(self: LastCallStubber, result: ResultsProvider) -> None:
         self._method_mock.custom_result_for_last_call(result)
 
-    def use_side_effects(self, *side_effects: Union[T, BaseException]) -> None:
+    def use_side_effects(
+        self: LastCallStubber, *side_effects: Union[T, BaseException]
+    ) -> None:
         if not self._method_mock.calls:
             raise ValueError(
-                f"Mocked methods do not match: when({self._method_mock.full_name}).called_with(<different_method>)"
+                (
+                    "Mocked methods do not match: "
+                    f"when({self._method_mock.full_name})"
+                    ".called_with(<different_method>)"
+                ),
             )
 
         self._method_mock.stub_last_call(list(side_effects))
```

### Comparing `mocksafe-0.4.0a0/pyproject.toml` & `mocksafe-0.4.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mocksafe"
-version = "0.4.0-alpha"
+version = "0.4.1-alpha"
 
 description = "A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code."
 
 requires-python = ">= 3.9"
 readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
@@ -36,15 +36,15 @@
 Source = "https://github.com/dmayo3/mocksafe"
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [tool.bumpver]
-current_version = "0.4.0-alpha"
+current_version = "0.4.1-alpha"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mocksafe-0.4.0a0/tests/test_mocksafe.py` & `mocksafe-0.4.1a0/tests/test_mocksafe.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     assert mock_object.foo("d", 3) == 0
 
 
 def test_stub_call_with_raises_error():
     mock_object: MyClass = mock(MyClass)
 
     when(mock_object.foo).called_with(mock_object.foo("bad")).then_raise(
-        ValueError("Invalid argument")
+        ValueError("Invalid argument"),
     )
 
     mock_object.foo("good")
 
     with pytest.raises(ValueError):
         mock_object.foo("bad")
```

