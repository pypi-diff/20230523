# Comparing `tmp/bitorch-0.3.0.dev1.tar.gz` & `tmp/bitorch-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitorch-0.3.0.dev1.tar", last modified: Thu Jul  7 14:58:40 2022, max compression
+gzip compressed data, was "bitorch-0.4.0.dev0.tar", last modified: Tue May 23 11:28:16 2023, max compression
```

## Comparing `bitorch-0.3.0.dev1.tar` & `bitorch-0.4.0.dev0.tar`

### file list

```diff
@@ -1,115 +1,158 @@
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.193680 bitorch-0.3.0.dev1/
--rw-r--r--   0 joseph     (501) staff       (20)      296 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/AUTHORS
--rw-r--r--   0 joseph     (501) staff       (20)     2642 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/CHANGELOG.md
--rw-r--r--   0 joseph     (501) staff       (20)    35149 2022-01-06 10:00:15.000000 bitorch-0.3.0.dev1/LICENSE
--rw-r--r--   0 joseph     (501) staff       (20)     4405 2022-07-07 14:58:40.193749 bitorch-0.3.0.dev1/PKG-INFO
--rw-r--r--   0 joseph     (501) staff       (20)     3639 2022-07-07 09:55:00.000000 bitorch-0.3.0.dev1/README.md
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.180913 bitorch-0.3.0.dev1/bitorch/
--rw-r--r--   0 joseph     (501) staff       (20)     2795 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     2838 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/bitorch/config.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.182631 bitorch-0.3.0.dev1/bitorch/datasets/
--rw-r--r--   0 joseph     (501) staff       (20)     1224 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/datasets/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     5937 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/datasets/base.py
--rw-r--r--   0 joseph     (501) staff       (20)     1732 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/datasets/cifar.py
--rw-r--r--   0 joseph     (501) staff       (20)      825 2022-05-19 13:28:26.000000 bitorch-0.3.0.dev1/bitorch/datasets/dummy_dataset.py
--rw-r--r--   0 joseph     (501) staff       (20)     1693 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/datasets/imagenet.py
--rw-r--r--   0 joseph     (501) staff       (20)      554 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/datasets/mnist.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.184301 bitorch-0.3.0.dev1/bitorch/layers/
--rw-r--r--   0 joseph     (501) staff       (20)     2017 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     1515 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/config.py
--rw-r--r--   0 joseph     (501) staff       (20)     7963 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/debug_layers.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.185233 bitorch-0.3.0.dev1/bitorch/layers/extensions/
--rw-r--r--   0 joseph     (501) staff       (20)      533 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/extensions/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     3430 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_container.py
--rw-r--r--   0 joseph     (501) staff       (20)     2874 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_implementation.py
--rw-r--r--   0 joseph     (501) staff       (20)     1298 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_recipe.py
--rw-r--r--   0 joseph     (501) staff       (20)     4649 2022-07-07 11:59:22.000000 bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_registration.py
--rw-r--r--   0 joseph     (501) staff       (20)     5068 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_registry.py
--rw-r--r--   0 joseph     (501) staff       (20)     2138 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/pact.py
--rw-r--r--   0 joseph     (501) staff       (20)     3064 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/qactivation.py
--rw-r--r--   0 joseph     (501) staff       (20)     4983 2022-07-07 14:47:04.000000 bitorch-0.3.0.dev1/bitorch/layers/qconv1d.py
--rw-r--r--   0 joseph     (501) staff       (20)     4839 2022-07-07 14:47:04.000000 bitorch-0.3.0.dev1/bitorch/layers/qconv2d.py
--rw-r--r--   0 joseph     (501) staff       (20)     4839 2022-07-07 14:47:04.000000 bitorch-0.3.0.dev1/bitorch/layers/qconv3d.py
--rw-r--r--   0 joseph     (501) staff       (20)     1265 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/qconv_mixin.py
--rw-r--r--   0 joseph     (501) staff       (20)     4616 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/qembedding.py
--rw-r--r--   0 joseph     (501) staff       (20)     3921 2022-07-07 14:47:04.000000 bitorch-0.3.0.dev1/bitorch/layers/qlinear.py
--rw-r--r--   0 joseph     (501) staff       (20)     2767 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/layers/register.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.186084 bitorch-0.3.0.dev1/bitorch/models/
--rw-r--r--   0 joseph     (501) staff       (20)     1506 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/models/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     2943 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/models/base.py
--rw-r--r--   0 joseph     (501) staff       (20)      841 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/models/common_layers.py
--rw-r--r--   0 joseph     (501) staff       (20)     3514 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/models/lenet.py
--rw-r--r--   0 joseph     (501) staff       (20)    22866 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/models/resnet.py
--rw-r--r--   0 joseph     (501) staff       (20)     9977 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/models/resnet_e.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.187684 bitorch-0.3.0.dev1/bitorch/quantizations/
--rw-r--r--   0 joseph     (501) staff       (20)     1586 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/bitorch/quantizations/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     2117 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/quantizations/approx_sign.py
--rw-r--r--   0 joseph     (501) staff       (20)     2225 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/bitorch/quantizations/base.py
--rw-r--r--   0 joseph     (501) staff       (20)      440 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/bitorch/quantizations/config.py
--rw-r--r--   0 joseph     (501) staff       (20)     3585 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/quantizations/dorefa.py
--rw-r--r--   0 joseph     (501) staff       (20)      525 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/quantizations/identity.py
--rw-r--r--   0 joseph     (501) staff       (20)     3824 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/bitorch/quantizations/progressive_sign.py
--rw-r--r--   0 joseph     (501) staff       (20)     1204 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/quantizations/sign.py
--rw-r--r--   0 joseph     (501) staff       (20)     1273 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/quantizations/ste_heaviside.py
--rw-r--r--   0 joseph     (501) staff       (20)     2728 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/quantizations/swish_sign.py
--rw-r--r--   0 joseph     (501) staff       (20)     4325 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/runtime_mode.py
--rw-r--r--   0 joseph     (501) staff       (20)     1607 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/bitorch/util.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.181514 bitorch-0.3.0.dev1/bitorch.egg-info/
--rw-r--r--   0 joseph     (501) staff       (20)     4405 2022-07-07 14:58:40.000000 bitorch-0.3.0.dev1/bitorch.egg-info/PKG-INFO
--rw-r--r--   0 joseph     (501) staff       (20)     2975 2022-07-07 14:58:40.000000 bitorch-0.3.0.dev1/bitorch.egg-info/SOURCES.txt
--rw-r--r--   0 joseph     (501) staff       (20)        1 2022-07-07 14:58:40.000000 bitorch-0.3.0.dev1/bitorch.egg-info/dependency_links.txt
--rw-r--r--   0 joseph     (501) staff       (20)      287 2022-07-07 14:58:40.000000 bitorch-0.3.0.dev1/bitorch.egg-info/requires.txt
--rw-r--r--   0 joseph     (501) staff       (20)       23 2022-07-07 14:58:40.000000 bitorch-0.3.0.dev1/bitorch.egg-info/top_level.txt
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.187866 bitorch-0.3.0.dev1/examples/
--rw-r--r--   0 joseph     (501) staff       (20)       50 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/__init__.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.188596 bitorch-0.3.0.dev1/examples/mnist/
--rw-r--r--   0 joseph     (501) staff       (20)      587 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/mnist/README.md
--rw-r--r--   0 joseph     (501) staff       (20)      163 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/mnist/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)       33 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/mnist/requirements.txt
--rw-r--r--   0 joseph     (501) staff       (20)     6706 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/mnist/train_mnist.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.189134 bitorch-0.3.0.dev1/examples/pytorch_lightning/
--rw-r--r--   0 joseph     (501) staff       (20)     2919 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/README.md
--rw-r--r--   0 joseph     (501) staff       (20)       78 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     7340 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/image_classification.py
--rw-r--r--   0 joseph     (501) staff       (20)       65 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/requirements.txt
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.190541 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/
--rw-r--r--   0 joseph     (501) staff       (20)       50 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     9501 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/arg_parser.py
--rw-r--r--   0 joseph     (501) staff       (20)      867 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/callbacks.py
--rw-r--r--   0 joseph     (501) staff       (20)     1461 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/kd_loss.py
--rw-r--r--   0 joseph     (501) staff       (20)     4539 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/lightning_model.py
--rw-r--r--   0 joseph     (501) staff       (20)     6656 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/log.py
--rw-r--r--   0 joseph     (501) staff       (20)     1147 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/teachers.py
--rw-r--r--   0 joseph     (501) staff       (20)     1955 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/unused_args.py
--rw-r--r--   0 joseph     (501) staff       (20)     3933 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/utils.py
--rw-r--r--   0 joseph     (501) staff       (20)     1193 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/wandb_logger.py
--rw-r--r--   0 joseph     (501) staff       (20)     1015 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/mypy.ini
--rw-r--r--   0 joseph     (501) staff       (20)      187 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/pyproject.toml
--rw-r--r--   0 joseph     (501) staff       (20)      165 2022-07-07 12:07:21.000000 bitorch-0.3.0.dev1/requirements-dev.txt
--rw-r--r--   0 joseph     (501) staff       (20)       51 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/requirements.txt
--rw-r--r--   0 joseph     (501) staff       (20)      575 2022-07-07 14:58:40.194058 bitorch-0.3.0.dev1/setup.cfg
--rw-r--r--   0 joseph     (501) staff       (20)     2497 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/setup.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.191329 bitorch-0.3.0.dev1/tests/
--rw-r--r--   0 joseph     (501) staff       (20)        0 2021-11-04 09:15:03.000000 bitorch-0.3.0.dev1/tests/__init__.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.192965 bitorch-0.3.0.dev1/tests/layers/
--rw-r--r--   0 joseph     (501) staff       (20)        0 2021-11-04 09:15:03.000000 bitorch-0.3.0.dev1/tests/layers/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     1610 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_layer_arg_retrieval.py
--rw-r--r--   0 joseph     (501) staff       (20)     4279 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/tests/layers/test_layer_implementation.py
--rw-r--r--   0 joseph     (501) staff       (20)      667 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_pact.py
--rw-r--r--   0 joseph     (501) staff       (20)     1117 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_qactivation.py
--rw-r--r--   0 joseph     (501) staff       (20)     3050 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_qconv.py
--rw-r--r--   0 joseph     (501) staff       (20)     2209 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_qconv_noact.py
--rw-r--r--   0 joseph     (501) staff       (20)     5559 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_qembeddings.py
--rw-r--r--   0 joseph     (501) staff       (20)     1160 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/layers/test_qlinear.py
--rw-r--r--   0 joseph     (501) staff       (20)     1451 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/tests/layers/test_switchable_layer.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.193318 bitorch-0.3.0.dev1/tests/models/
--rw-r--r--   0 joseph     (501) staff       (20)        0 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/models/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     5212 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/models/test_model_conversion.py
--rw-r--r--   0 joseph     (501) staff       (20)     2182 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/models/test_models.py
-drwxr-xr-x   0 joseph     (501) staff       (20)        0 2022-07-07 14:58:40.193540 bitorch-0.3.0.dev1/tests/quantizations/
--rw-r--r--   0 joseph     (501) staff       (20)        0 2021-11-04 09:15:03.000000 bitorch-0.3.0.dev1/tests/quantizations/__init__.py
--rw-r--r--   0 joseph     (501) staff       (20)     3879 2022-07-07 12:22:40.000000 bitorch-0.3.0.dev1/tests/quantizations/test_quantizations.py
--rw-r--r--   0 joseph     (501) staff       (20)      347 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/test_argparse.py
--rw-r--r--   0 joseph     (501) staff       (20)      909 2021-11-04 09:15:03.000000 bitorch-0.3.0.dev1/tests/test_configs.py
--rw-r--r--   0 joseph     (501) staff       (20)     2226 2022-07-01 14:01:55.000000 bitorch-0.3.0.dev1/tests/test_runtime_mode.py
--rw-r--r--   0 joseph     (501) staff       (20)       11 2022-07-07 14:56:52.000000 bitorch-0.3.0.dev1/version.txt
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.068859 bitorch-0.4.0.dev0/
+-rw-r--r--   0 joseph     (501) staff       (20)      296 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/AUTHORS
+-rw-r--r--   0 joseph     (501) staff       (20)     3429 2023-05-23 11:17:20.000000 bitorch-0.4.0.dev0/CHANGELOG.md
+-rw-r--r--   0 joseph     (501) staff       (20)    35149 2022-08-11 13:53:57.000000 bitorch-0.4.0.dev0/LICENSE
+-rw-r--r--   0 joseph     (501) staff       (20)     4506 2023-05-23 11:28:16.068930 bitorch-0.4.0.dev0/PKG-INFO
+-rw-r--r--   0 joseph     (501) staff       (20)     3639 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/README.md
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.040837 bitorch-0.4.0.dev0/bitorch/
+-rw-r--r--   0 joseph     (501) staff       (20)     3080 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/bitorch/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2838 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/config.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.044832 bitorch-0.4.0.dev0/bitorch/layers/
+-rw-r--r--   0 joseph     (501) staff       (20)     2081 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/bitorch/layers/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9754 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/layers/bembedding.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1522 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/config.py
+-rw-r--r--   0 joseph     (501) staff       (20)     8013 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/debug_layers.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.046203 bitorch-0.4.0.dev0/bitorch/layers/extensions/
+-rw-r--r--   0 joseph     (501) staff       (20)      533 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/extensions/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3430 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_container.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2914 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_implementation.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1298 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_recipe.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4669 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_registration.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5088 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_registry.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2158 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/pact.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1104 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/bitorch/layers/pad.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3074 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qactivation.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5033 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qconv1d.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4889 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qconv2d.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4889 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qconv3d.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1265 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qconv_mixin.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4661 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qembedding.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3951 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/qlinear.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2790 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/layers/register.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.049506 bitorch-0.4.0.dev0/bitorch/models/
+-rw-r--r--   0 joseph     (501) staff       (20)     2532 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/bitorch/models/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9284 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/base.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2667 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/common_layers.py
+-rw-r--r--   0 joseph     (501) staff       (20)    13528 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/densenet.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9780 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/models/dlrm.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4007 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/lenet.py
+-rw-r--r--   0 joseph     (501) staff       (20)     8918 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/meliusnet.py
+-rw-r--r--   0 joseph     (501) staff       (20)    18203 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/model_hub.py
+-rw-r--r--   0 joseph     (501) staff       (20)     7212 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/quicknet.py
+-rw-r--r--   0 joseph     (501) staff       (20)    22928 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/resnet.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9910 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/bitorch/models/resnet_e.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.055330 bitorch-0.4.0.dev0/bitorch/quantizations/
+-rw-r--r--   0 joseph     (501) staff       (20)     2174 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2117 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/approx_sign.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2225 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/base.py
+-rw-r--r--   0 joseph     (501) staff       (20)      287 2022-10-26 12:55:05.000000 bitorch-0.4.0.dev0/bitorch/quantizations/config.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4685 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/dorefa.py
+-rw-r--r--   0 joseph     (501) staff       (20)      525 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/identity.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5622 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/progressive_sign.py
+-rw-r--r--   0 joseph     (501) staff       (20)     8164 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/bitorch/quantizations/quantization_scheduler.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1206 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/sign.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1967 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/ste_heaviside.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2728 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/quantizations/swish_sign.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4325 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/bitorch/runtime_mode.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1600 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/bitorch/util.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.041530 bitorch-0.4.0.dev0/bitorch.egg-info/
+-rw-r--r--   0 joseph     (501) staff       (20)     4506 2023-05-23 11:28:16.000000 bitorch-0.4.0.dev0/bitorch.egg-info/PKG-INFO
+-rw-r--r--   0 joseph     (501) staff       (20)     4340 2023-05-23 11:28:16.000000 bitorch-0.4.0.dev0/bitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 joseph     (501) staff       (20)        1 2023-05-23 11:28:16.000000 bitorch-0.4.0.dev0/bitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 joseph     (501) staff       (20)      401 2023-05-23 11:28:16.000000 bitorch-0.4.0.dev0/bitorch.egg-info/requires.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       23 2023-05-23 11:28:16.000000 bitorch-0.4.0.dev0/bitorch.egg-info/top_level.txt
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.055547 bitorch-0.4.0.dev0/examples/
+-rw-r--r--   0 joseph     (501) staff       (20)       50 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/__init__.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.056456 bitorch-0.4.0.dev0/examples/dlrm/
+-rw-r--r--   0 joseph     (501) staff       (20)     3013 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/README.md
+-rw-r--r--   0 joseph     (501) staff       (20)       78 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/__init__.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.057179 bitorch-0.4.0.dev0/examples/dlrm/datasets/
+-rw-r--r--   0 joseph     (501) staff       (20)     1001 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/datasets/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5023 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/datasets/base.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3271 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/datasets/criteo.py
+-rw-r--r--   0 joseph     (501) staff       (20)      825 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/datasets/dummy_dataset.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.057694 bitorch-0.4.0.dev0/examples/dlrm/facebook_dataloading/
+-rw-r--r--   0 joseph     (501) staff       (20)      103 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/facebook_dataloading/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)    26434 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/facebook_dataloading/data_utils.py
+-rw-r--r--   0 joseph     (501) staff       (20)    15437 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/facebook_dataloading/dataloading_fb.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.036881 bitorch-0.4.0.dev0/examples/dlrm/logs/
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.036928 bitorch-0.4.0.dev0/examples/dlrm/logs/wandb/
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.036975 bitorch-0.4.0.dev0/examples/dlrm/logs/wandb/run-20230215_164956-1rvl0swm/
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.057850 bitorch-0.4.0.dev0/examples/dlrm/logs/wandb/run-20230215_164956-1rvl0swm/files/
+-rw-r--r--   0 joseph     (501) staff       (20)     3239 2023-02-15 15:49:57.000000 bitorch-0.4.0.dev0/examples/dlrm/logs/wandb/run-20230215_164956-1rvl0swm/files/requirements.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       63 2023-03-22 16:47:40.000000 bitorch-0.4.0.dev0/examples/dlrm/requirements.txt
+-rw-r--r--   0 joseph     (501) staff       (20)     7984 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/examples/dlrm/train_dlrm.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.059184 bitorch-0.4.0.dev0/examples/dlrm/utils/
+-rw-r--r--   0 joseph     (501) staff       (20)       50 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/utils/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9252 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/examples/dlrm/utils/arg_parser.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5359 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/utils/lightning_model.py
+-rw-r--r--   0 joseph     (501) staff       (20)     6656 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/utils/log.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1955 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/utils/unused_args.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3933 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/dlrm/utils/utils.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.059936 bitorch-0.4.0.dev0/examples/image_classification/
+-rw-r--r--   0 joseph     (501) staff       (20)     2956 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/examples/image_classification/README.md
+-rw-r--r--   0 joseph     (501) staff       (20)       78 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/__init__.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.060876 bitorch-0.4.0.dev0/examples/image_classification/datasets/
+-rw-r--r--   0 joseph     (501) staff       (20)     1215 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/datasets/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5023 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/datasets/base.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1667 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/datasets/cifar.py
+-rw-r--r--   0 joseph     (501) staff       (20)      825 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/datasets/dummy_dataset.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1628 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/datasets/imagenet.py
+-rw-r--r--   0 joseph     (501) staff       (20)      554 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/datasets/mnist.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9575 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/image_classification.py
+-rw-r--r--   0 joseph     (501) staff       (20)      102 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/requirements.txt
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.062927 bitorch-0.4.0.dev0/examples/image_classification/utils/
+-rw-r--r--   0 joseph     (501) staff       (20)       50 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)    13091 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/arg_parser.py
+-rw-r--r--   0 joseph     (501) staff       (20)      900 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/callbacks.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1461 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/kd_loss.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5765 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/lightning_model.py
+-rw-r--r--   0 joseph     (501) staff       (20)     6717 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/log.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1147 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/teachers.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1955 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/unused_args.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3898 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/utils.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1931 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/examples/image_classification/utils/wandb_logger.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.063613 bitorch-0.4.0.dev0/examples/mnist/
+-rw-r--r--   0 joseph     (501) staff       (20)      587 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/README.md
+-rw-r--r--   0 joseph     (501) staff       (20)      163 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/__init__.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.064281 bitorch-0.4.0.dev0/examples/mnist/datasets/
+-rw-r--r--   0 joseph     (501) staff       (20)     1042 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/datasets/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5033 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/datasets/base.py
+-rw-r--r--   0 joseph     (501) staff       (20)      825 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/datasets/dummy_dataset.py
+-rw-r--r--   0 joseph     (501) staff       (20)      554 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/datasets/mnist.py
+-rw-r--r--   0 joseph     (501) staff       (20)       23 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/requirements.txt
+-rw-r--r--   0 joseph     (501) staff       (20)     6666 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/examples/mnist/train_mnist.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1022 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/mypy.ini
+-rw-r--r--   0 joseph     (501) staff       (20)      187 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/pyproject.toml
+-rw-r--r--   0 joseph     (501) staff       (20)      213 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/requirements-dev.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       57 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/requirements.txt
+-rw-r--r--   0 joseph     (501) staff       (20)      575 2023-05-23 11:28:16.069326 bitorch-0.4.0.dev0/setup.cfg
+-rw-r--r--   0 joseph     (501) staff       (20)     2691 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/setup.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.065114 bitorch-0.4.0.dev0/tests/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2021-11-04 09:15:03.000000 bitorch-0.4.0.dev0/tests/__init__.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.067330 bitorch-0.4.0.dev0/tests/layers/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2021-11-04 09:15:03.000000 bitorch-0.4.0.dev0/tests/layers/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)    12859 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_bembedding.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1610 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_layer_arg_retrieval.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4336 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/tests/layers/test_layer_implementation.py
+-rw-r--r--   0 joseph     (501) staff       (20)      667 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_pact.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1117 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_qactivation.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3050 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_qconv.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2209 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_qconv_noact.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5558 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/tests/layers/test_qembeddings.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1160 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_qlinear.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1451 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/layers/test_switchable_layer.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.068360 bitorch-0.4.0.dev0/tests/models/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/models/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5198 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/models/test_model_conversion.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2045 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/tests/models/test_model_hub.py
+-rw-r--r--   0 joseph     (501) staff       (20)      468 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/models/test_model_names.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4195 2023-04-17 13:46:18.000000 bitorch-0.4.0.dev0/tests/models/test_models.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2023-05-23 11:28:16.068723 bitorch-0.4.0.dev0/tests/quantizations/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2021-11-04 09:15:03.000000 bitorch-0.4.0.dev0/tests/quantizations/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1326 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/quantizations/test_quantization_scheduler.py
+-rw-r--r--   0 joseph     (501) staff       (20)     3907 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/quantizations/test_quantizations.py
+-rw-r--r--   0 joseph     (501) staff       (20)      327 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/test_argparse.py
+-rw-r--r--   0 joseph     (501) staff       (20)      909 2022-08-11 13:53:57.000000 bitorch-0.4.0.dev0/tests/test_configs.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2226 2023-01-13 16:04:16.000000 bitorch-0.4.0.dev0/tests/test_runtime_mode.py
+-rw-r--r--   0 joseph     (501) staff       (20)       11 2023-05-23 11:17:11.000000 bitorch-0.4.0.dev0/version.txt
```

### Comparing `bitorch-0.3.0.dev1/CHANGELOG.md` & `bitorch-0.4.0.dev0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,58 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
-## [0.3.0] - Unreleased
+## [0.4.0] - Unreleased
 
 ### Added
 
