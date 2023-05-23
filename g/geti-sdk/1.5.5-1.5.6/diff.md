# Comparing `tmp/geti-sdk-1.5.5.tar.gz` & `tmp/geti-sdk-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.5.5.tar", last modified: Mon May 15 14:05:10 2023, max compression
+gzip compressed data, was "geti-sdk-1.5.6.tar", last modified: Tue May 23 14:37:51 2023, max compression
```

## Comparing `geti-sdk-1.5.5.tar` & `geti-sdk-1.5.6.tar`

### file list

```diff
@@ -1,171 +1,175 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      961 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.376739 geti-sdk-1.5.5/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.368739 geti-sdk-1.5.5/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5702 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/demos/demo_projects/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26479 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55163 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.380739 geti-sdk-1.5.5/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6554 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3660 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/active_learning_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/dataset_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.384739 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/rest_converters/status_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.372739 geti-sdk-1.5.5/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5766 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-15 14:05:10.000000 geti-sdk-1.5.5/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-15 14:05:10.388739 geti-sdk-1.5.5/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-15 13:42:22.000000 geti-sdk-1.5.5/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.632274 geti-sdk-1.5.6/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.636274 geti-sdk-1.5.6/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.636274 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5107 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      979 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3018 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/test_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.632274 geti-sdk-1.5.6/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.640274 geti-sdk-1.5.6/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5727 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/demos/demo_projects/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26692 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55163 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6554 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3723 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2203 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/active_learning_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.644274 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26172 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4808 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/testing_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12260 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2163 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6393 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6909 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2411 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/status_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1545 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/rest_converters/test_result_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.648274 geti-sdk-1.5.6/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5753 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/job_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.636274 geti-sdk-1.5.6/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5927 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-23 14:37:51.000000 geti-sdk-1.5.6/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-23 14:21:56.000000 geti-sdk-1.5.6/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-23 14:37:51.652274 geti-sdk-1.5.6/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-23 14:21:57.000000 geti-sdk-1.5.6/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.5.5/LICENSE` & `geti-sdk-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/PKG-INFO` & `geti-sdk-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.5
+Version: 1.5.6
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.5/README.md` & `geti-sdk-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/__init__.py` & `geti-sdk-1.5.6/geti_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.5.5"
+__version__ = "1.5.6"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.5.6/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/__init__.py` & `geti-sdk-1.5.6/geti_sdk/data_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 from .model import Model, OptimizedModel
 from .model_group import ModelGroup, ModelSummary
 from .performance import Performance
 from .predictions import Prediction
 from .project import Dataset, Pipeline, Project
 from .status import ProjectStatus
 from .task import Task
+from .test_result import Score, TestResult
 
 __all__ = [
     "TaskType",
     "AnnotationKind",
     "Project",
     "Label",
     "Task",
@@ -207,8 +208,10 @@
     "ModelGroup",
     "OptimizedModel",
     "ModelSummary",
     "ProjectStatus",
     "Job",
     "CodeDeploymentInformation",
     "Dataset",
+    "TestResult",
+    "Score",
 ]
```

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.5.6/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.5.6/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/annotations.py` & `geti-sdk-1.5.6/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.5.6/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.5.6/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/configuration.py` & `geti-sdk-1.5.6/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.5.6/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.5.6/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.5.6/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.5.6/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/optimization_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,13 +20,14 @@
     Enum representing the optimization type for an OptimizedModel in Intel® Geti™.
     """
 
     NNCF = "NNCF"
     POT = "POT"
     MO = "MO"
     ONNX = "ONNX"
+    NONE = "NONE"
 
     def __str__(self) -> str:
         """
         Return the string representation of the OptimizationType instance.
         """
         return self.value
```

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.5.6/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/job.py` & `geti-sdk-1.5.6/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/label.py` & `geti-sdk-1.5.6/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/media.py` & `geti-sdk-1.5.6/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.5.6/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/model.py` & `geti-sdk-1.5.6/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/model_group.py` & `geti-sdk-1.5.6/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/performance.py` & `geti-sdk-1.5.6/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/predictions.py` & `geti-sdk-1.5.6/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/project.py` & `geti-sdk-1.5.6/geti_sdk/data_models/project.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/shapes.py` & `geti-sdk-1.5.6/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/status.py` & `geti-sdk-1.5.6/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/task.py` & `geti-sdk-1.5.6/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.5.6/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/data_models/utils.py` & `geti-sdk-1.5.6/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/__init__.py` & `geti-sdk-1.5.6/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/constants.py` & `geti-sdk-1.5.6/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.5.6/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 valid_file_exists = False
     if valid_file_exists:
         logging.info(
             f"File {filename} exists at {path_to_file}. No new data was downloaded."
         )
         return path_to_file
 
