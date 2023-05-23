# Comparing `tmp/optree-0.9.0.tar.gz` & `tmp/optree-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optree-0.9.0.tar", last modified: Thu Mar 23 08:56:03 2023, max compression
+gzip compressed data, was "optree-0.9.1.tar", last modified: Tue May 23 14:34:29 2023, max compression
```

## Comparing `optree-0.9.0.tar` & `optree-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.829459 optree-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-03-23 08:55:49.000000 optree-0.9.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-03-23 08:55:49.000000 optree-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-23 08:55:49.000000 optree-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-03-23 08:56:03.829459 optree-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    41735 2023-03-23 08:55:49.000000 optree-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.825459 optree-0.9.0/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-23 08:55:49.000000 optree-0.9.0/include/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-23 08:55:49.000000 optree-0.9.0/include/registry.h
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-03-23 08:55:49.000000 optree-0.9.0/include/treespec.h
--rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-03-23 08:55:49.000000 optree-0.9.0/include/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.829459 optree-0.9.0/optree/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-23 08:55:49.000000 optree-0.9.0/optree/_C.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-23 08:55:49.000000 optree-0.9.0/optree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72246 2023-03-23 08:55:49.000000 optree-0.9.0/optree/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:55:49.000000 optree-0.9.0/optree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-03-23 08:55:49.000000 optree-0.9.0/optree/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-03-23 08:55:49.000000 optree-0.9.0/optree/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-23 08:55:49.000000 optree-0.9.0/optree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-23 08:55:49.000000 optree-0.9.0/optree/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.829459 optree-0.9.0/optree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-03-23 08:56:03.000000 optree-0.9.0/optree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-23 08:56:03.000000 optree-0.9.0/optree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:56:03.000000 optree-0.9.0/optree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-23 08:56:03.000000 optree-0.9.0/optree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 08:56:03.000000 optree-0.9.0/optree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-03-23 08:55:49.000000 optree-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 08:56:03.829459 optree-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-03-23 08:55:49.000000 optree-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.829459 optree-0.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-23 08:55:49.000000 optree-0.9.0/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-03-23 08:55:49.000000 optree-0.9.0/src/optree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-03-23 08:55:49.000000 optree-0.9.0/src/registry.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.829459 optree-0.9.0/src/treespec/
--rw-r--r--   0 runner    (1001) docker     (123)    29724 2023-03-23 08:55:49.000000 optree-0.9.0/src/treespec/flatten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-23 08:55:49.000000 optree-0.9.0/src/treespec/traversal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32864 2023-03-23 08:55:49.000000 optree-0.9.0/src/treespec/treespec.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-23 08:55:49.000000 optree-0.9.0/src/treespec/unflatten.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:56:03.829459 optree-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35005 2023-03-23 08:55:49.000000 optree-0.9.0/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-03-23 08:55:49.000000 optree-0.9.0/tests/test_prefix_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-03-23 08:55:49.000000 optree-0.9.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-03-23 08:55:49.000000 optree-0.9.0/tests/test_treespec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-03-23 08:55:49.000000 optree-0.9.0/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-23 08:55:49.000000 optree-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.293072 optree-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-23 14:34:11.000000 optree-0.9.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-23 14:34:11.000000 optree-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 14:34:11.000000 optree-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43150 2023-05-23 14:34:29.293072 optree-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    41739 2023-05-23 14:34:11.000000 optree-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.289072 optree-0.9.1/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-23 14:34:11.000000 optree-0.9.1/include/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-23 14:34:11.000000 optree-0.9.1/include/registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-23 14:34:11.000000 optree-0.9.1/include/treespec.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20320 2023-05-23 14:34:11.000000 optree-0.9.1/include/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.289072 optree-0.9.1/optree/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-23 14:34:11.000000 optree-0.9.1/optree/_C.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-23 14:34:11.000000 optree-0.9.1/optree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72246 2023-05-23 14:34:11.000000 optree-0.9.1/optree/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:11.000000 optree-0.9.1/optree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21650 2023-05-23 14:34:11.000000 optree-0.9.1/optree/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-23 14:34:11.000000 optree-0.9.1/optree/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-23 14:34:11.000000 optree-0.9.1/optree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-23 14:34:12.000000 optree-0.9.1/optree/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.293072 optree-0.9.1/optree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43150 2023-05-23 14:34:29.000000 optree-0.9.1/optree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 14:34:29.000000 optree-0.9.1/optree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:34:29.000000 optree-0.9.1/optree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 14:34:29.000000 optree-0.9.1/optree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 14:34:29.000000 optree-0.9.1/optree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-23 14:34:11.000000 optree-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:34:29.293072 optree-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-23 14:34:11.000000 optree-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.293072 optree-0.9.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-23 14:34:11.000000 optree-0.9.1/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-23 14:34:11.000000 optree-0.9.1/src/optree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-23 14:34:11.000000 optree-0.9.1/src/registry.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.293072 optree-0.9.1/src/treespec/
+-rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-05-23 14:34:11.000000 optree-0.9.1/src/treespec/flatten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-23 14:34:11.000000 optree-0.9.1/src/treespec/traversal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32874 2023-05-23 14:34:11.000000 optree-0.9.1/src/treespec/treespec.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-23 14:34:11.000000 optree-0.9.1/src/treespec/unflatten.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:34:29.293072 optree-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35001 2023-05-23 14:34:11.000000 optree-0.9.1/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-05-23 14:34:11.000000 optree-0.9.1/tests/test_prefix_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-05-23 14:34:11.000000 optree-0.9.1/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-05-23 14:34:11.000000 optree-0.9.1/tests/test_treespec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-23 14:34:11.000000 optree-0.9.1/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-23 14:34:11.000000 optree-0.9.1/tests/test_utils.py
```

### Comparing `optree-0.9.0/CMakeLists.txt` & `optree-0.9.1/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 
 cmake_minimum_required(VERSION 3.11)  # for FetchContent
 project(optree LANGUAGES CXX)
 
 include(FetchContent)
 set(PYBIND11_VERSION v2.10.4)
