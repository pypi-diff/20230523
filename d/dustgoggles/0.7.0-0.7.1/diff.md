# Comparing `tmp/dustgoggles-0.7.0.tar.gz` & `tmp/dustgoggles-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustgoggles-0.7.0.tar", last modified: Wed May 17 00:54:22 2023, max compression
+gzip compressed data, was "dustgoggles-0.7.1.tar", last modified: Tue May 23 10:03:42 2023, max compression
```

## Comparing `dustgoggles-0.7.0.tar` & `dustgoggles-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:22.021237 dustgoggles-0.7.0/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1524 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/LICENSE
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-17 00:54:22.016133 dustgoggles-0.7.0/PKG-INFO
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.446418 dustgoggles-0.7.0/dustgoggles/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       22 2023-05-17 00:39:26.000000 dustgoggles-0.7.0/dustgoggles/__init__.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.876911 dustgoggles-0.7.0/dustgoggles/codex/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3518 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/_array_holding_area.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5794 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/codecs.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    33342 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/implements.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3351 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/codex/memutilz.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8366 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/composition.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5772 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/dynamic.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3738 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/func.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5422 2023-02-21 14:57:17.000000 dustgoggles-0.7.0/dustgoggles/mosaic.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8112 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/pivot.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     4035 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/scrape.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)    10211 2023-05-17 00:39:32.000000 dustgoggles-0.7.0/dustgoggles/structures.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.970492 dustgoggles-0.7.0/dustgoggles/test_utils/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       20 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/test_utils/__init__.py
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2519 2022-11-22 17:27:47.000000 dustgoggles-0.7.0/dustgoggles/test_utils/core.py
-drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-17 00:54:21.626714 dustgoggles-0.7.0/dustgoggles.egg-info/
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/PKG-INFO
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      602 2023-05-17 00:54:21.000000 dustgoggles-0.7.0/dustgoggles.egg-info/SOURCES.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)        1 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/dependency_links.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       87 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/requires.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       12 2023-05-17 00:54:20.000000 dustgoggles-0.7.0/dustgoggles.egg-info/top_level.txt
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)       38 2023-05-17 00:54:22.021899 dustgoggles-0.7.0/setup.cfg
--rwxrwxrwx   0 sierra    (1000) sierra    (1000)      494 2023-05-17 00:31:09.000000 dustgoggles-0.7.0/setup.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.689968 dustgoggles-0.7.1/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     1524 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/LICENSE
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-23 17:27:12.686968 dustgoggles-0.7.1/PKG-INFO
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.206017 dustgoggles-0.7.1/dustgoggles/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       22 2023-05-23 17:20:52.000000 dustgoggles-0.7.1/dustgoggles/__init__.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.566031 dustgoggles-0.7.1/dustgoggles/codex/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/__init__.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3518 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/_array_holding_area.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5794 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/codecs.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)    33342 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/implements.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3351 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/codex/memutilz.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8366 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/composition.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5842 2023-05-23 17:19:20.000000 dustgoggles-0.7.1/dustgoggles/dynamic.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     3738 2023-05-17 00:39:32.000000 dustgoggles-0.7.1/dustgoggles/func.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     5422 2023-02-21 14:57:17.000000 dustgoggles-0.7.1/dustgoggles/mosaic.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     8593 2023-05-23 17:19:20.000000 dustgoggles-0.7.1/dustgoggles/pivot.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     4035 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/scrape.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)    13514 2023-05-23 17:19:20.000000 dustgoggles-0.7.1/dustgoggles/structures.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.654385 dustgoggles-0.7.1/dustgoggles/test_utils/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       20 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/test_utils/__init__.py
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)     2519 2022-11-22 17:27:47.000000 dustgoggles-0.7.1/dustgoggles/test_utils/core.py
+drwxrwxrwx   0 sierra    (1000) sierra    (1000)        0 2023-05-23 17:27:12.351568 dustgoggles-0.7.1/dustgoggles.egg-info/
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      326 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/PKG-INFO
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      602 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)        1 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       87 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/requires.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       12 2023-05-23 17:27:11.000000 dustgoggles-0.7.1/dustgoggles.egg-info/top_level.txt
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)       38 2023-05-23 17:27:12.691966 dustgoggles-0.7.1/setup.cfg
+-rwxrwxrwx   0 sierra    (1000) sierra    (1000)      494 2023-05-23 17:20:52.000000 dustgoggles-0.7.1/setup.py
```

### Comparing `dustgoggles-0.7.0/LICENSE` & `dustgoggles-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/codex/_array_holding_area.py` & `dustgoggles-0.7.1/dustgoggles/codex/_array_holding_area.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/codex/codecs.py` & `dustgoggles-0.7.1/dustgoggles/codex/codecs.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/codex/implements.py` & `dustgoggles-0.7.1/dustgoggles/codex/implements.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/codex/memutilz.py` & `dustgoggles-0.7.1/dustgoggles/codex/memutilz.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/composition.py` & `dustgoggles-0.7.1/dustgoggles/composition.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/dynamic.py` & `dustgoggles-0.7.1/dustgoggles/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,20 @@
     globals_ = globals_ if globals_ is not None else globals()
     return FunctionType(code, globals_)
 
 
 def exc_report(exc):
     if exc is None:
         return {}