-    proxies = get_proxies(url)
+    proxies = get_proxies(url, verify_cert=verify_cert)
     logging.info(f"Downloading {filename}...")
     with requests.get(url, stream=True, proxies=proxies, verify=verify_cert) as r:
         if r.status_code != 200:
             r.raise_for_status()
             raise RuntimeError(
                 f"Request to {url} failed, returned status code {r.status_code}"
             )
```

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.5.6/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.5.6/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/__init__.py` & `geti-sdk-1.5.6/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.5.6/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.5.6/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.5.6/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.5.6/geti_sdk/deployment/deployed_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import tempfile
 import time
 import zipfile
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import attr
 import numpy as np
+from otx.algorithms.classification.utils import get_cls_inferencer_configuration
 from otx.api.entities.color import Color
 from otx.api.entities.label import Domain as OTEDomain
 from otx.api.entities.label import LabelEntity
 from otx.api.entities.label_schema import LabelGroup, LabelGroupType, LabelSchemaEntity
 
 from geti_sdk.data_models import OptimizedModel, Project, TaskConfiguration
 from geti_sdk.http_session import GetiSession
@@ -301,14 +302,17 @@
             except ImportError as ex:
                 raise ImportError(
                     f"Unable to load inference model for {self}. A custom model wrapper"
                     f"is required, but could not be found at path "
                     f"{wrapper_module_path}."
                 ) from ex
 
+        if model_type == "otx_classification":
+            configuration = get_cls_inferencer_configuration(self.ote_label_schema)
+
         model = OMZModel.create_model(
             name=model_type,
             model_adapter=model_adapter,
             configuration=configuration,
             preload=True,
         )
         self.openvino_model_parameters = configuration
```

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/deployment.py` & `geti-sdk-1.5.6/geti_sdk/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.5.6/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.5.6/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/deployment/utils.py` & `geti-sdk-1.5.6/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/geti.py` & `geti-sdk-1.5.6/geti_sdk/geti.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/http_session/__init__.py` & `geti-sdk-1.5.6/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/http_session/exception.py` & `geti-sdk-1.5.6/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.5.6/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/http_session/server_config.py` & `geti-sdk-1.5.6/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/platform_versions.py` & `geti-sdk-1.5.6/geti_sdk/platform_versions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,22 +93,24 @@
 from .configuration_client import ConfigurationClient
 from .dataset_client import DatasetClient
 from .deployment_client import DeploymentClient
 from .media_client import ImageClient, VideoClient
 from .model_client import ModelClient
 from .prediction_client import PredictionClient
 from .project_client import ProjectClient
+from .testing_client import TestingClient
 from .training_client import TrainingClient
 
 __all__ = [
     "AnnotationClient",
     "ConfigurationClient",
     "DatasetClient",
     "ProjectClient",
     "VideoClient",
     "ImageClient",
     "PredictionClient",
     "ModelClient",
     "TrainingClient",
     "DeploymentClient",
     "ActiveLearningClient",
+    "TestingClient",
 ]
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/active_learning_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/active_learning_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/dataset_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/media_client/video_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/media_client/video_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions
 # and limitations under the License.
 
 import copy
 import json
 import logging
 import os
