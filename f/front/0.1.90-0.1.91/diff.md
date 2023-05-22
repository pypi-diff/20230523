# Comparing `tmp/front-0.1.90.tar.gz` & `tmp/front-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "front-0.1.90.tar", last modified: Sat May 20 02:21:28 2023, max compression
+gzip compressed data, was "front-0.1.91.tar", last modified: Mon May 22 22:02:18 2023, max compression
```

## Comparing `front-0.1.90.tar` & `front-0.1.91.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.361309 front-0.1.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 02:20:38.000000 front-0.1.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-20 02:21:28.361309 front-0.1.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-20 02:20:38.000000 front-0.1.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.357309 front-0.1.90/front/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-20 02:20:38.000000 front-0.1.90/front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-20 02:20:38.000000 front-0.1.90/front/app_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-20 02:20:38.000000 front-0.1.90/front/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-05-20 02:20:38.000000 front-0.1.90/front/crude.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-20 02:20:38.000000 front-0.1.90/front/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-20 02:20:38.000000 front-0.1.90/front/data_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.361309 front-0.1.90/front/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-20 02:20:38.000000 front-0.1.90/front/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-20 02:20:38.000000 front-0.1.90/front/elements/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-20 02:20:38.000000 front-0.1.90/front/elements/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-20 02:20:38.000000 front-0.1.90/front/elements/tree_maker_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.361309 front-0.1.90/front/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/kaggle_front.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/pos_key_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/simple_ml_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/tw_data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-20 02:20:38.000000 front-0.1.90/front/examples/wordle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-20 02:20:38.000000 front-0.1.90/front/py2pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.361309 front-0.1.90/front/scrap/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 02:20:38.000000 front-0.1.90/front/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-20 02:20:38.000000 front-0.1.90/front/scrap/binder_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-20 02:20:38.000000 front-0.1.90/front/scrap/binder_proposal_no_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-20 02:20:38.000000 front-0.1.90/front/scrap/state_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-20 02:20:38.000000 front-0.1.90/front/scrap/tw_simple_new_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-20 02:20:38.000000 front-0.1.90/front/spec_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-20 02:20:38.000000 front-0.1.90/front/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.361309 front-0.1.90/front/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/app_identity_pydantic_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/app_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_crude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_crudify_based_on_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_py2pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/test_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-20 02:20:38.000000 front-0.1.90/front/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-20 02:20:38.000000 front-0.1.90/front/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-20 02:20:38.000000 front-0.1.90/front/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-20 02:20:38.000000 front-0.1.90/front/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:21:28.361309 front-0.1.90/front.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-20 02:21:28.000000 front-0.1.90/front.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-20 02:21:28.000000 front-0.1.90/front.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:21:28.000000 front-0.1.90/front.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:21:28.000000 front-0.1.90/front.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 02:21:28.000000 front-0.1.90/front.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 02:21:28.000000 front-0.1.90/front.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-20 02:21:28.365309 front-0.1.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-20 02:20:38.000000 front-0.1.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 22:01:31.000000 front-0.1.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-22 22:02:18.483954 front-0.1.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-22 22:01:31.000000 front-0.1.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.479954 front-0.1.91/front/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-22 22:01:31.000000 front-0.1.91/front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-22 22:01:31.000000 front-0.1.91/front/app_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 22:01:31.000000 front-0.1.91/front/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-05-22 22:01:31.000000 front-0.1.91/front/crude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-22 22:01:31.000000 front-0.1.91/front/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-22 22:01:31.000000 front-0.1.91/front/data_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 22:01:31.000000 front-0.1.91/front/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-05-22 22:02:17.000000 front-0.1.91/front/elements/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-22 22:01:31.000000 front-0.1.91/front/elements/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-22 22:01:31.000000 front-0.1.91/front/elements/tree_maker_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/kaggle_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/pos_key_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/simple_ml_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/tw_data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/wordle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-22 22:01:31.000000 front-0.1.91/front/py2pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/scrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/binder_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/binder_proposal_no_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/state_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/tw_simple_new_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-22 22:01:31.000000 front-0.1.91/front/spec_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-22 22:01:31.000000 front-0.1.91/front/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/app_identity_pydantic_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/app_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_crude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_crudify_based_on_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_py2pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-22 22:01:31.000000 front-0.1.91/front/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 22:01:31.000000 front-0.1.91/front/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-22 22:01:31.000000 front-0.1.91/front/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.479954 front-0.1.91/front.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 22:02:18.483954 front-0.1.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 22:01:31.000000 front-0.1.91/setup.py
```

### Comparing `front-0.1.90/LICENSE` & `front-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `front-0.1.90/PKG-INFO` & `front-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: front
-Version: 0.1.90
+Version: 0.1.91
 Summary: Getting from python objects to UIs exposing them
 Home-page: https://github.com/i2mint/front
 Author: OtoSense
 License: apache-2.0
 Description: # front
         
         [Documentation here](https://i2mint.github.io/front/)
```