+- ability to load models pretrained on ImageNet
+- Jupyter notebooks for demonstration purposes
+- support for PyTorch version 2.0, Python 3.10
+
+### Fixed
+
+- BEmbedding bag
+
+## [0.3.0] - 2023/01/13
+
+### Added
+
+- new models:
+  - [MeliusNet](bitorch/models/meliusnet.py)
+  - [BinaryDenseNet](bitorch/models/densenet.py)
+  - [QuickNet](bitorch/models/quicknet.py)
 - simple example script for MNIST
 - support for integration of bitorch's inference engine for the following layers
   - QLinear
   - QConv
-- New quantization function: [Progressive Sign](bitorch/quantizations/progressive_sign.py)
-- New features in PyTorch Lightning example:
-  - Training with Knowledge Distillation
-  - Improved Logging
-  - Callback to update Progressive Sign modules
+- a quantized DLRM version, derived from [this](https://github.com/facebookresearch/dlrm) implementation
+- example code for training the quantized DLRM model
+- new quantization function: [Progressive Sign](bitorch/quantizations/progressive_sign.py)
+- new features in PyTorch Lightning example:
+  - training with Knowledge Distillation
+  - improved logging
+  - callback to update Progressive Sign module
+- option to integrate custom models, datasets, quantization functions
+- a quantization scheduler which lets you change quantization methods during training
+- a padding layer
 
 ### Changed
 
 - requirements changed:
   - code now depends on torch 1.12.x and torchvision 0.13.x
   - requirements for examples are now stored at their respective folders
   - optional requirements now install everything needed to run all examples
 - code is now formatted with the black code formatter
 - using PyTorch's implementation of RAdam
 - renamed the `bitwidth` attribute of quantization functions to `bit_width`
+- moved the image datasets out of the bitorch core package into the image classification example
 
 ### Fixed
 
 - fix error from updated protobuf package
 
 ## [0.2.0] - 2022/05/19
```

### Comparing `bitorch-0.3.0.dev1/LICENSE` & `bitorch-0.4.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/PKG-INFO` & `bitorch-0.4.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: bitorch
-Version: 0.3.0.dev1
+Version: 0.4.0.dev0
 Summary: A package for building and training quantized and binary neural networks with Pytorch
 Home-page: https://github.com/hpi-xnor/bitorch
 Author: Hasso Plattner Institute
 Author-email: fb10-xnor@hpi.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: opt
 License-File: LICENSE
 
 # BITorch
```

### Comparing `bitorch-0.3.0.dev1/README.md` & `bitorch-0.4.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/__init__.py` & `bitorch-0.4.0.dev0/bitorch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 configs_by_name = {}
 
 current_dir = Path(__file__).resolve().parent
 files_to_iterate = list(current_dir.iterdir())
 # grep all python files recursively (bfs method)
 for file in files_to_iterate:
     if file.suffix == ".py" and file.stem != "__init__":
-
         rel_path = Path(os.path.relpath(file, current_dir))
         path_parts = list(rel_path.parent.parts) + [rel_path.stem]
         import_path = f"{__name__}.{'.'.join(path_parts)}"
         module = import_module(import_path)
 
         for attr_name in dir(module):
             attr = getattr(module, attr_name)
@@ -53,33 +52,42 @@
     """
     if name not in configs_by_name:
         raise ValueError(f"{name} config not found!")
     return configs_by_name[name]
 
 
 def config_names() -> List:
-    """getter for list of config names for argparse
+    """Get the list of config names for argparse.
 
     Returns:
         List: the config names
     """
     return list(configs_by_name.keys())
 
 
 def add_config_args(parser: ArgumentParser) -> None:
-    """adds all config arguments
+    """Adds all arguments from all registered configs.
 
     Args:
         parser (ArgumentParser): parser to add the arguments to
     """
     for config_ in configs_by_name.values():
         config_.add_config_arguments(parser)
 
 
 def apply_args_to_configuration(args: Namespace) -> None:
-    """applys the cli configurations to the config objects.
+    """Applies the cli configurations to the config objects.
 
     Args:
         args (Namespace): the cli configurations
     """
     for config_ in configs_by_name.values():
         config_.apply_args_to_configuration(args)
+
+
+def register_custom_config(custom_config: Config) -> None:
+    """Register a custom (external) config in bitorch.
+
+    Args:
+        custom_config: the custom config which should be added to bitorch
+    """
+    configs_by_name[custom_config.name] = custom_config
```

### Comparing `bitorch-0.3.0.dev1/bitorch/config.py` & `bitorch-0.4.0.dev0/bitorch/config.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/datasets/__init__.py` & `bitorch-0.4.0.dev0/examples/dlrm/datasets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,51 +2,41 @@
 This submodule contains data preparation code for some of the datasets used with our models,
 i.e. MNIST, CIFAR 10 and 100 and ImageNet.
 """
 
 from typing import List, Type
 
 from .base import BasicDataset
-from .cifar import CIFAR10, CIFAR100
-from .imagenet import ImageNet
-from .mnist import MNIST
-from ..util import build_lookup_dictionary
+from .criteo import Criteo
 
 __all__ = [
     "BasicDataset",
-    "dataset_from_name",
-    "dataset_names",
-    "MNIST",
-    "CIFAR10",
-    "CIFAR100",
-    "ImageNet",
+    "Criteo",
 ]
 
 
-datasets_by_name = build_lookup_dictionary(__name__, __all__, BasicDataset)
-
-
 def dataset_from_name(name: str) -> Type[BasicDataset]:
     """returns the dataset to which the name belongs to (name has to be the value of the datasets
     name-attribute)
 
     Args:
-        name: name of the dataset
+        name (str): name of the dataset
 
     Raises:
         ValueError: raised if no dataset under that name was found
 
     Returns:
         dataset: the dataset
     """
-    if name not in datasets_by_name:
-        raise ValueError(f"{name} dataset not found!")
-    return datasets_by_name[name]
+    for dataset_class in [Criteo]:
+        if dataset_class.name == name:
+            return dataset_class
+    raise Exception(f"unknown dataset: {name}")
 
 
 def dataset_names() -> List[str]:
     """getter for list of dataset names for argparse
 
     Returns:
         List: the dataset names
     """
-    return list(datasets_by_name.keys())
+    return [dataset_class.name for dataset_class in [Criteo]]
```

### Comparing `bitorch-0.3.0.dev1/bitorch/datasets/cifar.py` & `bitorch-0.4.0.dev0/examples/image_classification/datasets/cifar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from abc import ABC
 
 from torch.utils.data import Dataset
 from torchvision.datasets import cifar
 from torchvision.transforms import transforms
 
-from .base import BasicDataset, Augmentation
+from .base import BasicDataset
 
 __all__ = ["CIFAR10", "CIFAR100"]
 
 
 class CIFAR(BasicDataset, ABC):
     shape = (1, 3, 32, 32)
     num_train_samples = 50000
     num_val_samples = 10000
 
     @classmethod
-    def train_transform(cls, augmentation: Augmentation = Augmentation.DEFAULT) -> transforms.Compose:
+    def train_transform(cls) -> transforms.Compose:
         return transforms.Compose(
             [
                 transforms.RandomCrop(32, padding=4),
                 transforms.RandomHorizontalFlip(),
                 transforms.ToTensor(),
                 cls.get_normalize_transform(),
             ]
```

### Comparing `bitorch-0.3.0.dev1/bitorch/datasets/dummy_dataset.py` & `bitorch-0.4.0.dev0/examples/dlrm/datasets/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/datasets/imagenet.py` & `bitorch-0.4.0.dev0/examples/image_classification/datasets/imagenet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from torch.utils.data import Dataset
 from torchvision import transforms
 from torchvision.datasets import ImageFolder
 
-from .base import BasicDataset, Augmentation
+from .base import BasicDataset
 
 
 class ImageNet(BasicDataset):
     name = "imagenet"
     num_classes = 1000
     shape = (1, 3, 224, 224)
     mean = (0.485, 0.456, 0.406)
@@ -25,15 +25,15 @@
         directory = self.get_data_dir()
         print("got directory for imagenet:", directory)
         if download and not directory.is_dir():
             raise RuntimeError("ImageNet dataset must be downloaded and prepared manually.")
         return ImageFolder(directory, transform=self.get_transform())
 
     @classmethod
-    def train_transform(cls, augmentation: Augmentation = Augmentation.DEFAULT) -> transforms.Compose:
+    def train_transform(cls) -> transforms.Compose:
         crop_scale = 0.08
         return transforms.Compose(
             [
                 transforms.RandomResizedCrop(224, scale=(crop_scale, 1.0)),
                 transforms.RandomHorizontalFlip(),
                 transforms.ToTensor(),
                 cls.get_normalize_transform(),
```

### Comparing `bitorch-0.3.0.dev1/bitorch/datasets/mnist.py` & `bitorch-0.4.0.dev0/examples/image_classification/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/__init__.py` & `bitorch-0.4.0.dev0/bitorch/layers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This submodule contains adapted pytorch layers that use quantization functions on their weights
 and activations before forwarding them. These layers use the quantization functions specified in the
 quantization submodule.
 """
-from typing import TypeVar
+from typing import Optional, TypeVar
 
 import torch
 from torch import nn
 
 from bitorch import RuntimeMode
 from .debug_layers import InputGraphicalDebug, InputPrintDebug, WeightGraphicalDebug, WeightPrintDebug, ShapePrintDebug
 from .extensions import CustomImplementationMixin
@@ -15,14 +15,15 @@
 from .qactivation import QActivation
 from .qconv1d import QConv1d, QConv1dBase, QConv1d_NoAct
 from .qconv2d import QConv2d, QConv2dBase, QConv2d_NoAct
 from .qconv3d import QConv3d, QConv3dBase, QConv3d_NoAct
 from .qembedding import QEmbedding, QEmbeddingBag
 from .qlinear import QLinear, QLinearBase
 from .register import all_layer_registries
+from .pad import PadModule
 
 __all__ = [
     "InputGraphicalDebug",
     "InputPrintDebug",
     "WeightGraphicalDebug",
     "WeightPrintDebug",
     "ShapePrintDebug",
@@ -39,21 +40,22 @@
     "QLinear",
     "QLinearBase",
     "QEmbedding",
     "QEmbeddingBag",
     "Pact",
     "CustomImplementationMixin",
     "convert",
+    "PadModule",
 ]
 
 
 T = TypeVar("T", bound=nn.Module)
 
 
-def convert(module: T, new_mode: RuntimeMode, device: torch.device = None, verbose: bool = False) -> T:
+def convert(module: T, new_mode: RuntimeMode, device: Optional[torch.device] = None, verbose: bool = False) -> T:
     """
     Convert the given module to a new bitorch RuntimeMode. Needs to have custom implementations installed.
 
     Args:
         module: the module to be converted
         new_mode: the new mode for the module
         device: an optional device
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/config.py` & `bitorch-0.4.0.dev0/bitorch/layers/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class LayerConfig(Config):
     """Class to provide layer configurations."""
 
     name = "layer_config"
 
     def get_quantization_function(self, quantization: Union[str, Quantization]) -> Quantization:
-        """Returns the quantization module specified in quantization_name.
+        """Returns the quantization module specified by the given name or object.
 
         Args:
             quantization: quantization module or name of quantization function.
 
         Returns:
             the quantization module
         """
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/debug_layers.py` & `bitorch-0.4.0.dev0/bitorch/layers/debug_layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Optional, Any
 import torch
 from .config import config
 
 
 class _Debug(torch.nn.Module):
     def __init__(self, debug_interval: int = 100, num_outputs: int = 10, name: str = "Debug") -> None:
         """inits values.
@@ -45,16 +45,16 @@
             self.name, ":", debug_tensor if len(debug_tensor) < self._num_outputs else debug_tensor[: self._num_outputs]
         )
 
 
 class _GraphicalDebug(_Debug):
     def __init__(
         self,
-        figure: object = None,
-        images: list = None,
+        figure: Optional[object] = None,
+        images: Optional[list] = None,
         debug_interval: int = 100,
         num_outputs: int = 10,
     ) -> None:
         """Debugs the given layer by drawing weights/inputs in given matplotlib plot images.
 
         Args:
             figure (object): figure to draw in
@@ -65,23 +65,23 @@
         Raises:
             ValueError: raised if number of images does not match desired number of outputs.
         """
         super(_GraphicalDebug, self).__init__(debug_interval, num_outputs)
         self.set_figure(figure)
         self.set_images(images)
 
-    def set_figure(self, figure: object = None) -> None:
+    def set_figure(self, figure: Optional[object] = None) -> None:
         """setter for figure object
 
         Args:
             figure (object): the figure object
         """
         self._figure = figure
 
-    def set_images(self, images: list = None) -> None:
+    def set_images(self, images: Optional[list] = None) -> None:
         """setter for images list
 
         Args:
             images (list): list of image objects to output the graphical information to
 
         Raises:
             ValueError: raised if number of images does not match desired number of outputs.
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/extensions/__init__.py` & `bitorch-0.4.0.dev0/bitorch/layers/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_container.py` & `bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_container.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_implementation.py` & `bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_implementation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import Any, Tuple, TYPE_CHECKING
+from typing import Optional, Any, Tuple, TYPE_CHECKING
 
 import torch
 
 if TYPE_CHECKING:
     from . import LayerRecipe
 
 
@@ -31,15 +31,15 @@
 
         Returns:
             Whether the layer can be cloned or not and an info message if it can not be cloned
         """
         raise NotImplementedError("A custom layer should implement their own compatibility check.")
 
     @classmethod
-    def create_clone_from(cls, recipe: "LayerRecipe", device: torch.device = None) -> Any:
+    def create_clone_from(cls, recipe: "LayerRecipe", device: Optional[torch.device] = None) -> Any:
         """
         Create a new layer based on a given layer recipe (can be expected to be from the default category).
 
         Args:
             recipe: the layer which should be cloned
             device: the device on which the layer is going to be run
 
@@ -57,15 +57,15 @@
         return True
 
     @classmethod
     def can_clone(cls, recipe: "LayerRecipe") -> Tuple[bool, str]:
         return True, ""
 
     @classmethod
-    def create_clone_from(cls, recipe: "LayerRecipe", device: torch.device = None) -> Any:
+    def create_clone_from(cls, recipe: "LayerRecipe", device: Optional[torch.device] = None) -> Any:
         return cls(*recipe.args, **recipe.kwargs)
 
 
 class CustomImplementationMixin(BaseImplementation, ABC):
     """Defines the class interface of a custom layer implementation of a certain layer type."""
 
     @classmethod
@@ -73,9 +73,9 @@
         return False
 
     @classmethod
     def can_clone(cls, recipe: "LayerRecipe") -> Tuple[bool, str]:
         raise NotImplementedError("A custom layer should implement their own compatibility check.")
 
     @classmethod
-    def create_clone_from(cls, recipe: "LayerRecipe", device: torch.device = None) -> Any:
+    def create_clone_from(cls, recipe: "LayerRecipe", device: Optional[torch.device] = None) -> Any:
         raise NotImplementedError("A custom layer should implement a method to create a cloned layer.")
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_recipe.py` & `bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_recipe.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_registration.py` & `bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import Any, Type, Union, Tuple, TYPE_CHECKING
+from typing import Optional, Any, Type, Union, Tuple, TYPE_CHECKING
 
 import torch
 
 import bitorch
 from bitorch import runtime_mode_type, RuntimeMode
 from .layer_container import LayerContainer
 from .layer_implementation import DefaultImplementationMixin, BaseImplementation, CustomImplementationMixin
@@ -96,12 +96,12 @@
             True if the given mode is supported, False otherwise
         """
         return mode.is_supported_by(self._supported_modes)
 
     def can_create_clone_from(self, recipe: LayerRecipe) -> Tuple[bool, str]:
         return self.class_.can_clone(recipe)
 
-    def get_replacement(self, recipe: LayerRecipe, device: torch.device = None) -> Any:
+    def get_replacement(self, recipe: LayerRecipe, device: Optional[torch.device] = None) -> Any:
         return self.class_.create_clone_from(recipe, device)
 
     def is_default(self) -> bool:
         return self.class_.is_default_implementation()
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/extensions/layer_registry.py` & `bitorch-0.4.0.dev0/bitorch/layers/extensions/layer_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return set(x.layer for x in self._instance_recipes)
 
     def get_recipe_for(self, layer: Any) -> Optional["LayerRecipe"]:
         if layer not in map(lambda x: x.layer, self._instance_recipes):
             return None
         return next(filter(lambda x: x.layer == layer, self._instance_recipes))
 
-    def get_replacement(self, mode: RuntimeMode, recipe: LayerRecipe, device: torch.device = None) -> Any:
+    def get_replacement(self, mode: RuntimeMode, recipe: LayerRecipe, device: Optional[torch.device] = None) -> Any:
         layer = self.get_layer(mode, recipe)
         return layer.get_replacement(recipe, device)
 
     def add_recipe(self, new_recipe: LayerRecipe) -> None:
         if self.is_replacing:
             return
         self._instance_recipes.add(new_recipe)
@@ -106,15 +106,15 @@
         for i in to_remove:
             self.layer_implementations.remove(i)
 
     def convert_layers_to(
         self,
         new_mode: RuntimeMode,
         only: Optional[Iterable[Any]] = None,
-        device: torch.device = None,
+        device: Optional[torch.device] = None,
         verbose: bool = False,
     ) -> None:
         for recipe in list(self._instance_recipes):
             module = recipe.layer
             if only is not None and module.layer_implementation not in only and module not in only:
                 continue
             assert isinstance(module, LayerContainer)
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/pact.py` & `bitorch-0.4.0.dev0/bitorch/layers/pact.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Optional, Tuple
 from torch.autograd import Function
 from torch.nn import Module
 import torch
 
 from .config import config
 
 
@@ -38,14 +38,14 @@
 
 class Pact(Module):
     """Pact activation function taken from https://github.com/KwangHoonAn/PACT.
     Initially proposed in
     Choi, Jungwook, et al. "Pact: Parameterized clipping activation for quantized neural networks." (2018)
     """
 
-    def __init__(self, bits: int = None) -> None:
+    def __init__(self, bits: Optional[int] = None) -> None:
         super().__init__()
         self.alpha = torch.nn.parameter.Parameter(torch.tensor(10.0))
         self.bits = bits or config.pact_bits
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         return PactActFn.apply(x, self.alpha, self.bits)
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qactivation.py` & `bitorch-0.4.0.dev0/bitorch/layers/qactivation.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 class QActivation(nn.Module):
     """Activation layer for quantization"""
 
     def __init__(
         self,
-        activation: Union[str, Quantization] = None,
+        activation: Optional[Union[str, Quantization]] = None,
         gradient_cancellation_threshold: Optional[float] = 0.0,
     ) -> None:
         """initialization function for fetching suitable activation function.
 
         Args:
             activation (Union[str, Quantization], optional): quantization module or name of quantization function.
                 Defaults to None.
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qconv1d.py` & `bitorch-0.4.0.dev0/bitorch/layers/qconv1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module containing the quantized 1d convolution layer"""
 
-from typing import Any, Type, Union
+from typing import Optional, Any, Type, Union
 
 from torch import Tensor
 from torch.nn import Conv1d, init
 from torch.nn.functional import pad, conv1d
 
 from bitorch import RuntimeMode
 from bitorch.quantizations import Quantization
@@ -20,16 +20,16 @@
     Quantized 1d Convolutional Layer. Has the same api as Conv1d but lets you specify a weight quantization, that is
     applied before the convolutional operation.
     """
 
     def __init__(
         self,
         *args: Any,
-        weight_quantization: Union[str, Quantization] = None,
-        pad_value: float = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
+        pad_value: Optional[float] = None,
         bias: bool = False,
         **kwargs: Any,
     ) -> None:
         """
         initialization function for padding and quantization.
 
         Args:
@@ -78,16 +78,16 @@
         )
 
 
 class QConv1dBase(QConvArgsProviderMixin, QConv1d_NoAct):  # type: ignore
     def __init__(
         self,  # type: ignore
         *args: Any,
-        input_quantization: Union[str, Quantization] = None,
-        weight_quantization: Union[str, Quantization] = None,
+        input_quantization: Optional[Union[str, Quantization]] = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
         gradient_cancellation_threshold: Union[float, None] = None,
         **kwargs: Any,
     ) -> None:
         """initialization function for quantization of inputs and weights.
 
         Args:
             input_quantization (Union[str, Quantization], optional): quantization module or name of quantization
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qconv2d.py` & `bitorch-0.4.0.dev0/bitorch/layers/qconv2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module containing the quantized 2d convolution layer"""
 
-from typing import Any, Type, Union
+from typing import Optional, Any, Type, Union
 
 from torch import Tensor
 from torch.nn import Conv2d, init
 from torch.nn.functional import pad, conv2d
 
 from bitorch import RuntimeMode
 from bitorch.quantizations import Quantization
@@ -15,16 +15,16 @@
 from .register import QConv2dImplementation
 
 
 class QConv2d_NoAct(Conv2d):  # type: ignore # noqa: N801
     def __init__(
         self,  # type: ignore
         *args: Any,
-        weight_quantization: Union[str, Quantization] = None,
-        pad_value: float = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
+        pad_value: Optional[float] = None,
         bias: bool = False,
         **kwargs: Any,
     ) -> None:
         """initialization function for padding and quantization.
 
         Args:
             weight_quantization (Union[str, Quantization], optional): quantization module or name of quantization
@@ -72,16 +72,16 @@
         )
 
 
 class QConv2dBase(QConvArgsProviderMixin, QConv2d_NoAct):  # type: ignore
     def __init__(
         self,  # type: ignore
         *args: Any,
-        input_quantization: Union[str, Quantization] = None,
-        weight_quantization: Union[str, Quantization] = None,
+        input_quantization: Optional[Union[str, Quantization]] = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
         gradient_cancellation_threshold: Union[float, None] = None,
         **kwargs: Any,
     ) -> None:
         """initialization function for quantization of inputs and weights.
 
         Args:
             input_quantization (Union[str, Quantization], optional): quantization module or name of quantization
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qconv3d.py` & `bitorch-0.4.0.dev0/bitorch/layers/qconv3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module containing the quantized 3d convolution layer"""
 