+import time
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from geti_sdk.data_models import Project, Task, TaskType
 from geti_sdk.data_models.utils import remove_null_fields
 from geti_sdk.http_session import GetiRequestException, GetiSession
 from geti_sdk.rest_clients.dataset_client import DatasetClient
 from geti_sdk.rest_converters import ProjectRESTConverter
@@ -166,14 +167,15 @@
                 project_name=project_name, project_type=project_type, labels=labels
             )
             project = self.session.get_rest_response(
                 url=f"{self.base_url}projects", method="POST", data=project_template
             )
             logging.info("Project created successfully.")
             project = ProjectRESTConverter.from_dict(project)
+            self._await_project_ready(project=project)
         return project
 
     def download_project_info(self, project_name: str, path_to_folder: str) -> None:
         """
         Get the project data that can be used for project creation for a project on
         the Intel® Geti™ server, named `project_name`. From the returned data, the
         method `ProjectClient.get_or_create_project` can create a project on the
@@ -584,7 +586,36 @@
         task_data["labels"] = label_list
         remove_null_fields(project_data)
         logging.info(project_data)
         response = self.session.get_rest_response(
             url=f"{self.base_url}projects/{project.id}", method="PUT", data=project_data
         )
         return ProjectRESTConverter.from_dict(response)
+
+    def _await_project_ready(
+        self, project: Project, timeout: int = 5, interval: int = 1
+    ) -> None:
+        """
+        Await the completion of the project creation process on the Intel® Geti™ server
+
+        :param project: Project object representing the project
+        :param timeout: Time (in seconds) after which the method will time out and
+            raise an error
+        :param interval: Interval (in seconds) between status checks of the project
+        :raises: TimeoutError if the project does not become ready after the specified
+            timeout
+        """
+        t_start = time.time()
+        error: Optional[BaseException] = None
+        while time.time() - t_start < timeout:
+            try:
+                self.session.get_rest_response(
+                    url=f"{self.base_url}projects/{project.id}/status", method="GET"
+                )
+                return
+            except GetiRequestException as latest_error:
+                time.sleep(interval)
+                error = latest_error
+        raise TimeoutError(
+            f"Project has not become ready within the specified timeout ({timeout} "
+            f"seconds)."
+        ) from error
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.5.6/geti_sdk/rest_clients/training_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 import logging
-import time
 from typing import Any, Dict, List, Optional, Union
 
 from geti_sdk.data_models import (
     Algorithm,
     Job,
     Project,
     ProjectStatus,
     Task,
     TaskConfiguration,
 )
 from geti_sdk.data_models.containers import AlgorithmList
 from geti_sdk.data_models.enums import JobState, JobType
 from geti_sdk.data_models.project import Dataset
-from geti_sdk.http_session import GetiRequestException, GetiSession
+from geti_sdk.http_session import GetiSession
 from geti_sdk.platform_versions import GETI_11_VERSION
 from geti_sdk.rest_converters import (
     ConfigurationRESTConverter,
     JobRESTConverter,
     StatusRESTConverter,
 )
 from geti_sdk.utils import get_supported_algorithms
+from geti_sdk.utils.job_helpers import get_job_with_timeout, monitor_jobs
 
 
 class TrainingClient:
     """