+    stack = traceback.extract_stack()[:-3]
     return {
-        "time": dt.datetime.now().isoformat()[:-3],
         "exception": exc,
-        "stack": tuple([a.name for a in traceback.extract_stack()[:-3]]),
+        "lineno": tuple([a.lineno for a in stack]),
+        "stack": tuple([a.name for a in stack]),
+        "time": dt.datetime.now().isoformat()[:-3],
     }
 
 
 class Dynamic:
     """
     simple class to help manage function definition / execution from
     dynamically-generated source.
```

### Comparing `dustgoggles-0.7.0/dustgoggles/func.py` & `dustgoggles-0.7.1/dustgoggles/func.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/mosaic.py` & `dustgoggles-0.7.1/dustgoggles/mosaic.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/pivot.py` & `dustgoggles-0.7.1/dustgoggles/pivot.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,21 +66,34 @@
     """
     if how == "rows":
         axis = 0
     elif how == "columns":
         axis = 1
     else:
         raise ValueError(f"unknown how {how}")
-    constant_indices = df.nunique(axis=axis, dropna=dropna) <= 1
+    try:
+        constant_indices = df.nunique(axis=axis, dropna=dropna) <= 1
+    except TypeError:
+        constant_indices = []
+        for c in df.columns:
+            if isinstance(df[c].iloc[0], list):
+                test_series = df[c].map(tuple)
+            else:
+                test_series = df[c]
+            if test_series.nunique(dropna=dropna) <= 1:
+                constant_indices.append(c)
+
     if axis == 0:
+        var_indices = [c for c in df.columns if c not in constant_indices]
         constants = df.loc[:, constant_indices]
-        variables = df.loc[:, ~constant_indices]
+        variables = df.loc[:, var_indices]
     else:
+        var_indices = [c for c in df.indices if c not in constant_indices]
         constants = df.loc[constant_indices]
-        variables = df.loc[~constant_indices]
+        variables = df.loc[var_indices]
     if to_dict:
         constants = constants.iloc[0].to_dict()
     if drop_constants:
         return constants, variables
     return constants, df
```

### Comparing `dustgoggles-0.7.0/dustgoggles/scrape.py` & `dustgoggles-0.7.1/dustgoggles/scrape.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles/structures.py` & `dustgoggles-0.7.1/dustgoggles/structures.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """structured data and manipulators thereof"""
 from collections import defaultdict, OrderedDict
 from copy import copy
 from functools import reduce, partial
 from itertools import chain
+from multiprocessing import Pool
 from operator import methodcaller, add, getitem, eq
 from typing import (
     Mapping,
     Collection,
     Any,
     Union,
     Sequence,
     MutableMapping,
     Callable,
     Type,
     Hashable,
 )
 
 from cytoolz import merge
