# Comparing `tmp/irisml-tasks-training-0.0.8.tar.gz` & `tmp/irisml-tasks-training-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-training-0.0.8.tar", last modified: Tue Aug  9 23:56:30 2022, max compression
+gzip compressed data, was "irisml-tasks-training-0.0.9.tar", last modified: Wed Aug 10 05:23:37 2022, max compression
```

## Comparing `irisml-tasks-training-0.0.8.tar` & `irisml-tasks-training-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.441422 irisml-tasks-training-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-08-09 23:56:30.441422 irisml-tasks-training-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4612 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.433422 irisml-tasks-training-0.0.8/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.437422 irisml-tasks-training-0.0.8/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/append_classifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/build_classification_prompt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/build_zero_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/create_classification_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/evaluate_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/evaluate_detection_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/get_targets_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/make_feature_extractor_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/make_image_text_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/make_image_text_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/predict.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/split_image_text_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.437422 irisml-tasks-training-0.0.8/irisml/tasks/train/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/build_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/build_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/build_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/ddp_trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/ddp_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/plugin_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.437422 irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/ddp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/log_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/log_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/irisml/tasks/train/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.441422 irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-08-09 23:56:30.000000 irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-08-09 23:56:30.000000 irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 23:56:30.000000 irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-09 23:56:30.000000 irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-09 23:56:30.000000 irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-08-09 23:56:30.441422 irisml-tasks-training-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 23:56:30.441422 irisml-tasks-training-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_append_classifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_build_classification_prompt_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_build_zero_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_create_classification_prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_ddp_trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_evaluate_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_evaluate_detection_average_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_get_targets_from_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_make_feature_extractor_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_make_image_text_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_make_image_text_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-08-09 23:54:37.000000 irisml-tasks-training-0.0.8/test/test_split_image_text_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4612 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.804559 irisml-tasks-training-0.0.9/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.804559 irisml-tasks-training-0.0.9/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/append_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/build_classification_prompt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/build_zero_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/create_classification_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/evaluate_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/evaluate_detection_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/get_targets_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/make_feature_extractor_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/split_image_text_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.804559 irisml-tasks-training-0.0.9/irisml/tasks/train/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/build_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/build_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/build_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4622 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugin_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/irisml/tasks/train/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-10 05:23:37.000000 irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 05:23:37.808559 irisml-tasks-training-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_append_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_build_classification_prompt_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_build_zero_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_create_classification_prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_ddp_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_evaluate_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_evaluate_detection_average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_get_targets_from_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_make_feature_extractor_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_make_image_text_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_make_image_text_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-08-10 05:22:00.000000 irisml-tasks-training-0.0.9/test/test_split_image_text_model.py
```

### Comparing `irisml-tasks-training-0.0.8/LICENSE` & `irisml-tasks-training-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/PKG-INFO` & `irisml-tasks-training-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-training
-Version: 0.0.8
+Version: 0.0.9
 Summary: IrisML tasks for pytorch training
 Home-page: https://github.com/microsoft/irisml-tasks-training
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-training-0.0.8/README.md` & `irisml-tasks-training-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/append_classifier.py` & `irisml-tasks-training-0.0.9/irisml/tasks/append_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/build_classification_prompt_dataset.py` & `irisml-tasks-training-0.0.9/irisml/tasks/build_classification_prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/build_zero_shot_classifier.py` & `irisml-tasks-training-0.0.9/irisml/tasks/build_zero_shot_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import collections
 import dataclasses
 import logging
 import typing
 import torch
 import irisml.core
 
 logger = logging.getLogger(__name__)
@@ -11,45 +10,50 @@
 class Task(irisml.core.TaskBase):
     """Create a zero-shot classification layer."""
     VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Inputs:
         text_features: typing.List[torch.Tensor]