-    Class to manage training jobs for a certain project.
+    Class to manage training jobs for a certain Intel® Geti™ project.
     """
 
     def __init__(self, workspace_id: str, project: Project, session: GetiSession):
         self.session = session
         self.project = project
         self.workspace_id = workspace_id
         self.base_url = f"workspaces/{workspace_id}/projects/{project.id}"
@@ -92,34 +92,14 @@
         elif project_only and self.session.version.is_geti:
             return [
                 job for job in job_list if job.metadata.project.id == self.project.id
             ]
         else:
             return job_list
 
-    def get_job_by_id(self, job_id: str) -> Optional[Job]:
-        """
-        Return the details of a Job by its `job_id`.
-
-        :param job_id: ID of the job to retrieve
-        :return: Job instance containing detailed information and status of the job.
-            If no job by the specified ID is found on the Intel® Geti™ platform, this
-            method returns None
-        """
-        try:
-            response = self.session.get_rest_response(
-                url=f"workspaces/{self.workspace_id}/jobs/{job_id}", method="GET"
-            )
-        except GetiRequestException as error:
-            if error.status_code == 404:
-                return None
-            else:
-                raise error
-        return JobRESTConverter.from_dict(response)
-
     def get_algorithms_for_task(self, task: Union[Task, int]) -> AlgorithmList:
         """
         Return a list of supported algorithms for a specific task.
 
         The `task` parameter accepts both a Task object and an integer. If an int is
         passed, this will be considered the index of the task in the list of trainable
         tasks for the project which is managed by the TrainingClient.
@@ -239,34 +219,27 @@
         )
 
         if self.session.version < GETI_11_VERSION:
             job = JobRESTConverter.from_dict(response)
             job_id = job.id
         else:
             job_id = response["job_ids"][0]
-            job = self.get_job_by_id(job_id=job_id)
-
-        if job is not None:
-            logging.info(f"Training job with ID {job_id} submitted successfully.")
-        else:
-            t_start = time.time()
-            while job is None and (time.time() - t_start < 10):
-                logging.info(
-                    f"Training request was submitted but the training job status could "
-                    f"not be retrieved from the platform yet. Re-attempting to fetch "
-                    f"job status. Looking for job with ID {job_id}"
-                )
-                time.sleep(2)
-                job = self.get_job_by_id(job_id=job_id)
-            if job is None:
-                raise RuntimeError(
-                    "Train request was submitted but the TrainingClient was unable to "
-                    "find the resulting training job on the Intel® Geti™ server."
-                )
-        job.workspace_id = self.workspace_id
+        try:
+            job = get_job_with_timeout(
+                job_id=job_id,
+                session=self.session,
+                workspace_id=self.workspace_id,
+                job_type="training",
+            )
+        except RuntimeError:
+            raise RuntimeError(
+                "Training job was submitted, but the TrainingClient was unable to "
+                "find the resulting job on the platform."
+            )
+        logging.info(f"Training job with id {job.id} submitted successfully.")
         return job
 
     def monitor_jobs(
         self, jobs: List[Job], timeout: int = 10000, interval: int = 15
     ) -> List[Job]:
         """
         Monitor and print the progress of all jobs in the list `jobs`. Execution is
@@ -276,58 +249,17 @@
 
         :param jobs: List of jobs to monitor
         :param timeout: Timeout (in seconds) after which to stop the monitoring
         :param interval: Time interval (in seconds) at which the TrainingClient polls
             the server to update the status of the jobs. Defaults to 15 seconds
         :return: List of finished (or failed) jobs with their status updated
         """