-from typing import Any, Type, Union
+from typing import Optional, Any, Type, Union
 
 from torch import Tensor
 from torch.nn import Conv3d, init
 from torch.nn.functional import pad, conv3d
 
 from bitorch import RuntimeMode
 from bitorch.quantizations import Quantization
@@ -15,16 +15,16 @@
 from .register import QConv3dImplementation
 
 
 class QConv3d_NoAct(Conv3d):  # type: ignore # noqa: N801
     def __init__(
         self,  # type: ignore
         *args: Any,
-        weight_quantization: Union[str, Quantization] = None,
-        pad_value: float = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
+        pad_value: Optional[float] = None,
         bias: bool = False,
         **kwargs: Any,
     ) -> None:
         """initialization function for padding and quantization.
 
         Args:
             weight_quantization (Union[str, Quantization], optional): quantization module or name of quantization
@@ -72,16 +72,16 @@
         )
 
 
 class QConv3dBase(QConvArgsProviderMixin, QConv3d_NoAct):  # type: ignore
     def __init__(
         self,  # type: ignore
         *args: Any,
-        input_quantization: Union[str, Quantization] = None,
-        weight_quantization: Union[str, Quantization] = None,
+        input_quantization: Optional[Union[str, Quantization]] = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
         gradient_cancellation_threshold: Union[float, None] = None,
         **kwargs: Any,
     ) -> None:
         """initialization function for quantization of inputs and weights.
 
         Args:
             input_quantization (Union[str, Quantization], optional): quantization module or name of quantization
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qconv_mixin.py` & `bitorch-0.4.0.dev0/bitorch/layers/qconv_mixin.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qembedding.py` & `bitorch-0.4.0.dev0/bitorch/layers/qembedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Optional
+from typing import Any, Union, Optional
 from torch import Tensor
 from torch.nn import EmbeddingBag, Embedding
 from torch.nn.functional import embedding_bag, embedding
 
 
 from bitorch.layers.config import config
 from bitorch.quantizations import Quantization