-set(ABSEIL_CPP_VERSION 20230125.1)
+set(ABSEIL_CPP_VERSION 20230125.3)
 set(THIRD_PARTY_DIR "${CMAKE_SOURCE_DIR}/third-party")
 
 if(NOT CMAKE_BUILD_TYPE)
     set(CMAKE_BUILD_TYPE Release)
 endif()
 
 set(CMAKE_CXX_STANDARD 20)  # for likely/unlikely attributes
```

### Comparing `optree-0.9.0/LICENSE` & `optree-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/PKG-INFO` & `optree-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optree
-Version: 0.9.0
+Version: 0.9.1
 Summary: Optimized PyTree Utilities.
 Author: OpTree Contributors
 Author-email: Xuehai Pan <XuehaiPan@pku.edu.cn>, Jie Ren <jieren9806@gmail.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/metaopt/optree
 Project-URL: Repository, https://github.com/metaopt/optree
 Project-URL: Documentation, https://optree.readthedocs.io
@@ -97,15 +97,15 @@
 
 ```bash
 git clone --depth=1 https://github.com/metaopt/optree.git
 cd optree
 pip3 install .
 ```
 
-Compiling from the source requires Python 3.7+, a compiler (`gcc` / `clang` / `icc` / `cl.exe`) supports C++20 and a `cmake` installation.
+Compiling from the source requires Python 3.7+, a compiler (`gcc` / `clang` / `icc` / `cl.exe`) that supports C++20 and a `cmake` installation.
 
 --------------------------------------------------------------------------------
 
 ## PyTrees
 
 A PyTree is a recursive structure that can be an arbitrarily nested Python container (e.g., `tuple`, `list`, `dict`, `OrderedDict`, `NamedTuple`, etc.) or an opaque Python object.
 The key concepts of tree operations are tree flattening and its inverse (tree unflattening).