### Comparing `front-0.1.90/README.md` & `front-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/__init__.py` & `front-0.1.91/front/__init__.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/app_maker.py` & `front-0.1.91/front/app_maker.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/base.py` & `front-0.1.91/front/base.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/crude.py` & `front-0.1.91/front/crude.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/dag.py` & `front-0.1.91/front/dag.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/data_binding.py` & `front-0.1.91/front/data_binding.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/elements/elements.py` & `front-0.1.91/front/elements/elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,43 +13,46 @@
     get_args,
     get_origin,
     Sequence,
 )
 from front.data_binding import BoundData, ValueNotSet
 from i2 import Sig
 from inspect import _empty
-from front.types import FrontElementName
+from front.types import FrontElementDisplay, FrontElementName
 from front.util import deep_merge, get_value
 from i2.signatures import call_forgivingly
 from pydantic import validate_arguments
 from front.data_binding import Binder as b
 
 
 @dataclass
 class FrontElementBase(ABC):
     obj: Any = None
     name: FrontElementName = None
+    display: FrontElementDisplay = True
 
     def __post_init__(self):
         self.name = get_value(self.name, self.obj) or ''
+        self.display = get_value(self.display, self.obj)
 
     def pre_render(self):
         pass
 
     @abstractmethod
     def render(self):
         pass
 
     def post_render(self, render_result):
         return render_result
 
     def __call__(self):
-        self.pre_render()
-        r = self.render()
-        return self.post_render(r)
+        if self.display:
+            self.pre_render()
+            r = self.render()
+            return self.post_render(r)
 
 
 ELEMENT_KEY = '_front_element'
 DEFAULT_INPUT_KEY = '_default'
 FrontElementSpec = TypedDict('FrontElementSpec', {ELEMENT_KEY: FrontElementBase})
 
 
@@ -60,14 +63,17 @@
     except KeyError:
         raise RuntimeError(
             f'Key "{ELEMENT_KEY}" is missing in the following element specification: {spec}'
         )
     try:
         return factory(**_spec)
     except Exception as e:
+        from i2 import Sig
+
+        print('COUCOU', Sig(factory))
         print(f'An error occurred when trying to build element {factory}')
         raise e
 
 
 def mk_input_element_specs(obj, inputs):
     def mk_input_spec(p):
         input_spec = inputs_spec.get(p.name, {})
@@ -102,17 +108,21 @@
     return elements_spec
 
 
 class FrontContainerBase(FrontElementBase):
     children: Iterable[FrontElementBase]
 
     def __init__(
-        self, obj=None, name: FrontElementName = None, **kwargs: FrontElementSpec
+        self,
+        obj=None,
+        name: FrontElementName = None,
+        display: FrontElementDisplay = True,
+        **kwargs: FrontElementSpec,
     ):
-        super().__init__(obj=obj, name=name)
+        super().__init__(obj=obj, name=name, display=display)
         specs = [dict(dict(name=k, obj=obj), **v) for k, v in kwargs.items()]
         self.children = list(map(mk_element_from_spec, specs))
 
     def _render_children(self):
         for child in self.children:
             child()
 
@@ -125,17 +135,18 @@
 class TextSectionBase(FrontComponentBase):
     def __init__(
         self,
         content: str,
         kind: str = 'text',
         obj: Any = None,
         name: FrontElementName = None,
+        display: FrontElementDisplay = True,
         **kwargs,
     ):
-        super().__init__(obj, name)
+        super().__init__(obj=obj, name=name, display=display)
         self.content = get_value(content, self.obj) or ''
         self.kind = get_value(kind, self.obj)
         self.kwargs = kwargs
 
 
 @dataclass
 class InputBase(FrontComponentBase):