@@ -11,19 +11,19 @@
 class QEmbeddingBag(EmbeddingBag):
     """Quantized version of pytorchs embedding bag. With the input indices the embedding is computed with a quantized
     version of the layers weight table. The output embedding will be also quantized before return.
     """
 
     def __init__(
         self,
-        *args: int,
+        *args: Any,
         embedding_dim: int,
-        weight_quantization: Union[Quantization, str] = None,
-        output_quantization: Union[Quantization, str] = None,
-        **kwargs: int,
+        weight_quantization: Optional[Union[Quantization, str]] = None,
+        output_quantization: Optional[Union[Quantization, str]] = None,
+        **kwargs: Any,
     ) -> None:
         super(QEmbeddingBag, self).__init__(*args, embedding_dim=embedding_dim, **kwargs)  # type: ignore
         """load quantization functions"""
         self.embedding_weight_quantization = config.get_quantization_function(
             weight_quantization or config.weight_quantization
         )
         self.embedding_input_quantization = config.get_quantization_function(
@@ -82,19 +82,19 @@
 class QEmbedding(Embedding):
     """Quantized version of pytorchs embedding layer. With input indices the embedding is computed with a quantized
     version of the layers weight table. The output embedding will be also quantized before return.
     """
 
     def __init__(
         self,
-        *args: int,
+        *args: Any,
         embedding_dim: int,
-        weight_quantization: Union[Quantization, str] = None,
-        output_quantization: Union[Quantization, str] = None,
-        **kwargs: int,
+        weight_quantization: Optional[Union[Quantization, str]] = None,
+        output_quantization: Optional[Union[Quantization, str]] = None,
+        **kwargs: Any,
     ) -> None:
         super(QEmbedding, self).__init__(*args, embedding_dim=embedding_dim, **kwargs)  # type: ignore
         """load quantization functions"""
         self.embedding_weight_quantization = config.get_quantization_function(
             weight_quantization or config.weight_quantization
         )
         self.embedding_output_quantization = config.get_quantization_function(
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/qlinear.py` & `bitorch-0.4.0.dev0/bitorch/layers/qlinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module containing the quantized linear layer"""
 
-from typing import Any, Type, Union, Dict
+from typing import Optional, Any, Type, Union, Dict
 
 import torch
 from torch.nn import Linear
 from torch.nn.functional import linear
 
 from bitorch import RuntimeMode
 from bitorch.quantizations import Quantization
@@ -14,17 +14,17 @@
 from .register import QLinearImplementation
 
 
 class QLinearBase(Linear):
     def __init__(
         self,
         *args: int,
-        input_quantization: Union[str, Quantization] = None,
+        input_quantization: Optional[Union[str, Quantization]] = None,
         gradient_cancellation_threshold: Union[float, None] = None,
-        weight_quantization: Union[str, Quantization] = None,
+        weight_quantization: Optional[Union[str, Quantization]] = None,
         **kwargs: bool,
     ) -> None:
         """Applies the given quantization functions on weights and inputs before applying the linear operation.
 
         Args:
             *args: positional arguments for linear layer
             input_quantization (Union[str, Quantization], optional): quantization module used for input
```

### Comparing `bitorch-0.3.0.dev1/bitorch/layers/register.py` & `bitorch-0.4.0.dev0/bitorch/layers/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         q_conv2d_registry,
         q_conv3d_registry,
         q_linear_registry,
     ]
 
 
 def convert_layers_to(
-    new_mode: RuntimeMode, only: Optional[Iterable[Any]] = None, device: torch.device = None, verbose: bool = False
+    new_mode: RuntimeMode,
+    only: Optional[Iterable[Any]] = None,
+    device: Optional[torch.device] = None,
+    verbose: bool = False,
 ) -> None:
     """
     Convert all wrapped layers (or a given subset of them) to a new mode.
     Args:
         new_mode: the new RuntimeMode
         only: optional white"list" (Iterable) of layers or wrapped layers which should be converted
         device: the new device for the layers
```

### Comparing `bitorch-0.3.0.dev1/bitorch/models/lenet.py` & `bitorch-0.4.0.dev0/bitorch/models/lenet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import argparse
+from typing import Optional, List
 from bitorch.layers.debug_layers import ShapePrintDebug
-from bitorch.datasets.base import BasicDataset
 from bitorch.layers import QLinear, QConv2d, QActivation
 from torch import nn
 from .base import Model
 
 
 class LeNet(Model):
     """LeNet model, both in quantized and full precision version"""
 
     num_channels_conv = 64
     activation_function = nn.Tanh
     num_fc = 1000
-    name = "lenet"
+    name = "LeNet"
 
     def generate_quant_model(
         self,
         weight_quant: str,
         input_quant: str,
-        weight_quant_2: str = None,
-        input_quant_2: str = None,
+        weight_quant_2: Optional[str] = None,
+        input_quant_2: Optional[str] = None,
     ) -> nn.Sequential:
         weight_quant_2 = weight_quant_2 or weight_quant
         input_quant_2 = input_quant_2 or input_quant
 
         model = nn.Sequential(
             nn.Conv2d(self.input_channels, self.num_channels_conv, kernel_size=5),
             self.activation_function(),
@@ -37,30 +37,40 @@
                 weight_quantization=weight_quant,
             ),
             nn.BatchNorm2d(self.num_channels_conv),
             nn.MaxPool2d(2, 2),
             ShapePrintDebug(),
             nn.Flatten(),
             QActivation(activation=input_quant_2),
-            QLinear(self.num_channels_conv * 4 * 4, self.num_fc, weight_quantization=weight_quant_2),
+            QLinear(
+                self.num_channels_conv * 4 * 4,
+                self.num_fc,
+                weight_quantization=weight_quant_2,
+            ),
             nn.BatchNorm1d(self.num_fc),
             self.activation_function(),
             nn.Linear(self.num_fc, self.num_output),
         )
         return model
 
-    def __init__(self, dataset: BasicDataset, lenet_version: int = 0) -> None:
-        """builds the model, depending on mode in either quantized or full_precision mode
+    def __init__(self, input_shape: List[int], num_classes: int = 0, lenet_version: int = 0) -> None:
+        """builds the model depending on mode in either quantized or full_precision mode
 
         Args:
-            lenet_quantized (bool, optional): toggles use of quantized version of lenet. Default is False.
+            input_shape (List[int]): input shape of images
+            num_classes (int, optional): number of output classes. Defaults to None.
+            lenet_version (int, optional): lenet version. if version outside of [0, 3], the full precision version is used. Defaults to 0.
+
+        Raises:
+            ValueError: thrown if num classes is none
         """
-        super(LeNet, self).__init__(dataset)
-        self.input_channels = dataset.shape[1]
-        self.num_output = dataset.num_classes
+        super(LeNet, self).__init__(input_shape, num_classes)
+        self.input_channels = self._input_shape[1]
+        self.num_output = self._num_classes
+
         if lenet_version == 0:
             self._model = self.generate_quant_model("sign", "sign")
         elif lenet_version == 1:
             self._model = self.generate_quant_model("weightdorefa", "weightdorefa")
         elif lenet_version == 2:
             self._model = self.generate_quant_model("sign", "weightdorefa", weight_quant_2="sign")
         elif lenet_version == 3:
@@ -78,10 +88,14 @@
                 nn.Flatten(),
                 nn.Linear(self.num_channels_conv * 4 * 4, self.num_fc),
                 nn.BatchNorm1d(self.num_fc),
                 self.activation_function(),
                 nn.Linear(self.num_fc, self.num_output),
             )
 
+    @classmethod
+    def _load_default_model(cls) -> Model:
+        return cls.from_pretrained(input_shape=(1, 1, 28, 28), num_classes=10)
+
     @staticmethod
     def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        parser.add_argument("--lenet-version", type=int, default=0, help="choose a version of lenet")
+        parser.add_argument("--version", type=int, default=0, help="choose a version of lenet")
```

### Comparing `bitorch-0.3.0.dev1/bitorch/models/resnet.py` & `bitorch-0.4.0.dev0/bitorch/models/resnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from bitorch.datasets.base import BasicDataset
-from .base import Model
-from typing import List, Any
+from .base import Model, NoArgparseArgsMixin
+from typing import Optional, List, Any
 from bitorch.layers import QConv2d_NoAct
 import torch
 import argparse
 import logging
 from torch import nn
 from torch.nn import Module
 
 from bitorch.layers import QConv2d
-from bitorch.models.common_layers import get_initial_layers
+from bitorch.models.common_layers import get_initial_layers, IMAGENET_INPUT_SHAPE, IMAGENET_CLASSES
 
 
 class BasicBlockV1(Module):
     """BasicBlock V1 from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     This is used for ResNet V1 for 18, 34 layers.
     """
