# Comparing `tmp/typing_extensions-4.5.0.tar.gz` & `tmp/typing_extensions-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_extensions-4.5.0.tar", last modified: Wed Feb 15 00:16:48 2023, max compression
+gzip compressed data, was "typing_extensions-4.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typing_extensions-4.5.0.tar` & `typing_extensions-4.6.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     4861 2023-02-15 00:16:30.774229 typing_extensions-4.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.5.0/LICENSE
--rw-r--r--   0        0        0     7044 2023-02-15 00:13:43.618730 typing_extensions-4.5.0/README.md
--rw-r--r--   0        0        0     1894 2023-02-15 00:16:30.774688 typing_extensions-4.5.0/pyproject.toml
--rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.5.0/src/_typed_dict_test_helper.py
--rw-r--r--   0        0        0   124478 2023-02-15 00:13:43.620018 typing_extensions-4.5.0/src/test_typing_extensions.py
--rw-r--r--   0        0        0    84065 2023-02-15 00:13:43.620782 typing_extensions-4.5.0/src/typing_extensions.py
--rw-r--r--   0        0        0     8529 1970-01-01 00:00:00.000000 typing_extensions-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10106 2023-05-23 00:07:02.454501 typing_extensions-4.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.6.0/LICENSE
+-rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.0/README.md
+-rw-r--r--   0        0        0     1916 2023-05-23 00:07:02.456585 typing_extensions-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.6.0/src/_typed_dict_test_helper.py
+-rw-r--r--   0        0        0   165606 2023-05-22 14:09:42.548954 typing_extensions-4.6.0/src/test_typing_extensions.py
+-rw-r--r--   0        0        0   102170 2023-05-23 00:00:42.513644 typing_extensions-4.6.0/src/typing_extensions.py
+-rw-r--r--   0        0        0      135 2023-05-22 00:37:39.060665 typing_extensions-4.6.0/tox.ini
+-rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.0/PKG-INFO
```

### Comparing `typing_extensions-4.5.0/LICENSE` & `typing_extensions-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.5.0/pyproject.toml` & `typing_extensions-4.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "typing_extensions"
-version = "4.5.0"
+version = "4.6.0"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = [
     "annotations",
     "backport",
@@ -42,20 +42,20 @@
     "Topic :: Software Development",
 ]
 
 [project.urls]
 Home = "https://github.com/python/typing_extensions"
 Repository = "https://github.com/python/typing_extensions"
 Changes = "https://github.com/python/typing_extensions/blob/main/CHANGELOG.md"
-Documentation = "https://typing.readthedocs.io/"
+Documentation = "https://typing-extensions.readthedocs.io/"
 "Bug Tracker" = "https://github.com/python/typing_extensions/issues"
 "Q & A" = "https://github.com/python/typing/discussions"
 
 # Project metadata -- authors. Flit stores this as a list of dicts, so it can't
 # be inline above.
 [[project.authors]]
 name = "Guido van Rossum, Jukka Lehtosalo, Łukasz Langa, Michael Lee"
 email = "levkivskyi@gmail.com"
 
 [tool.flit.sdist]
-include = ["CHANGELOG.md", "README.md", "*/*test*.py"]
+include = ["CHANGELOG.md", "README.md", "tox.ini", "*/*test*.py"]
 exclude = []
```

### Comparing `typing_extensions-4.5.0/src/test_typing_extensions.py` & `typing_extensions-4.6.0/src/test_typing_extensions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,170 @@
 import sys
 import os
 import abc
+import io
 import contextlib
 import collections
 from collections import defaultdict
 import collections.abc
 import copy
 from functools import lru_cache
+import importlib
 import inspect
 import pickle
+import re
 import subprocess
+import tempfile
+import textwrap
 import types
+from pathlib import Path
 from unittest import TestCase, main, skipUnless, skipIf
 from unittest.mock import patch
-from test import ann_module, ann_module2, ann_module3
 import typing
-from typing import TypeVar, Optional, Union, AnyStr
+from typing import Optional, Union, AnyStr
 from typing import T, KT, VT  # Not in __all__.
-from typing import Tuple, List, Dict, Iterable, Iterator, Callable
+from typing import Tuple, List, Set, Dict, Iterable, Iterator, Callable
 from typing import Generic
 from typing import no_type_check
+import warnings
+
 import typing_extensions
 from typing_extensions import NoReturn, Any, ClassVar, Final, IntVar, Literal, Type, NewType, TypedDict, Self
 from typing_extensions import TypeAlias, ParamSpec, Concatenate, ParamSpecArgs, ParamSpecKwargs, TypeGuard
 from typing_extensions import Awaitable, AsyncIterator, AsyncContextManager, Required, NotRequired
 from typing_extensions import Protocol, runtime, runtime_checkable, Annotated, final, is_typeddict
 from typing_extensions import TypeVarTuple, Unpack, dataclass_transform, reveal_type, Never, assert_never, LiteralString
-from typing_extensions import assert_type, get_type_hints, get_origin, get_args
+from typing_extensions import assert_type, get_type_hints, get_origin, get_args, get_original_bases
 from typing_extensions import clear_overloads, get_overloads, overload
 from typing_extensions import NamedTuple
-from typing_extensions import override, deprecated
+from typing_extensions import override, deprecated, Buffer, TypeAliasType, TypeVar
 from _typed_dict_test_helper import Foo, FooGeneric
-import warnings
 
 # Flags used to mark tests that only apply after a specific
 # version of the typing module.
 TYPING_3_8_0 = sys.version_info[:3] >= (3, 8, 0)
 TYPING_3_9_0 = sys.version_info[:3] >= (3, 9, 0)
 TYPING_3_10_0 = sys.version_info[:3] >= (3, 10, 0)
 
 # 3.11 makes runtime type checks (_type_check) more lenient.
 TYPING_3_11_0 = sys.version_info[:3] >= (3, 11, 0)
 
+# 3.12 changes the representation of Unpack[] (PEP 692)
+TYPING_3_12_0 = sys.version_info[:3] >= (3, 12, 0)
+
 # https://github.com/python/cpython/pull/27017 was backported into some 3.9 and 3.10
 # versions, but not all
 HAS_FORWARD_MODULE = "module" in inspect.signature(typing._type_check).parameters
 
+ANN_MODULE_SOURCE = '''\
+from typing import Optional
+from functools import wraps
+
+__annotations__[1] = 2
+
+class C:
+
+    x = 5; y: Optional['C'] = None
+
+from typing import Tuple
+x: int = 5; y: str = x; f: Tuple[int, int]
+
+class M(type):
+
+    __annotations__['123'] = 123
+    o: type = object
+
+(pars): bool = True
+
+class D(C):
+    j: str = 'hi'; k: str= 'bye'
+
+from types import new_class
+h_class = new_class('H', (C,))
+j_class = new_class('J')
+
+class F():
+    z: int = 5
+    def __init__(self, x):
+        pass
+
+class Y(F):
+    def __init__(self):
+        super(F, self).__init__(123)
+
+class Meta(type):
+    def __new__(meta, name, bases, namespace):
+        return super().__new__(meta, name, bases, namespace)
+
+class S(metaclass = Meta):
+    x: str = 'something'
+    y: str = 'something else'
+
+def foo(x: int = 10):
+    def bar(y: List[str]):
+        x: str = 'yes'
+    bar()
+
+def dec(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+    return wrapper
+'''
+
+ANN_MODULE_2_SOURCE = '''\
+from typing import no_type_check, ClassVar
+
+i: int = 1
+j: int
+x: float = i/10
+
+def f():
+    class C: ...
+    return C()
+
+f().new_attr: object = object()
+
+class C:
+    def __init__(self, x: int) -> None:
+        self.x = x
+
+c = C(5)
+c.new_attr: int = 10
+
+__annotations__ = {}
+
+
+@no_type_check
+class NTC:
+    def meth(self, param: complex) -> None:
+        ...
+
+class CV:
+    var: ClassVar['CV']
+
+CV.var = CV()
+'''
+
+ANN_MODULE_3_SOURCE = '''\
+def f_bad_ann():
+    __annotations__[1] = 2
+
+class C_OK:
+    def __init__(self, x: int) -> None:
+        self.x: no_such_name = x  # This one is OK as proposed by Guido
+
+class D_bad_ann:
+    def __init__(self, x: int) -> None:
+        sfel.y: int = 0
+
+def g_bad_ann():
+    no_such_name.attr: int = 0
+'''
+
 
 class BaseTestCase(TestCase):
     def assertIsSubclass(self, cls, class_or_tuple, msg=None):
         if not issubclass(cls, class_or_tuple):
             message = f'{cls!r} is not a subclass of {repr(class_or_tuple)}'
             if msg is not None:
                 message += f' : {msg}'
@@ -234,16 +349,17 @@
     def test_class(self):
         @deprecated("A will go away soon")
         class A:
             pass
 
         with self.assertWarnsRegex(DeprecationWarning, "A will go away soon"):
             A()
-        with self.assertRaises(TypeError):
-            A(42)
+        with self.assertWarnsRegex(DeprecationWarning, "A will go away soon"):
+            with self.assertRaises(TypeError):
+                A(42)
 
         @deprecated("HasInit will go away soon")
         class HasInit:
             def __init__(self, x):
                 self.x = x
 
         with self.assertWarnsRegex(DeprecationWarning, "HasInit will go away soon"):
@@ -371,16 +487,21 @@
 
     def test_repr(self):
         if sys.version_info >= (3, 11):
             mod_name = 'typing'
         else:
             mod_name = 'typing_extensions'
         self.assertEqual(repr(Any), f"{mod_name}.Any")
-        if sys.version_info < (3, 11):  # skip for now on 3.11+ see python/cpython#95987
-            self.assertEqual(repr(self.SubclassesAny), "<class 'test_typing_extensions.AnyTests.SubclassesAny'>")
+
+    @skipIf(sys.version_info[:3] == (3, 11, 0), "A bug was fixed in 3.11.1")
+    def test_repr_on_Any_subclass(self):
+        self.assertEqual(
+            repr(self.SubclassesAny),
+            f"<class '{self.SubclassesAny.__module__}.AnyTests.SubclassesAny'>"
+        )
 
     def test_instantiation(self):
         with self.assertRaises(TypeError):
             Any()
 
         self.SubclassesAny()
 
@@ -569,32 +690,39 @@
             isinstance(1, NotRequired[int])
         with self.assertRaises(TypeError):
             issubclass(int, NotRequired)
 
 
 class IntVarTests(BaseTestCase):
     def test_valid(self):
-        T_ints = IntVar("T_ints")  # noqa
+        T_ints = IntVar("T_ints")
 
     def test_invalid(self):
         with self.assertRaises(TypeError):
             T_ints = IntVar("T_ints", int)
         with self.assertRaises(TypeError):
             T_ints = IntVar("T_ints", bound=int)
         with self.assertRaises(TypeError):
-            T_ints = IntVar("T_ints", covariant=True)  # noqa
+            T_ints = IntVar("T_ints", covariant=True)
 
 
 class LiteralTests(BaseTestCase):
     def test_basics(self):
         Literal[1]
         Literal[1, 2, 3]
         Literal["x", "y", "z"]
         Literal[None]
 
+    def test_enum(self):
+        import enum
+        class My(enum.Enum):
+            A = 'A'
+
+        self.assertEqual(Literal[My.A].__args__, (My.A,))
+
     def test_illegal_parameters_do_not_raise_runtime_errors(self):
         # Type checkers should reject these types, but we do not
         # raise errors at runtime to maintain maximum flexibility
         Literal[int]
         Literal[Literal[1, 2], Literal[4, 5]]
         Literal[3j + 2, ..., ()]
         Literal[b"foo", u"bar"]
@@ -602,23 +730,25 @@
         Literal[T]
 
     def test_literals_inside_other_types(self):
         List[Literal[1, 2, 3]]
         List[Literal[("foo", "bar", "baz")]]
 
     def test_repr(self):
-        if hasattr(typing, 'Literal'):
+        # we backport various bugfixes that were added in 3.10.1 and earlier
+        if sys.version_info >= (3, 10, 1):
             mod_name = 'typing'
         else:
             mod_name = 'typing_extensions'
         self.assertEqual(repr(Literal[1]), mod_name + ".Literal[1]")
         self.assertEqual(repr(Literal[1, True, "foo"]), mod_name + ".Literal[1, True, 'foo']")
         self.assertEqual(repr(Literal[int]), mod_name + ".Literal[int]")
         self.assertEqual(repr(Literal), mod_name + ".Literal")
         self.assertEqual(repr(Literal[None]), mod_name + ".Literal[None]")
+        self.assertEqual(repr(Literal[1, 2, 3, 3]), mod_name + ".Literal[1, 2, 3]")
 
     def test_cannot_init(self):
         with self.assertRaises(TypeError):
             Literal()
         with self.assertRaises(TypeError):
             Literal[1]()
         with self.assertRaises(TypeError):
@@ -642,14 +772,121 @@
         with self.assertRaises(TypeError):
             class Bar(Literal): pass
 
     def test_no_multiple_subscripts(self):
         with self.assertRaises(TypeError):
             Literal[1][1]
 
+    def test_equal(self):
+        self.assertNotEqual(Literal[0], Literal[False])
+        self.assertNotEqual(Literal[True], Literal[1])
+        self.assertNotEqual(Literal[1], Literal[2])
+        self.assertNotEqual(Literal[1, True], Literal[1])
+        self.assertNotEqual(Literal[1, True], Literal[1, 1])
+        self.assertNotEqual(Literal[1, 2], Literal[True, 2])
+        self.assertEqual(Literal[1], Literal[1])
+        self.assertEqual(Literal[1, 2], Literal[2, 1])
+        self.assertEqual(Literal[1, 2, 3], Literal[1, 2, 3, 3])
+
+    def test_hash(self):
+        self.assertEqual(hash(Literal[1]), hash(Literal[1]))
+        self.assertEqual(hash(Literal[1, 2]), hash(Literal[2, 1]))
+        self.assertEqual(hash(Literal[1, 2, 3]), hash(Literal[1, 2, 3, 3]))
+
+    def test_args(self):
+        self.assertEqual(Literal[1, 2, 3].__args__, (1, 2, 3))
+        self.assertEqual(Literal[1, 2, 3, 3].__args__, (1, 2, 3))
+        self.assertEqual(Literal[1, Literal[2], Literal[3, 4]].__args__, (1, 2, 3, 4))
+        # Mutable arguments will not be deduplicated
+        self.assertEqual(Literal[[], []].__args__, ([], []))
+
+    def test_union_of_literals(self):
+        self.assertEqual(Union[Literal[1], Literal[2]].__args__,
+                         (Literal[1], Literal[2]))
+        self.assertEqual(Union[Literal[1], Literal[1]],
+                         Literal[1])
+
+        self.assertEqual(Union[Literal[False], Literal[0]].__args__,
+                         (Literal[False], Literal[0]))
+        self.assertEqual(Union[Literal[True], Literal[1]].__args__,
+                         (Literal[True], Literal[1]))
+
+        import enum
+        class Ints(enum.IntEnum):
+            A = 0
+            B = 1
+
+        self.assertEqual(Union[Literal[Ints.A], Literal[Ints.B]].__args__,
+                         (Literal[Ints.A], Literal[Ints.B]))
+
+        self.assertEqual(Union[Literal[Ints.A], Literal[Ints.A]],
+                         Literal[Ints.A])
+        self.assertEqual(Union[Literal[Ints.B], Literal[Ints.B]],
+                         Literal[Ints.B])
+
+        self.assertEqual(Union[Literal[0], Literal[Ints.A], Literal[False]].__args__,
+                         (Literal[0], Literal[Ints.A], Literal[False]))
+        self.assertEqual(Union[Literal[1], Literal[Ints.B], Literal[True]].__args__,
+                         (Literal[1], Literal[Ints.B], Literal[True]))
+
+    @skipUnless(TYPING_3_10_0, "Python 3.10+ required")
+    def test_or_type_operator_with_Literal(self):
+        self.assertEqual((Literal[1] | Literal[2]).__args__,
+                         (Literal[1], Literal[2]))
+
+        self.assertEqual((Literal[0] | Literal[False]).__args__,
+                         (Literal[0], Literal[False]))
+        self.assertEqual((Literal[1] | Literal[True]).__args__,
+                         (Literal[1], Literal[True]))
+
+        self.assertEqual(Literal[1] | Literal[1], Literal[1])
+        self.assertEqual(Literal['a'] | Literal['a'], Literal['a'])
+
+        import enum
+        class Ints(enum.IntEnum):
+            A = 0
+            B = 1
+
+        self.assertEqual(Literal[Ints.A] | Literal[Ints.A], Literal[Ints.A])
+        self.assertEqual(Literal[Ints.B] | Literal[Ints.B], Literal[Ints.B])
+
+        self.assertEqual((Literal[Ints.B] | Literal[Ints.A]).__args__,
+                         (Literal[Ints.B], Literal[Ints.A]))
+
+        self.assertEqual((Literal[0] | Literal[Ints.A]).__args__,
+                         (Literal[0], Literal[Ints.A]))
+        self.assertEqual((Literal[1] | Literal[Ints.B]).__args__,
+                         (Literal[1], Literal[Ints.B]))
+
+    def test_flatten(self):
+        l1 = Literal[Literal[1], Literal[2], Literal[3]]
+        l2 = Literal[Literal[1, 2], 3]
+        l3 = Literal[Literal[1, 2, 3]]
+        for lit in l1, l2, l3:
+            self.assertEqual(lit, Literal[1, 2, 3])
+            self.assertEqual(lit.__args__, (1, 2, 3))
+
+    def test_does_not_flatten_enum(self):
+        import enum
+        class Ints(enum.IntEnum):
+            A = 1
+            B = 2
+
+        literal = Literal[
+            Literal[Ints.A],
+            Literal[Ints.B],
+            Literal[1],
+            Literal[2],
+        ]
+        self.assertEqual(literal.__args__, (Ints.A, Ints.B, 1, 2))
+
+    def test_caching_of_Literal_respects_type(self):
+        self.assertIs(type(Literal[1].__args__[0]), int)
+        self.assertIs(type(Literal[True].__args__[0]), bool)
+
 
 class MethodHolder:
     @classmethod
     def clsmethod(cls): ...
     @staticmethod
     def stmethod(): ...
     def method(self): ...
