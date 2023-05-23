# Comparing `tmp/PVNet-0.0.8.tar.gz` & `tmp/PVNet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-0.0.8.tar", last modified: Thu Nov 24 16:33:59 2022, max compression
+gzip compressed data, was "PVNet-0.0.9.tar", last modified: Thu May 18 16:08:24 2023, max compression
```

## Comparing `PVNet-0.0.8.tar` & `PVNet-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:59.699701 PVNet-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-11-24 16:33:42.000000 PVNet-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-11-24 16:33:42.000000 PVNet-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-11-24 16:33:59.699701 PVNet-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:59.695701 PVNet-0.0.8/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-11-24 16:33:59.000000 PVNet-0.0.8/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-11-24 16:33:59.000000 PVNet-0.0.8/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-24 16:33:59.000000 PVNet-0.0.8/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-11-24 16:33:59.000000 PVNet-0.0.8/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-11-24 16:33:59.000000 PVNet-0.0.8/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-11-24 16:33:42.000000 PVNet-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:59.695701 PVNet-0.0.8/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:42.000000 PVNet-0.0.8/pvnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:59.695701 PVNet-0.0.8/pvnet/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:42.000000 PVNet-0.0.8/pvnet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2022-11-24 16:33:42.000000 PVNet-0.0.8/pvnet/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2022-11-24 16:33:43.000000 PVNet-0.0.8/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2022-11-24 16:33:43.000000 PVNet-0.0.8/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-11-24 16:33:43.000000 PVNet-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-11-24 16:33:43.000000 PVNet-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-11-24 16:33:43.000000 PVNet-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-24 16:33:59.699701 PVNet-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      723 2022-11-24 16:33:45.000000 PVNet-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:59.699701 PVNet-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 16:33:43.000000 PVNet-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2022-11-24 16:33:43.000000 PVNet-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-11-24 16:33:43.000000 PVNet-0.0.8/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2022-11-24 16:33:43.000000 PVNet-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-18 16:08:10.000000 PVNet-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 16:08:10.000000 PVNet-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 16:08:24.583270 PVNet-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-18 16:08:10.000000 PVNet-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/pvnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/data/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/pvnet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-18 16:08:10.000000 PVNet-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 16:08:10.000000 PVNet-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 16:08:10.000000 PVNet-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:08:24.583270 PVNet-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-18 16:08:10.000000 PVNet-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-18 16:08:10.000000 PVNet-0.0.9/tests/conftest.py
```

### Comparing `PVNet-0.0.8/LICENSE` & `PVNet-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-0.0.8/PKG-INFO` & `PVNet-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: PVNet
-Version: 0.0.8
-Summary: PVNet
-Author: Peter Dudfield
-Author-email: info@openclimatefix.org
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PVNet
 [![test-release](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml/badge.svg)](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml)
 
 ## Setup
 ```bash
 git clone https://github.com/openclimatefix/PVNet.git
 cd PVNet
@@ -25,7 +15,16 @@
 ```
 
 ## Development
 ```bash
 pip install -r requirements.txt -r requirements-dev.txt
 pytest
 ```
