# Comparing `tmp/lightning-graphcore-0.1.0rc0.tar.gz` & `tmp/lightning-graphcore-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-graphcore-0.1.0rc0.tar", last modified: Thu Apr 27 14:17:44 2023, max compression
+gzip compressed data, was "lightning-graphcore-0.1.0rc1.tar", last modified: Tue May 23 13:36:27 2023, max compression
```

## Comparing `lightning-graphcore-0.1.0rc0.tar` & `lightning-graphcore-0.1.0rc1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-04-27 14:17:27.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:17:44.244911 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 14:17:44.000000 lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.528030 lightning-graphcore-0.1.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-23 13:36:16.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:36:27.532030 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 13:36:27.000000 lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/top_level.txt
```

### Comparing `lightning-graphcore-0.1.0rc0/LICENSE` & `lightning-graphcore-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc0/MANIFEST.in` & `lightning-graphcore-0.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc0/PKG-INFO` & `lightning-graphcore-0.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
```

### Comparing `lightning-graphcore-0.1.0rc0/README.md` & `lightning-graphcore-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc0/setup.py` & `lightning-graphcore-0.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc0/src/lightning_graphcore/accelerator.py` & `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc0/src/lightning_graphcore/precision.py` & `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.1.0rc0/src/lightning_graphcore/strategy.py` & `lightning-graphcore-0.1.0rc1/src/lightning_graphcore/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 if package_available("lightning"):
     import lightning.pytorch as pl
     from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning.fabric.utilities.cloud_io import get_filesystem
     from lightning.pytorch import Trainer
     from lightning.pytorch.accelerators import Accelerator
-    from lightning.pytorch.overrides.base import _LightningModuleWrapperBase
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.parallel import ParallelStrategy
     from lightning.pytorch.strategies.strategy import TBroadcast
     from lightning.pytorch.strategies.utils import _fp_to_half
     from lightning.pytorch.trainer.states import RunningStage, TrainerFn
     from lightning.pytorch.utilities import rank_zero_warn
     from lightning.pytorch.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
@@ -40,29 +39,29 @@
     from lightning.pytorch.utilities.types import STEP_OUTPUT
 elif package_available("pytorch_lightning"):
     import pytorch_lightning as pl
     from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
     from lightning_fabric.utilities.cloud_io import get_filesystem
     from pytorch_lightning import Trainer
     from pytorch_lightning.accelerators import Accelerator
-    from pytorch_lightning.overrides.base import _LightningModuleWrapperBase
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.parallel import ParallelStrategy
     from pytorch_lightning.strategies.strategy import TBroadcast
     from pytorch_lightning.strategies.utils import _fp_to_half
     from pytorch_lightning.trainer.states import RunningStage, TrainerFn
     from pytorch_lightning.utilities import rank_zero_warn
     from pytorch_lightning.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
     from pytorch_lightning.utilities.exceptions import MisconfigurationException
     from pytorch_lightning.utilities.model_helpers import is_overridden
     from pytorch_lightning.utilities.types import STEP_OUTPUT
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 from lightning_graphcore.accelerator import _IPU_AVAILABLE, _POPTORCH_AVAILABLE
+from lightning_graphcore.utils import _LightningModuleWrapperBase
 
 if _POPTORCH_AVAILABLE:
     import poptorch
 else:
     poptorch = None
```

### Comparing `lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/PKG-INFO` & `lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-graphcore
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Lightning support for GraphCore accelerators
 Home-page: https://github.com/Lightning-AI/lightning-graphcore
 Download-URL: https://github.com/Lightning-AI/lightning-graphcore
 Author: Lightning-AI et al.
 Author-email: name@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-graphcore/issues
```

### Comparing `lightning-graphcore-0.1.0rc0/src/lightning_graphcore.egg-info/SOURCES.txt` & `lightning-graphcore-0.1.0rc1/src/lightning_graphcore.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 requirements.txt
 setup.py
 src/lightning_graphcore/__about__.py
 src/lightning_graphcore/__init__.py
 src/lightning_graphcore/accelerator.py
 src/lightning_graphcore/precision.py
 src/lightning_graphcore/strategy.py
+src/lightning_graphcore/utils.py
 src/lightning_graphcore.egg-info/PKG-INFO
 src/lightning_graphcore.egg-info/SOURCES.txt
 src/lightning_graphcore.egg-info/dependency_links.txt
 src/lightning_graphcore.egg-info/not-zip-safe
 src/lightning_graphcore.egg-info/requires.txt
 src/lightning_graphcore.egg-info/top_level.txt
```

