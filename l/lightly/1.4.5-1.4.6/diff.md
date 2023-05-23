# Comparing `tmp/lightly-1.4.5.tar.gz` & `tmp/lightly-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.4.5.tar", last modified: Thu May 11 16:27:59 2023, max compression
+gzip compressed data, was "lightly-1.4.6.tar", last modified: Tue May 23 16:32:10 2023, max compression
```

## Comparing `lightly-1.4.5.tar` & `lightly-1.4.6.tar`

### file list

```diff
@@ -1,410 +1,410 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 16:27:51.000000 lightly-1.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 16:27:51.000000 lightly-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 16:27:59.601920 lightly-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-05-11 16:27:51.000000 lightly-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/agents/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/config/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/config/selection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/scorers/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/active_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/keypoint_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/active_learning/utils/object_detection_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.569920 lightly-1.4.5/lightly/api/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_compute_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    29042 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_datasources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_upload_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/api_workflow_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/bitmask.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/swagger_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/swagger_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/api/version_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.569920 lightly-1.4.5/lightly/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/_cli_simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.569920 lightly-1.4.5/lightly/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/config/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/crop_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/embed_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/lightly_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/train_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/upload_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/cli/version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/data/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_image_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/_video.py
--rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/lightly_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/data/multi_view_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/embedding/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/dcl_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/dino_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/hypersphere_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/msn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/negative_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/ntx_ent_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/pmsn_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/loss/regularizer/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/regularizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/regularizer/co2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/sym_neg_cos_sim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/tico_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/loss/vicregl_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/byol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/moco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/models/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/heads.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/masked_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/modules/nn_memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/nnclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)    18480 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly/openapi_generated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.573920 lightly-1.4.5/lightly/openapi_generated/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    25152 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.577920 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    78621 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasources_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/docker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/predictions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52413 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samples_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samplings_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/scores_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api/versioning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.597920 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    23521 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/access_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/async_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_license_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_name_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/general_job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/jobs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/path_safe_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/probabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/version_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/video_frame_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/openapi_generated/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/lightly/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/dino_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/fast_siam_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/image_grid_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/mae_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/moco_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/msn_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/multi_crop_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/multi_view_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/pirl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/random_crop_and_flip_with_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/simclr_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/simsiam_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/smog_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/swav_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/vicreg_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/transforms/vicregl_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/lightly/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.601920 lightly-1.4.5/lightly/utils/cropping/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/cropping/crop_image_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/cropping/read_yolo_label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/embeddings_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/hipify.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/reordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-11 16:27:51.000000 lightly-1.4.5/lightly/utils/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:27:59.565920 lightly-1.4.5/lightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 16:27:59.000000 lightly-1.4.5/lightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 16:27:51.000000 lightly-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 16:27:59.601920 lightly-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-11 16:27:51.000000 lightly-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.647479 lightly-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-23 16:31:57.000000 lightly-1.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 16:31:57.000000 lightly-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-23 16:32:10.647479 lightly-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-05-23 16:31:57.000000 lightly-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.611479 lightly-1.4.6/lightly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/agents/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/config/selection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/scorers/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/active_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/keypoint_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/active_learning/utils/object_detection_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.615479 lightly-1.4.6/lightly/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_compute_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29042 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_upload_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/api_workflow_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/swagger_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/swagger_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/api/version_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/_cli_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/config/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/crop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/embed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/lightly_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/train_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/upload_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/cli/version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_image_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49756 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/lightly_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/data/multi_view_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/embedding/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/dcl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/dino_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/hypersphere_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/msn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/negative_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/ntx_ent_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/pmsn_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/loss/regularizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/regularizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/regularizer/co2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/sym_neg_cos_sim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/tico_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/loss/vicregl_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.619479 lightly-1.4.6/lightly/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/byol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/moco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.623479 lightly-1.4.6/lightly/models/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23563 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/masked_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/modules/nn_memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/nnclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18480 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.611479 lightly-1.4.6/lightly/openapi_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.623479 lightly-1.4.6/lightly/openapi_generated/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    25152 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.623479 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48008 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78621 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasources_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160419 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/docker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20444 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38782 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/predictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52413 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samples_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samplings_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/scores_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97324 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api/versioning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    23521 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/access_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/async_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16339 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_license_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_name_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/general_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/jobs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/mongo_object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/path_safe_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/redirected_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/version_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/video_frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/openapi_generated/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/dino_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/fast_siam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/image_grid_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/mae_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/moco_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/msn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/multi_crop_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/multi_view_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/pirl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/random_crop_and_flip_with_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/simclr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/simsiam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/smog_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/swav_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/vicreg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/transforms/vicregl_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.643479 lightly-1.4.6/lightly/utils/cropping/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/cropping/crop_image_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/cropping/read_yolo_label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/embeddings_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/hipify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/reordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 16:31:57.000000 lightly-1.4.6/lightly/utils/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:32:10.611479 lightly-1.4.6/lightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 16:32:10.000000 lightly-1.4.6/lightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 16:31:57.000000 lightly-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 16:32:10.647479 lightly-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-23 16:31:57.000000 lightly-1.4.6/setup.py
```

### Comparing `lightly-1.4.5/LICENSE.txt` & `lightly-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/PKG-INFO` & `lightly-1.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.5
+Version: 1.4.6
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.5/README.md` & `lightly-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/__init__.py` & `lightly-1.4.6/lightly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 __name__ = "lightly"
-__version__ = "1.4.5"
+__version__ = "1.4.6"
 
 import os
 
 try:
     # See (https://github.com/PyTorchLightning/pytorch-lightning)
     # This variable is injected in the __builtins__ by the build
     # process. It used to enable importing subpackages of skimage when