-        monitoring = True
-        completed_states = [
-            JobState.FINISHED,
-            JobState.CANCELLED,
-            JobState.FAILED,
-            JobState.ERROR,
-        ]
-        logging.info("---------------- Monitoring progress -------------------")
-        jobs_to_monitor = [
-            job for job in jobs if job.status.state not in completed_states
-        ]
-        try:
-            t_start = time.time()
-            t_elapsed = 0
-            while monitoring and t_elapsed < timeout:
-                msg = ""
-                complete_count = 0
-                for job in jobs_to_monitor:
-                    job.update(self.session)
-                    msg += (
-                        f"{job.name}  -- "
-                        f"  Phase: {job.status.user_friendly_message} "
-                        f"  State: {job.status.state} "
-                        f"  Progress: {job.status.progress:.1f}%"
-                    )
-                    if job.status.state in completed_states:
-                        complete_count += 1
-                if complete_count == len(jobs_to_monitor):
-                    monitoring = False
-                logging.info(msg)
-                time.sleep(interval)
-                t_elapsed = time.time() - t_start
-        except KeyboardInterrupt:
-            logging.info("Job monitoring interrupted, stopping...")
-            for job in jobs:
-                job.update(self.session)
-            return jobs
-        if t_elapsed < timeout:
-            logging.info("All jobs completed, monitoring stopped.")
-        else:
-            logging.info(
-                f"Monitoring stopped after {t_elapsed:.1f} seconds due to timeout."
-            )
-        return jobs
+        return monitor_jobs(
+            session=self.session, jobs=jobs, timeout=timeout, interval=interval
+        )
 
     def get_jobs_for_task(self, task: Task, running_only: bool = True) -> List[Job]:
         """
         Return a list of current jobs for the task, if any
 
         :param task: Task to retrieve the jobs for
         :param running_only: True to return only jobs that are currently running,
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,27 +46,31 @@
 
 .. autoclass:: StatusRESTConverter
    :members:
 
 .. autoclass:: JobRESTConverter
    :members:
 
+.. autoclass:: TestResultRESTConverter
+   :members:
 """
 from .annotation_rest_converter import AnnotationRESTConverter
 from .configuration_rest_converter import ConfigurationRESTConverter
 from .job_rest_converter import JobRESTConverter
 from .media_rest_converter import MediaRESTConverter
 from .model_rest_converter import ModelRESTConverter
 from .prediction_rest_converter import PredictionRESTConverter
 from .project_rest_converter import ProjectRESTConverter
 from .status_rest_converter import StatusRESTConverter
+from .test_result_rest_converter import TestResultRESTConverter
 
 __all__ = [
     "ProjectRESTConverter",
     "MediaRESTConverter",
     "AnnotationRESTConverter",
     "PredictionRESTConverter",
     "ConfigurationRESTConverter",
     "ModelRESTConverter",
     "StatusRESTConverter",
     "JobRESTConverter",
+    "TestResultRESTConverter",
 ]
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 import copy
 from typing import Any, Dict, List, cast
 
 import attr
 from omegaconf import OmegaConf
 
-from geti_sdk.data_models import Annotation, AnnotationScene, MediaType, ScoredLabel
+from geti_sdk.data_models import Annotation, AnnotationScene
 from geti_sdk.data_models.enums import ShapeType