+from more_itertools import chunked, divide
 
 from dustgoggles.func import naturals, is_it, splat
 
 
 def to_records(nested: Mapping, accumulated_levels=None, level_names=None):
     level_names = naturals() if level_names is None else iter(level_names)
     records = []
@@ -329,7 +331,127 @@
         return (
             f"HashDict with {len(self.dict_)} keys storing "
             f"{len(self.reverse)} unique values"
         )
 
     def __repr__(self):
         return self.__str__()
+
+
+class MaybeResult:
+    def __init__(self, func, args, kwargs):
+        try:
+            self.value = func(*args, **kwargs)
+        except KeyboardInterrupt:
+            raise
+        except Exception as ex:
+            self.value = ex
+
+    def get(self):
+        if isinstance(self.value, Exception):
+            raise self.value
+        return self.value
+
+    @staticmethod
+    def ready():
+        return True
+
+
+def _chunkwrap(func, argrecs):
+    return {
+        rec['key']: func(*rec['args'], **rec['kwargs'])
+        for rec in argrecs
+    }
+
+
+class MaybePool:
+    def __init__(self, threads=None):
+        self.threads, self.results, self.chunked = threads, {}, False
+        if threads is None:
+            self.pool = None
+        else:
+            self.pool = Pool(threads)
+
+    def map(self, func, argrecs, as_chunks=False):
+        for i, rec in enumerate(argrecs):
+            rec['key'] = rec.get('key', i)
+            rec['args'] = rec.get('args', ())
+            rec['kwargs'] = rec.get('kwargs', {})
+        if (as_chunks is False) or (self.pool is None):
+            self.results = {
+                rec['key']: self.apply(func, rec['args'], rec['kwargs'])
+                for rec in argrecs
+            }
+        else:
+            self.chunked = True
+            chunks = divide(self.threads, argrecs)
+            self.results = {
+                f"chunk_{i}": self.apply(_chunkwrap, (func, chunk))
+                for i, chunk in enumerate(chunks)
+            }
+
+    def apply(self, func, args=(), kwargs=None):
+        """note: does apply_async by default"""
+        kwargs = {} if kwargs is None else kwargs
+        if self.pool is None:
+            return MaybeResult(func, args, kwargs)
+        return self.pool.apply_async(func, args, kwargs)
+
+    def close(self):
+        if self.pool is None:
+            return
+        return self.pool.close()
+
+    def join(self):
+        if self.pool is None:
+            return
+        return self.pool.join()
+
+    def get(self, raise_exc=False):
+        output = {}
+        for k, v in self.results.items():
+            try:
+                if self.chunked is True:
+                    output |= v.get()
+                else:
+                    output[k] = v.get()
+            except KeyboardInterrupt:
+                raise
+            except Exception as ex:
+                if raise_exc:
+                    raise ex
+                output[k] = ex
+        return output
+
+    def results_ready(self):
+        return {k: v.ready() for k, v in self.results.items()}
+
+    def ready(self):
+        return all(v.ready() for v in self.results.values())
+
+    def terminate(self):
+        if self.pool is not None:
+            self.pool.terminate()
+        self.results = {}
+
+
+def map_into_pool(
+    func,
+    argrecs,
+    threads=None,
+    filter_exc=False,
+    as_chunks=True
+):
+    pool = MaybePool(threads)
+    try:
+        pool.map(func, argrecs, as_chunks=as_chunks)
+        pool.close()
+        pool.join()
+        results = pool.get()
+        if filter_exc is True:
+            results = {
+                k: v for k, v in results.items()
+                if not isinstance(v, Exception)
+            }
+    finally:
+        pool.terminate()
+    return results
```

### Comparing `dustgoggles-0.7.0/dustgoggles/test_utils/core.py` & `dustgoggles-0.7.1/dustgoggles/test_utils/core.py`

 * *Files identical despite different names*

### Comparing `dustgoggles-0.7.0/dustgoggles.egg-info/SOURCES.txt` & `dustgoggles-0.7.1/dustgoggles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

