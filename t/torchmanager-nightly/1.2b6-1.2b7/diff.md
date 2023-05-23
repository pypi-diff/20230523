# Comparing `tmp/torchmanager_nightly-1.2b6.tar.gz` & `tmp/torchmanager_nightly-1.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2b6.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2b7.tar", max compression
```

## Comparing `torchmanager_nightly-1.2b6.tar` & `torchmanager_nightly-1.2b7.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b6/LICENSE
--rw-r--r--   0        0        0      659 2023-05-16 17:55:19.687071 torchmanager_nightly-1.2b6/pyproject.toml
--rw-r--r--   0        0        0      290 2023-05-11 18:30:52.166030 torchmanager_nightly-1.2b6/torchmanager/__init__.py
--rw-r--r--   0        0        0    10862 2023-05-11 18:30:52.166340 torchmanager_nightly-1.2b6/torchmanager/basic.py
--rw-r--r--   0        0        0      638 2023-05-11 18:30:52.166882 torchmanager_nightly-1.2b6/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-05-11 18:30:52.167385 torchmanager_nightly-1.2b6/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4628 2023-05-11 18:16:52.815262 torchmanager_nightly-1.2b6/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-05-11 14:13:25.691390 torchmanager_nightly-1.2b6/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-05-11 14:13:25.691561 torchmanager_nightly-1.2b6/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4642 2023-05-11 18:30:52.167957 torchmanager_nightly-1.2b6/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-05-11 14:13:25.691701 torchmanager_nightly-1.2b6/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2599 2023-05-11 18:30:52.168441 torchmanager_nightly-1.2b6/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      963 2023-05-11 14:13:25.691910 torchmanager_nightly-1.2b6/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-05-11 18:30:52.168697 torchmanager_nightly-1.2b6/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     2930 2023-05-16 17:55:19.687727 torchmanager_nightly-1.2b6/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-05-11 14:13:25.692993 torchmanager_nightly-1.2b6/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6968 2023-05-11 18:30:52.169618 torchmanager_nightly-1.2b6/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-05-11 18:30:52.170275 torchmanager_nightly-1.2b6/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-05-11 18:30:52.170737 torchmanager_nightly-1.2b6/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-05-11 14:13:25.694420 torchmanager_nightly-1.2b6/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-05-11 18:30:52.171245 torchmanager_nightly-1.2b6/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5757 2023-05-11 18:30:52.171684 torchmanager_nightly-1.2b6/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3117 2023-05-11 18:30:52.172126 torchmanager_nightly-1.2b6/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      333 2023-05-11 18:30:52.172601 torchmanager_nightly-1.2b6/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-11 18:30:52.173018 torchmanager_nightly-1.2b6/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3678 2023-05-11 18:30:52.173338 torchmanager_nightly-1.2b6/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-05-11 18:30:52.173571 torchmanager_nightly-1.2b6/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-05-11 18:30:52.173883 torchmanager_nightly-1.2b6/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4003 2023-05-11 18:30:52.174208 torchmanager_nightly-1.2b6/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     9558 2023-05-16 21:36:19.364793 torchmanager_nightly-1.2b6/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-05-11 18:30:52.175047 torchmanager_nightly-1.2b6/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-11 14:13:25.700320 torchmanager_nightly-1.2b6/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-05-11 18:30:52.175406 torchmanager_nightly-1.2b6/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    14038 2023-05-16 21:36:41.276799 torchmanager_nightly-1.2b6/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-05-11 18:30:52.176395 torchmanager_nightly-1.2b6/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-05-11 18:30:52.176766 torchmanager_nightly-1.2b6/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-05-11 18:30:52.177250 torchmanager_nightly-1.2b6/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-05-11 14:13:25.702386 torchmanager_nightly-1.2b6/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-05-11 14:13:30.152271 torchmanager_nightly-1.2b6/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-05-11 14:13:25.703024 torchmanager_nightly-1.2b6/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-05-11 14:13:25.703150 torchmanager_nightly-1.2b6/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2772 2023-05-11 18:30:52.178286 torchmanager_nightly-1.2b6/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-05-11 18:30:52.178624 torchmanager_nightly-1.2b6/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-05-11 18:30:52.178907 torchmanager_nightly-1.2b6/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-05-11 14:13:25.704534 torchmanager_nightly-1.2b6/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5260 2023-05-16 17:55:19.688600 torchmanager_nightly-1.2b6/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-05-11 18:30:52.179903 torchmanager_nightly-1.2b6/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-05-11 14:13:25.706452 torchmanager_nightly-1.2b6/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b6/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-03-14 14:54:20.813363 torchmanager_nightly-1.2b7/LICENSE
+-rw-r--r--   0        0        0      659 2023-05-23 18:57:38.725893 torchmanager_nightly-1.2b7/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-05-23 18:57:38.726329 torchmanager_nightly-1.2b7/torchmanager/__init__.py
+-rw-r--r--   0        0        0    10862 2023-05-23 18:57:38.726797 torchmanager_nightly-1.2b7/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-05-23 18:57:38.727334 torchmanager_nightly-1.2b7/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-05-23 18:57:38.727736 torchmanager_nightly-1.2b7/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4628 2023-05-15 18:28:33.014982 torchmanager_nightly-1.2b7/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-05-09 14:19:55.056821 torchmanager_nightly-1.2b7/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-05-09 14:19:55.056902 torchmanager_nightly-1.2b7/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-05-23 18:57:38.728136 torchmanager_nightly-1.2b7/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-05-09 14:19:55.057101 torchmanager_nightly-1.2b7/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-05-23 18:57:38.728530 torchmanager_nightly-1.2b7/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      964 2023-05-23 18:57:38.729162 torchmanager_nightly-1.2b7/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-05-23 18:57:38.729492 torchmanager_nightly-1.2b7/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-23 18:57:38.729718 torchmanager_nightly-1.2b7/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-05-09 14:19:55.057599 torchmanager_nightly-1.2b7/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6968 2023-05-23 18:57:38.730045 torchmanager_nightly-1.2b7/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-05-23 18:57:38.730234 torchmanager_nightly-1.2b7/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-05-23 18:57:38.730592 torchmanager_nightly-1.2b7/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-05-09 14:19:55.058468 torchmanager_nightly-1.2b7/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-05-23 18:57:38.731189 torchmanager_nightly-1.2b7/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5757 2023-05-23 18:57:38.731564 torchmanager_nightly-1.2b7/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3117 2023-05-23 18:57:38.731935 torchmanager_nightly-1.2b7/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      362 2023-05-23 18:58:49.721266 torchmanager_nightly-1.2b7/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-23 18:57:38.732808 torchmanager_nightly-1.2b7/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3678 2023-05-23 18:57:38.733030 torchmanager_nightly-1.2b7/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-05-23 18:57:38.733329 torchmanager_nightly-1.2b7/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-05-23 18:57:38.733518 torchmanager_nightly-1.2b7/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4003 2023-05-23 18:57:38.734103 torchmanager_nightly-1.2b7/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2220 2023-05-23 18:57:38.734335 torchmanager_nightly-1.2b7/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     9558 2023-05-23 18:57:38.734660 torchmanager_nightly-1.2b7/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-05-23 18:57:38.734979 torchmanager_nightly-1.2b7/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-05-09 14:19:55.060536 torchmanager_nightly-1.2b7/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-05-23 18:57:38.735541 torchmanager_nightly-1.2b7/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    13808 2023-05-23 18:57:38.736027 torchmanager_nightly-1.2b7/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-05-23 18:57:38.736545 torchmanager_nightly-1.2b7/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-23 18:57:38.737397 torchmanager_nightly-1.2b7/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-05-23 18:57:38.737605 torchmanager_nightly-1.2b7/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-05-09 14:19:55.062103 torchmanager_nightly-1.2b7/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-05-09 14:25:54.610406 torchmanager_nightly-1.2b7/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-05-09 14:19:55.062828 torchmanager_nightly-1.2b7/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-05-09 14:19:55.063042 torchmanager_nightly-1.2b7/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2772 2023-05-23 18:57:38.737932 torchmanager_nightly-1.2b7/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-05-23 18:57:38.738272 torchmanager_nightly-1.2b7/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-23 18:57:38.738579 torchmanager_nightly-1.2b7/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-05-09 14:19:55.064483 torchmanager_nightly-1.2b7/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5260 2023-05-23 18:57:38.738874 torchmanager_nightly-1.2b7/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-05-23 18:57:38.739234 torchmanager_nightly-1.2b7/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-09 14:19:55.065240 torchmanager_nightly-1.2b7/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b7/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2b6/LICENSE` & `torchmanager_nightly-1.2b7/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/pyproject.toml` & `torchmanager_nightly-1.2b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2b6"
-description = "PyTorch Training Manager v1.2 (Beta 6)"
+version = "1.2b7"
+description = "PyTorch Training Manager v1.2 (Beta 7)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
```

### Comparing `torchmanager_nightly-1.2b6/torchmanager/basic.py` & `torchmanager_nightly-1.2b7/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.2b7/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/compatibility.py` & `torchmanager_nightly-1.2b7/torchmanager/compatibility.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
             obj.replace_nan = False
         elif isinstance(obj, KLDiv) and not hasattr(obj, "_t"):
             obj._t = None
 
         # convert Accuracy and MAE
         if isinstance(obj, Accuracy) and isinstance(obj, MAE) and not hasattr(obj, "reduction"):
             obj.reduction = Reduction.MEAN