@@ -40,27 +39,39 @@
     def _build_downsampling(self) -> nn.Sequential:
         """builds the downsampling layers for rediual tensor processing
 
         Returns:
             nn.Sequential: the downsampling model
         """
         return nn.Sequential(
-            QConv2d(self.in_channels, self.out_channels, kernel_size=1, stride=self.stride, padding=0),
+            QConv2d(
+                self.in_channels,
+                self.out_channels,
+                kernel_size=1,
+                stride=self.stride,
+                padding=0,
+            ),
             nn.BatchNorm2d(self.out_channels),
         )
 
     def _build_body(self) -> nn.Sequential:
         """builds body of building block, i.e. two binary convolutions with batchnorms in between. Check referenced paper for
         more details.
 
         Returns:
             nn.Sequential: the basic building block body model
         """
         return nn.Sequential(
-            QConv2d(self.in_channels, self.out_channels, kernel_size=3, stride=self.stride, padding=1),
+            QConv2d(
+                self.in_channels,
+                self.out_channels,
+                kernel_size=3,
+                stride=self.stride,
+                padding=1,
+            ),
             nn.BatchNorm2d(self.out_channels),
             QConv2d(self.out_channels, self.out_channels, kernel_size=3, stride=1, padding=1),
             nn.BatchNorm2d(self.out_channels),
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """forwards the input tensor x through the building block.
@@ -108,30 +119,46 @@
         """builds the downsampling layers for rediual tensor processing
 
         Returns:
             nn.Sequential: the downsampling model
         """
         return nn.Sequential(
             QConv2d_NoAct(
-                self.in_channels, self.out_channels, kernel_size=1, stride=self.stride, padding=0, bias=False
+                self.in_channels,
+                self.out_channels,
+                kernel_size=1,
+                stride=self.stride,
+                padding=0,
+                bias=False,
             ),
             nn.BatchNorm2d(self.out_channels),
         )
 
     def _build_body(self) -> nn.Sequential:
         """builds body of building block. Check referenced paper for more details.
 
         Returns:
             nn.Sequential: the bottleneck body model
         """
         return nn.Sequential(
-            QConv2d_NoAct(self.in_channels, self.out_channels // 4, kernel_size=1, stride=self.stride),
+            QConv2d_NoAct(
+                self.in_channels,
+                self.out_channels // 4,
+                kernel_size=1,
+                stride=self.stride,
+            ),
             nn.BatchNorm2d(self.out_channels // 4),
             nn.ReLU(),
-            QConv2d_NoAct(self.out_channels // 4, self.out_channels // 4, kernel_size=3, stride=1, padding=1),
+            QConv2d_NoAct(
+                self.out_channels // 4,
+                self.out_channels // 4,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+            ),
             nn.BatchNorm2d(self.out_channels // 4),
             nn.ReLU(),
             QConv2d_NoAct(self.out_channels // 4, self.out_channels, kernel_size=1, stride=1),
             nn.BatchNorm2d(self.out_channels),
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
@@ -179,24 +206,36 @@
 
     def _build_downsampling(self) -> nn.Module:
         """builds the downsampling layers for rediual tensor processing
 
         Returns:
             QConv2d: the downsampling convolution layer
         """
-        return QConv2d(self.in_channels, self.out_channels, kernel_size=1, stride=self.stride, padding=0)
+        return QConv2d(
+            self.in_channels,
+            self.out_channels,
+            kernel_size=1,
+            stride=self.stride,
+            padding=0,
+        )
 
     def _build_body(self) -> nn.Sequential:
         """builds body of building block. Check referenced paper for more details.
 
         Returns:
             nn.Sequential: the bottleneck body model
         """
         return nn.Sequential(
-            QConv2d(self.in_channels, self.out_channels, kernel_size=3, stride=self.stride, padding=1),
+            QConv2d(
+                self.in_channels,
+                self.out_channels,
+                kernel_size=3,
+                stride=self.stride,
+                padding=1,
+            ),
             nn.BatchNorm2d(self.out_channels),
             QConv2d(self.out_channels, self.out_channels, kernel_size=3, stride=1, padding=1),
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """forwards the input tensor x through the building block.
 
@@ -238,27 +277,44 @@
 
     def _build_downsampling(self) -> nn.Module:
         """builds the downsampling layers for rediual tensor processing
 
         Returns:
             QConv2d: the downsampling convolution layer
         """
-        return QConv2d_NoAct(self.in_channels, self.out_channels, kernel_size=1, stride=self.stride, bias=False)
+        return QConv2d_NoAct(
+            self.in_channels,
+            self.out_channels,
+            kernel_size=1,
+            stride=self.stride,
+            bias=False,
+        )
 
     def _build_body(self) -> nn.Sequential:
         """builds body of building block. Check referenced paper for more details.
 
         Returns:
             nn.Sequential: the bottleneck body model
         """
         return nn.Sequential(
-            QConv2d_NoAct(self.in_channels, self.out_channels // 4, kernel_size=1, stride=self.stride),
+            QConv2d_NoAct(
+                self.in_channels,
+                self.out_channels // 4,
+                kernel_size=1,
+                stride=self.stride,
+            ),
             nn.BatchNorm2d(self.out_channels // 4),
             nn.ReLU(),
-            QConv2d_NoAct(self.out_channels // 4, self.out_channels // 4, kernel_size=3, stride=1, padding=1),
+            QConv2d_NoAct(
+                self.out_channels // 4,
+                self.out_channels // 4,
+                kernel_size=3,
+                stride=1,
+                padding=1,
+            ),
             nn.BatchNorm2d(self.out_channels // 4),
             nn.ReLU(),
             QConv2d_NoAct(self.out_channels // 4, self.out_channels, kernel_size=1, stride=1),
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """forwards the input tensor x through the building block.
@@ -288,15 +344,22 @@
             classes (int): number of output classes
             channels (list): the channels used in the net
         """
         super(SpecificResnet, self).__init__()
         self.features = nn.Sequential()
         self.output_layer = nn.Linear(channels[-1], classes)
 
-    def make_layer(self, block: Module, layers: int, in_channels: int, out_channels: int, stride: int) -> nn.Sequential:
+    def make_layer(
+        self,
+        block: Module,
+        layers: int,
+        in_channels: int,
+        out_channels: int,
+        stride: int,
+    ) -> nn.Sequential:
         """builds a layer by stacking blocks in a sequential models.
 
         Args:
             block (Module): the block of which the layer shall consist
             layers (int): the number of blocks to stack
             in_channels (int): the input channels of this layer
             out_channels (int): the output channels of this layer
@@ -350,41 +413,41 @@
 
     def __init__(
         self,
         block: Module,
         layers: list,
         channels: list,
         classes: int,
-        initial_layers: str = "imagenet",
+        image_resolution: Optional[List[int]] = None,
         image_channels: int = 3,
     ) -> None:
         """Creates ResNetV1 model.
 
         Args:
             block (Module): Block to be used for building the layers.
             layers (list): layer sizes
             channels (list): channel num used for input/output channel size of layers. there must always be one more
                 channels than there are layers.
             classes (int): number of output classes
-            initial_layers (str, optional): name of set for initial layers. refer to common_layers.py.
-                Defaults to "imagenet".
+            image_resolution (List[int], optional): resolution of input image. refer to common_layers.py.
+                Defaults to None.
             image_channels (int, optional): input channels of images. Defaults to 3.
 
         Raises:
             ValueError: raised if the number of channels does not match number of layer + 1
         """
         super(ResNetV1, self).__init__(classes, channels)
         if len(channels) != (len(layers) + 1):
             raise ValueError(
                 f"the len of channels ({len(channels)}) must be exactly the len of layers ({len(layers)}) + 1!"
             )
 
         feature_layers: List[nn.Module] = []
         feature_layers.append(nn.BatchNorm2d(image_channels))
-        feature_layers.extend(get_initial_layers(initial_layers, image_channels, channels[0]))
+        feature_layers.extend(get_initial_layers(image_resolution, image_channels, channels[0]))
         feature_layers.append(nn.BatchNorm2d(channels[0]))
 
         feature_layers.extend(self.make_feature_layers(block, layers, channels))
 
         feature_layers.append(nn.ReLU())
         feature_layers.append(nn.AdaptiveAvgPool2d(1))
         feature_layers.append(nn.Flatten())
@@ -400,41 +463,41 @@
 
     def __init__(
         self,
         block: Module,
         layers: list,
         channels: list,
         classes: int = 1000,
-        initial_layers: str = "imagenet",
+        image_resolution: Optional[List[int]] = None,
         image_channels: int = 3,
     ) -> None:
         """Creates ResNetV2 model.
 
         Args:
             block (Module): Block to be used for building the layers.
             layers (list): layer sizes
             channels (list): channel num used for input/output channel size of layers. there must always be one more
                 channels than there are layers.
             classes (int): number of output classes
-            initial_layers (str, optional): name of set for initial layers. refer to common_layers.py.
-                Defaults to "imagenet".
+            image_resolution (List[int], optional): resolution of input image. refer to common_layers.py.
+                Defaults to None.
             image_channels (int, optional): input channels of images. Defaults to 3.
 
         Raises:
             ValueError: raised if the number of channels does not match number of layer + 1
         """
         super(ResNetV2, self).__init__(classes, channels)
         if len(channels) != (len(layers) + 1):
             raise ValueError(
                 f"the len of channels ({len(channels)}) must be exactly the len of layers ({len(layers)}) + 1!"
             )
 
         feature_layers: List[nn.Module] = []
         feature_layers.append(nn.BatchNorm2d(image_channels))
-        feature_layers.extend(get_initial_layers(initial_layers, image_channels, channels[0]))
+        feature_layers.extend(get_initial_layers(image_resolution, image_channels, channels[0]))
 
         feature_layers.extend(self.make_feature_layers(block, layers, channels))
 
         feature_layers.append(nn.BatchNorm2d(channels[-1]))
         feature_layers.append(nn.ReLU())
         feature_layers.append(nn.AdaptiveAvgPool2d(1))
         feature_layers.append(nn.Flatten())
@@ -444,204 +507,167 @@
 
 """
 Resnet specifications
 """
 
 
 class Resnet(Model):
-
-    name = "resnet"
+    name = "Resnet"
 
     resnet_spec = {
         18: ("basic_block", [2, 2, 2, 2], [64, 64, 128, 256, 512]),
         34: ("basic_block", [3, 4, 6, 3], [64, 64, 128, 256, 512]),
         50: ("bottle_neck", [3, 4, 6, 3], [64, 256, 512, 1024, 2048]),
         101: ("bottle_neck", [3, 4, 23, 3], [64, 256, 512, 1024, 2048]),
         152: ("bottle_neck", [3, 8, 36, 3], [64, 256, 512, 1024, 2048]),
     }
     resnet_net_versions = [ResNetV1, ResNetV2]
     resnet_block_versions = [
         {"basic_block": BasicBlockV1, "bottle_neck": BottleneckV1},
         {"basic_block": BasicBlockV2, "bottle_neck": BottleneckV2},
     ]
 
-    def __init__(self, resnet_version: int, resnet_num_layers: int, dataset: BasicDataset) -> None:
-        super(Resnet, self).__init__(dataset)
-        self._model = self.create_resnet(
-            resnet_version,
-            resnet_num_layers,
-            self._dataset.num_classes,
-            self._dataset.name,
-            self._dataset.shape[1],
-        )
+    def __init__(
+        self,
+        resnet_version: int,
+        resnet_num_layers: int,
+        input_shape: List[int],
+        num_classes: int = 0,
+    ) -> None:
+        super(Resnet, self).__init__(input_shape, num_classes)
+        self._model = self.create_resnet(resnet_version, resnet_num_layers)
         logging.info(f"building Resnetv{str(resnet_version)} with {str(resnet_num_layers)} layers...")
 
-    def create_resnet(
-        self,
-        version: int,
-        num_layers: int,
-        classes: int = 1000,
-        initial_layers: str = "imagenet",
-        image_channels: int = 3,
-    ) -> Module:
+    def create_resnet(self, version: int, num_layers: int) -> Module:
         """Creates a resnet complying to given version and layer number.
 
         Args:
             version (int): version of resnet to be used. availavle versions are 1 or 2
             num_layers (int): number of layers to be build.
-            classes (int, optional): number of output classes. Defaults to 1000.
-            initial_layers (str, optional): name of set of initial layers to be used. Defaults to "imagenet".
-            image_channels (int, optional): number of channels of input images. Defaults to 3.
 
         Raises:
             ValueError: raised if no resnet specification for given num_layers is listed in the resnet_spec dict above
             ValueError: raised if invalid resnet version was passed
 
         Returns:
             Module: resnet model
         """
         if num_layers not in self.resnet_spec:
             raise ValueError(f"No resnet spec for {num_layers} available!")
         if version not in [1, 2]:
             raise ValueError(f"invalid resnet version {version}, only 1 or 2 allowed")
 
+        image_channels = self._input_shape[1]
+        image_resolution = self._input_shape[-2:]
         block_type, layers, channels = self.resnet_spec[num_layers]
         resnet = self.resnet_net_versions[version - 1]
         block = self.resnet_block_versions[version - 1][block_type]
-        return resnet(block, layers, channels, classes, initial_layers, image_channels)
+        return resnet(block, layers, channels, self._num_classes, image_resolution, image_channels)
+
+    @classmethod
+    def _load_default_model(cls) -> Model:
+        return cls.from_pretrained(input_shape=IMAGENET_INPUT_SHAPE, num_classes=IMAGENET_CLASSES)
 
     @staticmethod
     def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
-            "--resnet-version",
+            "--version",
             type=int,
             choices=[1, 2],
             required=True,
             help="version of resnet to be used",
         )
         parser.add_argument(
-            "--resnet-num-layers",
+            "--num-layers",
             type=int,
             choices=[18, 34, 50, 152],
             required=True,
             help="number of layers to be used inside resnet",
         )
 
 
-class Resnet18V1(Resnet):
+class Resnet18V1(NoArgparseArgsMixin, Resnet):
     """ResNet-18 V1 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet18v1"
+    name = "Resnet18V1"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet18V1, self).__init__(1, 18, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet34V1(Resnet):
+class Resnet34V1(NoArgparseArgsMixin, Resnet):
     """ResNet-34 V1 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet34v1"
+    name = "Resnet34V1"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet34V1, self).__init__(1, 34, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet50V1(Resnet):
+class Resnet50V1(NoArgparseArgsMixin, Resnet):
     """ResNet-50 V1 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet50v1"
+    name = "Resnet50V1"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet50V1, self).__init__(1, 50, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet152V1(Resnet):
+class Resnet152V1(NoArgparseArgsMixin, Resnet):
     """ResNet-152 V1 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet152v1"
+    name = "Resnet152V1"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet152V1, self).__init__(1, 152, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet18V2(Resnet):
+class Resnet18V2(NoArgparseArgsMixin, Resnet):
     """ResNet-18 V2 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet18v2"
+    name = "Resnet18V2"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet18V2, self).__init__(2, 18, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet34V2(Resnet):
+class Resnet34V2(NoArgparseArgsMixin, Resnet):
     """ResNet-34 V2 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet34v2"
+    name = "Resnet34V2"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet34V2, self).__init__(2, 34, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet50V2(Resnet):
+class Resnet50V2(NoArgparseArgsMixin, Resnet):
     """ResNet-50 V2 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet50v2"
+    name = "Resnet50V2"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet50V2, self).__init__(2, 50, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class Resnet152V2(Resnet):
+class Resnet152V2(NoArgparseArgsMixin, Resnet):
     """ResNet-152 V2 model from `"Deep Residual Learning for Image Recognition"
     <http://arxiv.org/abs/1512.03385>`_ paper.
     """
 
-    name = "resnet152v2"
+    name = "Resnet152V2"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(Resnet152V2, self).__init__(2, 152, *args, **kwargs)
-
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
```

### Comparing `bitorch-0.3.0.dev1/bitorch/models/resnet_e.py` & `bitorch-0.4.0.dev0/bitorch/models/resnet_e.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Resnet_E implementation from `"Back to Simplicity: How to Train Accurate BNNs from Scratch?"
 <https://arxiv.org/abs/1906.08637>`_ paper.
 """
-from bitorch.datasets.base import BasicDataset
-from .base import Model
-from typing import List, Any
+from .base import Model, NoArgparseArgsMixin
+from typing import Optional, List, Any
 import torch
 import argparse
 from torch import nn
 import logging
 
 from bitorch.layers import QConv2d
-from bitorch.models.common_layers import get_initial_layers
+from bitorch.models.common_layers import get_initial_layers, IMAGENET_INPUT_SHAPE, IMAGENET_CLASSES
 
 __all__ = ["ResnetE34", "ResnetE18", "ResnetE"]
 
 
 class BasicBlock(nn.Module):
     """BasicBlock from `"Back to Simplicity: How to Train Accurate BNNs from Scratch?"
     <https://arxiv.org/abs/1906.08637>`_ paper.
@@ -45,27 +44,41 @@
         """builds the downsampling layers for rediual tensor processing
             ResNetE uses the full-precision downsampling layer
         Returns:
             nn.Sequential: the downsampling model
         """
         return nn.Sequential(
             nn.AvgPool2d(kernel_size=2, stride=self.stride),
-            nn.Conv2d(self.in_channels, self.out_channels, kernel_size=1, stride=1, padding=0, bias=False),
+            nn.Conv2d(
+                self.in_channels,
+                self.out_channels,
+                kernel_size=1,
+                stride=1,
+                padding=0,
+                bias=False,
+            ),
             nn.BatchNorm2d(self.out_channels, momentum=0.9),
         )
 
     def _build_body(self) -> nn.Sequential:
-        """Builds the body of a building block, i.e. two binary convolutions with BatchNorms in between.
-        Check the referenced paper for more details.
+        """builds body of building block, i.e. two binary convolutions with batchnorms in between. Check referenced paper for
+        more details.
 
         Returns:
             nn.Sequential: the basic building block body model
         """
         return nn.Sequential(
-            QConv2d(self.in_channels, self.out_channels, kernel_size=3, stride=self.stride, padding=1, bias=False),
+            QConv2d(
+                self.in_channels,
+                self.out_channels,
+                kernel_size=3,
+                stride=self.stride,
+                padding=1,
+                bias=False,
+            ),
             nn.BatchNorm2d(self.out_channels, momentum=0.9),
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """forwards the input tensor x through the building block.
 
         Args:
@@ -104,15 +117,15 @@
             in_channels (int): the input channels of this layer
             out_channels (int): the output channels of this layer
             stride (int): the stride to be used in the convolution layers
 
         Returns:
             nn.Sequential: the model containing the building blocks
         """
-        # this trick adds shortcut connections between original resnet blocks
+        # this tricks adds shortcut connections between original resnet blocks
         # we multiple number of blocks by 2, but add only one layer instead of two in each block
         layers = layers * 2
 
         layer_list: List[nn.Module] = []
         layer_list.append(BasicBlock(in_channels, out_channels, stride))
         for _ in range(layers - 1):
             layer_list.append(BasicBlock(out_channels, out_channels, 1))
@@ -151,39 +164,44 @@
 class _ResnetE(SpecificResnetE):
     """ResNetE-18 model from
     `"Back to Simplicity: How to Train Accurate BNNs from Scratch?"
     <https://arxiv.org/abs/1906.08637>`_ paper.
     """
 
     def __init__(
-        self, layers: list, channels: list, classes: int, initial_layers: str = "imagenet", image_channels: int = 3
+        self,
+        layers: list,
+        channels: list,
+        classes: int,
+        image_resolution: Optional[List[int]] = None,
+        image_channels: int = 3,
     ) -> None:
         """Creates ResNetE model.
 
         Args:
             layers (list): layer sizes
             channels (list): channel num used for input/output channel size of layers. there must always be one more
                 channels than there are layers.
             classes (int): number of output classes
-            initial_layers (str, optional): name of set for initial layers. refer to common_layers.py.
-                Defaults to "imagenet".
+            image_resolution (List[int], optional): resolution of input image. refer to common_layers.py.
+                Defaults to None.
             image_channels (int, optional): input channels of images. Defaults to 3.
 
         Raises:
             ValueError: raised if the number of channels does not match number of layer + 1
         """
         super(_ResnetE, self).__init__(classes, channels)
         if len(channels) != (len(layers) + 1):
             raise ValueError(
                 f"the len of channels ({len(channels)}) must be exactly the len of layers ({len(layers)}) + 1!"
             )
 
         feature_layers: List[nn.Module] = []
         # feature_layers.append(nn.BatchNorm2d(image_channels, eps=2e-5, momentum=0.9))
-        feature_layers.extend(get_initial_layers(initial_layers, image_channels, channels[0]))
+        feature_layers.extend(get_initial_layers(image_resolution, image_channels, channels[0]))
         feature_layers.append(nn.BatchNorm2d(channels[0], momentum=0.9))
 
         feature_layers.extend(self.make_feature_layers(layers, channels))
 
         feature_layers.append(nn.ReLU())
         feature_layers.append(nn.AdaptiveAvgPool2d(1))
         feature_layers.append(nn.Flatten())
@@ -193,86 +211,75 @@
 
 """
 ResNet-e specifications
 """
 
 
 class ResnetE(Model):
-
-    name = "resnete"
+    name = "ResnetE"
 
     resnet_spec = {
         18: ([2, 2, 2, 2], [64, 64, 128, 256, 512]),
         34: ([3, 4, 6, 3], [64, 64, 128, 256, 512]),
     }
 
-    def __init__(self, resnete_num_layers: int, dataset: BasicDataset) -> None:
-        super(ResnetE, self).__init__(dataset)
-        self._model = self.create(
-            resnete_num_layers, self._dataset.num_classes, self._dataset.name, self._dataset.shape[1]
-        )
+    def __init__(self, resnete_num_layers: int, input_shape: List[int], num_classes: int = 0) -> None:
+        super(ResnetE, self).__init__(input_shape, num_classes)
+        self._model = self.create(resnete_num_layers)
         logging.info(f"building ResnetE with {str(resnete_num_layers)} layers...")
 
-    @classmethod
-    def create(
-        cls, num_layers: int, classes: int = 1000, initial_layers: str = "imagenet", image_channels: int = 3
-    ) -> nn.Module:
+    def create(self, num_layers: int) -> nn.Module:
         """Creates a ResNetE complying to given layer number.
 
         Args:
             num_layers (int): number of layers to be build.
-            classes (int, optional): number of output classes. Defaults to 1000.
-            initial_layers (str, optional): name of set of initial layers to be used. Defaults to "imagenet".
-            image_channels (int, optional): number of channels of input images. Defaults to 3.
 
         Raises:
             ValueError: raised if no resnet specification for given num_layers is listed in the resnet_spec dict above
 
         Returns:
             Module: resnetE model
         """
-        if num_layers not in cls.resnet_spec:
+        if num_layers not in self.resnet_spec:
             raise ValueError(f"No resnet spec for {num_layers} available!")
 
-        layers, channels = cls.resnet_spec[num_layers]
+        layers, channels = self.resnet_spec[num_layers]
+        image_channels = self._input_shape[1]
+        image_resolution = self._input_shape[-2:]
 
-        return _ResnetE(layers, channels, classes, initial_layers, image_channels)
+        return _ResnetE(layers, channels, self._num_classes, image_resolution, image_channels)
+
+    @classmethod
+    def _load_default_model(cls) -> Model:
+        return cls.from_pretrained(input_shape=IMAGENET_INPUT_SHAPE, num_classes=IMAGENET_CLASSES)
 
     @staticmethod
     def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
-            "--resnetE-num-layers",
+            "--num-layers",
             type=int,
             choices=[18, 34],
             required=True,
             help="number of layers to be used inside resnetE",
         )
 
 
-class ResnetE18(ResnetE):
+class ResnetE18(NoArgparseArgsMixin, ResnetE):
     """ResNetE-18 model from `"Back to Simplicity: How to Train Accurate BNNs from Scratch?"
     <https://arxiv.org/abs/1906.08637>`_ paper.
     """
 
-    name = "resnete18"
+    name = "ResnetE18"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(ResnetE18, self).__init__(18, *args, **kwargs)
 
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
-
 
-class ResnetE34(ResnetE):
+class ResnetE34(NoArgparseArgsMixin, ResnetE):
     """ResNetE-34 model from `"Back to Simplicity: How to Train Accurate BNNs from Scratch?"
     <https://arxiv.org/abs/1906.08637>`_ paper.
     """
 
-    name = "resnete34"
+    name = "ResnetE34"
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(ResnetE34, self).__init__(34, *args, **kwargs)
-
-    @staticmethod
-    def add_argparse_arguments(parser: argparse.ArgumentParser) -> None:
-        pass
```

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/approx_sign.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/approx_sign.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/base.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/base.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/identity.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/identity.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/progressive_sign.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/progressive_sign.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 """Progressive Sign Function"""
 import typing
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Union
 
 import torch
 import torch.nn.functional as F
+from torch.autograd.function import Function
 
-from .base import Quantization, STE
-from .config import config
+from bitorch.config import Config
+from .base import Quantization
 from .sign import SignFunction
 
 EPSILON = 1e-7
 
 
-class ProgressiveSignFunctionTrain(STE):
+class ProgressiveSignConfig(Config):
+    name = "progressive_sign_config"
+
+    # scaling of progressive sign function, should be zero at the start of the training, and (close to) one at the end
+    progressive_sign_scale = 0.0
+
+    # alpha of default progressive sign transform function, should be between 2 and 10
+    progressive_sign_alpha = 4
+
+    # beta of default progressive sign transform function, should be between 2 and 10
+    progressive_sign_beta = 10
+
+
+config = ProgressiveSignConfig()
+
+
+class ProgressiveSignFunctionTrain(Function):
     @staticmethod
     @typing.no_type_check
     def forward(
         ctx: torch.autograd.function.BackwardCFunction,  # type: ignore
         input_tensor: torch.Tensor,
         temperature: float,
     ) -> torch.Tensor:
@@ -26,14 +43,15 @@
             ctx (Any): autograd context
             input_tensor (torch.Tensor): input tensor
             temperature: the temperature of the incline
 
         Returns:
             torch.Tensor: the sign tensor
         """
+        ctx.save_for_backward(input_tensor)
         # avoid division by zero with EPSILON
         return F.hardtanh(input_tensor / max(1.0 - temperature, EPSILON))
 
     @staticmethod
     @typing.no_type_check
     def backward(ctx: Any, output_gradient: torch.Tensor) -> torch.Tensor:
         return output_gradient, None  # type: ignore
@@ -49,57 +67,85 @@
     """
 
     name = "progressive_sign"
     bit_width = 1
 
     scale: float
     global_scaling: bool
+    alpha: Union[int, float]
+    beta: Union[int, float]
 
     def __init__(
         self,
         use_global_scaling: bool = True,
         initial_scale: Optional[float] = None,
         custom_transform: Optional[Callable[[float], float]] = None,
+        alpha: Optional[Union[int, float]] = None,
+        beta: Optional[Union[int, float]] = None,
     ) -> None:
         """
         Initialize the progressive sign module (can be used for progressive weight binarization).
 
         If `use_global_scaling` is set to False, the scale of this module must be set manually.
         Otherwise, the value can be set for all progressive sign modules in the config.
 
         Args:
             use_global_scaling: whether to use the global scaling variable stored in the config
             initial_scale: if not using global scaling you can set an initial scale
             custom_transform: to use a custom transform function from scale to temperature, add it here
+            alpha: parameters of default transform function
+            beta: parameters of default transform function
         """
         super().__init__()
         if initial_scale is not None and use_global_scaling:
             raise RuntimeWarning(
                 "An initial scale was set on ProgressiveSign, but this has not effect, "
                 "since use_global_scaling is True."
             )
         self.global_scaling = use_global_scaling
         self.scale = initial_scale or config.progressive_sign_scale
         self.custom_transform = custom_transform
+        self.alpha = alpha or config.progressive_sign_alpha
+        self.beta = beta or config.progressive_sign_beta
 
     @property
     def current_scale(self) -> float:
+        """Return the current scale of this Progressive Sign layer."""
         if self.global_scaling:
             return config.progressive_sign_scale
         return self.scale
 
     @staticmethod
-    def default_transform(x: float) -> float:
-        return 1 - (5 ** (-3 * x))
+    def default_transform(
+        scale: float, alpha: Optional[Union[int, float]] = None, beta: Optional[Union[int, float]] = None
+    ) -> float:
+        """Transform the given scale into the temperature of the progressive sign function with the default function.
 
-    def transform(self, x: float) -> float:
-        """Transform x for a steady temperature increase, higher at the beginning, and much less at the end."""
+        The formula is as follows: 1 - (alpha ** (-beta * scale))
+
+        Args:
+            scale: the current scale
+            alpha: base of default exponential function
+            beta: (negative) factor of scale exponent
+        """
+        if alpha is None:
+            alpha = config.progressive_sign_alpha
+        if beta is None:
+            beta = config.progressive_sign_beta
+        return 1 - (alpha ** (-beta * scale))
+
+    def transform(self, scale: float) -> float:
+        """Transform the given scale into a steady temperature increase, higher at the start, and much less at the end.
+
+        Args:
+            scale: the current scale
+        """
         if self.custom_transform is not None:
-            return self.custom_transform(x)
-        return self.default_transform(x)
+            return self.custom_transform(scale)
+        return self.default_transform(scale, self.alpha, self.beta)
 
     def quantize(self, x: torch.Tensor) -> torch.Tensor:
         """Forwards the tensor through the sign function.
 
         Args:
             x (torch.Tensor): tensor to be forwarded.
```

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/sign.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 class SignFunction(STE):
     @staticmethod
     @typing.no_type_check
     def forward(
         ctx: torch.autograd.function.BackwardCFunction,  # type: ignore
         input_tensor: torch.Tensor,
     ) -> torch.Tensor:
-        """Binarize the input tensor using the sign function
+        """Binarize the input tensor using the sign function.
 
         Args:
             ctx (Any): autograd context
             input_tensor (torch.Tensor): input tensor
 
         Returns:
             torch.Tensor: the sign tensor
         """
         sign_tensor = torch.sign(input_tensor)
         sign_tensor = torch.where(sign_tensor == 0, torch.tensor(1.0, device=sign_tensor.device), sign_tensor)
         return sign_tensor
 
 
 class Sign(Quantization):
-    """Module for applying the sign function with straight through estimator in backward pass"""
+    """Module for applying the sign function with straight through estimator in backward pass."""
 
     name = "sign"
     bit_width = 1
 
     def quantize(self, x: torch.Tensor) -> torch.Tensor:
         """Forwards the tensor through the sign function.
```

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/ste_heaviside.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/ste_heaviside.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Sign Function Implementation"""
 import torch
 import typing
+from typing import Any
 from .base import STE, Quantization
 
 
 class SteHeavisideFunction(STE):
     @staticmethod
     @typing.no_type_check
     def forward(
@@ -16,21 +17,40 @@
         Args:
             ctx (Any): autograd context
             input_tensor (torch.Tensor): input tensor
 
         Returns:
             torch.Tensor: the quantized input tensor
         """
+        ctx.save_for_backward(input_tensor)
+
         quantized_tensor = torch.where(
             input_tensor > 0,
             torch.tensor(1.0, device=input_tensor.device),
-            torch.tensor(0.0, device=input_tensor.device),
+            torch.tensor(-1.0, device=input_tensor.device),
         )
         return quantized_tensor
 
+    @staticmethod
+    @typing.no_type_check
+    def backward(ctx: Any, output_gradient: torch.Tensor) -> torch.Tensor:
+        """just passes the unchanged output gradient as input gradient.
+
+        Args:
+            ctx (Any): autograd context
+            output_gradient (torch.Tensor): output gradient
+
+        Returns:
+            torch.Tensor: the unchanged output gradient
+        """
+        input_tensor = ctx.saved_tensors[0]
+        inside_threshold = torch.abs(input_tensor) <= 1
+        print("over threshold:", len(input_tensor) - torch.sum(inside_threshold))
+        return output_gradient * inside_threshold
+
 
 class SteHeaviside(Quantization):
     """Module for applying the SteHeaviside quantization, using an ste in backward pass"""
 
     name = "steheaviside"
     bit_width = 1
```

### Comparing `bitorch-0.3.0.dev1/bitorch/quantizations/swish_sign.py` & `bitorch-0.4.0.dev0/bitorch/quantizations/swish_sign.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/runtime_mode.py` & `bitorch-0.4.0.dev0/bitorch/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/bitorch/util.py` & `bitorch-0.4.0.dev0/bitorch/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# import sys
 import typing
 import importlib
-from typing import Callable, List, Any, Dict
+from typing import Optional, Callable, List, Any, Dict
 
 
 @typing.no_type_check
 def build_lookup_dictionary(
     current_module_name: str,
     class_strings: List[str],
-    filter_by_superclass: Any = None,
-    filter_fn: Callable[[Any], bool] = None,
+    filter_by_superclass: Optional[Any] = None,
+    filter_fn: Optional[Callable[[Any], bool]] = None,
     key_fn: Callable[[Any], str] = lambda x: x.name,
 ) -> Dict[str, Any]:
     """Builds a lookup dictionary based on a list of strings of class names.
 
     Args:
         current_module_name (str): the module from where the classes are available
         class_strings (List[str]): the list of strings
@@ -29,15 +28,15 @@
 
         def filter_fn(x: Any) -> bool:
             return isinstance(x, type) and issubclass(x, filter_by_superclass) and x != filter_by_superclass
 
     lookup = {}
     current_module = importlib.import_module(current_module_name)
     for class_name in class_strings:
-        # current_module = sys.modules.get(current_module_name, None)
         if not hasattr(current_module, class_name):
             continue
         class_ = getattr(current_module, class_name)
         if filter_fn(class_):
-            lookup[key_fn(class_)] = class_
+            transformed_key = key_fn(class_)
+            lookup[transformed_key] = class_
 
     return lookup
```

### Comparing `bitorch-0.3.0.dev1/bitorch.egg-info/PKG-INFO` & `bitorch-0.4.0.dev0/bitorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: bitorch
-Version: 0.3.0.dev1
+Version: 0.4.0.dev0
 Summary: A package for building and training quantized and binary neural networks with Pytorch
 Home-page: https://github.com/hpi-xnor/bitorch
 Author: Hasso Plattner Institute
 Author-email: fb10-xnor@hpi.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: opt
 License-File: LICENSE
 
 # BITorch
```

### Comparing `bitorch-0.3.0.dev1/examples/mnist/README.md` & `bitorch-0.4.0.dev0/examples/mnist/README.md`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/examples/mnist/train_mnist.py` & `bitorch-0.4.0.dev0/examples/mnist/train_mnist.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 from torch.optim.lr_scheduler import StepLR
 
 import bitorch.layers as qnn
-from bitorch import datasets as bitorch_datasets, RuntimeMode
+from bitorch import RuntimeMode
+from datasets import MNIST
 from bitorch.layers import convert
-import bitorch_inference_engine
+import bitorch_engine
 
 
-bitorch_inference_engine.initialize()
+bitorch_engine.initialize()
 
 
 class QuantizedMLP(nn.Module):
     def __init__(self, num_hidden_units_1=256, num_hidden_units_2=128):
         super().__init__()
         self.flatten = nn.Flatten()
         self.fc1 = nn.Linear(784, num_hidden_units_1)
@@ -152,15 +153,15 @@
     if use_cuda:
         cuda_kwargs = {'num_workers': 1,
                        'pin_memory': True,
                        'shuffle': True}
         train_kwargs.update(cuda_kwargs)
         test_kwargs.update(cuda_kwargs)
 
-    train_dataset, test_dataset = bitorch_datasets.MNIST.get_train_and_test(download=True)
+    train_dataset, test_dataset = MNIST.get_train_and_test(download=True)
 
     train_loader = torch.utils.data.DataLoader(train_dataset, **train_kwargs)
     test_loader = torch.utils.data.DataLoader(test_dataset, **test_kwargs)
 
     if args.model == "mlp":
         model = QuantizedMLP().to(device)
     else:
```

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/README.md` & `bitorch-0.4.0.dev0/examples/image_classification/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -38,22 +38,22 @@
 - `--wandb` toggles logging to wandb. You need to specify a WANDB_API_TOKEN variable in your environment to use this. [details](https://docs.wandb.ai/guides/track/public-api-guide#authentication)
 - `--result-file` specifies path to a result file which will contain the evaluation metrics in csv format.
 - `--checkpoint-dir` path to where checkpoints shall be stored
 - `--checkpoint-load` path to checkpoint to load from
 
 ### model args
 
-- `--model` specify name of model you want to train. Choose from `lenet,resnet,resnet152v1,resnet152v2,resnet18v1,resnet18v2,resnet34v1,resnet34v2,resnet50v1,resnet50v2,resnete,resnete18` or `resnete34`
+- `--model` specify name of model you want to train. Choose from `Lenet,Resnet,Resnet152V1,Resnet152V2,Resnet18V1,Resnet18V2,Resnet34V1,Resnet34V2,Resnet50V1,Resnet50V2,ResnetE,ResnetE18,ResnetE34,Quicknet,QuicknetSmall` or `QuickNetLarge`
 
 Each model can have specific arguments. Check them by calling `python image_classification.py --help`.
 
 ### dataset args
 
 - `--datset` name of dataset to train on. Chose from `mnist, cifar10, cifar100` and `imagenet`
-- `--download` toggles if dataset if not present at `--dataset-dir` should be downloaded. Only available for `mnist` and `cifar10`.
+- `--download` toggles if dataset is not present at `--dataset-dir` should be downloaded. Only available for `mnist` and `cifar10`.
 - `--dataset-dir` path to dataset.
 - `--num-worker` sets number of workers for dataloading
 
 ### quantization args
 
 - `--input-quantization` chooses the default input quantization method.
 - `--weight-quantization` chooses the default weight quantization method.
```

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/image_classification.py` & `bitorch-0.4.0.dev0/examples/image_classification/image_classification.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,39 +10,56 @@
         stderrToServer=True,
     )
 
 import argparse
 import logging
 from pathlib import Path
 from typing import List, Any, Type
+import copy
 
 import fvbitcore.nn as fv_nn
 import torch
 import wandb
+import pytorch_lightning as pl
 from pytorch_lightning import Trainer
-from pytorch_lightning.callbacks import ModelCheckpoint, LearningRateMonitor
-from pytorch_lightning.loggers import CSVLogger, TensorBoardLogger, LightningLoggerBase
+from pytorch_lightning.callbacks import ModelCheckpoint, LearningRateMonitor, Callback
+from pytorch_lightning.loggers import CSVLogger, TensorBoardLogger, Logger
+from pytorch_lightning.utilities.types import STEP_OUTPUT
+from lightning_fabric.utilities.imports import _TORCH_GREATER_EQUAL_2_0
 from torch.utils.data import DataLoader
 
 import bitorch
 from bitorch import apply_args_to_configuration, RuntimeMode
-from bitorch.datasets import dataset_from_name
-from bitorch.datasets.base import Augmentation
+from bitorch.quantizations import Quantization_Scheduler, quantization_from_name
+from datasets import dataset_from_name
 from bitorch.models import model_from_name
 from bitorch.quantizations import Quantization
-from examples.pytorch_lightning.utils.callbacks import ProgressiveSignScalerCallback
-from examples.pytorch_lightning.utils.log import CommandLineLogger
-from examples.pytorch_lightning.utils.wandb_logger import CustomWandbLogger
+from examples.image_classification.utils.callbacks import ProgressiveSignScalerCallback
+from examples.image_classification.utils.log import CommandLineLogger
+from examples.image_classification.utils.wandb_logger import CustomWandbLogger
 from utils.arg_parser import create_argparser
 from utils.lightning_model import ModelWrapper, DistillationModelWrapper
 from utils.utils import configure_logging
 
 logger = logging.getLogger()
 
 
+class ModelCallback(Callback):
+    def on_train_batch_end(
+        self,
+        trainer: Trainer,
+        pl_module: pl.LightningModule,
+        outputs: STEP_OUTPUT,
+        batch: Any,
+        batch_idx: int,
+        unused: int = 0,
+    ) -> None:
+        pl_module.model.apply(pl_module.model.on_train_batch_end)  # type: ignore
+
+
 def main(args: argparse.Namespace, model_args: argparse.Namespace) -> None:
     """trains a model on the configured image dataset.
 
     Args:
         args (argparse.Namespace): cli arguments
         model_args (argparse.Namespace): model specific cli arguments
     """
@@ -52,19 +69,19 @@
     bitorch.mode = RuntimeMode.RAW
 
     apply_args_to_configuration(args)
 
     output_dir = Path(args.result_directory)
     output_dir.mkdir(exist_ok=True)
 
-    loggers: List[LightningLoggerBase] = []
+    loggers: List[Logger] = []
     if args.tensorboard_log:
-        loggers.append(TensorBoardLogger(str(output_dir), name="tensorboard"))
+        loggers.append(TensorBoardLogger(str(output_dir), name="tensorboard"))  # type: ignore
     if args.csv_log:
-        loggers.append(CSVLogger(str(output_dir), name="csv"))
+        loggers.append(CSVLogger(str(output_dir), name="csv"))  # type: ignore
     if args.wandb_log:
         loggers.append(
             CustomWandbLogger(
                 args,
                 project=args.wandb_project,
                 name=args.wandb_experiment,
                 save_dir=str(output_dir),
@@ -81,14 +98,16 @@
                 every_n_epochs=1,
                 monitor="metrics/test-top1-accuracy",
                 mode="max",
                 filename="{epoch:03d}",
             )
         )
 
+    callbacks.append(ModelCallback())
+
     # providing our own progress bar disables the default progress bar (not needed to disable later on)
     cmd_logger = CommandLineLogger(args.log_interval)
     callbacks.append(cmd_logger)
     configure_logging(cmd_logger.logger, args.log_file, args.log_level, args.log_stdout)
 
     # add scaling callback for progressive sign (not be needed for all models, but should not slow down training)
     callbacks.append(ProgressiveSignScalerCallback())
@@ -98,58 +117,78 @@
         callbacks.append(lr_monitor)
 
     dataset = dataset_from_name(args.dataset)
 
     model_kwargs = vars(model_args)
     logger.debug(f"got model args as dict: {model_kwargs}")
 
-    model = model_from_name(args.model)(**model_kwargs, dataset=dataset)  # type: ignore
-    model.initialize()
+    model_kwargs["input_shape"] = tuple(dataset.shape)
+    model_kwargs["num_classes"] = dataset.num_classes
+    if args.pretrained:
+        model = model_from_name(args.model).from_pretrained(args.checkpoint_load, **model_kwargs)
+    else:
+        model = model_from_name(args.model)(**model_kwargs)  # type: ignore
+        model.initialize()
+
+    # for model registry compliance
+    model_kwargs["model_name"] = args.model
+    if args.wandb_log:
+        wandb.config.update({"model_config": model_kwargs})
+
+    if args.quantization_scheduling:
+        quantization_scheduler = Quantization_Scheduler(
+            model,
+            quantizations=[quantization_from_name(name)() for name in args.scheduled_quantizations],
+            scheduling_procedure=args.quantization_scheduling_procedure,
+            schedule_all_quantizations=args.schedule_all_quantizations,
+            steps=args.max_epochs if args.max_epochs is not None else int(args.max_steps),
+        )
+    else:
+        quantization_scheduler = None
 
     wrapper_class: Type[ModelWrapper] = ModelWrapper
     if args.teacher:
         if args.dataset != "imagenet":
             raise ValueError(
                 f"Teacher '{args.teacher}' and dataset '{args.dataset}' selected, "
                 f"but teacher models are only supported for imagenet."
             )
         wrapper_class = DistillationModelWrapper
 
-    if args.checkpoint_load is not None and args.pretrained:
-        logger.info(f"starting training from pretrained model at checkpoint {args.checkpoint_load}")
+    if args.checkpoint_load is not None and args.resume_training:
+        logger.info(f"resuming training from pretrained model at checkpoint {args.checkpoint_load}")
         model_wrapped = wrapper_class.load_from_checkpoint(args.checkpoint_load)
     else:
-        model_wrapped = wrapper_class(model, dataset.num_classes, args)
+        model_wrapped = wrapper_class(model, dataset.num_classes, quantization_scheduler, args)
 
     trainer = Trainer(
         strategy=args.strategy,
         accelerator="cpu" if args.cpu else args.accelerator,
-        gpus=0 if args.cpu else args.gpus,
+        devices=args.devices,
         max_epochs=args.max_epochs,
         max_steps=args.max_steps,
         logger=loggers if len(loggers) > 0 else None,  # type: ignore
         callbacks=callbacks,  # type: ignore
         log_every_n_steps=args.log_interval,
         limit_train_batches=0.01 if args.dev_run else None,
         limit_val_batches=0.01 if args.dev_run else None,
     )
-    augmentation_level = Augmentation.from_string(args.augmentation)
     if args.dev_run:
-        logger.info("This run only uses 1 % of training and validation data (--dev-run)!")
+        logger.info("this run only uses 1 % of training and validation data (--dev-run)!")
     logger.info(f"model: {args.model}")
     logger.info(f"optimizer: {args.optimizer}")
     logger.info(f"lr: {args.lr}")
     logger.info(f"max_epochs: {args.max_epochs}")
     if args.fake_data:
         logger.info(f"dummy dataset: {dataset.name} (not using real data!)")
         train_dataset, test_dataset = dataset.get_dummy_train_and_test_datasets()  # type: ignore
     else:
         logger.info(f"dataset: {dataset.name}")
         train_dataset, test_dataset = dataset.get_train_and_test(  # type: ignore
-            root_directory=args.dataset_dir, download=args.download, augmentation=augmentation_level
+            root_directory=args.dataset_dir, download=args.download
         )
     train_loader = DataLoader(
         train_dataset,
         batch_size=args.batch_size,
         num_workers=args.num_workers,
         shuffle=True,
         pin_memory=True,
@@ -176,20 +215,35 @@
     if args.wandb_log:
         wandb.config.update(
             {
                 "mflops": total_flops / 1e6,
                 "size in MB": total_size / 1e6 / 8.0,
             }
         )
+    if not args.no_compile:
+        if not _TORCH_GREATER_EQUAL_2_0:
+            logging.info("torch.compile not supported in torch < 2.0, skipping compilation")
+        else:
+            logging.info("compiling model with torch.compile...")
+            model_before_compile = copy.deepcopy(model_wrapped.model)
+            try:
+                if args.accelerator in ["gpu", "auto"] and torch.cuda.is_available():
+                    model_wrapped = model_wrapped.cuda()
+
+                model_wrapped.model = torch.compile(model_wrapped.model, mode=args.compile_mode)
+                logging.info("model compiled successfully")
+            except RuntimeError as e:
+                logging.warning(f"model compilation failed: {e} - skipping compilation")
+                model_wrapped.model = model_before_compile
 
     trainer.fit(
         model_wrapped,
         train_dataloaders=train_loader,
         val_dataloaders=test_loader,
-        ckpt_path=args.checkpoint_load if not args.pretrained else None,
+        ckpt_path=args.checkpoint_load if args.resume_training else None,
     )
 
 
 if __name__ == "__main__":
     parser, model_parser = create_argparser()
     args_, unparsed_model_args = parser.parse_known_args()
     model_args_ = model_parser.parse_args(unparsed_model_args)
```

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/arg_parser.py` & `bitorch-0.4.0.dev0/examples/dlrm/utils/arg_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from argparse import ArgumentParser
 import sys
 from typing import Tuple
 
 from bitorch.models import model_from_name, model_names
-from bitorch.datasets import dataset_names
 from bitorch import add_config_args
+from bitorch.models.dlrm import DLRM
 from pytorch_lightning import Trainer
 
-from examples.pytorch_lightning.utils.teachers import available_teachers
-
 
 def add_logging_args(parser: ArgumentParser) -> None:
     """adds cli parameters for logging configuration
 
     Args:
         parser (ArgumentParser): the main argument parser
     """
@@ -100,20 +98,25 @@
         default=1,
         help="number of checkpoints to keep.",
     )
     checkpoint.add_argument(
         "--checkpoint-load",
         type=str,
         default=None,
-        help="path to checkpoint file to load state from. if omitted, a new model will be trained.",
+        help="path to checkpoint file to load state from. if omitted and --pretrained is activated, the model weights will be downloaded from the model hub. If --pretrained is not set, a new model will be trained.",
+    )
+    checkpoint.add_argument(
+        "--resume_training",
+        action="store_true",
+        help="resume training from given checkpoint",
     )
     checkpoint.add_argument(
         "--pretrained",
         action="store_true",
-        help="uses the given checkpoint as a pretrained model (only for initialization)",
+        help="load the state dict either from model hub or from checkpoint_load",
     )
 
 
 def add_optimizer_args(parser: ArgumentParser) -> None:
     """adds cli parameters for optimizer configuration
 
     Args:
@@ -155,43 +158,26 @@
         type=str,
         default="adam",
         choices=["adam", "sgd", "radam"],
         help="the optimizer to use. default is adam.",
     )
 
 
-def add_training_args(parser: ArgumentParser) -> None:
-    """
-    Add arguments for training strategies.
-
-    Args:
-        parser (ArgumentParser): the main argument parser
-    """
-    train = parser.add_argument_group("training", "parameters for the training strategies")
-    train.add_argument(
-        "--teacher",
-        type=str,
-        default="",
-        choices=available_teachers(),
-        help="name of the teacher model, the student is going to be trained with KD if not empty",
-    )
-
-
 def add_dataset_args(parser: ArgumentParser) -> None:
     """adds cli parameters for dataset configuration
 
     Args:
         parser (ArgumentParser): the main argument parser
     """
     data = parser.add_argument_group("dataset", "parameters for the dataset used for training")
     data.add_argument(
         "--dataset",
         type=str,
-        default="cifar10",
-        choices=dataset_names(),
+        default="criteo",
+        choices=["criteo"],
         help="name of the dataset to be used for training",
     )
     data.add_argument(
         "--dataset-dir",
         type=str,
         default=None,
         help="path to where the train dataset is saved / shall be downloaded to",
@@ -202,15 +188,27 @@
         help="toggles wether the dataset shall be downloaded if not present. "
         "only has effect with the cifar10 and mnist dataset so far.",
     )
     data.add_argument(
         "--batch-size",
         type=int,
         default=128,
-        help="batch size for training and testing (default: 128)",
+        help="batch size for training (default: 128)",
+    )
+    data.add_argument(
+        "--batch-size-test",
+        type=int,
+        default=128,
+        help="batch size for testing (might be higher than training) (default: 128)",
+    )
+    data.add_argument(
+        "--ignore-dataset-size",
+        type=float,
+        default=0.9,
+        help="portion of dataset that should be ignored for training (usefull for fast development) (default: 128)",
     )
     data.add_argument(
         "--num-workers",
         type=int,
         default=4,
         help="number of workers to be used for dataloading (default: 4)",
     )
@@ -272,47 +270,33 @@
         parser (ArgumentParser): parser to add the regular arguments to
     """
     Trainer.add_argparse_args(parser)
     add_logging_args(parser)
     add_dataset_args(parser)
     add_optimizer_args(parser)
     add_checkpoint_args(parser)
-    add_training_args(parser)
 
     add_config_args(parser)
-
-    parser.add_argument(
-        "--model",
-        type=str.lower,
-        choices=model_names(),
-        required=True,
-        help="name of the model to be trained",
-    )
     parser.add_argument(
         "--cpu",
         action="store_true",
         help="explicitly use the cpu. overwrites gpu settings",
     )
-    parser.add_argument(
-        "--dev-run",
-        action="store_true",
-        help="use only 1% of training/validation data for testing purposes",
-    )
 
 
-def create_argparser() -> Tuple[ArgumentParser, ArgumentParser]:
+def create_argparser(arguments=None) -> Tuple[ArgumentParser, ArgumentParser]:
     """creates a main argument parser for general options and a model parser for model specific options
 
     Returns:
         Tuple[ArgumentParser, ArgumentParser]: the main and model argument parser
     """
     parser = ArgumentParser(description="Bitorch Image Classification")
 
     add_regular_args(parser)
 
     if help_in_args():
-        add_all_model_args(parser)
+        model_group = parser.add_argument_group("DLRM", "parameters for DLRM model")
+        DLRM.add_argparse_arguments(model_group)
     args, _ = parser.parse_known_args()
 
-    model_class = model_from_name(args.model)
-    model_parser = create_model_argparser(model_class)
+    model_parser = create_model_argparser(DLRM)
     return parser, model_parser
```

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/callbacks.py` & `bitorch-0.4.0.dev0/examples/image_classification/utils/callbacks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+# type: ignore
 import pytorch_lightning as pl
 
 from bitorch.quantizations import ProgressiveSign
-from bitorch.quantizations.config import config as quantization_config
+from bitorch.quantizations.progressive_sign import config as progressive_sign_config
 
 
 class ProgressiveSignScalerCallback(pl.callbacks.Callback):
     """Callback that updates the scale of progressive sign functions based on current epoch."""
 
-    def on_epoch_start(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule") -> None:
+    def on_train_start(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule") -> None:
         scale = trainer.current_epoch / trainer.max_epochs
-        quantization_config.progressive_sign_scale = scale
+        progressive_sign_config.progressive_sign_scale = scale
         for logger in trainer.loggers:
             logger.log_metrics(
                 {
                     "_progressive_sign_scale": scale,
                     "_progressive_sign_temperature": ProgressiveSign.default_transform(scale),
                 },
                 step=trainer.fit_loop.epoch_loop._batches_that_stepped,
```

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/kd_loss.py` & `bitorch-0.4.0.dev0/examples/image_classification/utils/kd_loss.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/lightning_model.py` & `bitorch-0.4.0.dev0/examples/image_classification/utils/lightning_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 import logging
 from argparse import Namespace
 from typing import Union, Any
 
 import torch
 from pytorch_lightning import LightningModule
 from torch.nn import Module, CrossEntropyLoss
@@ -14,48 +15,68 @@
 
 
 class ModelWrapper(LightningModule):
     def __init__(
         self,
         model: Module,
         num_classes: int,
+        quantization_scheduler: Module,
         script_args: Namespace,
         add_f1_prec_recall: bool = False,
     ) -> None:
         super().__init__()
         self.save_hyperparameters(clean_hyperparameters(script_args))
         self.loss_function = CrossEntropyLoss()
         self.model = model
-        self.train_accuracy_top1 = Accuracy(num_classes=num_classes)
-        self.train_accuracy_top5 = Accuracy(top_k=5, num_classes=num_classes)
-        self.accuracy_top1 = Accuracy(num_classes=num_classes)
-        self.accuracy_top5 = Accuracy(top_k=5, num_classes=num_classes)
+        task = "binary" if num_classes == 2 else "multiclass"
+        self.batch_accuracy_top1 = Accuracy(task=task, num_classes=num_classes)
+        self.batch_accuracy_top5 = Accuracy(task=task, top_k=5, num_classes=num_classes)
+        self.train_accuracy_top1 = Accuracy(task=task, num_classes=num_classes)
+        self.train_accuracy_top5 = Accuracy(task=task, top_k=5, num_classes=num_classes)
+        self.accuracy_top1 = Accuracy(task=task, num_classes=num_classes)
+        self.accuracy_top5 = Accuracy(task=task, top_k=5, num_classes=num_classes)
         self.add_f1_prec_recall = add_f1_prec_recall
+        self.quantization_scheduler = quantization_scheduler
         if add_f1_prec_recall:
             self.f1 = F1Score(num_classes=num_classes)
             self.prec = Precision(num_classes=num_classes)
             self.recall = Recall(num_classes=num_classes)
 
-    def training_step(self, batch: torch.Tensor) -> torch.Tensor:  # type: ignore
+    def forward(self, *args: torch.Tensor, **kwargs: torch.Tensor) -> torch.Tensor:
+        return self.model(*args, **kwargs)
+
+    def training_step(self, batch: torch.Tensor, batch_idx: int) -> torch.Tensor:  # type: ignore
         x_train, y_train = batch
 
-        y_hat = self.model(x_train)
+        y_hat = self(x_train)
         loss = self.calculate_loss(x_train, y_train, y_hat)
+
+        self.batch_accuracy_top1(y_hat, y_train)
+        self.batch_accuracy_top5(y_hat, y_train)
         self.train_accuracy_top1(y_hat, y_train)
         self.train_accuracy_top5(y_hat, y_train)
+
         self.log_dict(
             {
-                "metrics/train-top1-accuracy": self.train_accuracy_top1,
-                "metrics/train-top5-accuracy": self.train_accuracy_top5,
+                "metrics/batch-top1-accuracy": self.batch_accuracy_top1,
+                "metrics/batch-top5-accuracy": self.batch_accuracy_top5,
+                "loss/train": loss,
             },
             prog_bar=True,
             on_step=True,
             on_epoch=False,
         )
-        self.log("loss/train", loss, on_step=True, on_epoch=False)
+        self.log_dict(
+            {
+                "metrics/train-top1-accuracy": self.train_accuracy_top1,
+                "metrics/train-top5-accuracy": self.train_accuracy_top5,
+            },
+            on_step=False,
+            on_epoch=True,
+        )
         return loss
 
     def calculate_loss(self, x_train: torch.Tensor, y_train: torch.Tensor, y_hat: torch.Tensor) -> torch.Tensor:
         return self.loss_function(y_hat, y_train)
 
     def validation_step(self, batch: torch.Tensor, batch_idx: int) -> None:  # type: ignore
         x_test, y_test = batch
@@ -83,14 +104,23 @@
                     "metrics/recall": self.recall,
                 }
             )
         self.log_dict(metrics_dict, prog_bar=True, on_step=False, on_epoch=True)
 
         return loss
 
+    def on_validation_epoch_end(self) -> None:
+        if self.quantization_scheduler is not None:
+            self.quantization_scheduler.step()
+            self.log(
+                "quantization_scheduler/factor",
+                self.quantization_scheduler.scheduled_quantizer_instances[0].factor,
+            )
+        return super().on_validation_epoch_end()
+
     def configure_optimizers(self) -> Union[dict, torch.optim.Optimizer]:  # type: ignore
         logging.info(f"Using {self.hparams.optimizer} optimizer and {self.hparams.lr_scheduler} lr scheduler...")
         optimizer = create_optimizer(self.hparams.optimizer, self.model, self.hparams.lr, self.hparams.momentum)
         if self.hparams.lr_scheduler is not None:
             scheduler = create_scheduler(
                 self.hparams.lr_scheduler,
                 optimizer,
```

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/log.py` & `bitorch-0.4.0.dev0/examples/dlrm/utils/log.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/teachers.py` & `bitorch-0.4.0.dev0/examples/image_classification/utils/teachers.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/unused_args.py` & `bitorch-0.4.0.dev0/examples/dlrm/utils/unused_args.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/examples/pytorch_lightning/utils/utils.py` & `bitorch-0.4.0.dev0/examples/dlrm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/mypy.ini` & `bitorch-0.4.0.dev0/mypy.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 show_error_codes = True
 follow_imports = silent
 pretty = True
 ignore_missing_imports = True
 disallow_untyped_defs = True
 disallow_any_explicit = False
 disable_error_code = attr-defined
-exclude = examples/mnist
+exclude = examples/(mnist|dlrm)
 
 [mypy-torchvision.io._video_opt.*]
 
 ignore_errors = True
 
 [mypy-torchvision.io.*]
```

### Comparing `bitorch-0.3.0.dev1/setup.cfg` & `bitorch-0.4.0.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/setup.py` & `bitorch-0.4.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
             version = version_content
 print("version:", version)
 
 
 def _get_requirements(*file_path: Union[Path, str]):
     requirements_list = []
     for fp in file_path:
-        requirements_list.extend(list(requirement.strip() for requirement in (root_path / fp).open().readlines()))
+        with (root_path / fp).open() as requirements_file:
+            requirements_list.extend(list(requirement.strip() for requirement in requirements_file.readlines()))
     # exclude bitorch from examples
     if "bitorch" in requirements_list:
         requirements_list.remove("bitorch")
     return requirements_list
 
 
 def _get_files_recursively(glob: str, root: str = ".") -> List[str]:
@@ -43,24 +44,26 @@
     long_description=readme_content,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=_get_requirements("requirements.txt"),
     extras_require={
         "dev": _get_requirements("requirements-dev.txt"),
         # "opt": _get_requirements(*_get_files_recursively("requirements*.txt", root="examples")),
-        "opt": _get_requirements("examples/pytorch_lightning/requirements.txt"),
+        "opt": _get_requirements("examples/image_classification/requirements.txt", "examples/mnist/requirements.txt"),
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.7",
     data_files=[
         (
             ".",
             [
                 "AUTHORS",
```

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_layer_arg_retrieval.py` & `bitorch-0.4.0.dev0/tests/layers/test_layer_arg_retrieval.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_layer_implementation.py` & `bitorch-0.4.0.dev0/tests/layers/test_layer_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,23 +81,24 @@
 
     s2_recipe = example_registry.get_recipe_for(s2)
     assert s2_recipe.args[0] == "Hello World"
     assert s2_recipe.args[1] == 21
 
 
 def test_default_impl():
+    print("bitorch test mode:", bitorch.mode)
     layer = Example("Hello World", val=21)
     assert layer.val == 21
     assert layer.class_name() == "BaseClass"
     assert isinstance(layer, Example.class_)
     assert isinstance(layer, LayerContainer)
-
+    print(layer)
     # TODO: pickling is currently only possible in RAW mode
     # content = pickle.dumps(layer)
-    #
+
     # layer_loaded = pickle.loads(content)
     # assert layer_loaded.val == 21
 
 
 def test_train_impl():
     bitorch.mode = TEST_MODE
     layer = Example("Hello World", val=21)
```

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_pact.py` & `bitorch-0.4.0.dev0/tests/layers/test_pact.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_qactivation.py` & `bitorch-0.4.0.dev0/tests/layers/test_qactivation.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_qconv.py` & `bitorch-0.4.0.dev0/tests/layers/test_qconv.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_qconv_noact.py` & `bitorch-0.4.0.dev0/tests/layers/test_qconv_noact.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_qembeddings.py` & `bitorch-0.4.0.dev0/tests/layers/test_qembeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     )
     assert torch.equal(output, quantization(raw_embeddings))
 
 
 @pytest.mark.parametrize("vocab_size, embedding_size", TEST_INPUT_DATA)
 @pytest.mark.parametrize("quantization_function", TEST_QUANTIZATION_FUNCTIONS)
 def test_qembeddingbag(vocab_size, embedding_size, quantization_function):
-
     qembeddingbag = QEmbeddingBag(
         num_embeddings=vocab_size,
         embedding_dim=embedding_size,
         weight_quantization=quantization_function(),
         output_quantization=quantization_function(),
         sparse=False,
         mode="mean",
```

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_qlinear.py` & `bitorch-0.4.0.dev0/tests/layers/test_qlinear.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/layers/test_switchable_layer.py` & `bitorch-0.4.0.dev0/tests/layers/test_switchable_layer.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/models/test_model_conversion.py` & `bitorch-0.4.0.dev0/tests/models/test_model_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,36 +4,34 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 import bitorch
 import bitorch.runtime_mode
 from bitorch import RuntimeMode
-from bitorch.datasets import MNIST
 from bitorch.layers import QConv2d, QLinear
 from bitorch.layers.extensions.layer_implementation import CustomImplementationMixin
 from bitorch.layers.extensions import LayerRecipe
 from bitorch.layers.qconv2d import QConv2dBase
 from bitorch.layers.qlinear import QLinearBase
 from bitorch.layers.register import (
     q_linear_registry,
     QLinearImplementation,
-    q_conv1d_registry,
     q_conv2d_registry,
     QConv2dImplementation,
-    q_conv3d_registry,
 )
 from bitorch.models import Model
 
 TEST_MODE = RuntimeMode.INFERENCE_AUTO
+MNIST = [(1, 1, 28, 28), 10, "MNIST"]
 
 
 class _TestModel(Model):
     def __init__(self):
-        super().__init__(dataset=MNIST)
+        super().__init__(input_shape=MNIST[0], num_classes=MNIST[1])
         self.q_conv2d = QConv2d(1, 32, 3, 1, 1)
         self.q_linear = QLinear(784, 64)
         self._model = nn.Sequential(
             self.q_conv2d,
             nn.Conv2d(32, 1, 3, 1, 1),
             nn.Flatten(),
             self.q_linear,
```

### Comparing `bitorch-0.3.0.dev1/tests/quantizations/test_quantizations.py` & `bitorch-0.4.0.dev0/tests/quantizations/test_quantizations.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,25 @@
         ProgressiveSign(),
         1,
         [-1.5, -1.0, -0.3, 0.0, 0.3, 1.0, 1.5],
         [-1.0, -1.0, -0.3, 0.0, 0.3, 1.0, 1.0],
         [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
     (
-        ProgressiveSign(use_global_scaling=False, initial_scale=0.2),
+        ProgressiveSign(use_global_scaling=False, initial_scale=0.05),
         1,
         [-1.5, -1.0, -0.3, -0.1, 0.0, 0.1, 0.3, 1.0, 1.5],
-        [-1.0, -1.0, -0.788, -0.2627, 0.0, 0.2627, 0.788, 1.0, 1.0],
+        [-1.0, -1.0, -0.6, -0.2, 0.0, 0.2, 0.6, 1.0, 1.0],
         [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
     (
         ProgressiveSign(use_global_scaling=False, initial_scale=0.5),
         1,
         [-1.5, -1.0, -0.3, -0.1, -0.05, 0.0, 0.05, 0.1, 0.3, 1.0, 1.5],
-        [-1.0, -1.0, -1.0, -1.0, -0.559, 0.0, 0.559, 1.0, 1.0, 1.0, 1.0],
+        [-1.0, -1.0, -1.0, -1.0, -1.0, 0.0, 1.0, 1.0, 1.0, 1.0, 1.0],
         [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
     (
         ProgressiveSign(use_global_scaling=False, initial_scale=0.2, custom_transform=lambda x: x),
         1,
         [-1.5, -1.0, -0.3, -0.1, 0.0, 0.1, 0.3, 1.0, 1.5],
         [-1.0, -1.0, -0.375, -0.125, 0.0, 0.125, 0.375, 1.0, 1.0],
@@ -55,16 +55,16 @@
         [-1.0, -1.0, -1.0, 1.0, 1.0, 1.0, 1.0],
         [0.0, 0.0, 1.4, 2.0, 1.4, 0.0, 0.0],
     ),
     (
         SteHeaviside(),
         1,
         [-1.5, -1.0, -0.3, 0.0, 0.3, 1.0, 1.5],
-        [0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0],
-        [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
+        [-1.0, -1.0, -1.0, -1.0, 1.0, 1.0, 1.0],
+        [0.0, 1.0, 1.0, 1.0, 1.0, 1.0, 0.0],
     ),
     (
         SwishSign(5.0),
         1,
         [-1.5, -1.0, -0.3, 0.0, 0.3, 1.0, 1.5],
         [-1.0, -1.0, -1.0, 1.0, 1.0, 1.0, 1.0],
         [-0.03, -0.195, 1.562, 5.0, 1.562, -0.195, -0.03],
@@ -77,29 +77,29 @@
         [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
     (
         WeightDoReFa(bits=2),
         2,
         [-1.5, -1.0, -0.3, 0.0, 0.3, 1.0, 1.5],
         [-1.0, -1.0, -1.0 / 3.0, 1.0 / 3.0, 1.0 / 3.0, 1.0, 1.0],
-        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
     (
         InputDoReFa(bits=1),
         1,
         [-1.5, -1.0, -0.3, 0.0, 0.3, 1.0, 1.5],
         [0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0],
         [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
     (
         WeightDoReFa(bits=1),
         1,
         [-1.5, -1.0, -0.3, 0.0, 0.3, 1.0, 1.5],
         [-1.0, -1.0, -1.0, -1.0, 1.0, 1.0, 1.0],
-        [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.0],
     ),
 ]
 
 
 @pytest.mark.parametrize(
     "quantization, bits, input_values, expected_output, expected_gradient_factors", TEST_INPUT_DATA
 )
@@ -113,14 +113,15 @@
     assert isinstance(quantization, quantization_from_name(quantization.name))
 
     y = quantization(x)
     assert len(y) == len(x_exp)
     assert torch.allclose(y, x_exp, atol=0.001)
     assert quantization.bit_width == bits
     with pytest.deprecated_call():
+        # noinspection PyDeprecation
         assert quantization.bitwidth == bits
 
     y.backward(x)
     computed_gradient = x.grad.clone()
     expected_gradient = x * exp_grad_factors
 
     assert torch.allclose(computed_gradient, expected_gradient, atol=0.001)
```

### Comparing `bitorch-0.3.0.dev1/tests/test_configs.py` & `bitorch-0.4.0.dev0/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `bitorch-0.3.0.dev1/tests/test_runtime_mode.py` & `bitorch-0.4.0.dev0/tests/test_runtime_mode.py`

 * *Files identical despite different names*