@@ -152,15 +152,15 @@
 - [`collections.defaultdict`](https://docs.python.org/3/library/collections.html#collections.defaultdict)
 - [`collections.deque`](https://docs.python.org/3/library/collections.html#collections.deque)
 - [`PyStructSequence`](https://docs.python.org/3/c-api/tuple.html#struct-sequence-objects) types created by C API [`PyStructSequence_NewType`](https://docs.python.org/3/c-api/tuple.html#c.PyStructSequence_NewType)
 
 which are considered non-leaf nodes in the tree.
 Python objects that the type is not registered will be treated as leaf nodes.
 The registration lookup uses the `is` operator to determine whether the type is matched.
-So subclasses will need to explicitly register in the registry, otherwise, an object of that type will be considered as a leaf.
+So subclasses will need to explicitly register in the registry, otherwise, an object of that type will be considered a leaf.
 The [`NoneType`](https://docs.python.org/3/library/constants.html#None) is a special case discussed in section [`None` is non-leaf Node vs. `None` is Leaf](#none-is-non-leaf-node-vs-none-is-leaf).
 
 #### Registering a Container-like Custom Type as Non-leaf Nodes
 
 A container-like Python type can be registered in the type registry with a pair of functions that specify:
 
 - `flatten_func(container) -> (children, metadata, entries)`: convert an instance of the container type to a `(children, metadata, entries)` triple, where `children` is an iterable of subtrees and `entries` is an iterable of path entries of the container (e.g., indices or keys).
@@ -553,15 +553,15 @@
 >>> restored_treespec = pickle.loads(pickle.dumps(treespec))
 >>> optree.tree_unflatten(treespec, leaves)
 {'b': [3], 'a': [1, 2]}
 >>> optree.tree_unflatten(restored_treespec, leaves)
 {'b': [3], 'a': [1, 2]}
 ```
 
-> Note that there are no restrictions on the `dict` to require the keys are comparable (sortable).
+> Note that there are no restrictions on the `dict` to require the keys to be comparable (sortable).
 > There can be multiple types of keys in the dictionary.
 > The keys are sorted in ascending order by `key=lambda k: k` first if capable otherwise fallback to `key=lambda k: (f'{k.__class__.__module__}.{k.__class__.__qualname__}', k)`. This handles most cases.
 >
 > ```python
 > >>> sorted({1: 2, 1.5: 1}.keys())
 > [1, 1.5]
 > >>> sorted({'a': 3, 1: 2, 1.5: 1}.keys())
```

### Comparing `optree-0.9.0/README.md` & `optree-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 ```bash
 git clone --depth=1 https://github.com/metaopt/optree.git
 cd optree
 pip3 install .
 ```
 
-Compiling from the source requires Python 3.7+, a compiler (`gcc` / `clang` / `icc` / `cl.exe`) supports C++20 and a `cmake` installation.
+Compiling from the source requires Python 3.7+, a compiler (`gcc` / `clang` / `icc` / `cl.exe`) that supports C++20 and a `cmake` installation.
 
 --------------------------------------------------------------------------------
 
 ## PyTrees
 
 A PyTree is a recursive structure that can be an arbitrarily nested Python container (e.g., `tuple`, `list`, `dict`, `OrderedDict`, `NamedTuple`, etc.) or an opaque Python object.
 The key concepts of tree operations are tree flattening and its inverse (tree unflattening).
@@ -118,15 +118,15 @@
 - [`collections.defaultdict`](https://docs.python.org/3/library/collections.html#collections.defaultdict)
 - [`collections.deque`](https://docs.python.org/3/library/collections.html#collections.deque)
 - [`PyStructSequence`](https://docs.python.org/3/c-api/tuple.html#struct-sequence-objects) types created by C API [`PyStructSequence_NewType`](https://docs.python.org/3/c-api/tuple.html#c.PyStructSequence_NewType)
 
 which are considered non-leaf nodes in the tree.
 Python objects that the type is not registered will be treated as leaf nodes.
 The registration lookup uses the `is` operator to determine whether the type is matched.
-So subclasses will need to explicitly register in the registry, otherwise, an object of that type will be considered as a leaf.
+So subclasses will need to explicitly register in the registry, otherwise, an object of that type will be considered a leaf.
 The [`NoneType`](https://docs.python.org/3/library/constants.html#None) is a special case discussed in section [`None` is non-leaf Node vs. `None` is Leaf](#none-is-non-leaf-node-vs-none-is-leaf).
 
 #### Registering a Container-like Custom Type as Non-leaf Nodes
 
 A container-like Python type can be registered in the type registry with a pair of functions that specify:
 
 - `flatten_func(container) -> (children, metadata, entries)`: convert an instance of the container type to a `(children, metadata, entries)` triple, where `children` is an iterable of subtrees and `entries` is an iterable of path entries of the container (e.g., indices or keys).
@@ -519,15 +519,15 @@
 >>> restored_treespec = pickle.loads(pickle.dumps(treespec))
 >>> optree.tree_unflatten(treespec, leaves)
 {'b': [3], 'a': [1, 2]}
 >>> optree.tree_unflatten(restored_treespec, leaves)
 {'b': [3], 'a': [1, 2]}
 ```
 
-> Note that there are no restrictions on the `dict` to require the keys are comparable (sortable).
+> Note that there are no restrictions on the `dict` to require the keys to be comparable (sortable).
 > There can be multiple types of keys in the dictionary.
 > The keys are sorted in ascending order by `key=lambda k: k` first if capable otherwise fallback to `key=lambda k: (f'{k.__class__.__module__}.{k.__class__.__qualname__}', k)`. This handles most cases.
 >
 > ```python
 > >>> sorted({1: 2, 1.5: 1}.keys())
 > [1, 1.5]
 > >>> sorted({'a': 3, 1: 2, 1.5: 1}.keys())
```

### Comparing `optree-0.9.0/include/exceptions.h` & `optree-0.9.1/include/exceptions.h`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/include/registry.h` & `optree-0.9.1/include/registry.h`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/include/treespec.h` & `optree-0.9.1/include/treespec.h`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/include/utils.h` & `optree-0.9.1/include/utils.h`

 * *Files 5% similar despite different names*

```diff
@@ -274,40 +274,41 @@
     if (!PyDict_CheckExact(object.ptr())) [[unlikely]] {
         throw py::value_error(
             absl::StrFormat("Expected an instance of dict, got %s.", py::repr(object)));
     }
 }
 
 inline void AssertExactOrderedDict(const py::handle& object) {
-    if (!object.get_type().is(PyOrderedDictTypeObject)) [[unlikely]] {
+    if (!py::type::handle_of(object).is(PyOrderedDictTypeObject)) [[unlikely]] {
         throw py::value_error(absl::StrFormat(
             "Expected an instance of collections.OrderedDict, got %s.", py::repr(object)));
     }
 }
 
 inline void AssertExactDefaultDict(const py::handle& object) {
-    if (!object.get_type().is(PyDefaultDictTypeObject)) [[unlikely]] {
+    if (!py::type::handle_of(object).is(PyDefaultDictTypeObject)) [[unlikely]] {
         throw py::value_error(absl::StrFormat(
             "Expected an instance of collections.defaultdict, got %s.", py::repr(object)));
     }
 }
 
 inline void AssertExactStandardDict(const py::handle& object) {
-    if (!(PyDict_CheckExact(object.ptr()) || object.get_type().is(PyOrderedDictTypeObject) ||
-          object.get_type().is(PyDefaultDictTypeObject))) [[unlikely]] {
+    if (!(PyDict_CheckExact(object.ptr()) ||
+          py::type::handle_of(object).is(PyOrderedDictTypeObject) ||
+          py::type::handle_of(object).is(PyDefaultDictTypeObject))) [[unlikely]] {
         throw py::value_error(
             absl::StrFormat("Expected an instance of "
                             "dict, collections.OrderedDict, or collections.defaultdict, "
                             "got %s.",
                             py::repr(object)));
     }
 }
 
 inline void AssertExactDeque(const py::handle& object) {
-    if (!object.get_type().is(PyDequeTypeObject)) [[unlikely]] {
+    if (!py::type::handle_of(object).is(PyDequeTypeObject)) [[unlikely]] {
         throw py::value_error(absl::StrFormat("Expected an instance of collections.deque, got %s.",
                                               py::repr(object)));
     }
 }
 
 inline bool IsNamedTupleClassImpl(const py::handle& type) {
     // We can only identify namedtuples heuristically, here by the presence of a _fields attribute.
@@ -330,18 +331,18 @@
     }
     return false;
 }
 inline bool IsNamedTupleClass(const py::handle& type) {
     return PyType_Check(type.ptr()) && IsNamedTupleClassImpl(type);
 }
 inline bool IsNamedTupleInstance(const py::handle& object) {
-    return IsNamedTupleClass(object.get_type());
+    return IsNamedTupleClass(py::type::handle_of(object));
 }
 inline bool IsNamedTuple(const py::handle& object) {
-    py::handle type = (PyType_Check(object.ptr()) ? object : object.get_type());
+    py::handle type = (PyType_Check(object.ptr()) ? object : py::type::handle_of(object));
     return IsNamedTupleClass(type);
 }
 inline void AssertExactNamedTuple(const py::handle& object) {
     if (!IsNamedTupleInstance(object)) [[unlikely]] {
         throw py::value_error(absl::StrFormat(
             "Expected an instance of collections.namedtuple, got %s.", py::repr(object)));
     }
@@ -351,15 +352,15 @@
     if (PyType_Check(object.ptr())) [[unlikely]] {
         type = object;
         if (!IsNamedTupleClass(type)) [[unlikely]] {
             throw py::type_error(absl::StrFormat("Expected a collections.namedtuple type, got %s.",
                                                  py::repr(object)));
         }
     } else [[likely]] {
-        type = object.get_type();
+        type = py::type::handle_of(object);
         if (!IsNamedTupleClass(type)) [[unlikely]] {
             throw py::type_error(absl::StrFormat(
                 "Expected an instance of collections.namedtuple type, got %s.", py::repr(object)));
         }
     }
     return py::getattr(type, "_fields");
 }
@@ -387,18 +388,18 @@
     }
     return false;
 }
 inline bool IsStructSequenceClass(const py::handle& type) {
     return PyType_Check(type.ptr()) && IsStructSequenceClassImpl(type);
 }
 inline bool IsStructSequenceInstance(const py::handle& object) {
-    return IsStructSequenceClass(object.get_type());
+    return IsStructSequenceClass(py::type::handle_of(object));
 }
 inline bool IsStructSequence(const py::handle& object) {
-    py::handle type = (PyType_Check(object.ptr()) ? object : object.get_type());
+    py::handle type = (PyType_Check(object.ptr()) ? object : py::type::handle_of(object));
     return IsStructSequenceClass(type);
 }
 inline void AssertExactStructSequence(const py::handle& object) {
     if (!IsStructSequenceInstance(object)) [[unlikely]] {
         throw py::value_error(absl::StrFormat(
             "Expected an instance of PyStructSequence type, got %s.", py::repr(object)));
     }
@@ -408,15 +409,15 @@
     if (PyType_Check(object.ptr())) [[unlikely]] {
         type = object;
         if (!IsStructSequenceClass(type)) [[unlikely]] {
             throw py::type_error(
                 absl::StrFormat("Expected a PyStructSequence type, got %s.", py::repr(object)));
         }
     } else [[likely]] {
-        type = object.get_type();
+        type = py::type::handle_of(object);
         if (!IsStructSequenceClass(type)) [[unlikely]] {
             throw py::type_error(absl::StrFormat(
                 "Expected an instance of PyStructSequence type, got %s.", py::repr(object)));
         }
     }
 
     const auto n_sequence_fields = getattr(type, "n_sequence_fields").cast<ssize_t>();
@@ -438,15 +439,15 @@
         }
     } catch (py::error_already_set& ex1) {
         if (ex1.matches(PyExc_TypeError)) [[likely]] {
             // Found incomparable keys (e.g. `int` vs. `str`, or user-defined types).
             try {
                 // Sort with `(f'{o.__class__.__module__}.{o.__class__.__qualname__}', o)`
                 auto sort_key_fn = py::cpp_function([](const py::object& o) {
-                    py::handle t = o.get_type();
+                    py::handle t = py::type::handle_of(o);
                     py::str qualname{absl::StrFormat(
                         "%s.%s",
                         static_cast<std::string>(py::getattr(t, "__module__").cast<py::str>()),
                         static_cast<std::string>(py::getattr(t, "__qualname__").cast<py::str>()))};
                     return py::make_tuple(qualname, o);
                 });
                 list.attr("sort")(py::arg("key") = sort_key_fn);
```

### Comparing `optree-0.9.0/optree/_C.pyi` & `optree-0.9.1/optree/_C.pyi`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/optree/__init__.py` & `optree-0.9.1/optree/__init__.py`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/optree/ops.py` & `optree-0.9.1/optree/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -879,19 +879,19 @@
     namespace: str = '',
 ) -> T:  # pragma: no cover
     ...
 
 
 @overload
 def tree_reduce(
-    func: Callable[[T, T], T],
-    tree: PyTree[T],
+    func: Callable[[T, S], T],
+    tree: PyTree[S],
     initial: T = __MISSING,
     *,
-    is_leaf: Callable[[T], bool] | None = None,
+    is_leaf: Callable[[S], bool] | None = None,
     none_is_leaf: bool = False,
     namespace: str = '',
 ) -> T:  # pragma: no cover
     ...
 
 
 def tree_reduce(
```

### Comparing `optree-0.9.0/optree/registry.py` & `optree-0.9.1/optree/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,15 @@
         namespace (str): A non-empty string that uniquely identifies the namespace of the type registry.
             This is used to isolate the registry from other modules that might register a different
             custom behavior for the same type.
 
     Returns:
         The same type as the input ``cls``.
 
-    Example::
-
+    Examples:
         >>> # Registry a Python type with lambda functions
         >>> register_pytree_node(
         ...     set,
         ...     lambda s: (sorted(s), None, None),
         ...     lambda _, children: set(children),
         ...     namespace='set',
         ... )
@@ -160,15 +159,15 @@
             )
         )
     """
     if not inspect.isclass(cls):
         raise TypeError(f'Expected a class, got {cls}.')
     if namespace is not __GLOBAL_NAMESPACE and not isinstance(namespace, str):
         raise TypeError(f'The namespace must be a string, got {namespace}.')
-    if namespace == '':  # noqa: PLC1901
+    if namespace == '':
         raise ValueError('The namespace cannot be an empty string.')
 
     registration_key: type | tuple[str, type]
     if namespace is __GLOBAL_NAMESPACE:
         registration_key = cls
         namespace = ''
     else:
@@ -254,23 +253,23 @@
             @classmethod
             def tree_unflatten(cls, metadata, children):
                 return cls(*children)
     """
     if cls is __GLOBAL_NAMESPACE or isinstance(cls, str):
         if namespace is not None:
             raise ValueError('Cannot specify `namespace` when the first argument is a string.')
-        if cls == '':  # noqa: PLC1901
+        if cls == '':
             raise ValueError('The namespace cannot be an empty string.')
         return functools.partial(register_pytree_node_class, namespace=cls)  # type: ignore[return-value]
 
     if namespace is None:
         raise ValueError('Must specify `namespace` when the first argument is a class.')
     if namespace is not __GLOBAL_NAMESPACE and not isinstance(namespace, str):
         raise TypeError(f'The namespace must be a string, got {namespace}')
-    if namespace == '':  # noqa: PLC1901
+    if namespace == '':
         raise ValueError('The namespace cannot be an empty string.')
 
     if cls is None:
         return functools.partial(register_pytree_node_class, namespace=namespace)  # type: ignore[return-value]
     if not inspect.isclass(cls):
         raise TypeError(f'Expected a class, got {cls}.')
     register_pytree_node(cls, methodcaller('tree_flatten'), cls.tree_unflatten, namespace)
@@ -340,15 +339,15 @@
 
 def _pytree_node_registry_get(
     cls: type,
     *,
     namespace: str = __GLOBAL_NAMESPACE,
 ) -> PyTreeNodeRegistryEntry | None:
     entry: PyTreeNodeRegistryEntry | None = _nodetype_registry.get(cls)
-    if entry is not None or namespace is __GLOBAL_NAMESPACE or namespace == '':  # noqa: PLC1901
+    if entry is not None or namespace is __GLOBAL_NAMESPACE or namespace == '':
         return entry
     return _nodetype_registry.get((namespace, cls))
 
 
 register_pytree_node.get = _pytree_node_registry_get  # type: ignore[attr-defined]
 del _pytree_node_registry_get
 
@@ -496,15 +495,15 @@
 
 
 class GetitemKeyPathEntry(KeyPathEntry):
     """The key path entry class for sequences and dictionaries."""
 
     def pprint(self) -> str:
         """Pretty name of the key path entry."""
-        return f'[{repr(self.key)}]'
+        return f'[{self.key!r}]'
 
 
 class AttributeKeyPathEntry(KeyPathEntry):
     """The key path entry class for namedtuples."""
 
     def pprint(self) -> str:
         """Pretty name of the key path entry."""
```

### Comparing `optree-0.9.0/optree/typing.py` & `optree-0.9.1/optree/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 from typing_extensions import OrderedDict  # Generic OrderedDict: Python 3.7.2+
-from typing_extensions import Protocol  # Python 3.8+
 from typing_extensions import TypeAlias  # Python 3.10+
+from typing_extensions import Protocol, runtime_checkable  # Python 3.8+
 
 from optree import _C
 
 
 try:
     # pylint: disable-next=ungrouped-imports
     from typing_extensions import NamedTuple  # Generic NamedTuple: Python 3.11+
@@ -95,14 +95,15 @@
 
 
 Children = Sequence[T]
 _MetaData = TypeVar('_MetaData', bound=Hashable)
 MetaData = Optional[_MetaData]
 
 
+@runtime_checkable
 class CustomTreeNode(Protocol[T]):
     """The abstract base class for custom pytree nodes."""
 
     def tree_flatten(
         self,
     ) -> (
         # Use `range(num_children)` as path entries
```

### Comparing `optree-0.9.0/optree/utils.py` & `optree-0.9.1/optree/utils.py`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/optree/version.py` & `optree-0.9.1/optree/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """OpTree: Optimized PyTree Utilities."""
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 __license__ = 'Apache License, Version 2.0'
 __author__ = 'OpTree Contributors'
 __release__ = True
 
 if not __release__:
     import os
     import subprocess
 
     try:
         prefix, sep, suffix = (
             subprocess.check_output(
-                ['git', 'describe', '--abbrev=7'],
+                ['git', 'describe', '--abbrev=7'],  # noqa: S603,S607
                 cwd=os.path.dirname(os.path.abspath(__file__)),
                 stderr=subprocess.DEVNULL,
                 text=True,
             )
             .strip()
             .lstrip('v')
             .replace('-', '.dev', 1)
```

### Comparing `optree-0.9.0/optree.egg-info/PKG-INFO` & `optree-0.9.1/optree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optree
-Version: 0.9.0
+Version: 0.9.1
 Summary: Optimized PyTree Utilities.
 Author: OpTree Contributors
 Author-email: Xuehai Pan <XuehaiPan@pku.edu.cn>, Jie Ren <jieren9806@gmail.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/metaopt/optree
 Project-URL: Repository, https://github.com/metaopt/optree
 Project-URL: Documentation, https://optree.readthedocs.io
@@ -97,15 +97,15 @@
 
 ```bash
 git clone --depth=1 https://github.com/metaopt/optree.git
 cd optree
 pip3 install .
 ```
 
-Compiling from the source requires Python 3.7+, a compiler (`gcc` / `clang` / `icc` / `cl.exe`) supports C++20 and a `cmake` installation.
+Compiling from the source requires Python 3.7+, a compiler (`gcc` / `clang` / `icc` / `cl.exe`) that supports C++20 and a `cmake` installation.
 
 --------------------------------------------------------------------------------
 
 ## PyTrees
 
 A PyTree is a recursive structure that can be an arbitrarily nested Python container (e.g., `tuple`, `list`, `dict`, `OrderedDict`, `NamedTuple`, etc.) or an opaque Python object.
 The key concepts of tree operations are tree flattening and its inverse (tree unflattening).
@@ -152,15 +152,15 @@
 - [`collections.defaultdict`](https://docs.python.org/3/library/collections.html#collections.defaultdict)
 - [`collections.deque`](https://docs.python.org/3/library/collections.html#collections.deque)
 - [`PyStructSequence`](https://docs.python.org/3/c-api/tuple.html#struct-sequence-objects) types created by C API [`PyStructSequence_NewType`](https://docs.python.org/3/c-api/tuple.html#c.PyStructSequence_NewType)
 
 which are considered non-leaf nodes in the tree.
 Python objects that the type is not registered will be treated as leaf nodes.
 The registration lookup uses the `is` operator to determine whether the type is matched.
-So subclasses will need to explicitly register in the registry, otherwise, an object of that type will be considered as a leaf.
+So subclasses will need to explicitly register in the registry, otherwise, an object of that type will be considered a leaf.
 The [`NoneType`](https://docs.python.org/3/library/constants.html#None) is a special case discussed in section [`None` is non-leaf Node vs. `None` is Leaf](#none-is-non-leaf-node-vs-none-is-leaf).
 
 #### Registering a Container-like Custom Type as Non-leaf Nodes
 
 A container-like Python type can be registered in the type registry with a pair of functions that specify:
 
 - `flatten_func(container) -> (children, metadata, entries)`: convert an instance of the container type to a `(children, metadata, entries)` triple, where `children` is an iterable of subtrees and `entries` is an iterable of path entries of the container (e.g., indices or keys).
@@ -553,15 +553,15 @@
 >>> restored_treespec = pickle.loads(pickle.dumps(treespec))
 >>> optree.tree_unflatten(treespec, leaves)
 {'b': [3], 'a': [1, 2]}
 >>> optree.tree_unflatten(restored_treespec, leaves)
 {'b': [3], 'a': [1, 2]}
 ```
 
-> Note that there are no restrictions on the `dict` to require the keys are comparable (sortable).
+> Note that there are no restrictions on the `dict` to require the keys to be comparable (sortable).
 > There can be multiple types of keys in the dictionary.
 > The keys are sorted in ascending order by `key=lambda k: k` first if capable otherwise fallback to `key=lambda k: (f'{k.__class__.__module__}.{k.__class__.__qualname__}', k)`. This handles most cases.
 >
 > ```python
 > >>> sorted({1: 2, 1.5: 1}.keys())
 > [1, 1.5]
 > >>> sorted({'a': 3, 1: 2, 1.5: 1}.keys())
```

### Comparing `optree-0.9.0/optree.egg-info/SOURCES.txt` & `optree-0.9.1/optree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/pyproject.toml` & `optree-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -63,28 +63,34 @@
     "doc8 < 1.0.0a0",  # unpin this when we drop support for Python 3.7
     "pydocstyle",
     "pyenchant",
     "xdoctest",
     "cpplint",
     "pre-commit",
 ]
-test = ['pytest', 'pytest-cov', 'pytest-xdist']
+test = ["pytest", "pytest-cov", "pytest-xdist"]
 benchmark = [
-    'jax[cpu] >= 0.4.6, < 0.5.0a0',
-    'torch >= 2.0, < 2.1.0a0',
-    'torchvision',
-    'dm-tree >= 0.1, < 0.2.0a0',
-    'pandas',
-    'tabulate',
-    'termcolor',
+    "jax[cpu] >= 0.4.6, < 0.5.0a0",
+    "torch >= 2.0, < 2.1.0a0",
+    "torchvision",
+    "dm-tree >= 0.1, < 0.2.0a0",
+    "pandas",
+    "tabulate",
+    "termcolor",
 ]
 
+[tool.setuptools]
+include-package-data = true
+
 [tool.setuptools.packages.find]
 include = ["optree", "optree.*"]
 
+[tool.setuptools.package-data]
+optree = ['*.so', '*.pyd']
+
 # Wheel builder ################################################################
 # Reference: https://cibuildwheel.readthedocs.io
 [tool.cibuildwheel]
 archs = ["auto64"]
 skip = "*musllinux*"
 build-frontend = "build"
 build-verbosity = 3
@@ -132,14 +138,17 @@
 
 [tool.pydocstyle]
 convention = "google"
 
 [tool.doc8]
 max-line-length = 500
 
+[tool.codespell]
+ignore-words = "docs/source/spelling_wordlist.txt"
+
 [tool.ruff]
 target-version = "py37"
 line-length = 100
 show-source = true
 src = ["optree", "tests"]
 select = [
     "E", "W",  # pycodestyle
@@ -158,15 +167,14 @@
     "PIE",     # flake8-pie
     "PYI",     # flake8-pyi
     "Q",       # flake8-quotes
     "RSE",     # flake8-raise
     "RET",     # flake8-return
     "SIM",     # flake8-simplify
     "TID",     # flake8-tidy-imports
-    "PL",      # pylint
     "RUF",     # ruff
 ]
 ignore = [
     # E501: line too long
     # W505: doc line too long
     # too long docstring due to long example blocks
     "E501",
@@ -197,34 +205,27 @@
     "E402",  # module-import-not-at-top-of-file
     "F722",  # forward-annotation-syntax-error
     "F811",  # redefined-while-unused
 ]
 "setup.py" = [
     "ANN",   # flake8-annotations
 ]
-"benchmark.py" = [
-    "PLW2901",  # redefined-loop-name
-]
 "tests/**/*.py" = [
     "ANN",   # flake8-annotations
     "S",     # flake8-bandit
     "BLE",   # flake8-blind-except
     "SIM",   # flake8-simplify
-    "PL",    # pylint
 ]
 
 [tool.ruff.flake8-annotations]
 allow-star-arg-any = true
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 multiline-quotes = "double"
 inline-quotes = "single"
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.pylint]
-allow-magic-value-types = ["int", "str", "float"]
-
 [tool.pytest.ini_options]
 filterwarnings = ["error"]
```

### Comparing `optree-0.9.0/setup.py` & `optree-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,31 +88,29 @@
 
 
 VERSION_CONTENT = None
 
 try:
     if not version.__release__:
         try:
-            VERSION_CONTENT = VERSION_FILE.read_text(encoding='UTF-8')
+            VERSION_CONTENT = VERSION_FILE.read_text(encoding='utf-8')
             VERSION_FILE.write_text(
                 data=re.sub(
                     r"""__version__\s*=\s*('[^']+'|"[^"]+")""",
                     f'__version__ = {version.__version__!r}',
                     string=VERSION_CONTENT,
                 ),
-                encoding='UTF-8',
+                encoding='utf-8',
             )
         except OSError:
             VERSION_CONTENT = None
 
     setup(
         name='optree',
         version=version.__version__,
-        package_data={'sharedlib': ['*.so', '*.pyd']},
-        include_package_data=True,
         cmdclass={'build_ext': cmake_build_ext},
         ext_modules=[CMakeExtension('optree._C', source_dir=HERE)],
     )
 finally:
     if VERSION_CONTENT is not None:
-        with VERSION_FILE.open(mode='wt', encoding='UTF-8', newline='') as file:
+        with VERSION_FILE.open(mode='wt', encoding='utf-8', newline='') as file:
             file.write(VERSION_CONTENT)
```

### Comparing `optree-0.9.0/src/CMakeLists.txt` & `optree-0.9.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/src/optree.cpp` & `optree-0.9.1/src/optree.cpp`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/src/registry.cpp` & `optree-0.9.1/src/registry.cpp`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/src/treespec/flatten.cpp` & `optree-0.9.1/src/treespec/flatten.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 break;
             }
 
             case PyTreeKind::NamedTuple:
             case PyTreeKind::StructSequence: {
                 auto tuple = py::reinterpret_borrow<py::tuple>(handle);
                 node.arity = GET_SIZE<py::tuple>(tuple);
-                node.node_data = py::reinterpret_borrow<py::object>(tuple.get_type());
+                node.node_data = py::reinterpret_borrow<py::object>(py::type::handle_of(tuple));
                 for (ssize_t i = 0; i < node.arity; ++i) {
                     recurse(GET_ITEM_HANDLE<py::tuple>(tuple, i));
                 }
                 break;
             }
 
             case PyTreeKind::Deque: {
@@ -279,15 +279,15 @@
                 break;
             }
 
             case PyTreeKind::NamedTuple:
             case PyTreeKind::StructSequence: {
                 auto tuple = py::reinterpret_borrow<py::tuple>(handle);
                 node.arity = GET_SIZE<py::tuple>(tuple);
-                node.node_data = py::reinterpret_borrow<py::object>(tuple.get_type());
+                node.node_data = py::reinterpret_borrow<py::object>(py::type::handle_of(tuple));
                 for (ssize_t i = 0; i < node.arity; ++i) {
                     recurse(GET_ITEM_HANDLE<py::tuple>(tuple, i), py::int_(i));
                 }
                 break;
             }
 
             case PyTreeKind::Deque: {
@@ -502,19 +502,19 @@
                 if (GET_SIZE<py::tuple>(tuple) != node.arity) [[unlikely]] {
                     throw py::value_error(absl::StrFormat(
                         "namedtuple arity mismatch; expected: %ld, got: %ld; tuple: %s.",
                         node.arity,
                         GET_SIZE<py::tuple>(tuple),
                         py::repr(object)));
                 }
-                if (object.get_type().not_equal(node.node_data)) [[unlikely]] {
+                if (py::type::handle_of(object).not_equal(node.node_data)) [[unlikely]] {
                     throw py::value_error(absl::StrFormat(
                         "namedtuple type mismatch; expected type: %s, got type: %s; tuple: %s.",
                         py::repr(node.node_data),
-                        py::repr(object.get_type()),
+                        py::repr(py::type::handle_of(object)),
                         py::repr(object)));
                 }
                 for (ssize_t i = 0; i < node.arity; ++i) {
                     agenda.emplace_back(GET_ITEM_BORROW<py::tuple>(tuple, i));
                 }
                 break;
             }
@@ -541,42 +541,42 @@
                 if (GET_SIZE<py::tuple>(tuple) != node.arity) [[unlikely]] {
                     throw py::value_error(absl::StrFormat(
                         "PyStructSequence arity mismatch; expected: %ld, got: %ld; tuple: %s.",
                         node.arity,
                         GET_SIZE<py::tuple>(tuple),
                         py::repr(object)));
                 }
-                if (object.get_type().not_equal(node.node_data)) [[unlikely]] {
+                if (py::type::handle_of(object).not_equal(node.node_data)) [[unlikely]] {
                     throw py::value_error(
                         absl::StrFormat("PyStructSequence type mismatch; "
                                         "expected type: %s, got type: %s; tuple: %s.",
                                         py::repr(node.node_data),
-                                        py::repr(object.get_type()),
+                                        py::repr(py::type::handle_of(object)),
                                         py::repr(object)));
                 }
                 for (ssize_t i = 0; i < node.arity; ++i) {
                     agenda.emplace_back(GET_ITEM_BORROW<py::tuple>(tuple, i));
                 }
                 break;
             }
 
             case PyTreeKind::Custom: {
                 const PyTreeTypeRegistry::Registration* registration = nullptr;
                 if (m_none_is_leaf) [[unlikely]] {
-                    registration =
-                        PyTreeTypeRegistry::Lookup<NONE_IS_LEAF>(object.get_type(), m_namespace);
+                    registration = PyTreeTypeRegistry::Lookup<NONE_IS_LEAF>(
+                        py::type::handle_of(object), m_namespace);
                 } else [[likely]] {
-                    registration =
-                        PyTreeTypeRegistry::Lookup<NONE_IS_NODE>(object.get_type(), m_namespace);
+                    registration = PyTreeTypeRegistry::Lookup<NONE_IS_NODE>(
+                        py::type::handle_of(object), m_namespace);
                 }
                 if (registration != node.custom) [[unlikely]] {
                     throw py::value_error(absl::StrFormat(
                         "Custom node type mismatch; expected type: %s, got type: %s; value: %s.",
                         py::repr(node.custom->type),
-                        py::repr(object.get_type()),
+                        py::repr(py::type::handle_of(object)),
                         py::repr(object)));
                 }
                 py::tuple out = py::cast<py::tuple>(node.custom->to_iterable(object));
                 const ssize_t num_out = GET_SIZE<py::tuple>(out);
                 if (num_out != 2 && num_out != 3) [[unlikely]] {
                     throw std::runtime_error(absl::StrFormat(
                         "PyTree custom flatten function for type %s should return a 2- or 3-tuple, "
```

### Comparing `optree-0.9.0/src/treespec/traversal.cpp` & `optree-0.9.1/src/treespec/traversal.cpp`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/src/treespec/treespec.cpp` & `optree-0.9.1/src/treespec/treespec.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,15 @@
 }
 
 template <bool NoneIsLeaf>
 /*static*/ PyTreeKind PyTreeSpec::GetKind(const py::handle& handle,
                                           PyTreeTypeRegistry::Registration const** custom,
                                           const std::string& registry_namespace) {
     const PyTreeTypeRegistry::Registration* registration =
-        PyTreeTypeRegistry::Lookup<NoneIsLeaf>(handle.get_type(), registry_namespace);
+        PyTreeTypeRegistry::Lookup<NoneIsLeaf>(py::type::handle_of(handle), registry_namespace);
     if (registration) [[likely]] {
         if (registration->kind == PyTreeKind::Custom) [[unlikely]] {
             *custom = registration;
         } else [[likely]] {
             *custom = nullptr;
         }
         return registration->kind;
```

### Comparing `optree-0.9.0/src/treespec/unflatten.cpp` & `optree-0.9.1/src/treespec/unflatten.cpp`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/tests/test_ops.py` & `optree-0.9.1/tests/test_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,16 @@
 
 
 @parametrize(
     tree=[
         [0, ((1, 2), 3, (4, (5, 6, 7))), 8, 9],
         [0, ((1, 2), 3, (4, (5, 6, 7))), 8, 9],
         [0, ((1, (2, 3)), (4, (5, 6, 7))), 8, 9],
-        [0, {'d': (4, (5, 6, 7)), 'c': ((1, {'b': 3, 'a': 2})), 'e': [8, 9]}],
-        [0, {1: (4, (5, 6, 7)), 1.1: ((1, {'b': 3, 'a': 2})), 'c': [8, 9]}],
+        [0, {'d': (4, (5, 6, 7)), 'c': (1, {'b': 3, 'a': 2}), 'e': [8, 9]}],
+        [0, {1: (4, (5, 6, 7)), 1.1: (1, {'b': 3, 'a': 2}), 'c': [8, 9]}],
         [0, OrderedDict([(1, (1, (2, 3, 4))), (1.1, ((5, {'b': 7, 'a': 6}))), ('c', [8, 9])])],
     ],
     none_is_leaf=[False, True],
 )
 def test_flatten_order(tree, none_is_leaf):
     flat, _ = optree.tree_flatten(tree, none_is_leaf=none_is_leaf)
```

### Comparing `optree-0.9.0/tests/test_prefix_errors.py` & `optree-0.9.1/tests/test_prefix_errors.py`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/tests/test_registry.py` & `optree-0.9.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/tests/test_treespec.py` & `optree-0.9.1/tests/test_treespec.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,37 +116,37 @@
 
 def test_with_namespace():
     tree = NAMESPACED_TREE
 
     for namespace in ('', 'undefined'):
         leaves, treespec = optree.tree_flatten(tree, none_is_leaf=False, namespace=namespace)
         assert leaves == [tree]
-        assert str(treespec) == ('PyTreeSpec(*)')
+        assert str(treespec) == 'PyTreeSpec(*)'
         paths, leaves, treespec = optree.tree_flatten_with_path(
             tree,
             none_is_leaf=False,
             namespace=namespace,
         )
         assert paths == [()]
         assert leaves == [tree]
         assert paths == treespec.paths()
-        assert str(treespec) == ('PyTreeSpec(*)')
+        assert str(treespec) == 'PyTreeSpec(*)'
     for namespace in ('', 'undefined'):
         leaves, treespec = optree.tree_flatten(tree, none_is_leaf=True, namespace=namespace)
         assert leaves == [tree]
-        assert str(treespec) == ('PyTreeSpec(*, NoneIsLeaf)')
+        assert str(treespec) == 'PyTreeSpec(*, NoneIsLeaf)'
         paths, leaves, treespec = optree.tree_flatten_with_path(
             tree,
             none_is_leaf=True,
             namespace=namespace,
         )
         assert paths == [()]
         assert leaves == [tree]
         assert paths == treespec.paths()
-        assert str(treespec) == ('PyTreeSpec(*, NoneIsLeaf)')
+        assert str(treespec) == 'PyTreeSpec(*, NoneIsLeaf)'
 
     expected_string = "PyTreeSpec(CustomTreeNode(MyAnotherDict[['foo', 'baz']], [CustomTreeNode(MyAnotherDict[['c', 'b', 'a']], [None, *, *]), *]), namespace='namespace')"
     leaves, treespec = optree.tree_flatten(tree, none_is_leaf=False, namespace='namespace')
     assert leaves == [2, 1, 101]
     assert str(treespec) == expected_string
     paths, leaves, treespec = optree.tree_flatten_with_path(
         tree,
```

### Comparing `optree-0.9.0/tests/test_typing.py` & `optree-0.9.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `optree-0.9.0/tests/test_utils.py` & `optree-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