@@ -837,15 +1074,15 @@
 
     def __str__(self):
         return f'{self.x} -> {self.y}'
 
     def __add__(self, other):
         return 0
 
-@runtime
+@runtime_checkable
 class HasCallProtocol(Protocol):
     __call__: typing.Callable
 
 
 async def g_with(am: AsyncContextManager[int]):
     x: int
     async with am as x:
@@ -894,56 +1131,70 @@
     year: NotRequired[Annotated[int, 2000]]
 
 
 gth = get_type_hints
 
 
 class GetTypeHintTests(BaseTestCase):
+    @classmethod
+    def setUpClass(cls):
+        with tempfile.TemporaryDirectory() as tempdir:
+            sys.path.append(tempdir)
+            Path(tempdir, "ann_module.py").write_text(ANN_MODULE_SOURCE)
+            Path(tempdir, "ann_module2.py").write_text(ANN_MODULE_2_SOURCE)
+            Path(tempdir, "ann_module3.py").write_text(ANN_MODULE_3_SOURCE)
+            cls.ann_module = importlib.import_module("ann_module")
+            cls.ann_module2 = importlib.import_module("ann_module2")
+            cls.ann_module3 = importlib.import_module("ann_module3")
+        sys.path.pop()
+
+    @classmethod
+    def tearDownClass(cls):
+        for modname in "ann_module", "ann_module2", "ann_module3":
+            delattr(cls, modname)
+            del sys.modules[modname]
+
     def test_get_type_hints_modules(self):
         ann_module_type_hints = {1: 2, 'f': Tuple[int, int], 'x': int, 'y': str}
-        if (TYPING_3_11_0
-                or (TYPING_3_10_0 and sys.version_info.releaselevel in {'candidate', 'final'})):
-            # More tests were added in 3.10rc1.
-            ann_module_type_hints['u'] = int | float
-        self.assertEqual(gth(ann_module), ann_module_type_hints)
-        self.assertEqual(gth(ann_module2), {})
-        self.assertEqual(gth(ann_module3), {})
+        self.assertEqual(gth(self.ann_module), ann_module_type_hints)
+        self.assertEqual(gth(self.ann_module2), {})
+        self.assertEqual(gth(self.ann_module3), {})
 
     def test_get_type_hints_classes(self):
-        self.assertEqual(gth(ann_module.C, ann_module.__dict__),
-                         {'y': Optional[ann_module.C]})
-        self.assertIsInstance(gth(ann_module.j_class), dict)
-        self.assertEqual(gth(ann_module.M), {'123': 123, 'o': type})
-        self.assertEqual(gth(ann_module.D),
-                         {'j': str, 'k': str, 'y': Optional[ann_module.C]})
-        self.assertEqual(gth(ann_module.Y), {'z': int})
-        self.assertEqual(gth(ann_module.h_class),
-                         {'y': Optional[ann_module.C]})
-        self.assertEqual(gth(ann_module.S), {'x': str, 'y': str})
-        self.assertEqual(gth(ann_module.foo), {'x': int})
+        self.assertEqual(gth(self.ann_module.C, self.ann_module.__dict__),
+                         {'y': Optional[self.ann_module.C]})
+        self.assertIsInstance(gth(self.ann_module.j_class), dict)
+        self.assertEqual(gth(self.ann_module.M), {'123': 123, 'o': type})
+        self.assertEqual(gth(self.ann_module.D),
+                         {'j': str, 'k': str, 'y': Optional[self.ann_module.C]})
+        self.assertEqual(gth(self.ann_module.Y), {'z': int})
+        self.assertEqual(gth(self.ann_module.h_class),
+                         {'y': Optional[self.ann_module.C]})
+        self.assertEqual(gth(self.ann_module.S), {'x': str, 'y': str})
+        self.assertEqual(gth(self.ann_module.foo), {'x': int})
         self.assertEqual(gth(NoneAndForward, globals()),
                          {'parent': NoneAndForward, 'meaning': type(None)})
 
     def test_respect_no_type_check(self):
         @no_type_check
         class NoTpCheck:
             class Inn:
-                def __init__(self, x: 'not a type'): ...  # noqa
+                def __init__(self, x: 'not a type'): ...
         self.assertTrue(NoTpCheck.__no_type_check__)
         self.assertTrue(NoTpCheck.Inn.__init__.__no_type_check__)
-        self.assertEqual(gth(ann_module2.NTC.meth), {})
+        self.assertEqual(gth(self.ann_module2.NTC.meth), {})
         class ABase(Generic[T]):
             def meth(x: int): ...
         @no_type_check
         class Der(ABase): ...
         self.assertEqual(gth(ABase.meth), {'x': int})
 
     def test_get_type_hints_ClassVar(self):
-        self.assertEqual(gth(ann_module2.CV, ann_module2.__dict__),
-                         {'var': ClassVar[ann_module2.CV]})
+        self.assertEqual(gth(self.ann_module2.CV, self.ann_module2.__dict__),
+                         {'var': ClassVar[self.ann_module2.CV]})
         self.assertEqual(gth(B, globals()),
                          {'y': int, 'x': ClassVar[Optional[B]], 'b': int})
         self.assertEqual(gth(CSub, globals()),
                          {'z': ClassVar[CSub], 'y': int, 'b': int,
                           'x': ClassVar[Optional[B]]})
         self.assertEqual(gth(G), {'lst': ClassVar[List[T]]})
 
@@ -1289,56 +1540,123 @@
                 return a()
 
         assert isinstance(foo(KeyboardInterrupt), KeyboardInterrupt)
         assert foo(None) is None
 
 
 class NewTypeTests(BaseTestCase):
+    @classmethod
+    def setUpClass(cls):
+        global UserId
+        UserId = NewType('UserId', int)
+        cls.UserName = NewType(cls.__qualname__ + '.UserName', str)
+
+    @classmethod
+    def tearDownClass(cls):
+        global UserId
+        del UserId
+        del cls.UserName
 
     def test_basic(self):
-        UserId = NewType('UserId', int)
-        UserName = NewType('UserName', str)
         self.assertIsInstance(UserId(5), int)
-        self.assertIsInstance(UserName('Joe'), str)
+        self.assertIsInstance(self.UserName('Joe'), str)
         self.assertEqual(UserId(5) + 1, 6)
 
     def test_errors(self):
-        UserId = NewType('UserId', int)
-        UserName = NewType('UserName', str)
         with self.assertRaises(TypeError):
             issubclass(UserId, int)
         with self.assertRaises(TypeError):
-            class D(UserName):
+            class D(UserId):
                 pass
 
+    @skipUnless(TYPING_3_10_0, "PEP 604 has yet to be")
+    def test_or(self):
+        for cls in (int, self.UserName):
+            with self.subTest(cls=cls):
+                self.assertEqual(UserId | cls, Union[UserId, cls])
+                self.assertEqual(cls | UserId, Union[cls, UserId])
+
+                self.assertEqual(get_args(UserId | cls), (UserId, cls))
+                self.assertEqual(get_args(cls | UserId), (cls, UserId))
+
+    def test_special_attrs(self):
+        self.assertEqual(UserId.__name__, 'UserId')
+        self.assertEqual(UserId.__qualname__, 'UserId')
+        self.assertEqual(UserId.__module__, __name__)
+        self.assertEqual(UserId.__supertype__, int)
+
+        UserName = self.UserName
+        self.assertEqual(UserName.__name__, 'UserName')
+        self.assertEqual(UserName.__qualname__,
+                         self.__class__.__qualname__ + '.UserName')
+        self.assertEqual(UserName.__module__, __name__)
+        self.assertEqual(UserName.__supertype__, str)
+
+    def test_repr(self):
+        self.assertEqual(repr(UserId), f'{__name__}.UserId')
+        self.assertEqual(repr(self.UserName),
+                         f'{__name__}.{self.__class__.__qualname__}.UserName')
+
+    def test_pickle(self):
+        UserAge = NewType('UserAge', float)
+        for proto in range(pickle.HIGHEST_PROTOCOL + 1):
+            with self.subTest(proto=proto):
+                pickled = pickle.dumps(UserId, proto)
+                loaded = pickle.loads(pickled)
+                self.assertIs(loaded, UserId)
+
+                pickled = pickle.dumps(self.UserName, proto)
+                loaded = pickle.loads(pickled)
+                self.assertIs(loaded, self.UserName)
+
+                with self.assertRaises(pickle.PicklingError):
+                    pickle.dumps(UserAge, proto)
+
+    def test_missing__name__(self):
+        code = ("import typing_extensions\n"
+                "NT = typing_extensions.NewType('NT', int)\n"
+                )
+        exec(code, {})
+
+    def test_error_message_when_subclassing(self):
+        with self.assertRaisesRegex(
+            TypeError,
+            re.escape(
+                "Cannot subclass an instance of NewType. Perhaps you were looking for: "
+                "`ProUserId = NewType('ProUserId', UserId)`"
+            )
+        ):
+            class ProUserId(UserId):
+                ...
+
 
 class Coordinate(Protocol):
     x: int
     y: int
 
-@runtime
+@runtime_checkable
 class Point(Coordinate, Protocol):
     label: str
 
 class MyPoint:
     x: int
     y: int
     label: str
 
 class XAxis(Protocol):
     x: int
 
 class YAxis(Protocol):
     y: int
 
-@runtime
+@runtime_checkable
 class Position(XAxis, YAxis, Protocol):
     pass
 
-@runtime
+@runtime_checkable
 class Proto(Protocol):
     attr: int
 
     def meth(self, arg: str) -> int:
         ...
 
 class Concrete(Proto):
@@ -1354,17 +1672,19 @@
 
 class NT(NamedTuple):
     x: int
     y: int
 
 
 class ProtocolTests(BaseTestCase):