```

### Comparing `lightly-1.4.5/lightly/active_learning/agents/agent.py` & `lightly-1.4.6/lightly/active_learning/agents/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,22 +59,20 @@
         >>> added_set = agent.added_set # access only the samples added by this query
 
     """
 
     def __init__(
         self,
         api_workflow_client: ApiWorkflowClient,
-        query_tag_name: str = "initial-tag",
+        query_tag_name: str,
         preselected_tag_name: str = None,
     ):
         raise_active_learning_deprecation_warning()
         self.api_workflow_client = api_workflow_client
 
-        # set the query_tag_id and preselected_tag_id
-        self._query_tag_id = None
         self._preselected_tag_id = None
 
         # build lookup table for tag_name to tag_id
         tag_name_id_dict = {}
         for tag in self.api_workflow_client.get_all_tags():
             tag_name_id_dict[tag.name] = tag.id
         # use lookup table to set ids
```

### Comparing `lightly-1.4.5/lightly/active_learning/config/selection_config.py` & `lightly-1.4.6/lightly/active_learning/config/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/scorers/classification.py` & `lightly-1.4.6/lightly/active_learning/scorers/classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/scorers/detection.py` & `lightly-1.4.6/lightly/active_learning/scorers/detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/scorers/keypoint_detection.py` & `lightly-1.4.6/lightly/active_learning/scorers/keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/scorers/semantic_segmentation.py` & `lightly-1.4.6/lightly/active_learning/scorers/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/utils/bounding_box.py` & `lightly-1.4.6/lightly/active_learning/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/utils/keypoint_predictions.py` & `lightly-1.4.6/lightly/active_learning/utils/keypoint_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/active_learning/utils/object_detection_output.py` & `lightly-1.4.6/lightly/active_learning/utils/object_detection_output.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/__init__.py` & `lightly-1.4.6/lightly/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" The lightly.api module provides access to the Lightly web-app. """
+""" The lightly.api module provides access to the Lightly API."""
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 from lightly.api import patch as _patch
 from lightly.api.api_workflow_artifacts import ArtifactNotExist
 from lightly.api.api_workflow_client import ApiWorkflowClient
 from lightly.openapi_generated.swagger_client import Configuration as _Configuration
```

### Comparing `lightly-1.4.5/lightly/api/api_workflow_artifacts.py` & `lightly-1.4.6/lightly/api/api_workflow_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_client.py` & `lightly-1.4.6/lightly/api/api_workflow_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_collaboration.py` & `lightly-1.4.6/lightly/api/api_workflow_collaboration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_compute_worker.py` & `lightly-1.4.6/lightly/api/api_workflow_compute_worker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_datasets.py` & `lightly-1.4.6/lightly/api/api_workflow_datasets.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_datasources.py` & `lightly-1.4.6/lightly/api/api_workflow_datasources.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_download_dataset.py` & `lightly-1.4.6/lightly/api/api_workflow_download_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_export.py` & `lightly-1.4.6/lightly/api/api_workflow_export.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_predictions.py` & `lightly-1.4.6/lightly/api/api_workflow_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_selection.py` & `lightly-1.4.6/lightly/api/api_workflow_selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,25 +29,15 @@
         scores = scores.astype(np.float64)
 
     # convert to list and return
     return list(scores)
 
 
 class _SelectionMixin:
-    def upload_scores(self, al_scores: Dict[str, np.ndarray], query_tag_id: str = None):
-        tags = self.get_all_tags()
-
-        # upload the active learning scores to the api
-        # change @20210422: we store the active learning scores with the query
-        # tag. policy is that if there's no explicit query tag, the whole dataset
-        # will be the query tag (i.e. query_tag = initial-tag)
-        # set the query tag to the initial-tag if necessary
-        if query_tag_id is None:
-            query_tag = next(t for t in tags if t.name == "initial-tag")
-            query_tag_id = query_tag.id
+    def upload_scores(self, al_scores: Dict[str, np.ndarray], query_tag_id: str):
         # iterate over all available score types and upload them
         for score_type, score_values in al_scores.items():
             body = ActiveLearningScoreCreateRequest(
                 score_type=score_type,
                 scores=_parse_active_learning_scores(score_values),
             )
             self._scores_api.create_or_update_active_learning_score_by_tag_id(
```

### Comparing `lightly-1.4.5/lightly/api/api_workflow_tags.py` & `lightly-1.4.6/lightly/api/api_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_upload_dataset.py` & `lightly-1.4.6/lightly/api/api_workflow_upload_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_upload_embeddings.py` & `lightly-1.4.6/lightly/api/api_workflow_upload_embeddings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/api_workflow_upload_metadata.py` & `lightly-1.4.6/lightly/api/api_workflow_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/bitmask.py` & `lightly-1.4.6/lightly/api/bitmask.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/download.py` & `lightly-1.4.6/lightly/api/download.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/patch.py` & `lightly-1.4.6/lightly/api/patch.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/prediction_singletons.py` & `lightly-1.4.6/lightly/api/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/swagger_api_client.py` & `lightly-1.4.6/lightly/api/swagger_api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/swagger_rest_client.py` & `lightly-1.4.6/lightly/api/swagger_rest_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/utils.py` & `lightly-1.4.6/lightly/api/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/api/version_checking.py` & `lightly-1.4.6/lightly/api/version_checking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/_cli_simclr.py` & `lightly-1.4.6/lightly/cli/_cli_simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/_helpers.py` & `lightly-1.4.6/lightly/cli/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/config/config.yaml` & `lightly-1.4.6/lightly/cli/config/config.yaml`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/crop_cli.py` & `lightly-1.4.6/lightly/cli/crop_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/download_cli.py` & `lightly-1.4.6/lightly/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/embed_cli.py` & `lightly-1.4.6/lightly/cli/embed_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/lightly_cli.py` & `lightly-1.4.6/lightly/cli/lightly_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/train_cli.py` & `lightly-1.4.6/lightly/cli/train_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/upload_cli.py` & `lightly-1.4.6/lightly/cli/upload_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/cli/version_cli.py` & `lightly-1.4.6/lightly/cli/version_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/core.py` & `lightly-1.4.6/lightly/core.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/__init__.py` & `lightly-1.4.6/lightly/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/_helpers.py` & `lightly-1.4.6/lightly/data/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/_image.py` & `lightly-1.4.6/lightly/data/_image.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/_image_loaders.py` & `lightly-1.4.6/lightly/data/_image_loaders.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/_utils.py` & `lightly-1.4.6/lightly/data/_utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/_video.py` & `lightly-1.4.6/lightly/data/_video.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/collate.py` & `lightly-1.4.6/lightly/data/collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/data/dataset.py` & `lightly-1.4.6/lightly/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Lightly Dataset """
-
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 import bisect
 import os
 import shutil
 import tempfile
```

### Comparing `lightly-1.4.5/lightly/data/lightly_subset.py` & `lightly-1.4.6/lightly/data/lightly_subset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/embedding/_base.py` & `lightly-1.4.6/lightly/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/embedding/callbacks.py` & `lightly-1.4.6/lightly/embedding/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/embedding/embedding.py` & `lightly-1.4.6/lightly/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/__init__.py` & `lightly-1.4.6/lightly/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/barlow_twins_loss.py` & `lightly-1.4.6/lightly/loss/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/dcl_loss.py` & `lightly-1.4.6/lightly/loss/dcl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/dino_loss.py` & `lightly-1.4.6/lightly/loss/dino_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/hypersphere_loss.py` & `lightly-1.4.6/lightly/loss/hypersphere_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/memory_bank.py` & `lightly-1.4.6/lightly/loss/memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/msn_loss.py` & `lightly-1.4.6/lightly/loss/msn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/negative_cosine_similarity.py` & `lightly-1.4.6/lightly/loss/negative_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/ntx_ent_loss.py` & `lightly-1.4.6/lightly/loss/ntx_ent_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/pmsn_loss.py` & `lightly-1.4.6/lightly/loss/pmsn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/regularizer/co2.py` & `lightly-1.4.6/lightly/loss/regularizer/co2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/swav_loss.py` & `lightly-1.4.6/lightly/loss/swav_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/sym_neg_cos_sim_loss.py` & `lightly-1.4.6/lightly/loss/sym_neg_cos_sim_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/tico_loss.py` & `lightly-1.4.6/lightly/loss/tico_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/vicreg_loss.py` & `lightly-1.4.6/lightly/loss/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/loss/vicregl_loss.py` & `lightly-1.4.6/lightly/loss/vicregl_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Sequence, Tuple
 
 import torch
-from torch import Tensor, dist
+import torch.distributed as dist
+from torch import Tensor
 
 from lightly.loss.vicreg_loss import (
     VICRegLoss,
     covariance_loss,
     invariance_loss,
     variance_loss,
 )
```

### Comparing `lightly-1.4.5/lightly/models/__init__.py` & `lightly-1.4.6/lightly/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/_momentum.py` & `lightly-1.4.6/lightly/models/_momentum.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/barlowtwins.py` & `lightly-1.4.6/lightly/models/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/batchnorm.py` & `lightly-1.4.6/lightly/models/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/byol.py` & `lightly-1.4.6/lightly/models/byol.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/moco.py` & `lightly-1.4.6/lightly/models/moco.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/modules/__init__.py` & `lightly-1.4.6/lightly/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/modules/heads.py` & `lightly-1.4.6/lightly/models/modules/heads.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/modules/masked_autoencoder.py` & `lightly-1.4.6/lightly/models/modules/masked_autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/modules/nn_memory_bank.py` & `lightly-1.4.6/lightly/models/modules/nn_memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/nnclr.py` & `lightly-1.4.6/lightly/models/nnclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/resnet.py` & `lightly-1.4.6/lightly/models/resnet.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/simclr.py` & `lightly-1.4.6/lightly/models/simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/simsiam.py` & `lightly-1.4.6/lightly/models/simsiam.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/utils.py` & `lightly-1.4.6/lightly/models/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/models/zoo.py` & `lightly-1.4.6/lightly/models/zoo.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/__init__.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/__init__.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/collaboration_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/collaboration_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasets_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/datasources_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/datasources_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/docker_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/embeddings_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/jobs_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/mappings_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/mappings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/predictions_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/predictions_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/quota_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samples_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samples_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/samplings_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/samplings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/scores_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/scores_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/tags_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/teams_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api/versioning_api.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api/versioning_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/api_client.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/configuration.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/__init__.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/access_role.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/access_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_score_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/active_learning_scores.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/active_learning_scores.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_code.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_code.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/api_error_response.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/async_task_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/async_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/bounding_box.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_id.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/category_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/category_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_entry.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_set_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_set_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_entity_response.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/creator.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/crop_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/crop_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/custom_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_creator.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_name_query.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_name_query.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dataset_update_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dataset_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_base.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_local.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_local.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_purpose.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_purpose.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_license_information.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_license_information.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_state.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_task_description.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_task_description.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_user_stats.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_user_stats.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_labels.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_state.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/docker_worker_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/docker_worker_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_coordinates.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding2d_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding2d_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/embedding_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_name_format.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_name_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/file_output_format.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/file_output_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/filename_and_read_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/general_job_result.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/general_job_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/image_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/image_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_result_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_result_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_state.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_data_result.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_data_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_meta.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_meta.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/jobs_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/jobs_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_row.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_box_v4_data_rows.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/label_studio_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/mongo_object_id.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/mongo_object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/object_id.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/object_id.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/path_safe_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/path_safe_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_singletons.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_singletons.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/probabilities.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/probabilities.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/questionnaire_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/questionnaire_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/read_url.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/redirected_read_url.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/redirected_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_region.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_region.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/s3_server_side_encryption_kms_key.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_task_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sama_tasks.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sama_tasks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_data_modes.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_data_modes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_meta_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_sort_by.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_sort_by.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_update_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sample_write_urls.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sample_write_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sampling_method.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sampling_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/score.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/score.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/sector.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_input_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_input_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/shared_access_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/shared_access_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_change_entry.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_change_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_create_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_creator.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_filenames_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_update_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_name.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/task_type.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_basic_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/team_role.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/timestamp_seconds.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/version_number.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/version_number.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/video_frame_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/video_frame_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/openapi_generated/swagger_client/rest.py` & `lightly-1.4.6/lightly/openapi_generated/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/__init__.py` & `lightly-1.4.6/lightly/transforms/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""The lightly.transforms package provides additional augmentations.
-
-    Contains implementations of Gaussian blur and random rotations which are
-    not part of torchvisions transforms.
+"""The lightly.transforms package transforms for various self-supervised learning
+methods.
 
+It also contains some additional transforms that are not part of torchvisions
+transforms.
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 from lightly.transforms.dino_transform import DINOTransform, DINOViewTransform
 from lightly.transforms.fast_siam_transform import FastSiamTransform
```

### Comparing `lightly-1.4.5/lightly/transforms/dino_transform.py` & `lightly-1.4.6/lightly/transforms/dino_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/fast_siam_transform.py` & `lightly-1.4.6/lightly/transforms/fast_siam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/gaussian_blur.py` & `lightly-1.4.6/lightly/transforms/gaussian_blur.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Gaussian Blur """
-
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 from typing import Tuple, Union
 from warnings import warn
 
 import numpy as np
```

### Comparing `lightly-1.4.5/lightly/transforms/image_grid_transform.py` & `lightly-1.4.6/lightly/transforms/image_grid_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/jigsaw.py` & `lightly-1.4.6/lightly/transforms/jigsaw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Jigsaw Crop """
-
 # Copyright (c) 2021. Lightly AG and its affiliates.
 # All Rights Reserved
 
 import numpy as np
 import torch
 from PIL import Image
 from torchvision import transforms
```

### Comparing `lightly-1.4.5/lightly/transforms/mae_transform.py` & `lightly-1.4.6/lightly/transforms/mae_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/moco_transform.py` & `lightly-1.4.6/lightly/transforms/moco_transform.py`

 * *Files 21% similar despite different names*

```diff
@@ -89,8 +89,59 @@
             hf_prob=hf_prob,
             rr_prob=rr_prob,
             rr_degrees=rr_degrees,
             normalize=normalize,
         )
 
 
-MoCoV2Transform = SimCLRTransform  # MoCo v2 uses the same transform as SimCLR
+class MoCoV2Transform(SimCLRTransform):
+    """Implements the transformations for MoCo v2 [0].
+
+    Identical to SimCLRTransform.
+
+    - [0]: MoCo v2, 2020, https://arxiv.org/abs/2003.04297
+
+    Attributes:
+        input_size:
+            Size of the input image in pixels.
+        cj_prob:
+            Probability that color jitter is applied.
+        cj_strength:
+            Strength of the color jitter. `cj_bright`, `cj_contrast`, `cj_sat`, and
+            `cj_hue` are multiplied by this value. For datasets with small images,
+            such as CIFAR, it is recommended to set `cj_strenght` to 0.5.
+        cj_bright:
+            How much to jitter brightness.
+        cj_contrast:
+            How much to jitter constrast.
+        cj_sat:
+            How much to jitter saturation.
+        cj_hue:
+            How much to jitter hue.
+        min_scale:
+            Minimum size of the randomized crop relative to the input_size.
+        random_gray_scale:
+            Probability of conversion to grayscale.
+        gaussian_blur:
+            Probability of Gaussian blur.
+        kernel_size:
+            Will be deprecated in favor of `sigmas` argument. If set, the old behavior applies and `sigmas` is ignored.
+            Used to calculate sigma of gaussian blur with kernel_size * input_size.
+        sigmas:
+            Tuple of min and max value from which the std of the gaussian kernel is sampled.
+            Is ignored if `kernel_size` is set.
+        vf_prob:
+            Probability that vertical flip is applied.
+        hf_prob:
+            Probability that horizontal flip is applied.
+        rr_prob:
+            Probability that random rotation is applied.
+        rr_degrees:
+            Range of degrees to select from for random rotation. If rr_degrees is None,
+            images are rotated by 90 degrees. If rr_degrees is a (min, max) tuple,
+            images are rotated by a random angle in [min, max]. If rr_degrees is a
+            single number, images are rotated by a random angle in
+            [-rr_degrees, +rr_degrees]. All rotations are counter-clockwise.
+        normalize:
+            Dictionary with 'mean' and 'std' for torchvision.transforms.Normalize.
+
+    """
```

### Comparing `lightly-1.4.5/lightly/transforms/msn_transform.py` & `lightly-1.4.6/lightly/transforms/msn_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/multi_crop_transform.py` & `lightly-1.4.6/lightly/transforms/multi_crop_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/multi_view_transform.py` & `lightly-1.4.6/lightly/transforms/multi_view_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/pirl_transform.py` & `lightly-1.4.6/lightly/transforms/pirl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/random_crop_and_flip_with_grid.py` & `lightly-1.4.6/lightly/transforms/random_crop_and_flip_with_grid.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/rotation.py` & `lightly-1.4.6/lightly/transforms/rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Random Rotation """
-
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 from typing import Tuple, Union
 
 import numpy as np
 import torchvision.transforms as T
```

### Comparing `lightly-1.4.5/lightly/transforms/simclr_transform.py` & `lightly-1.4.6/lightly/transforms/simsiam_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 from lightly.transforms.gaussian_blur import GaussianBlur
 from lightly.transforms.multi_view_transform import MultiViewTransform
 from lightly.transforms.rotation import random_rotation_transform
 from lightly.transforms.utils import IMAGENET_NORMALIZE
 
 
-class SimCLRTransform(MultiViewTransform):
-    """Implements the transformations for SimCLR.
+class SimSiamTransform(MultiViewTransform):
+    """Implements the transformations for SimSiam.
 
     Attributes:
         input_size:
             Size of the input image in pixels.
         cj_prob:
             Probability that color jitter is applied.
         cj_strength:
             Strength of the color jitter. `cj_bright`, `cj_contrast`, `cj_sat`, and
             `cj_hue` are multiplied by this value. For datasets with small images,
-            such as CIFAR, it is recommended to set `cj_strenght` to 0.5.
+            such as CIFAR, it is recommended to set `cj_strength` to 0.5.
         cj_bright:
             How much to jitter brightness.
         cj_contrast:
             How much to jitter constrast.
         cj_sat:
             How much to jitter saturation.
         cj_hue:
@@ -60,30 +60,30 @@
     """
 
     def __init__(
         self,
         input_size: int = 224,
         cj_prob: float = 0.8,
         cj_strength: float = 1.0,
-        cj_bright: float = 0.8,
-        cj_contrast: float = 0.8,
-        cj_sat: float = 0.8,
-        cj_hue: float = 0.2,
-        min_scale: float = 0.08,
+        cj_bright: float = 0.4,
+        cj_contrast: float = 0.4,
+        cj_sat: float = 0.4,
+        cj_hue: float = 0.1,
+        min_scale: float = 0.2,
         random_gray_scale: float = 0.2,
         gaussian_blur: float = 0.5,
         kernel_size: Optional[float] = None,
         sigmas: Tuple[float, float] = (0.1, 2),
         vf_prob: float = 0.0,
         hf_prob: float = 0.5,
         rr_prob: float = 0.0,
         rr_degrees: Union[None, float, Tuple[float, float]] = None,
         normalize: Union[None, dict] = IMAGENET_NORMALIZE,
     ):
-        view_transform = SimCLRViewTransform(
+        view_transform = SimSiamViewTransform(
             input_size=input_size,
             cj_prob=cj_prob,
             cj_strength=cj_strength,
             cj_bright=cj_bright,
             cj_contrast=cj_contrast,
             cj_sat=cj_sat,
             cj_hue=cj_hue,
@@ -97,25 +97,25 @@
             rr_prob=rr_prob,
             rr_degrees=rr_degrees,
             normalize=normalize,
         )
         super().__init__(transforms=[view_transform, view_transform])
 
 
-class SimCLRViewTransform:
+class SimSiamViewTransform:
     def __init__(
         self,
         input_size: int = 224,
         cj_prob: float = 0.8,
         cj_strength: float = 1.0,
-        cj_bright: float = 0.8,
-        cj_contrast: float = 0.8,
-        cj_sat: float = 0.8,
-        cj_hue: float = 0.2,
-        min_scale: float = 0.08,
+        cj_bright: float = 0.4,
+        cj_contrast: float = 0.4,
+        cj_sat: float = 0.4,
+        cj_hue: float = 0.1,
+        min_scale: float = 0.2,
         random_gray_scale: float = 0.2,
         gaussian_blur: float = 0.5,
         kernel_size: Optional[float] = None,
         sigmas: Tuple[float, float] = (0.1, 2),
         vf_prob: float = 0.0,
         hf_prob: float = 0.5,
         rr_prob: float = 0.0,
```

### Comparing `lightly-1.4.5/lightly/transforms/simsiam_transform.py` & `lightly-1.4.6/lightly/transforms/vicreg_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,45 @@
 import torchvision.transforms as T
 from PIL.Image import Image
 from torch import Tensor
 
 from lightly.transforms.gaussian_blur import GaussianBlur
 from lightly.transforms.multi_view_transform import MultiViewTransform
 from lightly.transforms.rotation import random_rotation_transform
+from lightly.transforms.solarize import RandomSolarization
 from lightly.transforms.utils import IMAGENET_NORMALIZE
 
 
-class SimSiamTransform(MultiViewTransform):
-    """Implements the transformations for SimSiam.
+class VICRegTransform(MultiViewTransform):
+    """Implements the transformations for VICReg.
+
+    Similar to SimCLR transform but with extra solarization.
 
     Attributes:
         input_size:
             Size of the input image in pixels.
         cj_prob:
             Probability that color jitter is applied.
         cj_strength:
             Strength of the color jitter. `cj_bright`, `cj_contrast`, `cj_sat`, and
-            `cj_hue` are multiplied by this value. For datasets with small images,
-            such as CIFAR, it is recommended to set `cj_strength` to 0.5.
+            `cj_hue` are multiplied by this value.
         cj_bright:
             How much to jitter brightness.
         cj_contrast:
             How much to jitter constrast.
         cj_sat:
             How much to jitter saturation.
         cj_hue:
             How much to jitter hue.
         min_scale:
             Minimum size of the randomized crop relative to the input_size.
         random_gray_scale:
             Probability of conversion to grayscale.
+        solarize_prob:
+            Probability of solarization.
         gaussian_blur:
             Probability of Gaussian blur.
         kernel_size:
             Will be deprecated in favor of `sigmas` argument. If set, the old behavior applies and `sigmas` is ignored.
             Used to calculate sigma of gaussian blur with kernel_size * input_size.
         sigmas:
             Tuple of min and max value from which the std of the gaussian kernel is sampled.
@@ -59,67 +63,70 @@
 
     """
 
     def __init__(
         self,
         input_size: int = 224,
         cj_prob: float = 0.8,
-        cj_strength: float = 1.0,
-        cj_bright: float = 0.4,
-        cj_contrast: float = 0.4,
+        cj_strength: float = 0.5,
+        cj_bright: float = 0.8,
+        cj_contrast: float = 0.8,
         cj_sat: float = 0.4,
-        cj_hue: float = 0.1,
-        min_scale: float = 0.2,
+        cj_hue: float = 0.2,
+        min_scale: float = 0.08,
         random_gray_scale: float = 0.2,
+        solarize_prob: float = 0.1,
         gaussian_blur: float = 0.5,
         kernel_size: Optional[float] = None,
         sigmas: Tuple[float, float] = (0.1, 2),
         vf_prob: float = 0.0,
         hf_prob: float = 0.5,
         rr_prob: float = 0.0,
         rr_degrees: Union[None, float, Tuple[float, float]] = None,
         normalize: Union[None, dict] = IMAGENET_NORMALIZE,
     ):
-        view_transform = SimSiamViewTransform(
+        view_transform = VICRegViewTransform(
             input_size=input_size,
             cj_prob=cj_prob,
             cj_strength=cj_strength,
             cj_bright=cj_bright,
             cj_contrast=cj_contrast,
             cj_sat=cj_sat,
             cj_hue=cj_hue,
             min_scale=min_scale,
             random_gray_scale=random_gray_scale,
+            solarize_prob=solarize_prob,
             gaussian_blur=gaussian_blur,
             kernel_size=kernel_size,
             sigmas=sigmas,
             vf_prob=vf_prob,
             hf_prob=hf_prob,
             rr_prob=rr_prob,
             rr_degrees=rr_degrees,
             normalize=normalize,
         )
         super().__init__(transforms=[view_transform, view_transform])
 
 
-class SimSiamViewTransform:
+class VICRegViewTransform:
     def __init__(
         self,
         input_size: int = 224,
         cj_prob: float = 0.8,
-        cj_strength: float = 1.0,
-        cj_bright: float = 0.4,
-        cj_contrast: float = 0.4,
+        cj_strength: float = 0.5,
+        cj_bright: float = 0.8,
+        cj_contrast: float = 0.8,
         cj_sat: float = 0.4,
-        cj_hue: float = 0.1,
-        min_scale: float = 0.2,
+        cj_hue: float = 0.2,
+        min_scale: float = 0.08,
         random_gray_scale: float = 0.2,
+        solarize_prob: float = 0.1,
         gaussian_blur: float = 0.5,
         kernel_size: Optional[float] = None,
-        sigmas: Tuple[float, float] = (0.1, 2),
+        sigmas: Tuple[float, float] = (0.2, 2),
         vf_prob: float = 0.0,
         hf_prob: float = 0.5,
         rr_prob: float = 0.0,
         rr_degrees: Union[None, float, Tuple[float, float]] = None,
         normalize: Union[None, dict] = IMAGENET_NORMALIZE,
     ):
         color_jitter = T.ColorJitter(
@@ -132,14 +139,15 @@
         transform = [
             T.RandomResizedCrop(size=input_size, scale=(min_scale, 1.0)),
             random_rotation_transform(rr_prob=rr_prob, rr_degrees=rr_degrees),
             T.RandomHorizontalFlip(p=hf_prob),
             T.RandomVerticalFlip(p=vf_prob),
             T.RandomApply([color_jitter], p=cj_prob),
             T.RandomGrayscale(p=random_gray_scale),
+            RandomSolarization(prob=solarize_prob),
             GaussianBlur(kernel_size=kernel_size, sigmas=sigmas, prob=gaussian_blur),
             T.ToTensor(),
         ]
         if normalize:
             transform += [T.Normalize(mean=normalize["mean"], std=normalize["std"])]
         self.transform = T.Compose(transform)
```

### Comparing `lightly-1.4.5/lightly/transforms/smog_transform.py` & `lightly-1.4.6/lightly/transforms/smog_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/solarize.py` & `lightly-1.4.6/lightly/transforms/solarize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Solarization """
-
 # Copyright (c) 2021. Lightly AG and its affiliates.
 # All Rights Reserved
 
 import numpy as np
 from PIL import ImageOps
```

### Comparing `lightly-1.4.5/lightly/transforms/swav_transform.py` & `lightly-1.4.6/lightly/transforms/swav_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/transforms/vicreg_transform.py` & `lightly-1.4.6/lightly/transforms/simclr_transform.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,45 +3,46 @@
 import torchvision.transforms as T
 from PIL.Image import Image
 from torch import Tensor
 
 from lightly.transforms.gaussian_blur import GaussianBlur
 from lightly.transforms.multi_view_transform import MultiViewTransform
 from lightly.transforms.rotation import random_rotation_transform
-from lightly.transforms.solarize import RandomSolarization
 from lightly.transforms.utils import IMAGENET_NORMALIZE
 
 
-class VICRegTransform(MultiViewTransform):
-    """Implements the transformations for VICReg.
+class SimCLRTransform(MultiViewTransform):
+    """Implements the transformations for SimCLR [0, 1].
 
-    Similar to SimCLR transform but with extra solarization.
+    Note that SimCLR v1 and v2 use the same data augmentations.
+
+    - [0]: SimCLR v1, 2020, https://arxiv.org/abs/2002.05709
+    - [1]: SimCLR v2, 2020, https://arxiv.org/abs/2006.10029
 
     Attributes:
         input_size:
             Size of the input image in pixels.
         cj_prob:
             Probability that color jitter is applied.
         cj_strength:
             Strength of the color jitter. `cj_bright`, `cj_contrast`, `cj_sat`, and
-            `cj_hue` are multiplied by this value.
+            `cj_hue` are multiplied by this value. For datasets with small images,
+            such as CIFAR, it is recommended to set `cj_strenght` to 0.5.
         cj_bright:
             How much to jitter brightness.
         cj_contrast:
             How much to jitter constrast.
         cj_sat:
             How much to jitter saturation.
         cj_hue:
             How much to jitter hue.
         min_scale:
             Minimum size of the randomized crop relative to the input_size.
         random_gray_scale:
             Probability of conversion to grayscale.
-        solarize_prob:
-            Probability of solarization.
         gaussian_blur:
             Probability of Gaussian blur.
         kernel_size:
             Will be deprecated in favor of `sigmas` argument. If set, the old behavior applies and `sigmas` is ignored.
             Used to calculate sigma of gaussian blur with kernel_size * input_size.
         sigmas:
             Tuple of min and max value from which the std of the gaussian kernel is sampled.
@@ -63,70 +64,67 @@
 
     """
 
     def __init__(
         self,
         input_size: int = 224,
         cj_prob: float = 0.8,
-        cj_strength: float = 0.5,
+        cj_strength: float = 1.0,
         cj_bright: float = 0.8,
         cj_contrast: float = 0.8,
-        cj_sat: float = 0.4,
+        cj_sat: float = 0.8,
         cj_hue: float = 0.2,
         min_scale: float = 0.08,
         random_gray_scale: float = 0.2,
-        solarize_prob: float = 0.1,
         gaussian_blur: float = 0.5,
         kernel_size: Optional[float] = None,
         sigmas: Tuple[float, float] = (0.1, 2),
         vf_prob: float = 0.0,
         hf_prob: float = 0.5,
         rr_prob: float = 0.0,
         rr_degrees: Union[None, float, Tuple[float, float]] = None,
         normalize: Union[None, dict] = IMAGENET_NORMALIZE,
     ):
-        view_transform = VICRegViewTransform(
+        view_transform = SimCLRViewTransform(
             input_size=input_size,
             cj_prob=cj_prob,
             cj_strength=cj_strength,
             cj_bright=cj_bright,
             cj_contrast=cj_contrast,
             cj_sat=cj_sat,
             cj_hue=cj_hue,
             min_scale=min_scale,
             random_gray_scale=random_gray_scale,
-            solarize_prob=solarize_prob,
             gaussian_blur=gaussian_blur,
             kernel_size=kernel_size,
             sigmas=sigmas,
             vf_prob=vf_prob,
             hf_prob=hf_prob,
             rr_prob=rr_prob,
             rr_degrees=rr_degrees,
             normalize=normalize,
         )
         super().__init__(transforms=[view_transform, view_transform])
 
 
-class VICRegViewTransform:
+class SimCLRViewTransform:
     def __init__(
         self,
         input_size: int = 224,
         cj_prob: float = 0.8,
-        cj_strength: float = 0.5,
+        cj_strength: float = 1.0,
         cj_bright: float = 0.8,
         cj_contrast: float = 0.8,
-        cj_sat: float = 0.4,
+        cj_sat: float = 0.8,
         cj_hue: float = 0.2,
         min_scale: float = 0.08,
         random_gray_scale: float = 0.2,
-        solarize_prob: float = 0.1,
         gaussian_blur: float = 0.5,
         kernel_size: Optional[float] = None,
-        sigmas: Tuple[float, float] = (0.2, 2),
+        sigmas: Tuple[float, float] = (0.1, 2),
         vf_prob: float = 0.0,
         hf_prob: float = 0.5,
         rr_prob: float = 0.0,
         rr_degrees: Union[None, float, Tuple[float, float]] = None,
         normalize: Union[None, dict] = IMAGENET_NORMALIZE,
     ):
         color_jitter = T.ColorJitter(
@@ -139,15 +137,14 @@
         transform = [
             T.RandomResizedCrop(size=input_size, scale=(min_scale, 1.0)),
             random_rotation_transform(rr_prob=rr_prob, rr_degrees=rr_degrees),
             T.RandomHorizontalFlip(p=hf_prob),
             T.RandomVerticalFlip(p=vf_prob),
             T.RandomApply([color_jitter], p=cj_prob),
             T.RandomGrayscale(p=random_gray_scale),
-            RandomSolarization(prob=solarize_prob),
             GaussianBlur(kernel_size=kernel_size, sigmas=sigmas, prob=gaussian_blur),
             T.ToTensor(),
         ]
         if normalize:
             transform += [T.Normalize(mean=normalize["mean"], std=normalize["std"])]
         self.transform = T.Compose(transform)
```

### Comparing `lightly-1.4.5/lightly/transforms/vicregl_transform.py` & `lightly-1.4.6/lightly/transforms/vicregl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/cropping/crop_image_by_bounding_boxes.py` & `lightly-1.4.6/lightly/utils/cropping/crop_image_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/cropping/read_yolo_label_file.py` & `lightly-1.4.6/lightly/utils/cropping/read_yolo_label_file.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/debug.py` & `lightly-1.4.6/lightly/utils/debug.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/dist.py` & `lightly-1.4.6/lightly/utils/dist.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/embeddings_2d.py` & `lightly-1.4.6/lightly/utils/embeddings_2d.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/hipify.py` & `lightly-1.4.6/lightly/utils/hipify.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/io.py` & `lightly-1.4.6/lightly/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/lars.py` & `lightly-1.4.6/lightly/utils/lars.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/reordering.py` & `lightly-1.4.6/lightly/utils/reordering.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/scheduler.py` & `lightly-1.4.6/lightly/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly/utils/version_compare.py` & `lightly-1.4.6/lightly/utils/version_compare.py`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly.egg-info/PKG-INFO` & `lightly-1.4.6/lightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.4.5
+Version: 1.4.6
 Summary: A deep learning package for self-supervised learning
 Author: Philipp Wirth & Igor Susmelj
 Author-email: philipp@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
```

### Comparing `lightly-1.4.5/lightly.egg-info/SOURCES.txt` & `lightly-1.4.6/lightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/lightly.egg-info/requires.txt` & `lightly-1.4.6/lightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.4.5/setup.py` & `lightly-1.4.6/setup.py`

 * *Files identical despite different names*