-    return obj
+    return obj
```

### Comparing `torchmanager_nightly-1.2b6/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2b7/torchmanager/configs/basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torchmanager_core import argparse, abc, os, shutil, torch, view
 from torchmanager_core.typing import Any, Union
-from torchmanager_core import VERSION
+from torchmanager_core import VERSION, DESCRIPTION
 
 
 class Configs(argparse.Namespace, abc.ABC):
     """
     Basic Configurations
     
     * extends: `argparse.Namespace`
@@ -58,13 +58,14 @@
 
     @staticmethod
     def get_arguments(parser: Union[argparse.ArgumentParser, argparse._ArgumentGroup] = argparse.ArgumentParser()) -> Union[argparse.ArgumentParser, argparse._ArgumentGroup]:
         parser.add_argument("-exp", "--experiment", type=str, default="test.exp", help="The name of experiment")
         parser.add_argument("--replace_experiment", action="store_true", default=False, help="The flag to replace given experiment if exists.")
         return parser
 
-    def show_environments(self) -> None:
+    def show_environments(self, description: str = DESCRIPTION) -> None:
+        view.logger.info(description)
         view.logger.info(f"torch={torch.__version__}, torchmanager={VERSION}")
 
     @abc.abstractmethod
     def show_settings(self) -> None:
         pass
```

### Comparing `torchmanager_nightly-1.2b6/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2b7/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2b7/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2b7/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2b7/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2b7/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2b7/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2b7/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2b7/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.2b7/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2b7/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.2b7/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/testing.py` & `torchmanager_nightly-1.2b7/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2b7/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2b7/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager/training.py` & `torchmanager_nightly-1.2b7/torchmanager/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,19 +124,15 @@
                 # check for iterations
                 if batch + 1 >= iterations:
                     break
         finally:
             # end epoch training
             if progress_bar is not None:
                 progress_bar.close()
-
-        # summarize
-        summary = {name: float(fn.result.detach()) for name, fn in self.metric_fns.items() if not name.startswith("val_")}
-        summary["loss"] = float(self.compiled_losses.result.detach())
-        return summary
+        return self.summary
 
     def backward(self, loss: torch.Tensor) -> None:
         """
         Backward function to calculate the gradients
         
         - Parameters:
             - loss: A `torch.Tensor` of loss value
