# Comparing `tmp/fast_depends-1.1.3.tar.gz` & `tmp/fast_depends-1.1.4.tar.gz`

## Comparing `fast_depends-1.1.3.tar` & `fast_depends-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/__init__.py
--rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/construct.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/injector.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/model.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/provider.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/types.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/usage.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.3/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.3/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.3/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.3/README.md
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/__init__.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/construct.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/injector.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/provider.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/types.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/usage.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.4/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.4/README.md
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.4/PKG-INFO
```

### Comparing `fast_depends-1.1.3/CONTRIBUTING.md` & `fast_depends-1.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/.github/workflows/documentation.yml` & `fast_depends-1.1.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/.github/workflows/publish_coverage.yml` & `fast_depends-1.1.4/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/.github/workflows/publish_pypi.yml` & `fast_depends-1.1.4/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/.github/workflows/tests.yml` & `fast_depends-1.1.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/fast_depends/construct.py` & `fast_depends-1.1.4/fast_depends/construct.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     if custom and custom.required is True:
         required = True
     else:
         required = field_info.default in (Required, Undefined, inspect._empty)
 
     field = create_response_field(
         name=param_name,
-        type_=annotation,
+        type_=Any if depends and depends.cast is False else annotation,
         default=None if any((depends, custom)) else field_info.default,
         alias=alias,
         required=required,
         field_info=field_info,
     )
 
     return custom, depends, field
```

### Comparing `fast_depends-1.1.3/fast_depends/injector.py` & `fast_depends-1.1.4/fast_depends/injector.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/fast_depends/model.py` & `fast_depends-1.1.4/fast_depends/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,22 @@
     def cast_response(self, response: Any) -> Tuple[Optional[Any], Optional[ErrorList]]:
         if self.return_field is None:
             return response, []
         return self.return_field.validate(response, {}, loc=RETURN_FIELD)
 
 
 class Depends:
-    def __init__(self, dependency: AnyCallable, *, use_cache: bool = True) -> None:
+    def __init__(
+        self,
+        dependency: AnyCallable,
+        *,
+        use_cache: bool = True,
+        cast: bool = True,
+    ) -> None:
         self.dependency = dependency
         self.use_cache = use_cache
+        self.cast = cast
 
     def __repr__(self) -> str:
         attr = getattr(self.dependency, "__name__", type(self.dependency).__name__)
         cache = "" if self.use_cache else ", use_cache=False"
         return f"{self.__class__.__name__}({attr}{cache})"
```

### Comparing `fast_depends-1.1.3/fast_depends/usage.py` & `fast_depends-1.1.4/fast_depends/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,21 @@
 from fast_depends.provider import dependency_provider
 from fast_depends.types import AnyCallable, P
 from fast_depends.utils import args_to_kwargs, is_coroutine_callable, run_async
 
 T = TypeVar("T")
 
 
-def Depends(dependency: AnyCallable, *, use_cache: bool = True) -> Any:  # noqa: N802
-    return model.Depends(dependency=dependency, use_cache=use_cache)
+def Depends(
+    dependency: AnyCallable,
+    *,
+    use_cache: bool = True,
+    cast: bool = True,
+) -> Any:  # noqa: N802
+    return model.Depends(dependency=dependency, use_cache=use_cache, cast=cast)
 
 
 def wrap_dependant(dependant: model.Dependant) -> model.Dependant:
     return dependant
 
 
 def inject(
```

### Comparing `fast_depends-1.1.3/fast_depends/utils.py` & `fast_depends-1.1.4/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/fast_depends/library/model.py` & `fast_depends-1.1.4/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/LICENSE` & `fast_depends-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/README.md` & `fast_depends-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/pyproject.toml` & `fast_depends-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.3/PKG-INFO` & `fast_depends-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.1.3
+Version: 1.1.4
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