+    def test_runtime_alias(self):
+        self.assertIs(runtime, runtime_checkable)
 
     def test_basic_protocol(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             def meth(self):
                 pass
         class C: pass
         class D:
             def meth(self):
                 pass
@@ -1374,15 +1694,15 @@
         self.assertIsInstance(D(), P)
         self.assertNotIsSubclass(C, P)
         self.assertNotIsInstance(C(), P)
         self.assertNotIsSubclass(types.FunctionType, P)
         self.assertNotIsInstance(f, P)
 
     def test_everything_implements_empty_protocol(self):
-        @runtime
+        @runtime_checkable
         class Empty(Protocol): pass
         class C: pass
         def f():
             pass
         for thing in (object, type, tuple, C, types.FunctionType):
             self.assertIsSubclass(thing, Empty)
         for thing in (object(), 1, (), typing, f):
@@ -1406,14 +1726,30 @@
             class P(BP, C, Protocol):
                 pass
         class D(BP, C): pass
         class E(C, BP): pass
         self.assertNotIsInstance(D(), E)
         self.assertNotIsInstance(E(), D)
 
+    @skipUnless(
+        hasattr(typing, "Protocol"),
+        "Test is only relevant if typing.Protocol exists"
+    )
+    def test_runtimecheckable_on_typing_dot_Protocol(self):
+        @runtime_checkable
+        class Foo(typing.Protocol):
+            x: int
+
+        class Bar:
+            def __init__(self):
+                self.x = 42
+
+        self.assertIsInstance(Bar(), Foo)
+        self.assertNotIsInstance(object(), Foo)
+
     def test_no_instantiation(self):
         class P(Protocol): pass
         with self.assertRaises(TypeError):
             P()
         class C(P): pass
         self.assertIsInstance(C(), C)
         T = TypeVar('T')
@@ -1423,16 +1759,42 @@
         with self.assertRaises(TypeError):
             PG[int]()
         with self.assertRaises(TypeError):
             PG[T]()
         class CG(PG[T]): pass
         self.assertIsInstance(CG[int](), CG)
 
+    def test_protocol_defining_init_does_not_get_overridden(self):
+        # check that P.__init__ doesn't get clobbered
+        # see https://bugs.python.org/issue44807
+
+        class P(Protocol):
+            x: int
+            def __init__(self, x: int) -> None:
+                self.x = x
+        class C: pass
+
+        c = C()
+        P.__init__(c, 1)
+        self.assertEqual(c.x, 1)
+
+    def test_concrete_class_inheriting_init_from_protocol(self):
+        class P(Protocol):
+            x: int
+            def __init__(self, x: int) -> None:
+                self.x = x
+
+        class C(P): pass
+
+        c = C(1)
+        self.assertIsInstance(c, C)
+        self.assertEqual(c.x, 1)
+
     def test_cannot_instantiate_abstract(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             @abc.abstractmethod
             def ameth(self) -> int:
                 raise NotImplementedError
         class B(P):
             pass
         class C(B):
@@ -1442,15 +1804,15 @@
             B()
         self.assertIsInstance(C(), P)
 
     def test_subprotocols_extending(self):
         class P1(Protocol):
             def meth1(self):
                 pass
-        @runtime
+        @runtime_checkable
         class P2(P1, Protocol):
             def meth2(self):
                 pass
         class C:
             def meth1(self):
                 pass
             def meth2(self):
@@ -1471,15 +1833,15 @@
     def test_subprotocols_merging(self):
         class P1(Protocol):
             def meth1(self):
                 pass
         class P2(Protocol):
             def meth2(self):
                 pass
-        @runtime
+        @runtime_checkable
         class P(P1, P2, Protocol):
             pass
         class C:
             def meth1(self):
                 pass
             def meth2(self):
                 pass
@@ -1494,18 +1856,18 @@
         self.assertNotIsSubclass(C1, P)
         self.assertNotIsSubclass(C2, P)
         self.assertIsInstance(C(), P)
         self.assertIsSubclass(C, P)
 
     def test_protocols_issubclass(self):
         T = TypeVar('T')
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             def x(self): ...
-        @runtime
+        @runtime_checkable
         class PG(Protocol[T]):
             def x(self): ...
         class BadP(Protocol):
             def x(self): ...
         class BadPG(Protocol[T]):
             def x(self): ...
         class C:
@@ -1525,15 +1887,15 @@
             issubclass(P, PG[T])
         with self.assertRaises(TypeError):
             issubclass(PG, PG[int])
 
     def test_protocols_issubclass_non_callable(self):
         class C:
             x = 1
-        @runtime
+        @runtime_checkable
         class PNonCall(Protocol):
             x = 1
         with self.assertRaises(TypeError):
             issubclass(C, PNonCall)
         self.assertIsInstance(C(), PNonCall)
         PNonCall.register(C)
         with self.assertRaises(TypeError):
@@ -1545,39 +1907,290 @@
         self.assertNotIsInstance(C(), D)
         D.register(C)
         self.assertIsSubclass(C, D)
         self.assertIsInstance(C(), D)
         with self.assertRaises(TypeError):
             issubclass(D, PNonCall)
 
+    def test_no_weird_caching_with_issubclass_after_isinstance(self):
+        @runtime_checkable
+        class Spam(Protocol):
+            x: int
+
+        class Eggs:
+            def __init__(self) -> None:
+                self.x = 42
+
+        self.assertIsInstance(Eggs(), Spam)
+
+        # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
+        # TypeError wouldn't be raised here,
+        # as the cached result of the isinstance() check immediately above
+        # would mean the issubclass() call would short-circuit
+        # before we got to the "raise TypeError" line
+        with self.assertRaises(TypeError):
+            issubclass(Eggs, Spam)
+
+    def test_no_weird_caching_with_issubclass_after_isinstance_2(self):
+        @runtime_checkable
+        class Spam(Protocol):
+            x: int
+
+        class Eggs: ...
+
+        self.assertNotIsInstance(Eggs(), Spam)
+
+        # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
+        # TypeError wouldn't be raised here,
+        # as the cached result of the isinstance() check immediately above
+        # would mean the issubclass() call would short-circuit
+        # before we got to the "raise TypeError" line
+        with self.assertRaises(TypeError):
+            issubclass(Eggs, Spam)
+
+    def test_no_weird_caching_with_issubclass_after_isinstance_3(self):
+        @runtime_checkable
+        class Spam(Protocol):
+            x: int
+
+        class Eggs:
+            def __getattr__(self, attr):
+                if attr == "x":
+                    return 42
+                raise AttributeError(attr)
+
+        self.assertNotIsInstance(Eggs(), Spam)
+
+        # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
+        # TypeError wouldn't be raised here,
+        # as the cached result of the isinstance() check immediately above
+        # would mean the issubclass() call would short-circuit
+        # before we got to the "raise TypeError" line
+        with self.assertRaises(TypeError):
+            issubclass(Eggs, Spam)
+
     def test_protocols_isinstance(self):
         T = TypeVar('T')
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             def meth(x): ...
-        @runtime
+        @runtime_checkable
         class PG(Protocol[T]):
             def meth(x): ...
+        @runtime_checkable
+        class WeirdProto(Protocol):
+            meth = str.maketrans
+        @runtime_checkable
+        class WeirdProto2(Protocol):
+            meth = lambda *args, **kwargs: None  # noqa: E731
+        class CustomCallable:
+            def __call__(self, *args, **kwargs):
+                pass
+        @runtime_checkable
+        class WeirderProto(Protocol):
+            meth = CustomCallable()
         class BadP(Protocol):
             def meth(x): ...
         class BadPG(Protocol[T]):
             def meth(x): ...
         class C:
             def meth(x): ...
-        self.assertIsInstance(C(), P)
-        self.assertIsInstance(C(), PG)
+        class C2:
+            def __init__(self):
+                self.meth = lambda: None
+        for klass in C, C2:
+            for proto in P, PG, WeirdProto, WeirdProto2, WeirderProto:
+                with self.subTest(klass=klass.__name__, proto=proto.__name__):
+                    self.assertIsInstance(klass(), proto)
         with self.assertRaises(TypeError):
             isinstance(C(), PG[T])
         with self.assertRaises(TypeError):
             isinstance(C(), PG[C])
         with self.assertRaises(TypeError):
             isinstance(C(), BadP)
         with self.assertRaises(TypeError):
             isinstance(C(), BadPG)
 
+    def test_protocols_isinstance_properties_and_descriptors(self):
+        class C:
+            @property
+            def attr(self):
+                return 42
+
+        class CustomDescriptor:
+            def __get__(self, obj, objtype=None):
+                return 42
+
+        class D:
+            attr = CustomDescriptor()
+
+        # Check that properties set on superclasses
+        # are still found by the isinstance() logic
+        class E(C): ...
+        class F(D): ...
+
+        class Empty: ...
+
+        T = TypeVar('T')
+
+        @runtime_checkable
+        class P(Protocol):
+            @property
+            def attr(self): ...
+
+        @runtime_checkable
+        class P1(Protocol):
+            attr: int
+
+        @runtime_checkable
+        class PG(Protocol[T]):
+            @property
+            def attr(self): ...
+
+        @runtime_checkable
+        class PG1(Protocol[T]):
+            attr: T
+
+        @runtime_checkable
+        class MethodP(Protocol):
+            def attr(self): ...
+
+        @runtime_checkable
+        class MethodPG(Protocol[T]):
+            def attr(self) -> T: ...
+
+        for protocol_class in P, P1, PG, PG1, MethodP, MethodPG:
+            for klass in C, D, E, F:
+                with self.subTest(
+                    klass=klass.__name__,
+                    protocol_class=protocol_class.__name__
+                ):
+                    self.assertIsInstance(klass(), protocol_class)
+
+            with self.subTest(klass="Empty", protocol_class=protocol_class.__name__):
+                self.assertNotIsInstance(Empty(), protocol_class)
+
+        class BadP(Protocol):
+            @property
+            def attr(self): ...
+
+        class BadP1(Protocol):
+            attr: int
+
+        class BadPG(Protocol[T]):
+            @property
+            def attr(self): ...
+
+        class BadPG1(Protocol[T]):
+            attr: T
+
+        cases = (
+            PG[T], PG[C], PG1[T], PG1[C], MethodPG[T],
+            MethodPG[C], BadP, BadP1, BadPG, BadPG1
+        )
+
+        for obj in cases:
+            for klass in C, D, E, F, Empty:
+                with self.subTest(klass=klass.__name__, obj=obj):
+                    with self.assertRaises(TypeError):
+                        isinstance(klass(), obj)
+
+    def test_protocols_isinstance_not_fooled_by_custom_dir(self):
+        @runtime_checkable
+        class HasX(Protocol):
+            x: int
+
+        class CustomDirWithX:
+            x = 10
+            def __dir__(self):
+                return []
+
+        class CustomDirWithoutX:
+            def __dir__(self):
+                return ["x"]
+
+        self.assertIsInstance(CustomDirWithX(), HasX)
+        self.assertNotIsInstance(CustomDirWithoutX(), HasX)
+
+    def test_protocols_isinstance_attribute_access_with_side_effects(self):
+        class C:
+            @property
+            def attr(self):
+                raise AttributeError('no')
+
+        class CustomDescriptor:
+            def __get__(self, obj, objtype=None):
+                raise RuntimeError("NO")
+
+        class D:
+            attr = CustomDescriptor()
+
+        # Check that properties set on superclasses
+        # are still found by the isinstance() logic
+        class E(C): ...
+        class F(D): ...
+
+        class WhyWouldYouDoThis:
+            def __getattr__(self, name):
+                raise RuntimeError("wut")
+
+        T = TypeVar('T')
+
+        @runtime_checkable
+        class P(Protocol):
+            @property
+            def attr(self): ...
+
+        @runtime_checkable
+        class P1(Protocol):
+            attr: int
+
+        @runtime_checkable
+        class PG(Protocol[T]):
+            @property
+            def attr(self): ...
+
+        @runtime_checkable
+        class PG1(Protocol[T]):
+            attr: T
+
+        @runtime_checkable
+        class MethodP(Protocol):
+            def attr(self): ...
+
+        @runtime_checkable
+        class MethodPG(Protocol[T]):
+            def attr(self) -> T: ...
+
+        for protocol_class in P, P1, PG, PG1, MethodP, MethodPG:
+            for klass in C, D, E, F:
+                with self.subTest(
+                    klass=klass.__name__,
+                    protocol_class=protocol_class.__name__
+                ):
+                    self.assertIsInstance(klass(), protocol_class)
+
+            with self.subTest(
+                klass="WhyWouldYouDoThis",
+                protocol_class=protocol_class.__name__
+            ):
+                self.assertNotIsInstance(WhyWouldYouDoThis(), protocol_class)
+
+    def test_protocols_isinstance___slots__(self):
+        # As per the consensus in https://github.com/python/typing/issues/1367,
+        # this is desirable behaviour
+        @runtime_checkable
+        class HasX(Protocol):
+            x: int
+
+        class HasNothingButSlots:
+            __slots__ = ("x",)
+
+        self.assertIsInstance(HasNothingButSlots(), HasX)
+
     def test_protocols_isinstance_py36(self):
         class APoint:
             def __init__(self, x, y, label):
                 self.x = x
                 self.y = y
                 self.label = label
         class BPoint:
@@ -1603,55 +2216,69 @@
         self.assertNotIsInstance(Bad(), Position)
         self.assertNotIsInstance(Bad(), Concrete)
         self.assertNotIsInstance(Other(), Concrete)
         self.assertIsInstance(NT(1, 2), Position)
 
     def test_protocols_isinstance_init(self):
         T = TypeVar('T')
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             x = 1
-        @runtime
+        @runtime_checkable
         class PG(Protocol[T]):
             x = 1
         class C:
             def __init__(self, x):
                 self.x = x
         self.assertIsInstance(C(1), P)
         self.assertIsInstance(C(1), PG)
 
+    def test_protocols_isinstance_monkeypatching(self):
+        @runtime_checkable
+        class HasX(Protocol):
+            x: int
+
+        class Foo: ...
+
+        f = Foo()
+        self.assertNotIsInstance(f, HasX)
+        f.x = 42
+        self.assertIsInstance(f, HasX)
+        del f.x
+        self.assertNotIsInstance(f, HasX)
+
     def test_protocols_support_register(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             x = 1
         class PM(Protocol):
             def meth(self): pass
         class D(PM): pass
         class C: pass
         D.register(C)
         P.register(C)
         self.assertIsInstance(C(), P)
         self.assertIsInstance(C(), D)
 
     def test_none_on_non_callable_doesnt_block_implementation(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             x = 1
         class A:
             x = 1
         class B(A):
             x = None
         class C:
             def __init__(self):
                 self.x = None
         self.assertIsInstance(B(), P)
         self.assertIsInstance(C(), P)
 
     def test_none_on_callable_blocks_implementation(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             def x(self): ...
         class A:
             def x(self): ...
         class B(A):
             x = None
         class C:
@@ -1659,31 +2286,45 @@
                 self.x = None
         self.assertNotIsInstance(B(), P)
         self.assertNotIsInstance(C(), P)
 
     def test_non_protocol_subclasses(self):
         class P(Protocol):
             x = 1
-        @runtime
+        @runtime_checkable
         class PR(Protocol):
             def meth(self): pass
         class NonP(P):
             x = 1
         class NonPR(PR): pass
-        class C:
+        class C(metaclass=abc.ABCMeta):
             x = 1
-        class D:
-            def meth(self): pass
+        class D(metaclass=abc.ABCMeta):  # noqa: B024
+            def meth(self): pass  # noqa: B027
         self.assertNotIsInstance(C(), NonP)
         self.assertNotIsInstance(D(), NonPR)
         self.assertNotIsSubclass(C, NonP)
         self.assertNotIsSubclass(D, NonPR)
         self.assertIsInstance(NonPR(), PR)
         self.assertIsSubclass(NonPR, PR)
 
+        self.assertNotIn("__protocol_attrs__", vars(NonP))
+        self.assertNotIn("__protocol_attrs__", vars(NonPR))
+        self.assertNotIn("__callable_proto_members_only__", vars(NonP))
+        self.assertNotIn("__callable_proto_members_only__", vars(NonPR))
+
+        acceptable_extra_attrs = {
+            '_is_protocol', '_is_runtime_protocol', '__parameters__',
+            '__init__', '__annotations__', '__subclasshook__',
+        }
+        self.assertLessEqual(vars(NonP).keys(), vars(C).keys() | acceptable_extra_attrs)
+        self.assertLessEqual(
+            vars(NonPR).keys(), vars(D).keys() | acceptable_extra_attrs
+        )
+
     def test_custom_subclasshook(self):
         class P(Protocol):
             x = 1
         class OKClass: pass
         class BadClass:
             x = 1
         class C(P):
@@ -1692,25 +2333,25 @@
                 return other.__name__.startswith("OK")
         self.assertIsInstance(OKClass(), C)
         self.assertNotIsInstance(BadClass(), C)
         self.assertIsSubclass(OKClass, C)
         self.assertNotIsSubclass(BadClass, C)
 
     def test_issubclass_fails_correctly(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             x = 1
         class C: pass
         with self.assertRaises(TypeError):
             issubclass(C(), P)
 
     def test_defining_generic_protocols(self):
         T = TypeVar('T')
         S = TypeVar('S')
-        @runtime
+        @runtime_checkable
         class PR(Protocol[T, S]):
             def meth(self): pass
         class P(PR[int, T], Protocol[T]):
             y = 1
         with self.assertRaises(TypeError):
             issubclass(PR[int, T], PR)
         with self.assertRaises(TypeError):
@@ -1726,15 +2367,15 @@
                 PR[int, ClassVar]
         class C(PR[int, T]): pass
         self.assertIsInstance(C[str](), C)
 
     def test_defining_generic_protocols_old_style(self):
         T = TypeVar('T')
         S = TypeVar('S')
-        @runtime
+        @runtime_checkable
         class PR(Protocol, Generic[T, S]):
             def meth(self): pass
         class P(PR[int, str], Protocol):
             y = 1
         with self.assertRaises(TypeError):
             self.assertIsSubclass(PR[int, str], PR)
         self.assertIsSubclass(P, PR)
@@ -1743,26 +2384,68 @@
         if not TYPING_3_10_0:
             with self.assertRaises(TypeError):
                 PR[int, 1]
         class P1(Protocol, Generic[T]):
             def bar(self, x: T) -> str: ...
         class P2(Generic[T], Protocol):
             def bar(self, x: T) -> str: ...
-        @runtime
+        @runtime_checkable
         class PSub(P1[str], Protocol):
             x = 1
         class Test:
             x = 1
             def bar(self, x: str) -> str:
                 return x
         self.assertIsInstance(Test(), PSub)
         if not TYPING_3_10_0:
             with self.assertRaises(TypeError):
                 PR[int, ClassVar]
 
+    if hasattr(typing, "TypeAliasType"):
+        exec(textwrap.dedent(
+            """
+            def test_pep695_generic_protocol_callable_members(self):
+                @runtime_checkable
+                class Foo[T](Protocol):
+                    def meth(self, x: T) -> None: ...
+
+                class Bar[T]:
+                    def meth(self, x: T) -> None: ...
+
+                self.assertIsInstance(Bar(), Foo)
+                self.assertIsSubclass(Bar, Foo)
+
+                @runtime_checkable
+                class SupportsTrunc[T](Protocol):
+                    def __trunc__(self) -> T: ...
+
+                self.assertIsInstance(0.0, SupportsTrunc)
+                self.assertIsSubclass(float, SupportsTrunc)
+
+            def test_no_weird_caching_with_issubclass_after_isinstance_pep695(self):
+                @runtime_checkable
+                class Spam[T](Protocol):
+                    x: T
+
+                class Eggs[T]:
+                    def __init__(self, x: T) -> None:
+                        self.x = x
+
+                self.assertIsInstance(Eggs(42), Spam)
+
+                # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
+                # TypeError wouldn't be raised here,
+                # as the cached result of the isinstance() check immediately above
+                # would mean the issubclass() call would short-circuit
+                # before we got to the "raise TypeError" line
+                with self.assertRaises(TypeError):
+                    issubclass(Eggs, Spam)
+            """
+        ))
+
     def test_init_called(self):
         T = TypeVar('T')
         class P(Protocol[T]): pass
         class C(P[T]):
             def __init__(self):
                 self.test = 'OK'
         self.assertEqual(C[int]().test, 'OK')
@@ -1800,53 +2483,49 @@
         class P(Protocol[T]): pass
         self.assertEqual(P.__parameters__, (T,))
         self.assertEqual(P[int].__parameters__, ())
         self.assertEqual(P[int].__args__, (int,))
         self.assertIs(P[int].__origin__, P)
 
     def test_generic_protocols_special_from_protocol(self):
-        @runtime
+        @runtime_checkable
         class PR(Protocol):
             x = 1
         class P(Protocol):
             def meth(self):
                 pass
         T = TypeVar('T')
         class PG(Protocol[T]):
             x = 1
             def meth(self):
                 pass
         self.assertTrue(P._is_protocol)
         self.assertTrue(PR._is_protocol)
         self.assertTrue(PG._is_protocol)
-        if hasattr(typing, 'Protocol'):
-            self.assertFalse(P._is_runtime_protocol)
-        else:
-            with self.assertRaises(AttributeError):
-                self.assertFalse(P._is_runtime_protocol)
+        self.assertFalse(P._is_runtime_protocol)
         self.assertTrue(PR._is_runtime_protocol)
         self.assertTrue(PG[int]._is_protocol)
         self.assertEqual(typing_extensions._get_protocol_attrs(P), {'meth'})
         self.assertEqual(typing_extensions._get_protocol_attrs(PR), {'x'})
         self.assertEqual(frozenset(typing_extensions._get_protocol_attrs(PG)),
                          frozenset({'x', 'meth'}))
 
     def test_no_runtime_deco_on_nominal(self):
         with self.assertRaises(TypeError):
-            @runtime
+            @runtime_checkable
             class C: pass
         class Proto(Protocol):
             x = 1
         with self.assertRaises(TypeError):
-            @runtime
+            @runtime_checkable
             class Concrete(Proto):
                 pass
 
     def test_none_treated_correctly(self):
-        @runtime
+        @runtime_checkable
         class P(Protocol):
             x: int = None
         class B(object): pass
         self.assertNotIsInstance(B(), P)
         class C:
             x = 1
         class D:
@@ -1855,29 +2534,29 @@
         self.assertIsInstance(D(), P)
         class CI:
             def __init__(self):
                 self.x = 1
         class DI:
             def __init__(self):
                 self.x = None
-        self.assertIsInstance(C(), P)
-        self.assertIsInstance(D(), P)
+        self.assertIsInstance(CI(), P)
+        self.assertIsInstance(DI(), P)
 
     def test_protocols_in_unions(self):
         class P(Protocol):
             x: int = None
         Alias = typing.Union[typing.Iterable, P]
         Alias2 = typing.Union[P, typing.Iterable]
         self.assertEqual(Alias, Alias2)
 
     def test_protocols_pickleable(self):
         global P, CP  # pickle wants to reference the class by name
         T = TypeVar('T')
 
-        @runtime
+        @runtime_checkable
         class P(Protocol[T]):
             x = 1
         class CP(P[int]):
             pass
 
         c = CP()
         c.foo = 42
@@ -1906,14 +2585,29 @@
                 return []
             def close(self):
                 return 0
 
         self.assertIsSubclass(B, Custom)
         self.assertNotIsSubclass(A, Custom)
 
+    def test_builtin_protocol_allowlist(self):
+        with self.assertRaises(TypeError):
+            class CustomProtocol(TestCase, Protocol):
+                pass
+
+        class CustomContextManager(typing.ContextManager, Protocol):
+            pass
+
+    def test_non_runtime_protocol_isinstance_check(self):
+        class P(Protocol):
+            x: int
+
+        with self.assertRaisesRegex(TypeError, "@runtime_checkable"):
+            isinstance(1, P)
+
     def test_no_init_same_for_different_protocol_implementations(self):
         class CustomProtocolWithoutInitA(Protocol):
             pass
 
         class CustomProtocolWithoutInitB(Protocol):
             pass
 
@@ -1947,31 +2641,33 @@
         self.assertEqual(Emp.__name__, 'Emp')
         self.assertEqual(Emp.__module__, __name__)
         self.assertEqual(Emp.__bases__, (dict,))
         self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
         self.assertEqual(Emp.__total__, True)
 
     def test_basics_keywords_syntax(self):
-        Emp = TypedDict('Emp', name=str, id=int)
+        with self.assertWarns(DeprecationWarning):
+            Emp = TypedDict('Emp', name=str, id=int)
         self.assertIsSubclass(Emp, dict)
         self.assertIsSubclass(Emp, typing.MutableMapping)
         self.assertNotIsSubclass(Emp, collections.abc.Sequence)
         jim = Emp(name='Jim', id=1)
         self.assertIs(type(jim), dict)
         self.assertEqual(jim['name'], 'Jim')
         self.assertEqual(jim['id'], 1)
         self.assertEqual(Emp.__name__, 'Emp')
         self.assertEqual(Emp.__module__, __name__)
         self.assertEqual(Emp.__bases__, (dict,))
         self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
         self.assertEqual(Emp.__total__, True)
 
     def test_typeddict_special_keyword_names(self):
-        TD = TypedDict("TD", cls=type, self=object, typename=str, _typename=int,
-                       fields=list, _fields=dict)
+        with self.assertWarns(DeprecationWarning):
+            TD = TypedDict("TD", cls=type, self=object, typename=str, _typename=int,
+                           fields=list, _fields=dict)
         self.assertEqual(TD.__name__, 'TD')
         self.assertEqual(TD.__annotations__, {'cls': type, 'self': object, 'typename': str,
                                               '_typename': int, 'fields': list, '_fields': dict})
         a = TD(cls=str, self=42, typename='foo', _typename=53,
                fields=[('bar', tuple)], _fields={'baz', set})
         self.assertEqual(a['cls'], str)
         self.assertEqual(a['self'], 42)
@@ -1997,28 +2693,28 @@
         with self.assertWarns(DeprecationWarning):
             Emp = TypedDict('Emp', _fields={'name': str, 'id': int})
         self.assertEqual(Emp.__name__, 'Emp')
         self.assertEqual(Emp.__annotations__, {'name': str, 'id': int})
 
     def test_typeddict_errors(self):
         Emp = TypedDict('Emp', {'name': str, 'id': int})
-        if hasattr(typing, "Required"):
+        if sys.version_info >= (3, 12):
             self.assertEqual(TypedDict.__module__, 'typing')
         else:
             self.assertEqual(TypedDict.__module__, 'typing_extensions')
         jim = Emp(name='Jim', id=1)
         with self.assertRaises(TypeError):
             isinstance({}, Emp)
         with self.assertRaises(TypeError):
             isinstance(jim, Emp)
         with self.assertRaises(TypeError):
             issubclass(dict, Emp)
 
         if not TYPING_3_11_0:
-            with self.assertRaises(TypeError):
+            with self.assertRaises(TypeError), self.assertWarns(DeprecationWarning):
                 TypedDict('Hi', x=1)
             with self.assertRaises(TypeError):
                 TypedDict('Hi', [('x', int), ('y', 1)])
         with self.assertRaises(TypeError):
             TypedDict('Hi', [('x', int)], y=int)
 
     def test_py36_class_syntax_usage(self):
@@ -2032,15 +2728,15 @@
         self.assertEqual(not_origin['x'], 0)
         self.assertEqual(not_origin['y'], 1)
         other = LabelPoint2D(x=0, y=1, label='hi')
         self.assertEqual(other['label'], 'hi')
 
     def test_pickle(self):
         global EmpD  # pickle wants to reference the class by name
-        EmpD = TypedDict('EmpD', name=str, id=int)
+        EmpD = TypedDict('EmpD', {"name": str, "id": int})
         jane = EmpD({'name': 'jane', 'id': 37})
         point = Point2DGeneric(a=5.0, b=3.0)
         for proto in range(pickle.HIGHEST_PROTOCOL + 1):
             # Test non-generic TypedDict
             z = pickle.dumps(jane, proto)
             jane2 = pickle.loads(z)
             self.assertEqual(jane2, jane)
@@ -2054,15 +2750,15 @@
             self.assertEqual(point, point2)
             self.assertEqual(point2, {'a': 5.0, 'b': 3.0})
             YY = pickle.dumps(Point2DGeneric, proto)
             Point2DGenericNew = pickle.loads(YY)
             self.assertEqual(Point2DGenericNew({'a': 5.0, 'b': 3.0}), point)
 
     def test_optional(self):
-        EmpD = TypedDict('EmpD', name=str, id=int)
+        EmpD = TypedDict('EmpD', {"name": str, "id": int})
 
         self.assertEqual(typing.Optional[EmpD], typing.Union[None, EmpD])
         self.assertNotEqual(typing.List[EmpD], typing.Tuple[EmpD])
 
     def test_total(self):
         D = TypedDict('D', {'x': int}, total=False)
         self.assertEqual(D(), {})
@@ -2364,24 +3060,14 @@
                 get_type_hints(C, globals())["classvar"],
                 Annotated[ClassVar[int], "a decoration"]
             )
             self.assertEqual(
                 get_type_hints(C, globals())["const"], Annotated[Final[int], "Const"]
             )
 
-    def test_hash_eq(self):
-        self.assertEqual(len({Annotated[int, 4, 5], Annotated[int, 4, 5]}), 1)
-        self.assertNotEqual(Annotated[int, 4, 5], Annotated[int, 5, 4])
-        self.assertNotEqual(Annotated[int, 4, 5], Annotated[str, 4, 5])
-        self.assertNotEqual(Annotated[int, 4], Annotated[int, 4, 4])
-        self.assertEqual(
-            {Annotated[int, 4, 5], Annotated[int, 4, 5], Annotated[T, 4, 5]},
-            {Annotated[int, 4, 5], Annotated[T, 4, 5]}
-        )
-
     def test_cannot_subclass(self):
         with self.assertRaisesRegex(TypeError, "Cannot subclass .*Annotated"):
             class C(Annotated):
                 pass
 
     def test_cannot_check_instance(self):
         with self.assertRaises(TypeError):
@@ -2524,14 +3210,57 @@
 
         assert get_type_hints(AnnotatedMovie) == {'title': str, 'year': int}
         assert get_type_hints(AnnotatedMovie, include_extras=True) == {
             'title': Annotated[Required[str], "foobar"],
             'year': NotRequired[Annotated[int, 2000]],
         }
 
+    def test_orig_bases(self):
+        T = TypeVar('T')
+
+        class Parent(TypedDict):
+            pass
+
+        class Child(Parent):
+            pass
+
+        class OtherChild(Parent):
+            pass
+
+        class MixedChild(Child, OtherChild, Parent):
+            pass
+
+        class GenericParent(TypedDict, Generic[T]):
+            pass
+
+        class GenericChild(GenericParent[int]):
+            pass
+
+        class OtherGenericChild(GenericParent[str]):
+            pass
+
+        class MixedGenericChild(GenericChild, OtherGenericChild, GenericParent[float]):
+            pass
+
+        class MultipleGenericBases(GenericParent[int], GenericParent[float]):
+            pass
+
+        CallTypedDict = TypedDict('CallTypedDict', {})
+
+        self.assertEqual(Parent.__orig_bases__, (TypedDict,))
+        self.assertEqual(Child.__orig_bases__, (Parent,))
+        self.assertEqual(OtherChild.__orig_bases__, (Parent,))
+        self.assertEqual(MixedChild.__orig_bases__, (Child, OtherChild, Parent,))
+        self.assertEqual(GenericParent.__orig_bases__, (TypedDict, Generic[T]))
+        self.assertEqual(GenericChild.__orig_bases__, (GenericParent[int],))
+        self.assertEqual(OtherGenericChild.__orig_bases__, (GenericParent[str],))
+        self.assertEqual(MixedGenericChild.__orig_bases__, (GenericChild, OtherGenericChild, GenericParent[float]))
+        self.assertEqual(MultipleGenericBases.__orig_bases__, (GenericParent[int], GenericParent[float]))
+        self.assertEqual(CallTypedDict.__orig_bases__, (TypedDict,))
+
 
 class TypeAliasTests(BaseTestCase):
     def test_canonical_usage_with_variable_annotation(self):
         ns = {}
         exec('Alias: TypeAlias = Employee', globals(), ns)
 
     def test_canonical_usage_with_type_comment(self):
@@ -2573,41 +3302,66 @@
 
 class ParamSpecTests(BaseTestCase):
 
     def test_basic_plain(self):
         P = ParamSpec('P')
         self.assertEqual(P, P)
         self.assertIsInstance(P, ParamSpec)
+        self.assertEqual(P.__name__, 'P')
         # Should be hashable
         hash(P)
 
     def test_repr(self):
         P = ParamSpec('P')
         P_co = ParamSpec('P_co', covariant=True)
         P_contra = ParamSpec('P_contra', contravariant=True)
+        P_infer = ParamSpec('P_infer', infer_variance=True)
         P_2 = ParamSpec('P_2')
         self.assertEqual(repr(P), '~P')
         self.assertEqual(repr(P_2), '~P_2')
 
         # Note: PEP 612 doesn't require these to be repr-ed correctly, but
         # just follow CPython.
         self.assertEqual(repr(P_co), '+P_co')
         self.assertEqual(repr(P_contra), '-P_contra')
+        # On other versions we use typing.ParamSpec, but it is not aware of
+        # infer_variance=. Not worth creating our own version of ParamSpec
+        # for this.
+        if hasattr(typing, 'TypeAliasType') or not hasattr(typing, 'ParamSpec'):
+            self.assertEqual(repr(P_infer), 'P_infer')
+        else:
+            self.assertEqual(repr(P_infer), '~P_infer')
+
+    def test_variance(self):
+        P_co = ParamSpec('P_co', covariant=True)
+        P_contra = ParamSpec('P_contra', contravariant=True)
+        P_infer = ParamSpec('P_infer', infer_variance=True)
+
+        self.assertIs(P_co.__covariant__, True)
+        self.assertIs(P_co.__contravariant__, False)
+        self.assertIs(P_co.__infer_variance__, False)
+
+        self.assertIs(P_contra.__covariant__, False)
+        self.assertIs(P_contra.__contravariant__, True)
+        self.assertIs(P_contra.__infer_variance__, False)
+
+        self.assertIs(P_infer.__covariant__, False)
+        self.assertIs(P_infer.__contravariant__, False)
+        self.assertIs(P_infer.__infer_variance__, True)
 
     def test_valid_uses(self):
         P = ParamSpec('P')
         T = TypeVar('T')
         C1 = typing.Callable[P, int]
         self.assertEqual(C1.__args__, (P, int))
         self.assertEqual(C1.__parameters__, (P,))
         C2 = typing.Callable[P, T]
         self.assertEqual(C2.__args__, (P, T))
         self.assertEqual(C2.__parameters__, (P, T))
 
-
         # Test collections.abc.Callable too.
         if sys.version_info[:2] >= (3, 9):
             # Note: no tests for Callable.__parameters__ here
             # because types.GenericAlias Callable is hardcoded to search
             # for tp_name "TypeVar" in C.  This was changed in 3.10.
             C3 = collections.abc.Callable[P, int]
             self.assertEqual(C3.__args__, (P, int))
@@ -2915,18 +3669,15 @@
         Ts = TypeVarTuple('Ts')
         self.assertEqual(Unpack[Ts], Unpack[Ts])
         with self.assertRaises(TypeError):
             Unpack()
 
     def test_repr(self):
         Ts = TypeVarTuple('Ts')
-        if TYPING_3_11_0:
-            self.assertEqual(repr(Unpack[Ts]), '*Ts')
-        else:
-            self.assertEqual(repr(Unpack[Ts]), 'typing_extensions.Unpack[Ts]')
+        self.assertEqual(repr(Unpack[Ts]), f'{Unpack.__module__}.Unpack[Ts]')
 
     def test_cannot_subclass_vars(self):
         with self.assertRaises(TypeError):
             class V(Unpack[TypeVarTuple('Ts')]):
                 pass
 
     def test_tuple(self):
@@ -3040,15 +3791,18 @@
         # Not legal at type checking time but we can't really check against it.
         Tuple[Ts]
 
     def test_args_and_parameters(self):
         Ts = TypeVarTuple('Ts')
 
         t = Tuple[tuple(Ts)]
-        self.assertEqual(t.__args__, (Unpack[Ts],))
+        if sys.version_info >= (3, 11):
+            self.assertEqual(t.__args__, (typing.Unpack[Ts],))
+        else:
+            self.assertEqual(t.__args__, (Unpack[Ts],))
         self.assertEqual(t.__parameters__, (Ts,))
 
     def test_pickle(self):
         global Ts, Ts_default  # pickle wants to reference the class by name
         Ts = TypeVarTuple('Ts')
         Ts_default = TypeVarTuple('Ts_default', default=Unpack[Tuple[int, str]])
 
@@ -3132,15 +3886,18 @@
         self.assertIs(True, Methods.prop.fget.__final__)
         self.assertIs(True, Methods.cached.__final__)
 
 
 class RevealTypeTests(BaseTestCase):
     def test_reveal_type(self):
         obj = object()
-        self.assertIs(obj, reveal_type(obj))
+
+        with contextlib.redirect_stderr(io.StringIO()) as stderr:
+            self.assertIs(obj, reveal_type(obj))
+            self.assertEqual("Runtime type is 'object'", stderr.getvalue().strip())
 
 
 class DataclassTransformTests(BaseTestCase):
     def test_decorator(self):
         def create_model(*, frozen: bool = False, kw_only: bool = True):
             return lambda cls: cls
 
@@ -3287,26 +4044,32 @@
 
     def test_typing_extensions_defers_when_possible(self):
         exclude = {
             'dataclass_transform',
             'overload',
             'ParamSpec',
             'Text',
-            'TypedDict',
             'TypeVar',
             'TypeVarTuple',
             'TYPE_CHECKING',
             'Final',
             'get_type_hints',
-            'is_typeddict',
         }
         if sys.version_info < (3, 10):
             exclude |= {'get_args', 'get_origin'}
+        if sys.version_info < (3, 10, 1):
+            exclude |= {"Literal"}
         if sys.version_info < (3, 11):
-            exclude |= {'final', 'NamedTuple', 'Any'}
+            exclude |= {'final', 'Any', 'NewType'}
+        if sys.version_info < (3, 12):
+            exclude |= {
+                'Protocol', 'runtime_checkable', 'SupportsAbs', 'SupportsBytes',
+                'SupportsComplex', 'SupportsFloat', 'SupportsIndex', 'SupportsInt',
+                'SupportsRound', 'TypedDict', 'is_typeddict', 'NamedTuple', 'Unpack',
+            }
         for item in typing_extensions.__all__:
             if item not in exclude and hasattr(typing, item):
                 self.assertIs(
                     getattr(typing_extensions, item),
                     getattr(typing, item))
 
     def test_typing_extensions_compiles_with_opt(self):
@@ -3344,15 +4107,14 @@
     def __str__(self):
         return f'{self.x} -> {self.y}'
 
     def __add__(self, other):
         return 0
 
 
-@skipIf(TYPING_3_11_0, "These invariants should all be tested upstream on 3.11+")
 class NamedTupleTests(BaseTestCase):
     class NestedEmployee(NamedTuple):
         name: str
         cool: int
 
     def test_basics(self):
         Emp = NamedTuple('Emp', [('name', str), ('id', int)])
@@ -3484,15 +4246,17 @@
                 self.assertEqual(A.__args__, (int,))
                 self.assertEqual(A.__parameters__, ())
 
                 a = A(3)
                 self.assertIs(type(a), G)
                 self.assertEqual(a.x, 3)
 
-                with self.assertRaisesRegex(TypeError, 'Too many parameters'):
+                things = "arguments" if sys.version_info >= (3, 11) else "parameters"
+
+                with self.assertRaisesRegex(TypeError, f'Too many {things}'):
                     G[int, str]
 
     @skipUnless(TYPING_3_9_0, "tuple.__class_getitem__ was added in 3.9")
     def test_non_generic_subscript_py39_plus(self):
         # For backward compatibility, subscription works
         # on arbitrary NamedTuple types.
         class Group(NamedTuple):
@@ -3603,51 +4367,227 @@
     def test_signature_on_37(self):
         self.assertIsInstance(inspect.signature(NamedTuple), inspect.Signature)
         self.assertFalse(hasattr(NamedTuple, "__text_signature__"))
 
     @skipUnless(TYPING_3_9_0, "NamedTuple was a class on 3.8 and lower")
     def test_same_as_typing_NamedTuple_39_plus(self):
         self.assertEqual(
-            set(dir(NamedTuple)),
-            set(dir(typing.NamedTuple)) | {"__text_signature__"}
+            set(dir(NamedTuple)) - {"__text_signature__"},
+            set(dir(typing.NamedTuple))
         )
         self.assertIs(type(NamedTuple), type(typing.NamedTuple))
 
     @skipIf(TYPING_3_9_0, "tests are only relevant to <=3.8")
     def test_same_as_typing_NamedTuple_38_minus(self):
         self.assertEqual(
             self.NestedEmployee.__annotations__,
             self.NestedEmployee._field_types
         )
 
+    def test_orig_bases(self):
+        T = TypeVar('T')
+
+        class SimpleNamedTuple(NamedTuple):
+            pass
+
+        class GenericNamedTuple(NamedTuple, Generic[T]):
+            pass
+
+        self.assertEqual(SimpleNamedTuple.__orig_bases__, (NamedTuple,))
+        self.assertEqual(GenericNamedTuple.__orig_bases__, (NamedTuple, Generic[T]))
+
+        CallNamedTuple = NamedTuple('CallNamedTuple', [])
+
+        self.assertEqual(CallNamedTuple.__orig_bases__, (NamedTuple,))
+
+
+class TypeVarTests(BaseTestCase):
+    def test_basic_plain(self):
+        T = TypeVar('T')
+        # T equals itself.
+        self.assertEqual(T, T)
+        # T is an instance of TypeVar
+        self.assertIsInstance(T, TypeVar)
+        self.assertEqual(T.__name__, 'T')
+        self.assertEqual(T.__constraints__, ())
+        self.assertIs(T.__bound__, None)
+        self.assertIs(T.__covariant__, False)
+        self.assertIs(T.__contravariant__, False)
+        self.assertIs(T.__infer_variance__, False)
+
+    def test_attributes(self):
+        T_bound = TypeVar('T_bound', bound=int)
+        self.assertEqual(T_bound.__name__, 'T_bound')
+        self.assertEqual(T_bound.__constraints__, ())
+        self.assertIs(T_bound.__bound__, int)
+
+        T_constraints = TypeVar('T_constraints', int, str)
+        self.assertEqual(T_constraints.__name__, 'T_constraints')
+        self.assertEqual(T_constraints.__constraints__, (int, str))
+        self.assertIs(T_constraints.__bound__, None)
+
+        T_co = TypeVar('T_co', covariant=True)
+        self.assertEqual(T_co.__name__, 'T_co')
+        self.assertIs(T_co.__covariant__, True)
+        self.assertIs(T_co.__contravariant__, False)
+        self.assertIs(T_co.__infer_variance__, False)
+
+        T_contra = TypeVar('T_contra', contravariant=True)
+        self.assertEqual(T_contra.__name__, 'T_contra')
+        self.assertIs(T_contra.__covariant__, False)
+        self.assertIs(T_contra.__contravariant__, True)
+        self.assertIs(T_contra.__infer_variance__, False)
+
+        T_infer = TypeVar('T_infer', infer_variance=True)
+        self.assertEqual(T_infer.__name__, 'T_infer')
+        self.assertIs(T_infer.__covariant__, False)
+        self.assertIs(T_infer.__contravariant__, False)
+        self.assertIs(T_infer.__infer_variance__, True)
+
+    def test_typevar_instance_type_error(self):
+        T = TypeVar('T')
+        with self.assertRaises(TypeError):
+            isinstance(42, T)
+
+    def test_typevar_subclass_type_error(self):
+        T = TypeVar('T')
+        with self.assertRaises(TypeError):
+            issubclass(int, T)
+        with self.assertRaises(TypeError):
+            issubclass(T, int)
+
+    def test_constrained_error(self):
+        with self.assertRaises(TypeError):
+            X = TypeVar('X', int)
+            X
+
+    def test_union_unique(self):
+        X = TypeVar('X')
+        Y = TypeVar('Y')
+        self.assertNotEqual(X, Y)
+        self.assertEqual(Union[X], X)
+        self.assertNotEqual(Union[X], Union[X, Y])
+        self.assertEqual(Union[X, X], X)
+        self.assertNotEqual(Union[X, int], Union[X])
+        self.assertNotEqual(Union[X, int], Union[int])
+        self.assertEqual(Union[X, int].__args__, (X, int))
+        self.assertEqual(Union[X, int].__parameters__, (X,))
+        self.assertIs(Union[X, int].__origin__, Union)
+
+    if hasattr(types, "UnionType"):
+        def test_or(self):
+            X = TypeVar('X')
+            # use a string because str doesn't implement
+            # __or__/__ror__ itself
+            self.assertEqual(X | "x", Union[X, "x"])
+            self.assertEqual("x" | X, Union["x", X])
+            # make sure the order is correct
+            self.assertEqual(get_args(X | "x"), (X, typing.ForwardRef("x")))
+            self.assertEqual(get_args("x" | X), (typing.ForwardRef("x"), X))
+
+    def test_union_constrained(self):
+        A = TypeVar('A', str, bytes)
+        self.assertNotEqual(Union[A, str], Union[A])
+
+    def test_repr(self):
+        self.assertEqual(repr(T), '~T')
+        self.assertEqual(repr(KT), '~KT')
+        self.assertEqual(repr(VT), '~VT')
+        self.assertEqual(repr(AnyStr), '~AnyStr')
+        T_co = TypeVar('T_co', covariant=True)
+        self.assertEqual(repr(T_co), '+T_co')
+        T_contra = TypeVar('T_contra', contravariant=True)
+        self.assertEqual(repr(T_contra), '-T_contra')
+
+    def test_no_redefinition(self):
+        self.assertNotEqual(TypeVar('T'), TypeVar('T'))
+        self.assertNotEqual(TypeVar('T', int, str), TypeVar('T', int, str))
+
+    def test_cannot_subclass(self):
+        with self.assertRaises(TypeError):
+            class V(TypeVar): pass
+        T = TypeVar("T")
+        with self.assertRaises(TypeError):
+            class V(T): pass
+
+    def test_cannot_instantiate_vars(self):
+        with self.assertRaises(TypeError):
+            TypeVar('A')()
+
+    def test_bound_errors(self):
+        with self.assertRaises(TypeError):
+            TypeVar('X', bound=Union)
+        with self.assertRaises(TypeError):
+            TypeVar('X', str, float, bound=Employee)
+        with self.assertRaisesRegex(TypeError,
+                                    r"Bound must be a type\. Got \(1, 2\)\."):
+            TypeVar('X', bound=(1, 2))
+
+    # Technically we could run it on later versions of 3.7 and 3.8,
+    # but that's not worth the effort.
+    @skipUnless(TYPING_3_9_0, "Fix was not backported")
+    def test_missing__name__(self):
+        # See bpo-39942
+        code = ("import typing\n"
+                "T = typing.TypeVar('T')\n"
+                )
+        exec(code, {})
+
+    def test_no_bivariant(self):
+        with self.assertRaises(ValueError):
+            TypeVar('T', covariant=True, contravariant=True)
+
+    def test_cannot_combine_explicit_and_infer(self):
+        with self.assertRaises(ValueError):
+            TypeVar('T', covariant=True, infer_variance=True)
+        with self.assertRaises(ValueError):
+            TypeVar('T', contravariant=True, infer_variance=True)
+
 
 class TypeVarLikeDefaultsTests(BaseTestCase):
     def test_typevar(self):
         T = typing_extensions.TypeVar('T', default=int)
+        typing_T = typing.TypeVar('T')
         self.assertEqual(T.__default__, int)
+        self.assertIsInstance(T, typing_extensions.TypeVar)
+        self.assertIsInstance(T, typing.TypeVar)
+        self.assertIsInstance(typing_T, typing.TypeVar)
+        self.assertIsInstance(typing_T, typing_extensions.TypeVar)
 
         class A(Generic[T]): ...
         Alias = Optional[T]
 
     def test_typevar_none(self):
         U = typing_extensions.TypeVar('U')
         U_None = typing_extensions.TypeVar('U_None', default=None)
         self.assertEqual(U.__default__, None)
         self.assertEqual(U_None.__default__, type(None))
 
     def test_paramspec(self):
         P = ParamSpec('P', default=(str, int))
         self.assertEqual(P.__default__, (str, int))
+        self.assertIsInstance(P, ParamSpec)
+        if hasattr(typing, "ParamSpec"):
+            self.assertIsInstance(P, typing.ParamSpec)
+            typing_P = typing.ParamSpec('P')
+            self.assertIsInstance(typing_P, typing.ParamSpec)
+            self.assertIsInstance(typing_P, ParamSpec)
 
         class A(Generic[P]): ...
         Alias = typing.Callable[P, None]
 
     def test_typevartuple(self):
         Ts = TypeVarTuple('Ts', default=Unpack[Tuple[str, int]])
         self.assertEqual(Ts.__default__, Unpack[Tuple[str, int]])
+        self.assertIsInstance(Ts, TypeVarTuple)
+        if hasattr(typing, "TypeVarTuple"):
+            self.assertIsInstance(Ts, typing.TypeVarTuple)
+            typing_Ts = typing.TypeVarTuple('Ts')
+            self.assertIsInstance(typing_Ts, typing.TypeVarTuple)
+            self.assertIsInstance(typing_Ts, TypeVarTuple)
 
         class A(Generic[Unpack[Ts]]): ...
         Alias = Optional[Unpack[Ts]]
 
     def test_pickle(self):
         global U, U_co, U_contra, U_default  # pickle wants to reference the class by name
         U = typing_extensions.TypeVar('U')
@@ -3683,9 +4623,240 @@
                 self.assertEqual(z.__name__, typevar.__name__)
                 self.assertEqual(z.__covariant__, typevar.__covariant__)
                 self.assertEqual(z.__contravariant__, typevar.__contravariant__)
                 self.assertEqual(z.__bound__, typevar.__bound__)
                 self.assertEqual(z.__infer_variance__, typevar.__infer_variance__)
 
 
+class BufferTests(BaseTestCase):
+    def test(self):
+        self.assertIsInstance(memoryview(b''), Buffer)
+        self.assertIsInstance(bytearray(), Buffer)
+        self.assertIsInstance(b"x", Buffer)
+        self.assertNotIsInstance(1, Buffer)
+
+        self.assertIsSubclass(bytearray, Buffer)
+        self.assertIsSubclass(memoryview, Buffer)
+        self.assertIsSubclass(bytes, Buffer)
+        self.assertNotIsSubclass(int, Buffer)
+
+        class MyRegisteredBuffer:
+            def __buffer__(self, flags: int) -> memoryview:
+                return memoryview(b'')
+
+        # On 3.12, collections.abc.Buffer does a structural compatibility check
+        if TYPING_3_12_0:
+            self.assertIsInstance(MyRegisteredBuffer(), Buffer)
+            self.assertIsSubclass(MyRegisteredBuffer, Buffer)
+        else:
+            self.assertNotIsInstance(MyRegisteredBuffer(), Buffer)
+            self.assertNotIsSubclass(MyRegisteredBuffer, Buffer)
+        Buffer.register(MyRegisteredBuffer)
+        self.assertIsInstance(MyRegisteredBuffer(), Buffer)
+        self.assertIsSubclass(MyRegisteredBuffer, Buffer)
+
+        class MySubclassedBuffer(Buffer):
+            def __buffer__(self, flags: int) -> memoryview:
+                return memoryview(b'')
+
+        self.assertIsInstance(MySubclassedBuffer(), Buffer)
+        self.assertIsSubclass(MySubclassedBuffer, Buffer)
+
+
+class GetOriginalBasesTests(BaseTestCase):
+    def test_basics(self):
+        T = TypeVar('T')
+        class A: pass
+        class B(Generic[T]): pass
+        class C(B[int]): pass
+        class D(B[str], float): pass
+        self.assertEqual(get_original_bases(A), (object,))
+        self.assertEqual(get_original_bases(B), (Generic[T],))
+        self.assertEqual(get_original_bases(C), (B[int],))
+        self.assertEqual(get_original_bases(int), (object,))
+        self.assertEqual(get_original_bases(D), (B[str], float))
+
+        with self.assertRaisesRegex(TypeError, "Expected an instance of type"):
+            get_original_bases(object())
+
+    @skipUnless(TYPING_3_9_0, "PEP 585 is yet to be")
+    def test_builtin_generics(self):
+        class E(list[T]): pass
+        class F(list[int]): pass
+
+        self.assertEqual(get_original_bases(E), (list[T],))
+        self.assertEqual(get_original_bases(F), (list[int],))
+
+    def test_namedtuples(self):
+        # On 3.12, this should work well with typing.NamedTuple and typing_extensions.NamedTuple
+        # On lower versions, it will only work fully with typing_extensions.NamedTuple
+        if sys.version_info >= (3, 12):
+            namedtuple_classes = (typing.NamedTuple, typing_extensions.NamedTuple)
+        else:
+            namedtuple_classes = (typing_extensions.NamedTuple,)
+
+        for NamedTuple in namedtuple_classes:  # noqa: F402
+            with self.subTest(cls=NamedTuple):
+                class ClassBasedNamedTuple(NamedTuple):
+                    x: int
+
+                class GenericNamedTuple(NamedTuple, Generic[T]):
+                    x: T
+
+                CallBasedNamedTuple = NamedTuple("CallBasedNamedTuple", [("x", int)])
+
+                self.assertIs(
+                    get_original_bases(ClassBasedNamedTuple)[0], NamedTuple
+                )
+                self.assertEqual(
+                    get_original_bases(GenericNamedTuple),
+                    (NamedTuple, Generic[T])
+                )
+                self.assertIs(
+                    get_original_bases(CallBasedNamedTuple)[0], NamedTuple
+                )
+
+    def test_typeddicts(self):
+        # On 3.12, this should work well with typing.TypedDict and typing_extensions.TypedDict
+        # On lower versions, it will only work fully with typing_extensions.TypedDict
+        if sys.version_info >= (3, 12):
+            typeddict_classes = (typing.TypedDict, typing_extensions.TypedDict)
+        else:
+            typeddict_classes = (typing_extensions.TypedDict,)
+
+        for TypedDict in typeddict_classes:  # noqa: F402
+            with self.subTest(cls=TypedDict):
+                class ClassBasedTypedDict(TypedDict):
+                    x: int
+
+                class GenericTypedDict(TypedDict, Generic[T]):
+                    x: T
+
+                CallBasedTypedDict = TypedDict("CallBasedTypedDict", {"x": int})
+
+                self.assertIs(
+                    get_original_bases(ClassBasedTypedDict)[0],
+                    TypedDict
+                )
+                self.assertEqual(
+                    get_original_bases(GenericTypedDict),
+                    (TypedDict, Generic[T])
+                )
+                self.assertIs(
+                    get_original_bases(CallBasedTypedDict)[0],
+                    TypedDict
+                )
+
+
+class TypeAliasTypeTests(BaseTestCase):
+    def test_attributes(self):
+        Simple = TypeAliasType("Simple", int)
+        self.assertEqual(Simple.__name__, "Simple")
+        self.assertIs(Simple.__value__, int)
+        self.assertEqual(Simple.__type_params__, ())
+        self.assertEqual(Simple.__parameters__, ())
+
+        T = TypeVar("T")
+        ListOrSetT = TypeAliasType("ListOrSetT", Union[List[T], Set[T]], type_params=(T,))
+        self.assertEqual(ListOrSetT.__name__, "ListOrSetT")
+        self.assertEqual(ListOrSetT.__value__, Union[List[T], Set[T]])
+        self.assertEqual(ListOrSetT.__type_params__, (T,))
+        self.assertEqual(ListOrSetT.__parameters__, (T,))
+
+        Ts = TypeVarTuple("Ts")
+        Variadic = TypeAliasType("Variadic", Tuple[int, Unpack[Ts]], type_params=(Ts,))
+        self.assertEqual(Variadic.__name__, "Variadic")
+        self.assertEqual(Variadic.__value__, Tuple[int, Unpack[Ts]])
+        self.assertEqual(Variadic.__type_params__, (Ts,))
+        self.assertEqual(Variadic.__parameters__, tuple(iter(Ts)))
+
+    def test_cannot_set_attributes(self):
+        Simple = TypeAliasType("Simple", int)
+        with self.assertRaisesRegex(AttributeError, "readonly attribute"):
+            Simple.__name__ = "NewName"
+        with self.assertRaisesRegex(
+            AttributeError,
+            "attribute '__value__' of 'typing.TypeAliasType' objects is not writable",
+        ):
+            Simple.__value__ = str
+        with self.assertRaisesRegex(
+            AttributeError,
+            "attribute '__type_params__' of 'typing.TypeAliasType' objects is not writable",
+        ):
+            Simple.__type_params__ = (T,)
+        with self.assertRaisesRegex(
+            AttributeError,
+            "attribute '__parameters__' of 'typing.TypeAliasType' objects is not writable",
+        ):
+            Simple.__parameters__ = (T,)
+        with self.assertRaisesRegex(
+            AttributeError,
+            "attribute '__module__' of 'typing.TypeAliasType' objects is not writable",
+        ):
+            Simple.__module__ = 42
+        with self.assertRaisesRegex(
+            AttributeError,
+            "'typing.TypeAliasType' object has no attribute 'some_attribute'",
+        ):
+            Simple.some_attribute = "not allowed"
+
+    def test_cannot_delete_attributes(self):
+        Simple = TypeAliasType("Simple", int)
+        with self.assertRaisesRegex(AttributeError, "readonly attribute"):
+            del Simple.__name__
+        with self.assertRaisesRegex(
+            AttributeError,
+            "attribute '__value__' of 'typing.TypeAliasType' objects is not writable",
+        ):
+            del Simple.__value__
+        with self.assertRaisesRegex(
+            AttributeError,
+            "'typing.TypeAliasType' object has no attribute 'some_attribute'",
+        ):
+            del Simple.some_attribute
+
+    def test_or(self):
+        Alias = TypeAliasType("Alias", int)
+        if sys.version_info >= (3, 10):
+            self.assertEqual(Alias | int, Union[Alias, int])
+            self.assertEqual(Alias | None, Union[Alias, None])
+            self.assertEqual(Alias | (int | str), Union[Alias, int | str])
+            self.assertEqual(Alias | list[float], Union[Alias, list[float]])
+        else:
+            with self.assertRaises(TypeError):
+                Alias | int
+        # Rejected on all versions
+        with self.assertRaises(TypeError):
+            Alias | "Ref"
+
+    def test_getitem(self):
+        ListOrSetT = TypeAliasType("ListOrSetT", Union[List[T], Set[T]], type_params=(T,))
+        subscripted = ListOrSetT[int]
+        self.assertEqual(get_args(subscripted), (int,))
+        self.assertIs(get_origin(subscripted), ListOrSetT)
+        with self.assertRaises(TypeError):
+            subscripted[str]
+
+        still_generic = ListOrSetT[Iterable[T]]
+        self.assertEqual(get_args(still_generic), (Iterable[T],))
+        self.assertIs(get_origin(still_generic), ListOrSetT)
+        fully_subscripted = still_generic[float]
+        self.assertEqual(get_args(fully_subscripted), (Iterable[float],))
+        self.assertIs(get_origin(fully_subscripted), ListOrSetT)
+
+    def test_pickle(self):
+        global Alias
+        Alias = TypeAliasType("Alias", int)
+        for proto in range(pickle.HIGHEST_PROTOCOL + 1):
+            with self.subTest(proto=proto):
+                pickled = pickle.dumps(Alias, proto)
+                unpickled = pickle.loads(pickled)
+                self.assertIs(unpickled, Alias)
+
+    def test_no_instance_subclassing(self):
+        with self.assertRaises(TypeError):
+            class MyAlias(TypeAliasType):
+                pass
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `typing_extensions-4.5.0/src/typing_extensions.py` & `typing_extensions-4.6.0/src/typing_extensions.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,52 +29,61 @@
     # ABCs (from collections.abc).
     'Awaitable',
     'AsyncIterator',
     'AsyncIterable',
     'Coroutine',
     'AsyncGenerator',
     'AsyncContextManager',
+    'Buffer',
     'ChainMap',
 
     # Concrete collection types.
     'ContextManager',
     'Counter',
     'Deque',
     'DefaultDict',
     'NamedTuple',
     'OrderedDict',
     'TypedDict',
 
     # Structural checks, a.k.a. protocols.
+    'SupportsAbs',
+    'SupportsBytes',
+    'SupportsComplex',
+    'SupportsFloat',
     'SupportsIndex',
+    'SupportsInt',
+    'SupportsRound',
 
     # One-off things.
     'Annotated',
     'assert_never',
     'assert_type',
     'clear_overloads',
     'dataclass_transform',
     'deprecated',
     'get_overloads',
     'final',
     'get_args',
     'get_origin',
+    'get_original_bases',
     'get_type_hints',
     'IntVar',
     'is_typeddict',
     'Literal',
     'NewType',
     'overload',
     'override',
     'Protocol',
     'reveal_type',
     'runtime',
     'runtime_checkable',
     'Text',
     'TypeAlias',
+    'TypeAliasType',
     'TypeGuard',
     'TYPE_CHECKING',
     'Never',
     'NoReturn',
     'Required',
     'NotRequired',
 ]
@@ -82,15 +91,21 @@
 # for backward compatibility
 PEP_560 = True
 GenericMeta = type
 
 # The functions below are modified copies of typing internal helpers.
 # They are needed by _ProtocolMeta and they provide support for PEP 646.
 
-_marker = object()
+
+class _Sentinel:
+    def __repr__(self):
+        return "<sentinel>"
+
+
+_marker = _Sentinel()
 
 
 def _check_generic(cls, parameters, elen=_marker):
     """Check correct count for parameters of a generic cls (internal helper).
     This gives a nice error message in case of count mismatch.
     """
     if not elen:
@@ -256,43 +271,92 @@
         return f
 
 
 def IntVar(name):
     return typing.TypeVar(name)
 
 
-# 3.8+:
-if hasattr(typing, 'Literal'):
+# A Literal bug was fixed in 3.11.0, 3.10.1 and 3.9.8
+if sys.version_info >= (3, 10, 1):
     Literal = typing.Literal
-# 3.7:
 else:
+    def _flatten_literal_params(parameters):
+        """An internal helper for Literal creation: flatten Literals among parameters"""
+        params = []
+        for p in parameters:
+            if isinstance(p, _LiteralGenericAlias):
+                params.extend(p.__args__)
+            else:
+                params.append(p)
+        return tuple(params)
+
+    def _value_and_type_iter(params):
+        for p in params:
+            yield p, type(p)
+
+    class _LiteralGenericAlias(typing._GenericAlias, _root=True):
+        def __eq__(self, other):
+            if not isinstance(other, _LiteralGenericAlias):
+                return NotImplemented
+            these_args_deduped = set(_value_and_type_iter(self.__args__))
+            other_args_deduped = set(_value_and_type_iter(other.__args__))
+            return these_args_deduped == other_args_deduped
+
+        def __hash__(self):
+            return hash(frozenset(_value_and_type_iter(self.__args__)))
+
     class _LiteralForm(typing._SpecialForm, _root=True):
+        def __init__(self, doc: str):
+            self._name = 'Literal'
+            self._doc = self.__doc__ = doc
 
         def __repr__(self):
             return 'typing_extensions.' + self._name
 
         def __getitem__(self, parameters):
-            return typing._GenericAlias(self, parameters)
+            if not isinstance(parameters, tuple):
+                parameters = (parameters,)
+
+            parameters = _flatten_literal_params(parameters)
+
+            val_type_pairs = list(_value_and_type_iter(parameters))
+            try:
+                deduped_pairs = set(val_type_pairs)
+            except TypeError:
+                # unhashable parameters
+                pass
+            else:
+                # similar logic to typing._deduplicate on Python 3.9+
+                if len(deduped_pairs) < len(val_type_pairs):
+                    new_parameters = []
+                    for pair in val_type_pairs:
+                        if pair in deduped_pairs:
+                            new_parameters.append(pair[0])
+                            deduped_pairs.remove(pair)
+                    assert not deduped_pairs, deduped_pairs
+                    parameters = tuple(new_parameters)
 
-    Literal = _LiteralForm('Literal',
-                           doc="""A type that can be used to indicate to type checkers
+            return _LiteralGenericAlias(self, parameters)
+
+    Literal = _LiteralForm(doc="""\
+                           A type that can be used to indicate to type checkers
                            that the corresponding value has a value literally equivalent
                            to the provided parameter. For example:
 
                                var: Literal[4] = 4
 
                            The type checker understands that 'var' is literally equal to
                            the value 4 and no other value.
 
                            Literal[...] cannot be subclassed. There is no runtime
                            checking verifying that the parameter is actually a value
                            instead of a type.""")
 
 
-_overload_dummy = typing._overload_dummy  # noqa
+_overload_dummy = typing._overload_dummy
 
 
 if hasattr(typing, "get_overloads"):  # 3.11+
     overload = typing.overload
     get_overloads = typing.get_overloads
     clear_overloads = typing.clear_overloads
 else:
@@ -379,58 +443,72 @@
 # 3.7.0-3.7.2
 else:
     OrderedDict = typing._alias(collections.OrderedDict, (KT, VT))
 
 Counter = typing.Counter
 ChainMap = typing.ChainMap
 AsyncGenerator = typing.AsyncGenerator
-NewType = typing.NewType
 Text = typing.Text
 TYPE_CHECKING = typing.TYPE_CHECKING
 
 
-_PROTO_WHITELIST = ['Callable', 'Awaitable',
-                    'Iterable', 'Iterator', 'AsyncIterable', 'AsyncIterator',
-                    'Hashable', 'Sized', 'Container', 'Collection', 'Reversible',
-                    'ContextManager', 'AsyncContextManager']
+_PROTO_ALLOWLIST = {
+    'collections.abc': [
+        'Callable', 'Awaitable', 'Iterable', 'Iterator', 'AsyncIterable',
+        'Hashable', 'Sized', 'Container', 'Collection', 'Reversible',
+    ],
+    'contextlib': ['AbstractContextManager', 'AbstractAsyncContextManager'],
+}
+
+
+_EXCLUDED_ATTRS = {
+    "__abstractmethods__", "__annotations__", "__weakref__", "_is_protocol",
+    "_is_runtime_protocol", "__dict__", "__slots__", "__parameters__",
+    "__orig_bases__", "__module__", "_MutableMapping__marker", "__doc__",
+    "__subclasshook__", "__orig_class__", "__init__", "__new__",
+    "__protocol_attrs__", "__callable_proto_members_only__",
+}
+
+if sys.version_info < (3, 8):
+    _EXCLUDED_ATTRS |= {
+        "_gorg", "__next_in_mro__", "__extra__", "__tree_hash__", "__args__",
+        "__origin__"
+    }
+
+if sys.version_info >= (3, 9):
+    _EXCLUDED_ATTRS.add("__class_getitem__")
+
+if sys.version_info >= (3, 12):
+    _EXCLUDED_ATTRS.add("__type_params__")
+
+_EXCLUDED_ATTRS = frozenset(_EXCLUDED_ATTRS)
 
 
 def _get_protocol_attrs(cls):
     attrs = set()
     for base in cls.__mro__[:-1]:  # without object
-        if base.__name__ in ('Protocol', 'Generic'):
+        if base.__name__ in {'Protocol', 'Generic'}:
             continue
         annotations = getattr(base, '__annotations__', {})
-        for attr in list(base.__dict__.keys()) + list(annotations.keys()):
-            if (not attr.startswith('_abc_') and attr not in (
-                    '__abstractmethods__', '__annotations__', '__weakref__',
-                    '_is_protocol', '_is_runtime_protocol', '__dict__',
-                    '__args__', '__slots__',
-                    '__next_in_mro__', '__parameters__', '__origin__',
-                    '__orig_bases__', '__extra__', '__tree_hash__',
-                    '__doc__', '__subclasshook__', '__init__', '__new__',
-                    '__module__', '_MutableMapping__marker', '_gorg')):
+        for attr in (*base.__dict__, *annotations):
+            if (not attr.startswith('_abc_') and attr not in _EXCLUDED_ATTRS):
                 attrs.add(attr)
     return attrs
 
 
-def _is_callable_members_only(cls):
-    return all(callable(getattr(cls, attr, None)) for attr in _get_protocol_attrs(cls))
-
-
 def _maybe_adjust_parameters(cls):
     """Helper function used in Protocol.__init_subclass__ and _TypedDictMeta.__new__.
 
     The contents of this function are very similar
     to logic found in typing.Generic.__init_subclass__
     on the CPython main branch.
     """
     tvars = []
     if '__orig_bases__' in cls.__dict__:
-        tvars = typing._collect_type_vars(cls.__orig_bases__)
+        tvars = _collect_type_vars(cls.__orig_bases__)
         # Look for Generic[T1, ..., Tn] or Protocol[T1, ..., Tn].
         # If found, tvars must be a subset of it.
         # If not found, tvars is it.
         # Also check for and reject plain Generic,
         # and reject multiple Generic[...] and/or Protocol[...].
         gvars = None
         for base in cls.__orig_bases__:
@@ -453,41 +531,90 @@
                 s_args = ', '.join(str(g) for g in gvars)
                 raise TypeError(f"Some type variables ({s_vars}) are"
                                 f" not listed in {the_base}[{s_args}]")
             tvars = gvars
     cls.__parameters__ = tuple(tvars)
 
 
-# 3.8+
-if hasattr(typing, 'Protocol'):
+def _caller(depth=2):
+    try:
+        return sys._getframe(depth).f_globals.get('__name__', '__main__')
+    except (AttributeError, ValueError):  # For platforms without _getframe()
+        return None
+
+
+# The performance of runtime-checkable protocols is significantly improved on Python 3.12,
+# so we backport the 3.12 version of Protocol to Python <=3.11
+if sys.version_info >= (3, 12):
     Protocol = typing.Protocol
-# 3.7
+    runtime_checkable = typing.runtime_checkable
 else:
+    def _allow_reckless_class_checks(depth=4):
+        """Allow instance and class checks for special stdlib modules.
+        The abc and functools modules indiscriminately call isinstance() and
+        issubclass() on the whole MRO of a user class, which may contain protocols.
+        """
+        return _caller(depth) in {'abc', 'functools', None}
 
     def _no_init(self, *args, **kwargs):
         if type(self)._is_protocol:
             raise TypeError('Protocols cannot be instantiated')
 
-    class _ProtocolMeta(abc.ABCMeta):  # noqa: B024
-        # This metaclass is a bit unfortunate and exists only because of the lack
-        # of __instancehook__.
+    class _ProtocolMeta(abc.ABCMeta):
+        # This metaclass is somewhat unfortunate,
+        # but is necessary for several reasons...
+        def __init__(cls, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            if getattr(cls, "_is_protocol", False):
+                cls.__protocol_attrs__ = _get_protocol_attrs(cls)
+                # PEP 544 prohibits using issubclass()
+                # with protocols that have non-method members.
+                cls.__callable_proto_members_only__ = all(
+                    callable(getattr(cls, attr, None)) for attr in cls.__protocol_attrs__
+                )
+
+        def __subclasscheck__(cls, other):
+            if (
+                getattr(cls, '_is_protocol', False)
+                and not cls.__callable_proto_members_only__
+                and not _allow_reckless_class_checks(depth=3)
+            ):
+                raise TypeError(
+                    "Protocols with non-method members don't support issubclass()"
+                )
+            return super().__subclasscheck__(other)
+
         def __instancecheck__(cls, instance):
             # We need this method for situations where attributes are
             # assigned in __init__.
-            if ((not getattr(cls, '_is_protocol', False) or
-                 _is_callable_members_only(cls)) and
-                    issubclass(instance.__class__, cls)):
+            if not getattr(cls, "_is_protocol", False):
+                # i.e., it's a concrete subclass of a protocol
+                return super().__instancecheck__(instance)
+
+            if (
+                not getattr(cls, '_is_runtime_protocol', False) and
+                not _allow_reckless_class_checks(depth=2)
+            ):
+                raise TypeError("Instance and class checks can only be used with"
+                                " @runtime_checkable protocols")
+
+            if super().__instancecheck__(instance):
+                return True
+
+            for attr in cls.__protocol_attrs__:
+                try:
+                    val = inspect.getattr_static(instance, attr)
+                except AttributeError:
+                    break
+                if val is None and callable(getattr(cls, attr, None)):
+                    break
+            else:
                 return True
-            if cls._is_protocol:
-                if all(hasattr(instance, attr) and
-                       (not callable(getattr(cls, attr, None)) or
-                        getattr(instance, attr) is not None)
-                       for attr in _get_protocol_attrs(cls)):
-                    return True
-            return super().__instancecheck__(instance)
+
+            return False
 
     class Protocol(metaclass=_ProtocolMeta):
         # There is quite a lot of overlapping code with typing.Generic.
         # Unfortunately it is hard to avoid this while these live in two different
         # modules. The duplicated code will be removed when Protocol is moved to typing.
         """Base class for protocol classes. Protocol classes are defined as::
 
@@ -515,14 +642,15 @@
 
             class GenProto(Protocol[T]):
                 def meth(self) -> T:
                     ...
         """
         __slots__ = ()
         _is_protocol = True
+        _is_runtime_protocol = False
 
         def __new__(cls, *args, **kwds):
             if cls is Protocol:
                 raise TypeError("Type Protocol cannot be instantiated; "
                                 "it can only be used as a base class")
             return super().__new__(cls)
 
@@ -530,15 +658,15 @@
         def __class_getitem__(cls, params):
             if not isinstance(params, tuple):
                 params = (params,)
             if not params and cls is not typing.Tuple:
                 raise TypeError(
                     f"Parameter list to {cls.__qualname__}[...] cannot be empty")
             msg = "Parameters to generic types must be types."
-            params = tuple(typing._type_check(p, msg) for p in params)  # noqa
+            params = tuple(typing._type_check(p, msg) for p in params)
             if cls is Protocol:
                 # Generic can only be subscripted with unique type variables.
                 if not all(isinstance(p, typing.TypeVar) for p in params):
                     i = 0
                     while isinstance(params[i], typing.TypeVar):
                         i += 1
                     raise TypeError(
@@ -566,27 +694,22 @@
                 cls._is_protocol = any(b is Protocol for b in cls.__bases__)
 
             # Set (or override) the protocol subclass hook.
             def _proto_hook(other):
                 if not cls.__dict__.get('_is_protocol', None):
                     return NotImplemented
                 if not getattr(cls, '_is_runtime_protocol', False):
-                    if sys._getframe(2).f_globals['__name__'] in ['abc', 'functools']:
+                    if _allow_reckless_class_checks():
                         return NotImplemented
                     raise TypeError("Instance and class checks can only be used with"
                                     " @runtime protocols")
-                if not _is_callable_members_only(cls):
-                    if sys._getframe(2).f_globals['__name__'] in ['abc', 'functools']:
-                        return NotImplemented
-                    raise TypeError("Protocols with non-method members"
-                                    " don't support issubclass()")
                 if not isinstance(other, type):
                     # Same error as for issubclass(1, int)
                     raise TypeError('issubclass() arg 1 must be a class')
-                for attr in _get_protocol_attrs(cls):
+                for attr in cls.__protocol_attrs__:
                     for base in other.__mro__:
                         if attr in base.__dict__:
                             if base.__dict__[attr] is None:
                                 return NotImplemented
                             break
                         annotations = getattr(base, '__annotations__', {})
                         if (isinstance(annotations, typing.Mapping) and
@@ -603,77 +726,138 @@
             # We have nothing more to do for non-protocols.
             if not cls._is_protocol:
                 return
 
             # Check consistency of bases.
             for base in cls.__bases__:
                 if not (base in (object, typing.Generic) or
-                        base.__module__ == 'collections.abc' and
-                        base.__name__ in _PROTO_WHITELIST or
+                        base.__module__ in _PROTO_ALLOWLIST and
+                        base.__name__ in _PROTO_ALLOWLIST[base.__module__] or
                         isinstance(base, _ProtocolMeta) and base._is_protocol):
                     raise TypeError('Protocols can only inherit from other'
                                     f' protocols, got {repr(base)}')
-            cls.__init__ = _no_init
-
+            if cls.__init__ is Protocol.__init__:
+                cls.__init__ = _no_init
 
-# 3.8+
-if hasattr(typing, 'runtime_checkable'):
-    runtime_checkable = typing.runtime_checkable
-# 3.7
-else:
     def runtime_checkable(cls):
         """Mark a protocol class as a runtime protocol, so that it
         can be used with isinstance() and issubclass(). Raise TypeError
         if applied to a non-protocol class.
 
         This allows a simple-minded structural check very similar to the
         one-offs in collections.abc such as Hashable.
         """
-        if not isinstance(cls, _ProtocolMeta) or not cls._is_protocol:
+        if not (
+            (isinstance(cls, _ProtocolMeta) or issubclass(cls, typing.Generic))
+            and getattr(cls, "_is_protocol", False)
+        ):
             raise TypeError('@runtime_checkable can be only applied to protocol classes,'
                             f' got {cls!r}')
         cls._is_runtime_protocol = True
         return cls
 
 
 # Exists for backwards compatibility.
 runtime = runtime_checkable
 
 
-# 3.8+
-if hasattr(typing, 'SupportsIndex'):
+# Our version of runtime-checkable protocols is faster on Python 3.7-3.11
+if sys.version_info >= (3, 12):
+    SupportsInt = typing.SupportsInt
+    SupportsFloat = typing.SupportsFloat
+    SupportsComplex = typing.SupportsComplex
+    SupportsBytes = typing.SupportsBytes
     SupportsIndex = typing.SupportsIndex
-# 3.7
+    SupportsAbs = typing.SupportsAbs
+    SupportsRound = typing.SupportsRound
 else:
     @runtime_checkable
+    class SupportsInt(Protocol):
+        """An ABC with one abstract method __int__."""
+        __slots__ = ()
+
+        @abc.abstractmethod
+        def __int__(self) -> int:
+            pass
+
+    @runtime_checkable
+    class SupportsFloat(Protocol):
+        """An ABC with one abstract method __float__."""
+        __slots__ = ()
+
+        @abc.abstractmethod
+        def __float__(self) -> float:
+            pass
+
+    @runtime_checkable
+    class SupportsComplex(Protocol):
+        """An ABC with one abstract method __complex__."""
+        __slots__ = ()
+
+        @abc.abstractmethod
+        def __complex__(self) -> complex:
+            pass
+
+    @runtime_checkable
+    class SupportsBytes(Protocol):
+        """An ABC with one abstract method __bytes__."""
+        __slots__ = ()
+
+        @abc.abstractmethod
+        def __bytes__(self) -> bytes:
+            pass
+
+    @runtime_checkable
     class SupportsIndex(Protocol):
         __slots__ = ()
 
         @abc.abstractmethod
         def __index__(self) -> int:
             pass
 
+    @runtime_checkable
+    class SupportsAbs(Protocol[T_co]):
+        """
+        An ABC with one abstract method __abs__ that is covariant in its return type.
+        """
+        __slots__ = ()
 
-if hasattr(typing, "Required"):
+        @abc.abstractmethod
+        def __abs__(self) -> T_co:
+            pass
+
+    @runtime_checkable
+    class SupportsRound(Protocol[T_co]):
+        """
+        An ABC with one abstract method __round__ that is covariant in its return type.
+        """
+        __slots__ = ()
+
+        @abc.abstractmethod
+        def __round__(self, ndigits: int = 0) -> T_co:
+            pass
+
+
+if sys.version_info >= (3, 12):
     # The standard library TypedDict in Python 3.8 does not store runtime information
     # about which (if any) keys are optional.  See https://bugs.python.org/issue38834
     # The standard library TypedDict in Python 3.9.0/1 does not honour the "total"
     # keyword with old-style TypedDict().  See https://bugs.python.org/issue42059
     # The standard library TypedDict below Python 3.11 does not store runtime
     # information about optional and required keys when using Required or NotRequired.
     # Generic TypedDicts are also impossible using typing.TypedDict on Python <3.11.
+    # Aaaand on 3.12 we add __orig_bases__ to TypedDict
+    # to enable better runtime introspection.
     TypedDict = typing.TypedDict
     _TypedDictMeta = typing._TypedDictMeta
     is_typeddict = typing.is_typeddict
 else:
     def _check_fails(cls, other):
         try:
-            if sys._getframe(1).f_globals['__name__'] not in ['abc',
-                                                              'functools',
-                                                              'typing']:
+            if _caller() not in {'abc', 'functools', 'typing'}:
                 # Typed dicts are only for static structural subtyping.
                 raise TypeError('TypedDict does not support instance and class checks')
         except (AttributeError, ValueError):
             pass
         return False
 
     def _dict_new(*args, **kwargs):
@@ -688,47 +872,53 @@
         if not args:
             raise TypeError('TypedDict.__new__(): not enough arguments')
         _, args = args[0], args[1:]  # allow the "cls" keyword be passed
         if args:
             typename, args = args[0], args[1:]  # allow the "_typename" keyword be passed
         elif '_typename' in kwargs:
             typename = kwargs.pop('_typename')
-            import warnings
             warnings.warn("Passing '_typename' as keyword argument is deprecated",
                           DeprecationWarning, stacklevel=2)
         else:
             raise TypeError("TypedDict.__new__() missing 1 required positional "
                             "argument: '_typename'")
         if args:
             try:
                 fields, = args  # allow the "_fields" keyword be passed
             except ValueError:
                 raise TypeError('TypedDict.__new__() takes from 2 to 3 '
                                 f'positional arguments but {len(args) + 2} '
                                 'were given')
         elif '_fields' in kwargs and len(kwargs) == 1:
             fields = kwargs.pop('_fields')
-            import warnings
             warnings.warn("Passing '_fields' as keyword argument is deprecated",
                           DeprecationWarning, stacklevel=2)
         else:
             fields = None
 
         if fields is None:
             fields = kwargs
         elif kwargs:
             raise TypeError("TypedDict takes either a dict or keyword arguments,"
                             " but not both")
 
+        if kwargs:
+            warnings.warn(
+                "The kwargs-based syntax for TypedDict definitions is deprecated, "
+                "may be removed in a future version, and may not be "
+                "understood by third-party type checkers.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
         ns = {'__annotations__': dict(fields)}
-        try:
+        module = _caller()
+        if module is not None:
             # Setting correct module is necessary to make typed dict classes pickleable.
-            ns['__module__'] = sys._getframe(1).f_globals.get('__name__', '__main__')
-        except (AttributeError, ValueError):
-            pass
+            ns['__module__'] = module
 
         return _TypedDictMeta(typename, (), ns, total=total)
 
     _typeddict_new.__text_signature__ = ('($cls, _typename, _fields=None,'
                                          ' /, *, total=True, **kwargs)')
 
     _TAKES_MODULE = "module" in inspect.signature(typing._type_check).parameters
@@ -747,17 +937,22 @@
             ns['__new__'] = _typeddict_new if name == 'TypedDict' else _dict_new
             # Don't insert typing.Generic into __bases__ here,
             # or Generic.__init_subclass__ will raise TypeError
             # in the super().__new__() call.
             # Instead, monkey-patch __bases__ onto the class after it's been created.
             tp_dict = super().__new__(cls, name, (dict,), ns)
 
-            if any(issubclass(base, typing.Generic) for base in bases):
+            is_generic = any(issubclass(base, typing.Generic) for base in bases)
+
+            if is_generic:
                 tp_dict.__bases__ = (typing.Generic, dict)
                 _maybe_adjust_parameters(tp_dict)
+            else:
+                # generic TypedDicts get __orig_bases__ from Generic
+                tp_dict.__orig_bases__ = bases or (TypedDict,)
 
             annotations = {}
             own_annotations = ns.get('__annotations__', {})
             msg = "TypedDict('Name', {f0: t0, f1: t1, ...}); each t must be a type"
             kwds = {"module": tp_dict.__module__} if _TAKES_MODULE else {}
             own_annotations = {
                 n: typing._type_check(tp, msg, **kwds)
@@ -868,35 +1063,32 @@
         """
         return __val
 
 
 if hasattr(typing, "Required"):
     get_type_hints = typing.get_type_hints
 else:
-    import functools
-    import types
-
     # replaces _strip_annotations()
     def _strip_extras(t):
         """Strips Annotated, Required and NotRequired from a given type."""
         if isinstance(t, _AnnotatedAlias):
             return _strip_extras(t.__origin__)
         if hasattr(t, "__origin__") and t.__origin__ in (Required, NotRequired):
             return _strip_extras(t.__args__[0])
         if isinstance(t, typing._GenericAlias):
             stripped_args = tuple(_strip_extras(a) for a in t.__args__)
             if stripped_args == t.__args__:
                 return t
             return t.copy_with(stripped_args)
-        if hasattr(types, "GenericAlias") and isinstance(t, types.GenericAlias):
+        if hasattr(_types, "GenericAlias") and isinstance(t, _types.GenericAlias):
             stripped_args = tuple(_strip_extras(a) for a in t.__args__)
             if stripped_args == t.__args__:
                 return t
-            return types.GenericAlias(t.__origin__, stripped_args)
-        if hasattr(types, "UnionType") and isinstance(t, types.UnionType):
+            return _types.GenericAlias(t.__origin__, stripped_args)
+        if hasattr(_types, "UnionType") and isinstance(t, _types.UnionType):
             stripped_args = tuple(_strip_extras(a) for a in t.__args__)
             if stripped_args == t.__args__:
                 return t
             return functools.reduce(operator.or_, stripped_args)
 
         return t
 
@@ -1151,50 +1343,70 @@
 
                                    Predicate: TypeAlias = Callable[..., bool]
 
                                It's invalid when used anywhere except as in the example
                                above.""")
 
 
+def _set_default(type_param, default):
+    if isinstance(default, (tuple, list)):
+        type_param.__default__ = tuple((typing._type_check(d, "Default must be a type")
+                                        for d in default))
+    elif default != _marker:
+        type_param.__default__ = typing._type_check(default, "Default must be a type")
+    else:
+        type_param.__default__ = None
+
+
+def _set_module(typevarlike):
+    # for pickling:
+    def_mod = _caller(depth=3)
+    if def_mod != 'typing_extensions':
+        typevarlike.__module__ = def_mod
+
+
 class _DefaultMixin:
     """Mixin for TypeVarLike defaults."""
 
     __slots__ = ()
+    __init__ = _set_default
 
-    def __init__(self, default):
-        if isinstance(default, (tuple, list)):
-            self.__default__ = tuple((typing._type_check(d, "Default must be a type")
-                                      for d in default))
-        elif default != _marker:
-            self.__default__ = typing._type_check(default, "Default must be a type")
-        else:
-            self.__default__ = None
+
+# Classes using this metaclass must provide a _backported_typevarlike ClassVar
+class _TypeVarLikeMeta(type):
+    def __instancecheck__(cls, __instance: Any) -> bool:
+        return isinstance(__instance, cls._backported_typevarlike)
 
 
 # Add default and infer_variance parameters from PEP 696 and 695
-class TypeVar(typing.TypeVar, _DefaultMixin, _root=True):
+class TypeVar(metaclass=_TypeVarLikeMeta):
     """Type variable."""
 
-    __module__ = 'typing'
+    _backported_typevarlike = typing.TypeVar
 
-    def __init__(self, name, *constraints, bound=None,
-                 covariant=False, contravariant=False,
-                 default=_marker, infer_variance=False):
-        super().__init__(name, *constraints, bound=bound, covariant=covariant,
-                         contravariant=contravariant)
-        _DefaultMixin.__init__(self, default)
-        self.__infer_variance__ = infer_variance
+    def __new__(cls, name, *constraints, bound=None,
+                covariant=False, contravariant=False,
+                default=_marker, infer_variance=False):
+        if hasattr(typing, "TypeAliasType"):
+            # PEP 695 implemented, can pass infer_variance to typing.TypeVar
+            typevar = typing.TypeVar(name, *constraints, bound=bound,
+                                     covariant=covariant, contravariant=contravariant,
+                                     infer_variance=infer_variance)
+        else:
+            typevar = typing.TypeVar(name, *constraints, bound=bound,
+                                     covariant=covariant, contravariant=contravariant)
+            if infer_variance and (covariant or contravariant):
+                raise ValueError("Variance cannot be specified with infer_variance.")
+            typevar.__infer_variance__ = infer_variance
+        _set_default(typevar, default)
+        _set_module(typevar)
+        return typevar
 
-        # for pickling:
-        try:
-            def_mod = sys._getframe(1).f_globals.get('__name__', '__main__')
-        except (AttributeError, ValueError):
-            def_mod = None
-        if def_mod != 'typing_extensions':
-            self.__module__ = def_mod
+    def __init_subclass__(cls) -> None:
+        raise TypeError(f"type '{__name__}.TypeVar' is not an acceptable base type")
 
 
 # Python 3.10+ has PEP 612
 if hasattr(typing, 'ParamSpecArgs'):
     ParamSpecArgs = typing.ParamSpecArgs
     ParamSpecKwargs = typing.ParamSpecKwargs
 # 3.7-3.9
@@ -1254,33 +1466,41 @@
             if not isinstance(other, ParamSpecKwargs):
                 return NotImplemented
             return self.__origin__ == other.__origin__
 
 # 3.10+
 if hasattr(typing, 'ParamSpec'):
 
-    # Add default Parameter - PEP 696
-    class ParamSpec(typing.ParamSpec, _DefaultMixin, _root=True):
-        """Parameter specification variable."""
-
-        __module__ = 'typing'
+    # Add default parameter - PEP 696
+    class ParamSpec(metaclass=_TypeVarLikeMeta):
+        """Parameter specification."""
+
+        _backported_typevarlike = typing.ParamSpec
+
+        def __new__(cls, name, *, bound=None,
+                    covariant=False, contravariant=False,
+                    infer_variance=False, default=_marker):
+            if hasattr(typing, "TypeAliasType"):
+                # PEP 695 implemented, can pass infer_variance to typing.TypeVar
+                paramspec = typing.ParamSpec(name, bound=bound,
+                                             covariant=covariant,
+                                             contravariant=contravariant,
+                                             infer_variance=infer_variance)
+            else:
+                paramspec = typing.ParamSpec(name, bound=bound,
+                                             covariant=covariant,
+                                             contravariant=contravariant)
+                paramspec.__infer_variance__ = infer_variance
+
+            _set_default(paramspec, default)
+            _set_module(paramspec)
+            return paramspec
 
-        def __init__(self, name, *, bound=None, covariant=False, contravariant=False,
-                     default=_marker):
-            super().__init__(name, bound=bound, covariant=covariant,
-                             contravariant=contravariant)
-            _DefaultMixin.__init__(self, default)
-
-            # for pickling:
-            try:
-                def_mod = sys._getframe(1).f_globals.get('__name__', '__main__')
-            except (AttributeError, ValueError):
-                def_mod = None
-            if def_mod != 'typing_extensions':
-                self.__module__ = def_mod
+        def __init_subclass__(cls) -> None:
+            raise TypeError(f"type '{__name__}.ParamSpec' is not an acceptable base type")
 
 # 3.7-3.9
 else:
 
     # Inherits from list as a workaround for Callable checks in Python < 3.9.2.
     class ParamSpec(list, _DefaultMixin):
         """Parameter specification variable.
@@ -1337,35 +1557,35 @@
             return ParamSpecArgs(self)
 
         @property
         def kwargs(self):
             return ParamSpecKwargs(self)
 
         def __init__(self, name, *, bound=None, covariant=False, contravariant=False,
-                     default=_marker):
+                     infer_variance=False, default=_marker):
             super().__init__([self])
             self.__name__ = name
             self.__covariant__ = bool(covariant)
             self.__contravariant__ = bool(contravariant)
+            self.__infer_variance__ = bool(infer_variance)
             if bound:
                 self.__bound__ = typing._type_check(bound, 'Bound must be a type.')
             else:
                 self.__bound__ = None
             _DefaultMixin.__init__(self, default)
 
             # for pickling:
-            try:
-                def_mod = sys._getframe(1).f_globals.get('__name__', '__main__')
-            except (AttributeError, ValueError):
-                def_mod = None
+            def_mod = _caller()
             if def_mod != 'typing_extensions':
                 self.__module__ = def_mod
 
         def __repr__(self):
-            if self.__covariant__:
+            if self.__infer_variance__:
+                prefix = ''
+            elif self.__covariant__:
                 prefix = '+'
             elif self.__contravariant__:
                 prefix = '-'
             else:
                 prefix = '~'
             return prefix + self.__name__
 
@@ -1432,15 +1652,15 @@
     parameters = tuple(typing._type_check(p, msg) for p in parameters)
     return _ConcatenateGenericAlias(self, parameters)
 
 
 # 3.10+
 if hasattr(typing, 'Concatenate'):
     Concatenate = typing.Concatenate
-    _ConcatenateGenericAlias = typing._ConcatenateGenericAlias # noqa
+    _ConcatenateGenericAlias = typing._ConcatenateGenericAlias  # noqa: F811
 # 3.9
 elif sys.version_info[:2] >= (3, 9):
     @_TypeAliasForm
     def Concatenate(self, parameters):
         """Used in conjunction with ``ParamSpec`` and ``Callable`` to represent a
         higher order function which adds, removes or transforms parameters of a
         callable.
@@ -1789,36 +2009,76 @@
             m = Movie(
                 title='The Matrix',  # typechecker error if key is omitted
                 year=1999,
             )
         """)
 
 
-if hasattr(typing, "Unpack"):  # 3.11+
+_UNPACK_DOC = """\
+Type unpack operator.
+
+The type unpack operator takes the child types from some container type,
+such as `tuple[int, str]` or a `TypeVarTuple`, and 'pulls them out'. For
+example:
+
+  # For some generic class `Foo`:
+  Foo[Unpack[tuple[int, str]]]  # Equivalent to Foo[int, str]
+
+  Ts = TypeVarTuple('Ts')
+  # Specifies that `Bar` is generic in an arbitrary number of types.
+  # (Think of `Ts` as a tuple of an arbitrary number of individual
+  #  `TypeVar`s, which the `Unpack` is 'pulling out' directly into the
+  #  `Generic[]`.)
+  class Bar(Generic[Unpack[Ts]]): ...
+  Bar[int]  # Valid
+  Bar[int, str]  # Also valid
+
+From Python 3.11, this can also be done using the `*` operator:
+
+    Foo[*tuple[int, str]]
+    class Bar(Generic[*Ts]): ...
+
+The operator can also be used along with a `TypedDict` to annotate
+`**kwargs` in a function signature. For instance:
+
+  class Movie(TypedDict):
+    name: str
+    year: int
+
+  # This function expects two keyword arguments - *name* of type `str` and
+  # *year* of type `int`.
+  def foo(**kwargs: Unpack[Movie]): ...
+
+Note that there is only some runtime checking of this operator. Not
+everything the runtime allows may be accepted by static type checkers.
+
+For more information, see PEP 646 and PEP 692.
+"""
+
+
+if sys.version_info >= (3, 12):  # PEP 692 changed the repr of Unpack[]
     Unpack = typing.Unpack
+
+    def _is_unpack(obj):
+        return get_origin(obj) is Unpack
+
 elif sys.version_info[:2] >= (3, 9):
     class _UnpackSpecialForm(typing._SpecialForm, _root=True):
+        def __init__(self, getitem):
+            super().__init__(getitem)
+            self.__doc__ = _UNPACK_DOC
+
         def __repr__(self):
             return 'typing_extensions.' + self._name
 
     class _UnpackAlias(typing._GenericAlias, _root=True):
         __class__ = typing.TypeVar
 
     @_UnpackSpecialForm
     def Unpack(self, parameters):
-        """A special typing construct to unpack a variadic type. For example:
-
-            Shape = TypeVarTuple('Shape')
-            Batch = NewType('Batch', int)
-
-            def add_batch_axis(
-                x: Array[Unpack[Shape]]
-            ) -> Array[Batch, Unpack[Shape]]: ...
-
-        """
         item = typing._type_check(parameters, f'{self._name} accepts only a single type.')
         return _UnpackAlias(self, (item,))
 
     def _is_unpack(obj):
         return isinstance(obj, _UnpackAlias)
 
 else:
@@ -1830,48 +2090,36 @@
             return 'typing_extensions.' + self._name
 
         def __getitem__(self, parameters):
             item = typing._type_check(parameters,
                                       f'{self._name} accepts only a single type.')
             return _UnpackAlias(self, (item,))
 
-    Unpack = _UnpackForm(
-        'Unpack',
-        doc="""A special typing construct to unpack a variadic type. For example:
-
-            Shape = TypeVarTuple('Shape')
-            Batch = NewType('Batch', int)
-
-            def add_batch_axis(
-                x: Array[Unpack[Shape]]
-            ) -> Array[Batch, Unpack[Shape]]: ...
-
-        """)
+    Unpack = _UnpackForm('Unpack', doc=_UNPACK_DOC)
 
     def _is_unpack(obj):
         return isinstance(obj, _UnpackAlias)
 
 
 if hasattr(typing, "TypeVarTuple"):  # 3.11+
 
-    # Add default Parameter - PEP 696
-    class TypeVarTuple(typing.TypeVarTuple, _DefaultMixin, _root=True):
+    # Add default parameter - PEP 696
+    class TypeVarTuple(metaclass=_TypeVarLikeMeta):
         """Type variable tuple."""
 
-        def __init__(self, name, *, default=_marker):
-            super().__init__(name)
-            _DefaultMixin.__init__(self, default)
+        _backported_typevarlike = typing.TypeVarTuple
 
-            # for pickling:
-            try:
-                def_mod = sys._getframe(1).f_globals.get('__name__', '__main__')
-            except (AttributeError, ValueError):
-                def_mod = None
-            if def_mod != 'typing_extensions':
-                self.__module__ = def_mod
+        def __new__(cls, name, *, default=_marker):
+            tvt = typing.TypeVarTuple(name)
+            _set_default(tvt, default)
+            _set_module(tvt)
+            return tvt
+
+        def __init_subclass__(self, *args, **kwds):
+            raise TypeError("Cannot subclass special typing classes")
 
 else:
     class TypeVarTuple(_DefaultMixin):
         """Type variable tuple.
 
         Usage::
 
@@ -1921,18 +2169,15 @@
             yield self.__unpacked__
 
         def __init__(self, name, *, default=_marker):
             self.__name__ = name
             _DefaultMixin.__init__(self, default)
 
             # for pickling:
-            try:
-                def_mod = sys._getframe(1).f_globals.get('__name__', '__main__')
-            except (AttributeError, ValueError):
-                def_mod = None
+            def_mod = _caller()
             if def_mod != 'typing_extensions':
                 self.__module__ = def_mod
 
             self.__unpacked__ = Unpack[self]
 
         def __repr__(self):
             return self.__name__
@@ -2159,15 +2404,23 @@
             def g(x: int) -> int: ...
             @overload
             def g(x: str) -> int: ...
 
         When this decorator is applied to an object, the type checker
         will generate a diagnostic on usage of the deprecated object.
 
-        No runtime warning is issued. The decorator sets the ``__deprecated__``
+        The warning specified by ``category`` will be emitted on use
+        of deprecated objects. For functions, that happens on calls;
+        for classes, on instantiation. If the ``category`` is ``None``,
+        no warning is emitted. The ``stacklevel`` determines where the
+        warning is emitted. If it is ``1`` (the default), the warning
+        is emitted at the direct caller of the deprecated object; if it
+        is higher, it is emitted further up the stack.
+
+        The decorator sets the ``__deprecated__``
         attribute on the decorated object to the deprecation message
         passed to the decorator. If applied to an overload, the decorator
         must be after the ``@overload`` decorator for the attribute to
         exist on the overload as returned by ``get_overloads()``.
 
         See PEP 702 for details.
 
@@ -2219,26 +2472,21 @@
 #   counting generic parameters, so that when we subscript a generic,
 #   the runtime doesn't try to substitute the Unpack with the subscripted type.
 if not hasattr(typing, "TypeVarTuple"):
     typing._collect_type_vars = _collect_type_vars
     typing._check_generic = _check_generic
 
 
-# Backport typing.NamedTuple as it exists in Python 3.11.
+# Backport typing.NamedTuple as it exists in Python 3.12.
 # In 3.11, the ability to define generic `NamedTuple`s was supported.
 # This was explicitly disallowed in 3.9-3.10, and only half-worked in <=3.8.
-if sys.version_info >= (3, 11):
+# On 3.12, we added __orig_bases__ to call-based NamedTuples
+if sys.version_info >= (3, 12):
     NamedTuple = typing.NamedTuple
 else:
-    def _caller():
-        try:
-            return sys._getframe(2).f_globals.get('__name__', '__main__')
-        except (AttributeError, ValueError):  # For platforms without _getframe()
-            return None
-
     def _make_nmtuple(name, types, module, defaults=()):
         fields = [n for n, t in types]
         annotations = {n: typing._type_check(t, f"field {n} annotation must be a type")
                        for n, t in types}
         nm_tpl = collections.namedtuple(name, fields,
                                         defaults=defaults, module=module)
         nm_tpl.__annotations__ = nm_tpl.__new__.__annotations__ = annotations
@@ -2290,15 +2538,17 @@
 
     def NamedTuple(__typename, __fields=None, **kwargs):
         if __fields is None:
             __fields = kwargs.items()
         elif kwargs:
             raise TypeError("Either list of fields or keywords"
                             " can be provided to NamedTuple, not both")
-        return _make_nmtuple(__typename, __fields, module=_caller())
+        nt = _make_nmtuple(__typename, __fields, module=_caller())
+        nt.__orig_bases__ = (NamedTuple,)
+        return nt
 
     NamedTuple.__doc__ = typing.NamedTuple.__doc__
     _NamedTuple = type.__new__(_NamedTupleMeta, 'NamedTuple', (), {})
 
     # On 3.8+, alter the signature so that it matches typing.NamedTuple.
     # The signature of typing.NamedTuple on >=3.8 is invalid syntax in Python 3.7,
     # so just leave the signature as it is on 3.7.
@@ -2306,7 +2556,259 @@
         NamedTuple.__text_signature__ = '(typename, fields=None, /, **kwargs)'
 
     def _namedtuple_mro_entries(bases):
         assert NamedTuple in bases
         return (_NamedTuple,)
 
     NamedTuple.__mro_entries__ = _namedtuple_mro_entries
+
+
+if hasattr(collections.abc, "Buffer"):
+    Buffer = collections.abc.Buffer
+else:
+    class Buffer(abc.ABC):
+        """Base class for classes that implement the buffer protocol.
+
+        The buffer protocol allows Python objects to expose a low-level
+        memory buffer interface. Before Python 3.12, it is not possible
+        to implement the buffer protocol in pure Python code, or even
+        to check whether a class implements the buffer protocol. In
+        Python 3.12 and higher, the ``__buffer__`` method allows access
+        to the buffer protocol from Python code, and the
+        ``collections.abc.Buffer`` ABC allows checking whether a class
+        implements the buffer protocol.
+
+        To indicate support for the buffer protocol in earlier versions,
+        inherit from this ABC, either in a stub file or at runtime,
+        or use ABC registration. This ABC provides no methods, because
+        there is no Python-accessible methods shared by pre-3.12 buffer
+        classes. It is useful primarily for static checks.
+
+        """
+
+    # As a courtesy, register the most common stdlib buffer classes.
+    Buffer.register(memoryview)
+    Buffer.register(bytearray)
+    Buffer.register(bytes)
+
+
+# Backport of types.get_original_bases, available on 3.12+ in CPython
+if hasattr(_types, "get_original_bases"):
+    get_original_bases = _types.get_original_bases
+else:
+    def get_original_bases(__cls):
+        """Return the class's "original" bases prior to modification by `__mro_entries__`.
+
+        Examples::
+
+            from typing import TypeVar, Generic
+            from typing_extensions import NamedTuple, TypedDict
+
+            T = TypeVar("T")
+            class Foo(Generic[T]): ...
+            class Bar(Foo[int], float): ...
+            class Baz(list[str]): ...
+            Eggs = NamedTuple("Eggs", [("a", int), ("b", str)])
+            Spam = TypedDict("Spam", {"a": int, "b": str})
+
+            assert get_original_bases(Bar) == (Foo[int], float)
+            assert get_original_bases(Baz) == (list[str],)
+            assert get_original_bases(Eggs) == (NamedTuple,)
+            assert get_original_bases(Spam) == (TypedDict,)
+            assert get_original_bases(int) == (object,)
+        """
+        try:
+            return __cls.__orig_bases__
+        except AttributeError:
+            try:
+                return __cls.__bases__
+            except AttributeError:
+                raise TypeError(
+                    f'Expected an instance of type, not {type(__cls).__name__!r}'
+                ) from None
+
+
+# NewType is a class on Python 3.10+, making it pickleable
+# The error message for subclassing instances of NewType was improved on 3.11+
+if sys.version_info >= (3, 11):
+    NewType = typing.NewType
+else:
+    class NewType:
+        """NewType creates simple unique types with almost zero
+        runtime overhead. NewType(name, tp) is considered a subtype of tp
+        by static type checkers. At runtime, NewType(name, tp) returns
+        a dummy callable that simply returns its argument. Usage::
+            UserId = NewType('UserId', int)
+            def name_by_id(user_id: UserId) -> str:
+                ...
+            UserId('user')          # Fails type check
+            name_by_id(42)          # Fails type check
+            name_by_id(UserId(42))  # OK
+            num = UserId(5) + 1     # type: int
+        """
+
+        def __call__(self, obj):
+            return obj
+
+        def __init__(self, name, tp):
+            self.__qualname__ = name
+            if '.' in name:
+                name = name.rpartition('.')[-1]
+            self.__name__ = name
+            self.__supertype__ = tp
+            def_mod = _caller()
+            if def_mod != 'typing_extensions':
+                self.__module__ = def_mod
+
+        def __mro_entries__(self, bases):
+            # We defined __mro_entries__ to get a better error message
+            # if a user attempts to subclass a NewType instance. bpo-46170
+            supercls_name = self.__name__
+
+            class Dummy:
+                def __init_subclass__(cls):
+                    subcls_name = cls.__name__
+                    raise TypeError(
+                        f"Cannot subclass an instance of NewType. "
+                        f"Perhaps you were looking for: "
+                        f"`{subcls_name} = NewType({subcls_name!r}, {supercls_name})`"
+                    )
+
+            return (Dummy,)
+
+        def __repr__(self):
+            return f'{self.__module__}.{self.__qualname__}'
+
+        def __reduce__(self):
+            return self.__qualname__
+
+        if sys.version_info >= (3, 10):
+            # PEP 604 methods
+            # It doesn't make sense to have these methods on Python <3.10
+
+            def __or__(self, other):
+                return typing.Union[self, other]
+
+            def __ror__(self, other):
+                return typing.Union[other, self]
+
+
+if hasattr(typing, "TypeAliasType"):
+    TypeAliasType = typing.TypeAliasType
+else:
+    def _is_unionable(obj):
+        """Corresponds to is_unionable() in unionobject.c in CPython."""
+        return obj is None or isinstance(obj, (
+            type,
+            _types.GenericAlias,
+            _types.UnionType,
+            TypeAliasType,
+        ))
+
+    class TypeAliasType:
+        """Create named, parameterized type aliases.
+
+        This provides a backport of the new `type` statement in Python 3.12:
+
+            type ListOrSet[T] = list[T] | set[T]
+
+        is equivalent to:
+
+            T = TypeVar("T")
+            ListOrSet = TypeAliasType("ListOrSet", list[T] | set[T], type_params=(T,))
+
+        The name ListOrSet can then be used as an alias for the type it refers to.
+
+        The type_params argument should contain all the type parameters used
+        in the value of the type alias. If the alias is not generic, this
+        argument is omitted.
+
+        Static type checkers should only support type aliases declared using
+        TypeAliasType that follow these rules:
+
+        - The first argument (the name) must be a string literal.
+        - The TypeAliasType instance must be immediately assigned to a variable
+          of the same name. (For example, 'X = TypeAliasType("Y", int)' is invalid,
+          as is 'X, Y = TypeAliasType("X", int), TypeAliasType("Y", int)').
+
+        """
+
+        def __init__(self, name: str, value, *, type_params=()):
+            if not isinstance(name, str):
+                raise TypeError("TypeAliasType name must be a string")
+            self.__value__ = value
+            self.__type_params__ = type_params
+
+            parameters = []
+            for type_param in type_params:
+                if isinstance(type_param, TypeVarTuple):
+                    parameters.extend(type_param)
+                else:
+                    parameters.append(type_param)
+            self.__parameters__ = tuple(parameters)
+            def_mod = _caller()
+            if def_mod != 'typing_extensions':
+                self.__module__ = def_mod
+            # Setting this attribute closes the TypeAliasType from further modification
+            self.__name__ = name
+
+        def __setattr__(self, __name: str, __value: object) -> None:
+            if hasattr(self, "__name__"):
+                self._raise_attribute_error(__name)
+            super().__setattr__(__name, __value)
+
+        def __delattr__(self, __name: str) -> Never:
+            self._raise_attribute_error(__name)
+
+        def _raise_attribute_error(self, name: str) -> Never:
+            # Match the Python 3.12 error messages exactly
+            if name == "__name__":
+                raise AttributeError("readonly attribute")
+            elif name in {"__value__", "__type_params__", "__parameters__", "__module__"}:
+                raise AttributeError(
+                    f"attribute '{name}' of 'typing.TypeAliasType' objects "
+                    "is not writable"
+                )
+            else:
+                raise AttributeError(
+                    f"'typing.TypeAliasType' object has no attribute '{name}'"
+                )
+
+        def __repr__(self) -> str:
+            return self.__name__
+
+        def __getitem__(self, parameters):
+            if not isinstance(parameters, tuple):
+                parameters = (parameters,)
+            parameters = [
+                typing._type_check(
+                    item, f'Subscripting {self.__name__} requires a type.'
+                )
+                for item in parameters
+            ]
+            return typing._GenericAlias(self, tuple(parameters))
+
+        def __reduce__(self):
+            return self.__name__
+
+        def __init_subclass__(cls, *args, **kwargs):
+            raise TypeError(
+                "type 'typing_extensions.TypeAliasType' is not an acceptable base type"
+            )
+
+        # The presence of this method convinces typing._type_check
+        # that TypeAliasTypes are types.
+        def __call__(self):
+            raise TypeError("Type alias is not callable")
+
+        if sys.version_info >= (3, 10):
+            def __or__(self, right):
+                # For forward compatibility with 3.12, reject Unions
+                # that are not accepted by the built-in Union.
+                if not _is_unionable(right):
+                    return NotImplemented
+                return typing.Union[self, right]
+
+            def __ror__(self, left):
+                if not _is_unionable(left):
+                    return NotImplemented
+                return typing.Union[left, self]
```