@@ -223,21 +234,22 @@
 class ExecContainerBase(FrontContainerBase):
     def __init__(
         self,
         obj: Callable,
         inputs: dict,
         output: dict,
         name: FrontElementName = None,
+        display: FrontElementDisplay = True,
         auto_submit: bool = False,
         on_submit: Callable[[Any], None] = None,
     ):
         self.inputs = inputs
         self._feed_kwargs_input_spec()
         element_specs = dict(mk_input_element_specs(obj, inputs), output=output)
-        super().__init__(obj=obj, name=name, **element_specs)
+        super().__init__(obj=obj, name=name, display=display, **element_specs)
         self.auto_submit = auto_submit
         self.on_submit = on_submit
 
     def _feed_kwargs_input_spec(self):
         inputs_spec = dict(self.inputs)
         kwargs_spec = inputs_spec.pop('kwargs', None)
         if kwargs_spec:
@@ -274,25 +286,27 @@
 
 
 class MultiSourceInputBase(InputBase):
     def __init__(
         self,
         obj=None,
         name: FrontElementName = None,
+        display: FrontElementDisplay = True,
         input_key: str = None,
         value: Any = ValueNotSet,
         on_value_change: Callable[..., None] = None,
         bound_data_factory: Callable = None,
         is_noneable: bool = False,
         disabled: bool = False,
         **kwargs: FrontElementSpec,
     ):
         super().__init__(
             obj=obj,
             name=name,
+            display=display,
             input_key=input_key,
             value=value,
             on_value_change=on_value_change,
             bound_data_factory=bound_data_factory,
             is_noneable=is_noneable,
             disabled=disabled,
         )
```

### Comparing `front-0.1.90/front/elements/implementation.py` & `front-0.1.91/front/elements/implementation.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/elements/tree_maker_base.py` & `front-0.1.91/front/elements/tree_maker_base.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/experimentation.py` & `front-0.1.91/front/examples/experimentation.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/issues.py` & `front-0.1.91/front/examples/issues.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/kaggle_front.py` & `front-0.1.91/front/examples/kaggle_front.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/pos_key_args.py` & `front-0.1.91/front/examples/pos_key_args.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/simple.py` & `front-0.1.91/front/examples/simple.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/simple_ml_1.py` & `front-0.1.91/front/examples/simple_ml_1.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/tw_data_binding.py` & `front-0.1.91/front/examples/tw_data_binding.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/examples/wordle.py` & `front-0.1.91/front/examples/wordle.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/py2pydantic.py` & `front-0.1.91/front/py2pydantic.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/scrap/binder_proposal.py` & `front-0.1.91/front/scrap/binder_proposal.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/scrap/binder_proposal_no_desc.py` & `front-0.1.91/front/scrap/binder_proposal_no_desc.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/scrap/state_proposal.py` & `front-0.1.91/front/scrap/state_proposal.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/spec_maker_base.py` & `front-0.1.91/front/spec_maker_base.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/state.py` & `front-0.1.91/front/state.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/test_combos.py` & `front-0.1.91/front/tests/test_combos.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/test_crude.py` & `front-0.1.91/front/tests/test_crude.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/test_crudify_based_on_names.py` & `front-0.1.91/front/tests/test_crudify_based_on_names.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/test_py2pydantic.py` & `front-0.1.91/front/tests/test_py2pydantic.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/test_state.py` & `front-0.1.91/front/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/test_use_case.py` & `front-0.1.91/front/tests/test_use_case.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tests/util.py` & `front-0.1.91/front/tests/util.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/tools.py` & `front-0.1.91/front/tools.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front/util.py` & `front-0.1.91/front/util.py`

 * *Files identical despite different names*

### Comparing `front-0.1.90/front.egg-info/PKG-INFO` & `front-0.1.91/front.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: front
-Version: 0.1.90
+Version: 0.1.91
 Summary: Getting from python objects to UIs exposing them
 Home-page: https://github.com/i2mint/front
 Author: OtoSense
 License: apache-2.0
 Description: # front
         
         [Documentation here](https://i2mint.github.io/front/)
```

### Comparing `front-0.1.90/front.egg-info/SOURCES.txt` & `front-0.1.91/front.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `front-0.1.90/setup.cfg` & `front-0.1.91/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = front
-version = 0.1.90
+version = 0.1.91
 url = https://github.com/i2mint/front
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Getting from python objects to UIs exposing them
```