-        text_classes: typing.List[int]
+        text_classes: typing.Union[typing.List[int], torch.Tensor]
 
     @dataclasses.dataclass
     class Config:
         num_classes: int
 
     @dataclasses.dataclass
     class Outputs:
         classifier: torch.nn.Module = None
 
     def execute(self, inputs):
         num_examples = len(inputs.text_features)
         if len(inputs.text_classes) != num_examples:
             raise RuntimeError(f"The number of examples doesn't match. features={num_examples}, classes={len(inputs.text_classes)}")
 
-        if max(inputs.text_classes) >= self.config.num_classes:
-            raise RuntimeError(f"The max class index is higher than {self.config.num_classes}: {max(inputs.text_classes)}")
         feature_shape = inputs.text_features[0].shape
-        logger.debug(f"Feature shape is {feature_shape}")
+        logger.debug(f"Feature shape is {feature_shape}. Got {num_examples} samples.")
 
-        features_per_class = collections.defaultdict(list)
+        features_per_class = [[] for _ in range(self.config.num_classes)]
         for c, f in zip(inputs.text_classes, inputs.text_features):
-            features_per_class[c].append(f)
+            index = int(c)
+            if not 0 <= index < self.config.num_classes:
+                raise RuntimeError(f"Unexpected class index: {index}")
+            features_per_class[index].append(f)
+
+        embeddings_per_class = []
+        for c in range(self.config.num_classes):
+            if features_per_class[c]:
+                class_embeddings = torch.stack(features_per_class[c])
+                class_embeddings /= class_embeddings.norm(dim=-1, keepdim=True)
+                class_embedding = class_embeddings.mean(dim=0)
+                class_embedding /= class_embedding.norm()
+            else:
+                logger.warning(f"No features are provided for class {c}. Initializing with zeros.")
+                class_embedding = torch.zeros(*feature_shape)
 
-        embeddings_per_class = {}
-        for c in features_per_class:
-            class_embeddings = torch.stack(features_per_class[c])
-            class_embeddings /= class_embeddings.norm(dim=-1, keepdim=True)
-            class_embedding = class_embeddings.mean(dim=0)
-            class_embedding /= class_embedding.norm()
-            embeddings_per_class[c] = class_embedding
-        weights_list = [embeddings_per_class[i] if i in embeddings_per_class else torch.zeros(*feature_shape) for i in range(self.config.num_classes)]
-        weights = torch.stack(weights_list, dim=1).transpose(0, 1)  # TODO: Multiply with logit_scale?
+            embeddings_per_class.append(class_embedding)
 
+        weights = torch.stack(embeddings_per_class, dim=1).transpose(0, 1)  # TODO: Multiply with logit_scale?
         with torch.no_grad():
             classifier = torch.nn.Linear(weights.shape[1], weights.shape[0], bias=False)
             classifier.weight.copy_(weights)
         return self.Outputs(classifier)