@@ -245,26 +241,26 @@
                         val_message += ", "
                     val_message += f"{name}={value:.4f}"
                 view.logger.info(val_message)
 
             # on train end
             for c in callbacks_list:
                 c.on_train_end(self.raw_model)
-            return self.raw_model
         except KeyboardInterrupt:
             view.logger.info("Training interrupted.")
-            return self.raw_model
+            pass
         except Exception as error:
             view.logger.error(error)
             runtime_error = errors.StopTraining(self.current_epoch, "Training failed.")
             raise runtime_error from error
         finally:
             self.model = self.raw_model.to(cpu)
             self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
             devices.empty_cache()
+        return self.raw_model
 
     def train_step(self, x_train: Any, y_train: Any) -> Dict[str, float]:
         """
         A single training step
 
         - Parameters:
             - x_train: The training data
```

### Comparing `torchmanager_nightly-1.2b6/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2b7/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2b7/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2b7/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2b7/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b6/torchmanager_core/version.py` & `torchmanager_nightly-1.2b7/torchmanager_core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b6")
-DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 6)"
+CURRENT = Version("v1.2b7")
+DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 7)"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2b6/PKG-INFO` & `torchmanager_nightly-1.2b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b6
-Summary: PyTorch Training Manager v1.2 (Beta 6)
+Version: 1.2b7
+Summary: PyTorch Training Manager v1.2 (Beta 7)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