+
+Might need to install PVLive
+```
+pip install git+https://github.com/SheffieldSolar/PV_Live-API#pvlive_api
+```
+
+## Experiments
+
+Notes on these experiments are [here](https://docs.google.com/document/d/1fbkfkBzp16WbnCg7RDuRDvgzInA6XQu3xh4NCjV-WDA/edit?usp=sharing).
```

### Comparing `PVNet-0.0.8/PVNet.egg-info/PKG-INFO` & `PVNet-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.0.8
+Version: 0.0.9
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
+Provides-Extra: all_models
 License-File: LICENSE
 
 # PVNet
 [![test-release](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml/badge.svg)](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml)
 
 ## Setup
 ```bash
@@ -25,7 +26,16 @@
 ```
 
 ## Development
 ```bash
 pip install -r requirements.txt -r requirements-dev.txt
 pytest
 ```
+
+Might need to install PVLive
+```
+pip install git+https://github.com/SheffieldSolar/PV_Live-API#pvlive_api
+```
+
+## Experiments
+
+Notes on these experiments are [here](https://docs.google.com/document/d/1fbkfkBzp16WbnCg7RDuRDvgzInA6XQu3xh4NCjV-WDA/edit?usp=sharing).
```

### Comparing `PVNet-0.0.8/pvnet/training.py` & `PVNet-0.0.9/pvnet/training.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from typing import Optional
 
 import hydra
 import torch
-from omegaconf import DictConfig
-from pytorch_lightning import (
+from lightning.pytorch import (
     Callback,
     LightningDataModule,
     LightningModule,
     Trainer,
     seed_everything,
 )
-from pytorch_lightning.loggers import LightningLoggerBase
+from lightning.pytorch.loggers import Logger
+from omegaconf import DictConfig
 
 from pvnet import utils
 
 log = utils.get_logger(__name__)
 
 torch.set_default_dtype(torch.float32)
 
 
+def callbacks_to_phase(callbacks, phase):
+    for c in callbacks:
+        if hasattr(c, "switch_phase"):
+            c.switch_phase(phase)
+
+
 def train(config: DictConfig) -> Optional[float]:
     """Contains training pipeline.
     Instantiates all PyTorch Lightning objects from config.
 
     Args:
         config (DictConfig): Configuration composed by Hydra.
 
@@ -38,58 +44,61 @@
     log.info(f"Instantiating datamodule <{config.datamodule._target_}>")
     datamodule: LightningDataModule = hydra.utils.instantiate(config.datamodule)
 
     # Init lightning model
     log.info(f"Instantiating model <{config.model._target_}>")
     model: LightningModule = hydra.utils.instantiate(config.model)
 
+    # Init lightning loggers
+    logger: list[Logger] = []
+    if "logger" in config:
+        for _, lg_conf in config.logger.items():
+            if "_target_" in lg_conf:
+                log.info(f"Instantiating logger <{lg_conf._target_}>")
+                logger.append(hydra.utils.instantiate(lg_conf))
+
     # Init lightning callbacks
     callbacks: list[Callback] = []
     if "callbacks" in config:
         for _, cb_conf in config.callbacks.items():
             if "_target_" in cb_conf:
                 log.info(f"Instantiating callback <{cb_conf._target_}>")
                 callbacks.append(hydra.utils.instantiate(cb_conf))
 
-    # Init lightning loggers
-    logger: list[LightningLoggerBase] = []
-    if "logger" in config:
-        for _, lg_conf in config.logger.items():
-            if "_target_" in lg_conf:
-                log.info(f"Instantiating logger <{lg_conf._target_}>")
-                logger.append(hydra.utils.instantiate(lg_conf))
+    should_pretrain = False
+    for c in callbacks:
+        should_pretrain |= hasattr(c, "training_phase") and c.training_phase == "pretrain"
 
-    # Init lightning trainer
-    log.info(f"Instantiating trainer <{config.trainer._target_}>")
-    trainer: Trainer = hydra.utils.instantiate(
-        config.trainer, callbacks=callbacks, logger=logger, _convert_="partial"
-    )
+    if should_pretrain:
+        callbacks_to_phase(callbacks, "pretrain")
 
-    # Send some parameters from config to all lightning loggers
-    log.info("Logging hyperparameters!")
-    utils.log_hyperparameters(
-        config=config,
-        model=model,
-        datamodule=datamodule,
-        trainer=trainer,
-        callbacks=callbacks,
+    trainer: Trainer = hydra.utils.instantiate(
+        config.trainer,
         logger=logger,
+        _convert_="partial",
+        callbacks=callbacks,
     )
 
-    # Train the model
-    log.info("Starting training!")
-    if "validate_only" in config:
-        trainer.validate(model=model, datamodule=datamodule)
-    else:
+    if should_pretrain:
+        # Pre-train the model
+        datamodule.block_nwp_and_sat = True
         trainer.fit(model=model, datamodule=datamodule)
 
-    # Evaluate model on test set, using the best model achieved during training
-    if config.get("test_after_training") and not config.trainer.get("fast_dev_run"):
+    callbacks_to_phase(callbacks, "main")
+
+    datamodule.block_nwp_and_sat = False
+    trainer.should_stop = False
+
+    # Train the model completely
+    trainer.fit(model=model, datamodule=datamodule)
+
+    if config.test_after_training:
+        # Evaluate model on test set, using the best model achieved during training
         log.info("Starting testing!")
-        trainer.test()
+        trainer.test(model=model, datamodule=datamodule, ckpt_path="best")
 
     # Make sure everything closed properly
     log.info("Finalizing!")
     utils.finish(
         config=config,
         model=model,
         datamodule=datamodule,
```

### Comparing `PVNet-0.0.8/setup.py` & `PVNet-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
+extras_require = {"all_models": ["pytorch-tabnet", "efficientnet_pytorch"]}
 
 setup(
     name="PVNet",
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     description="PVNet",
     author="Peter Dudfield",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
+    extras_require=extras_require,
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     packages=find_packages(),
 )
```