+from geti_sdk.data_models.label import ScoredLabel
+from geti_sdk.data_models.media import MediaType
 from geti_sdk.data_models.media_identifiers import (
     ImageIdentifier,
     MediaIdentifier,
     VideoFrameIdentifier,
 )
 from geti_sdk.data_models.shapes import (
     Ellipse,
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 # and limitations under the License.
 
 import copy
 from typing import Any, Dict, List
 
 import attr
 
-from geti_sdk.data_models import Annotation, AnnotationScene, ScoredLabel
+from geti_sdk.data_models import Annotation, AnnotationScene
 from geti_sdk.data_models.enums import ShapeType
+from geti_sdk.data_models.label import ScoredLabel
 from geti_sdk.data_models.shapes import Shape
 from geti_sdk.data_models.utils import (
     attr_value_serializer,
     remove_null_fields,
     str_to_shape_type,
 )
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions
 # and limitations under the License.
 
 from typing import Any, Dict
 
-from geti_sdk.data_models import Model, ModelGroup, OptimizedModel
+from geti_sdk.data_models.model import Model, OptimizedModel
+from geti_sdk.data_models.model_group import ModelGroup
 from geti_sdk.utils import deserialize_dictionary
 
 
 class ModelRESTConverter:
     """
     Class that handles conversion of Intel® Geti™ REST output for media entities to
     objects and vice versa.
```

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.5.6/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/__init__.py` & `geti-sdk-1.5.6/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.5.6/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.5.6/geti_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.5
+Version: 1.5.6
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.5/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.5.6/geti_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 geti_sdk/data_models/performance.py
 geti_sdk/data_models/predictions.py
 geti_sdk/data_models/project.py
 geti_sdk/data_models/shapes.py
 geti_sdk/data_models/status.py
 geti_sdk/data_models/task.py
 geti_sdk/data_models/task_annotation_state.py
+geti_sdk/data_models/test_result.py
 geti_sdk/data_models/utils.py
 geti_sdk/data_models/containers/__init__.py
 geti_sdk/data_models/containers/algorithm_list.py
 geti_sdk/data_models/containers/media_list.py
 geti_sdk/data_models/enums/__init__.py
 geti_sdk/data_models/enums/annotation_kind.py
 geti_sdk/data_models/enums/annotation_state.py
@@ -86,14 +87,15 @@
 geti_sdk/rest_clients/__init__.py
 geti_sdk/rest_clients/active_learning_client.py
 geti_sdk/rest_clients/configuration_client.py
 geti_sdk/rest_clients/dataset_client.py
 geti_sdk/rest_clients/deployment_client.py
 geti_sdk/rest_clients/model_client.py
 geti_sdk/rest_clients/prediction_client.py
+geti_sdk/rest_clients/testing_client.py
 geti_sdk/rest_clients/training_client.py
 geti_sdk/rest_clients/annotation_clients/__init__.py
 geti_sdk/rest_clients/annotation_clients/annotation_client.py
 geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
 geti_sdk/rest_clients/media_client/__init__.py
 geti_sdk/rest_clients/media_client/image_client.py
 geti_sdk/rest_clients/media_client/media_client.py
@@ -104,24 +106,26 @@
 geti_sdk/rest_converters/__init__.py
 geti_sdk/rest_converters/configuration_rest_converter.py
 geti_sdk/rest_converters/job_rest_converter.py
 geti_sdk/rest_converters/media_rest_converter.py
 geti_sdk/rest_converters/model_rest_converter.py
 geti_sdk/rest_converters/project_rest_converter.py
 geti_sdk/rest_converters/status_rest_converter.py
+geti_sdk/rest_converters/test_result_rest_converter.py
 geti_sdk/rest_converters/annotation_rest_converter/__init__.py
 geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
 geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
 geti_sdk/rest_converters/prediction_rest_converter/__init__.py
 geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
 geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
 geti_sdk/utils/__init__.py
 geti_sdk/utils/algorithm_helpers.py
 geti_sdk/utils/credentials_helpers.py
 geti_sdk/utils/dictionary_helpers.py
+geti_sdk/utils/job_helpers.py
 geti_sdk/utils/label_helpers.py
 geti_sdk/utils/plot_helpers.py
 geti_sdk/utils/project_helpers.py
 geti_sdk/utils/serialization_helpers.py
 geti_sdk/utils/workspace_helpers.py
 requirements/requirements-dev.txt
 requirements/requirements-docs.txt
```

### Comparing `geti-sdk-1.5.5/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.5.6/geti_sdk.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 datumaro==1.2.*
-requests==2.28.*
+requests==2.31.*
 numpy==1.22.*
 omegaconf==2.3.*
 opencv-python==4.5.*
 python-dotenv==1.0.*
 tqdm==4.65.*
 Pillow==9.5.*
 pathvalidate>=2.5.0
```

### Comparing `geti-sdk-1.5.5/setup.py` & `geti-sdk-1.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/__init__.py` & `geti-sdk-1.5.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/conftest.py` & `geti-sdk-1.5.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/__init__.py` & `geti-sdk-1.5.6/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/constants.py` & `geti-sdk-1.5.6/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/enums.py` & `geti-sdk-1.5.6/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/finalizers.py` & `geti-sdk-1.5.6/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/fixtures.py` & `geti-sdk-1.5.6/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/plotting.py` & `geti-sdk-1.5.6/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/project_helpers.py` & `geti-sdk-1.5.6/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/project_service.py` & `geti-sdk-1.5.6/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/training.py` & `geti-sdk-1.5.6/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.5/tests/helpers/vcr_helpers.py` & `geti-sdk-1.5.6/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