```

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/create_classification_prompt_generator.py` & `irisml-tasks-training-0.0.9/irisml/tasks/create_classification_prompt_generator.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/evaluate_accuracy.py` & `irisml-tasks-training-0.0.9/irisml/tasks/evaluate_accuracy.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/evaluate_detection_average_precision.py` & `irisml-tasks-training-0.0.9/irisml/tasks/evaluate_detection_average_precision.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/export_onnx.py` & `irisml-tasks-training-0.0.9/irisml/tasks/export_onnx.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/get_targets_from_dataset.py` & `irisml-tasks-training-0.0.9/irisml/tasks/get_targets_from_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/make_feature_extractor_model.py` & `irisml-tasks-training-0.0.9/irisml/tasks/make_feature_extractor_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/make_image_text_contrastive_model.py` & `irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/make_image_text_transform.py` & `irisml-tasks-training-0.0.9/irisml/tasks/make_image_text_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/predict.py` & `irisml-tasks-training-0.0.9/irisml/tasks/predict.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/split_image_text_model.py` & `irisml-tasks-training-0.0.9/irisml/tasks/split_image_text_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/build_dataloader.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/build_lr_scheduler.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/build_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/build_optimizer.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/ddp_trainer.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/ddp_utils.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/ddp_utils.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/plugin_list.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugin_list.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/log_summary.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_summary.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/log_tensorboard.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/log_tensorboard.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/plugin_base.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/plugins/progressbar.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/plugins/progressbar.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/task.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/task.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml/tasks/train/trainer.py` & `irisml-tasks-training-0.0.9/irisml/tasks/train/trainer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/PKG-INFO` & `irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-training
-Version: 0.0.8
+Version: 0.0.9
 Summary: IrisML tasks for pytorch training
 Home-page: https://github.com/microsoft/irisml-tasks-training
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-training-0.0.8/irisml_tasks_training.egg-info/SOURCES.txt` & `irisml-tasks-training-0.0.9/irisml_tasks_training.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/setup.cfg` & `irisml-tasks-training-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-training
-version = 0.0.8
+version = 0.0.9
 url = https://github.com/microsoft/irisml-tasks-training
 description = IrisML tasks for pytorch training
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-training-0.0.8/test/test_append_classifier.py` & `irisml-tasks-training-0.0.9/test/test_append_classifier.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_build_classification_prompt_dataset.py` & `irisml-tasks-training-0.0.9/test/test_build_classification_prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_build_zero_shot_classifier.py` & `irisml-tasks-training-0.0.9/test/test_build_zero_shot_classifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,7 +13,21 @@
         text_features = [one_feature, zero_feature, one_feature, zero_feature]
         text_classes = [1, 0, 1, 0]
         inputs = Task.Inputs(text_features, text_classes)
         outputs = Task(Task.Config(num_classes=2)).execute(inputs)
 
         self.assertEqual(torch.argmax(outputs.classifier(one_feature)), 1)
         self.assertEqual(torch.argmax(outputs.classifier(zero_feature)), 0)
+
+    def test_tensor_classes(self):
+        zero_feature = torch.ones(32)
+        zero_feature[0] = 10
+        one_feature = torch.ones(32)
+        one_feature[1] = 10
+
+        text_features = [one_feature, zero_feature, one_feature, zero_feature]
+        text_classes = torch.Tensor([1, 0, 1, 0])
+        inputs = Task.Inputs(text_features, text_classes)
+        outputs = Task(Task.Config(num_classes=2)).execute(inputs)
+
+        self.assertEqual(torch.argmax(outputs.classifier(one_feature)), 1)
+        self.assertEqual(torch.argmax(outputs.classifier(zero_feature)), 0)
```

### Comparing `irisml-tasks-training-0.0.8/test/test_dataloader.py` & `irisml-tasks-training-0.0.9/test/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_ddp_trainer.py` & `irisml-tasks-training-0.0.9/test/test_ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_evaluate_accuracy.py` & `irisml-tasks-training-0.0.9/test/test_evaluate_accuracy.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_evaluate_detection_average_precision.py` & `irisml-tasks-training-0.0.9/test/test_evaluate_detection_average_precision.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_export_onnx.py` & `irisml-tasks-training-0.0.9/test/test_export_onnx.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_get_targets_from_dataset.py` & `irisml-tasks-training-0.0.9/test/test_get_targets_from_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_make_feature_extractor_model.py` & `irisml-tasks-training-0.0.9/test/test_make_feature_extractor_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_make_image_text_contrastive_model.py` & `irisml-tasks-training-0.0.9/test/test_make_image_text_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_make_image_text_transform.py` & `irisml-tasks-training-0.0.9/test/test_make_image_text_transform.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_predict.py` & `irisml-tasks-training-0.0.9/test/test_predict.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-training-0.0.8/test/test_split_image_text_model.py` & `irisml-tasks-training-0.0.9/test/test_split_image_text_model.py`

 * *Files identical despite different names*

