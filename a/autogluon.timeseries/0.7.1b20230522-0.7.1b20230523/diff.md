# Comparing `tmp/autogluon.timeseries-0.7.1b20230522.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230522.tar", last modified: Mon May 22 09:04:59 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230523.tar", last modified: Tue May 23 09:04:21 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230522.tar` & `autogluon.timeseries-0.7.1b20230523.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.165983 autogluon.timeseries-0.7.1b20230522/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-22 09:04:59.165983 autogluon.timeseries-0.7.1b20230522/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 09:04:59.165983 autogluon.timeseries-0.7.1b20230522/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.157983 autogluon.timeseries-0.7.1b20230522/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.157983 autogluon.timeseries-0.7.1b20230522/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.161983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.165983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    46181 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.165983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.165983 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 09:04:10.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 09:04:58.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:04:59.157983 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:04:59.000000 autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.512649 autogluon.timeseries-0.7.1b20230523/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46181 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41222 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230522/PKG-INFO` & `autogluon.timeseries-0.7.1b20230523/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230522
+Version: 0.7.1b20230523
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230522/setup.py` & `autogluon.timeseries-0.7.1b20230523/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,26 @@
     AutoARIMAModel,
     AutoETSModel,
     DynamicOptimizedThetaModel,
     ETSModel,
     NaiveModel,
     SeasonalNaiveModel,
     ThetaModel,
+    ThetaStatsmodelsModel,
 )
 
 __all__ = [
     "DeepARModel",
     "SimpleFeedForwardModel",
     "TemporalFusionTransformerModel",
-    "ARIMAModel",
-    "ETSModel",
-    "ThetaModel",
     "AutoGluonTabularModel",
     "RecursiveTabularModel",
     "NaiveModel",
     "SeasonalNaiveModel",
     "AutoETSModel",
     "AutoARIMAModel",
     "DynamicOptimizedThetaModel",
+    "ThetaModel",
+    "ARIMAModel",
+    "ETSModel",
+    "ThetaStatsmodelsModel",
 ]
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-import hashlib
 import logging
-from multiprocessing import cpu_count
-from typing import Any, Dict, List, Optional, Union
+import time
+from multiprocessing import TimeoutError, cpu_count
+from typing import Any, Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
+from scipy.stats import norm
 
-from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
+from autogluon.core.utils.exceptions import TimeLimitExceeded
+from autogluon.timeseries.dataset import TimeSeriesDataFrame
+from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
+from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 from autogluon.timeseries.utils.seasonality import get_seasonality
-from autogluon.timeseries.utils.warning_filters import statsmodels_joblib_warning_filter
+from autogluon.timeseries.utils.warning_filters import statsmodels_joblib_warning_filter, statsmodels_warning_filter
 
 logger = logging.getLogger(__name__)
 
 
-def hash_ts_dataframe_items(ts_dataframe: TimeSeriesDataFrame) -> pd.Series:
-    """Hash each time series in the dataset to a 32-character hex string.
+class AbstractLocalModel(AbstractTimeSeriesModel):
+    """Abstract class for local forecasting models that are trained separately for each time series.
 
-    Hash is computed based on the timestamps and values of the time series (item_id is ignored).
+    Prediction is parallelized across CPU cores using joblib.Parallel.
 
-    This means that any model that doesn't use static features will make identical predictions for two time series
-    with the same hash value (assuming no collisions).
+    Attributes
+    ----------
+    allowed_local_model_args : List[str]
+        Argument that can be passed to the underlying local model.
+    max_ts_length : int, optional
+        If not None, only the last ``max_ts_length`` time steps of each time series will be used to train the model.
+    default_n_jobs : Union[int, float]
+        Default number of CPU cores used to train models. If float, this fraction of CPU cores will be used.
+    init_time_in_seconds : int
+        Time that it takes to initialize the model in seconds (e.g., because of JIT compilation by Numba).
+        If time_limit is below this number, model won't be trained.
     """
-    df_with_timestamp = ts_dataframe.reset_index(level=TIMESTAMP)
-    hash_per_timestep = pd.util.hash_pandas_object(df_with_timestamp, index=False)
-    # groupby preserves the order of the timesteps
-    return hash_per_timestep.groupby(level=ITEMID, sort=False).apply(lambda x: hashlib.md5(x.values).hexdigest())
-
 
-class AbstractLocalModel(AbstractTimeSeriesModel):
     allowed_local_model_args: List[str] = []
-    # Use 50% of the cores since some models rely on parallel ops and are actually slower if n_jobs=-1
-    DEFAULT_N_JOBS: Union[float, int] = 0.5
-    MAX_TS_LENGTH: Optional[int] = None
+    max_ts_length: Optional[int] = None
+    default_n_jobs: Union[int, float] = 0.5
+    init_time_in_seconds: int = 0
 
     def __init__(
         self,
         freq: Optional[str] = None,
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
@@ -52,26 +60,30 @@
             eval_metric=eval_metric,
             hyperparameters=hyperparameters,
             **kwargs,
         )
         if hyperparameters is None:
             hyperparameters = {}
         # TODO: Replace with 'num_cpus' argument passed to fit (after predictor API is changed)
-        n_jobs = hyperparameters.get("n_jobs", self.DEFAULT_N_JOBS)
+        n_jobs = hyperparameters.get("n_jobs", self.default_n_jobs)
         if isinstance(n_jobs, float) and 0 < n_jobs <= 1:
             self.n_jobs = max(int(cpu_count() * n_jobs), 1)
         elif isinstance(n_jobs, int):
             self.n_jobs = n_jobs
         else:
             raise ValueError(f"n_jobs must be a float between 0 and 1 or an integer (received n_jobs = {n_jobs})")
         self._local_model_args: Dict[str, Any] = None
-        self._cached_predictions: Dict[str, pd.DataFrame] = {}
+        self._seasonal_period: Optional[int] = None
+        self.time_limit: Optional[float] = None
 
     def _fit(self, train_data: TimeSeriesDataFrame, time_limit: int = None, **kwargs):
         self._check_fit_params()
+        if time_limit is not None and time_limit < self.init_time_in_seconds:
+            raise TimeLimitExceeded
+
         # Initialize parameters passed to each local model
         raw_local_model_args = self._get_model_params().copy()
         raw_local_model_args.pop("n_jobs", None)
 
         unused_local_model_args = []
         local_model_args = {}
         for key, value in raw_local_model_args.items():
@@ -84,73 +96,111 @@
             logger.warning(
                 f"{self.name} ignores following hyperparameters: {unused_local_model_args}. "
                 f"See the docstring of {self.name} for the list of supported hyperparameters."
             )
 
         if "seasonal_period" not in local_model_args or local_model_args["seasonal_period"] is None:
             local_model_args["seasonal_period"] = get_seasonality(train_data.freq)
-        self.freq = train_data.freq
+        self._seasonal_period = local_model_args["seasonal_period"]
 
-        self._local_model_args = self._update_local_model_args(local_model_args=local_model_args, data=train_data)
+        self._local_model_args = self._update_local_model_args(local_model_args=local_model_args)
+        self.time_limit = time_limit
 
         logger.debug(f"{self.name} is a local model, so the model will be fit at prediction time.")
         return self
 
-    def _update_local_model_args(
-        self, local_model_args: Dict[str, Any], data: TimeSeriesDataFrame, **kwargs
-    ) -> Dict[str, Any]:
+    def _update_local_model_args(self, local_model_args: Dict[str, Any]) -> Dict[str, Any]:
         return local_model_args
 
-    def predict(self, data: TimeSeriesDataFrame, quantile_levels: List[float] = None, **kwargs) -> TimeSeriesDataFrame:
-        if quantile_levels is None:
-            quantile_levels = self.quantile_levels
-
-        if self.freq != data.freq:
-            raise RuntimeError(
-                f"{self.name} has frequency '{self.freq}', which doesn't match the frequency "
-                f"of the dataset '{data.freq}'."
+    def predict(self, data: TimeSeriesDataFrame, **kwargs) -> TimeSeriesDataFrame:
+        if self.max_ts_length is not None:
+            logger.debug(f"Shortening all time series to at most {self.max_ts_length}")
+            data = data.groupby(level=ITEMID, sort=False).tail(self.max_ts_length)
+
+        df = pd.DataFrame(data).reset_index(level=ITEMID)
+        all_series = (ts for _, ts in df.groupby(by=ITEMID, as_index=False, sort=False)[self.target])
+
+        # timeout ensures that no individual job takes longer than time_limit
+        # TODO: a job started late may still exceed time_limit - how to prevent that?
+        timeout = None if self.n_jobs == 1 else self.time_limit
+        # end_time ensures that no new jobs are started after time_limit is exceeded
+        end_time = None if self.time_limit is None else time.time() + self.time_limit
+        executor = Parallel(self.n_jobs, timeout=timeout)
+
+        try:
+            with statsmodels_joblib_warning_filter(), statsmodels_warning_filter():
+                predictions_with_flags = executor(
+                    delayed(self._predict_wrapper)(ts, end_time=end_time) for ts in all_series
+                )
+        except TimeoutError:
+            raise TimeLimitExceeded
+
+        number_failed_models = sum(failed_flag for _, failed_flag in predictions_with_flags)
+        if number_failed_models > 0:
+            fraction_failed_models = number_failed_models / len(predictions_with_flags)
+            logger.warning(
+                f"\t{self.name} failed for {number_failed_models} time series ({100 * fraction_failed_models:.1f}%). "
+                "Fallback model SeasonalNaive was used for these time series."
             )
-        if self.MAX_TS_LENGTH is not None:
-            logger.debug(f"Shortening all time series to at most {self.MAX_TS_LENGTH}")
-            data = data.groupby(level=ITEMID, sort=False).tail(self.MAX_TS_LENGTH)
-
-        self._fit_and_cache_predictions(data, quantile_levels=quantile_levels)
-        item_id_to_prediction = {}
-        for item_id, ts_hash in hash_ts_dataframe_items(data).items():
-            item_id_to_prediction[item_id] = self._cached_predictions[ts_hash]
-        predictions_df = pd.concat(item_id_to_prediction)
-        predictions_df.index.rename([ITEMID, TIMESTAMP], inplace=True)
+        predictions_df = pd.concat([pred for pred, _ in predictions_with_flags])
+        predictions_df.index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
         return TimeSeriesDataFrame(predictions_df)
 
-    def _fit_and_cache_predictions(self, data: TimeSeriesDataFrame, quantile_levels: List[float]):
-        data_hash = hash_ts_dataframe_items(data)
-        items_to_fit = [item_id for item_id, ts_hash in data_hash.items() if ts_hash not in self._cached_predictions]
-        if len(items_to_fit) > 0:
-            logger.debug(f"{self.name} received {len(items_to_fit)} new items to predict, generating predictions")
-            target_series = data[self.target]
-            time_series_to_fit = (target_series.loc[item_id] for item_id in items_to_fit)
-            with statsmodels_joblib_warning_filter():
-                predictions = Parallel(n_jobs=self.n_jobs)(
-                    delayed(self._predict_with_local_model)(
-                        time_series=ts,
-                        prediction_length=self.prediction_length,
-                        freq=self.freq,
-                        quantile_levels=quantile_levels,
-                        local_model_args=self._local_model_args.copy(),
-                    )
-                    for ts in time_series_to_fit
-                )
-            for item_id, preds in zip(items_to_fit, predictions):
-                self._cached_predictions[data_hash.loc[item_id]] = preds
-            # Make sure cached predictions can be reused by other models
-            self.save()
+    def score_and_cache_oof(
+        self, val_data: TimeSeriesDataFrame, store_val_score: bool = False, store_predict_time: bool = False
+    ) -> None:
+        super().score_and_cache_oof(val_data, store_val_score, store_predict_time)
+        # Remove time_limit for future predictions
+        self.time_limit = None
+
+    def _predict_wrapper(self, time_series: pd.Series, end_time: Optional[float] = None) -> Tuple[pd.DataFrame, bool]:
+        if end_time is not None and time.time() >= end_time:
+            raise TimeLimitExceeded
+        try:
+            result = self._predict_with_local_model(
+                time_series=time_series,
+                local_model_args=self._local_model_args.copy(),
+            )
+            model_failed = False
+        except Exception as e:
+            result = seasonal_naive_forecast(
+                target=time_series.values.ravel(),
+                prediction_length=self.prediction_length,
+                quantile_levels=self.quantile_levels,
+                seasonal_period=self._seasonal_period,
+            )
+            model_failed = True
+        return result, model_failed
 
-    @staticmethod
     def _predict_with_local_model(
+        self,
         time_series: pd.Series,
-        freq: str,
-        prediction_length: int,
-        quantile_levels: List[float],
         local_model_args: dict,
-        **kwargs,
     ) -> pd.DataFrame:
         raise NotImplementedError
+
+
+def seasonal_naive_forecast(
+    target: np.ndarray, prediction_length: int, quantile_levels: List[float], seasonal_period: int
+) -> pd.DataFrame:
+    """Generate seasonal naive forecast, predicting the last observed value from the same period."""
+    forecast = {}
+    if len(target) > seasonal_period and seasonal_period > 1:
+        indices = [len(target) - seasonal_period + k % seasonal_period for k in range(prediction_length)]
+        forecast["mean"] = target[indices]
+        residuals = target[seasonal_period:] - target[:-seasonal_period]
+
+        sigma = np.sqrt(np.mean(np.square(residuals)))
+        num_full_seasons = np.arange(1, prediction_length + 1) // seasonal_period
+        sigma_per_timestep = sigma * np.sqrt(num_full_seasons + 1)
+    else:
+        # Fall back to naive forecast
+        forecast["mean"] = np.full(shape=[prediction_length], fill_value=target[-1])
+        residuals = target[1:] - target[:-1]
+
+        sigma = np.sqrt(np.mean(np.square(residuals)))
+        sigma_per_timestep = sigma * np.sqrt(np.arange(1, prediction_length + 1))
+
+    for q in quantile_levels:
+        forecast[str(q)] = forecast["mean"] + norm.ppf(q) * sigma_per_timestep
+
+    return pd.DataFrame(forecast)
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/naive.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,33 @@
-from typing import List
-
 import numpy as np
 import pandas as pd
-from scipy.stats import norm
-
-from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_single_time_series
-
-from .abstract_local_model import AbstractLocalModel
-
-
-def seasonal_naive_forecast(
-    time_series: pd.Series, freq: str, prediction_length: int, quantile_levels: List[float], seasonal_period: int
-):
-    forecast_timestamps = get_forecast_horizon_index_single_time_series(
-        past_timestamps=time_series.index, freq=freq, prediction_length=prediction_length
-    )
-
-    target = time_series.values.ravel()
-    forecast = {}
 
-    if len(target) > seasonal_period and seasonal_period > 1:
-        indices = [len(target) - seasonal_period + k % seasonal_period for k in range(prediction_length)]
-        forecast["mean"] = target[indices]
-        residuals = target[seasonal_period:] - target[:-seasonal_period]
-
-        sigma = np.sqrt(np.mean(np.square(residuals)))
-        num_full_seasons = np.arange(1, prediction_length + 1) // seasonal_period
-        sigma_per_timestep = sigma * np.sqrt(num_full_seasons + 1)
-    else:
-        # Fall back to naive forecast
-        forecast["mean"] = np.full(shape=[prediction_length], fill_value=target[-1])
-        residuals = target[1:] - target[:-1]
-
-        sigma = np.sqrt(np.mean(np.square(residuals)))
-        sigma_per_timestep = sigma * np.sqrt(np.arange(1, prediction_length + 1))
-
-    for q in quantile_levels:
-        forecast[str(q)] = forecast["mean"] + norm.ppf(q) * sigma_per_timestep
-
-    return pd.DataFrame(forecast, index=forecast_timestamps)
+from autogluon.timeseries.models.local.abstract_local_model import AbstractLocalModel, seasonal_naive_forecast
 
 
 class NaiveModel(AbstractLocalModel):
     """Baseline model that sets the forecast equal to the last observed value.
 
     Quantiles are obtained by assuming that the residuals follow zero-mean normal distribution, scale of which is
     estimated from the empirical distribution of the residuals.
     As described in https://otexts.com/fpp3/prediction-intervals.html
 
     """
 
     allowed_local_model_args = ["seasonal_period"]
 
-    @staticmethod
     def _predict_with_local_model(
+        self,
         time_series: pd.Series,
-        freq: str,
-        prediction_length: int,
-        quantile_levels: List[float],
         local_model_args: dict,
-        **kwargs,
     ) -> pd.DataFrame:
         return seasonal_naive_forecast(
-            time_series=time_series,
-            freq=freq,
-            prediction_length=prediction_length,
-            quantile_levels=quantile_levels,
+            target=time_series.values.ravel(),
+            prediction_length=self.prediction_length,
+            quantile_levels=self.quantile_levels,
             seasonal_period=1,
         )
 
 
 class SeasonalNaiveModel(AbstractLocalModel):
     """Baseline model that sets the forecast equal to the last observed value from the same season.
 
@@ -87,23 +45,18 @@
         specified manually by providing an integer > 1.
         If seasonal_period (inferred or provided) is equal to 1, will fall back to Naive forecast.
         Seasonality will also be disabled, if the length of the time series is < seasonal_period.
     """
 
     allowed_local_model_args = ["seasonal_period"]
 
-    @staticmethod
     def _predict_with_local_model(
-        time_series: pd.Series,
-        freq: str,
-        prediction_length: int,
-        quantile_levels: List[float],
+        self,
+        time_series: np.ndarray,
         local_model_args: dict,
-        **kwargs,
     ) -> pd.DataFrame:
         return seasonal_naive_forecast(
-            time_series=time_series,
-            freq=freq,
-            prediction_length=prediction_length,
-            quantile_levels=quantile_levels,
+            target=time_series.values.ravel(),
+            prediction_length=self.prediction_length,
+            quantile_levels=self.quantile_levels,
             seasonal_period=local_model_args["seasonal_period"],
         )
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,53 @@
 import logging
-from typing import List, Type, Union
+from typing import Any, Dict, Type
 
 import pandas as pd
 
-from autogluon.core.utils.exceptions import TimeLimitExceeded
-from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
-from autogluon.timeseries.models.local.abstract_local_model import AbstractLocalModel, hash_ts_dataframe_items
-from autogluon.timeseries.utils.warning_filters import statsmodels_joblib_warning_filter, statsmodels_warning_filter
+from .abstract_local_model import AbstractLocalModel
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractStatsForecastModel(AbstractLocalModel):
-    """Wrapper for StatsForecast models.
+    """Wrapper for StatsForecast models."""
 
-    Cached predictions are stored inside the model to speed up validation & ensemble training downstream.
+    init_time_in_seconds = 15  # numba compilation for the first run
 
-    Attributes
-    ----------
-    allowed_local_model_args : List[str]
-        List of allowed arguments that can be passed to the underlying model.
-        Arguments not in this list will be filtered out and not passed to the underlying model.
-    """
-
-    allowed_local_model_args: List[str] = []
-    DEFAULT_N_JOBS: Union[float, int] = -1
+    def _update_local_model_args(self, local_model_args: Dict[str, Any]) -> Dict[str, Any]:
+        seasonal_period = local_model_args.pop("seasonal_period")
+        local_model_args["season_length"] = seasonal_period
+        return local_model_args
 
-    def get_model_type(self) -> Type:
+    def _get_model_type(self) -> Type:
         raise NotImplementedError
 
-    def _fit(self, train_data, time_limit=None, verbosity=2, **kwargs) -> None:
-        """Prepare hyperparameters that will be passed to the underlying model.
-
-        As for all local models, actual fitting + predictions are delegated to the ``predict`` method.
-        """
-        # TODO: Find a way to ensure that SF models respect time_limit, e.g. https://docs.python.org/3/library/concurrent.futures.html
-        # Fitting usually takes >= 15 seconds
-        if time_limit is not None:
-            if time_limit < 10:
-                raise TimeLimitExceeded
-            elif time_limit < 30:
-                logger.warning(
-                    f"Warning: {self.__class__.__name__} does not support early stopping "
-                    f"and may exceed the remaining time_limit of {time_limit:.1f}s"
-                )
-        super()._fit(train_data=train_data, time_limit=time_limit, verbosity=verbosity, **kwargs)
-        # seasonal_period is called season_length in StatsForecast
-        self._local_model_args["season_length"] = self._local_model_args.pop("seasonal_period")
-        return self
-
-    def _to_statsforecast_dataframe(self, data: TimeSeriesDataFrame) -> pd.DataFrame:
-        target = data[[self.target]]
-        return target.reset_index().rename({ITEMID: "unique_id", TIMESTAMP: "ds", self.target: "y"}, axis=1)
-
-    def _fit_and_cache_predictions(self, data: TimeSeriesDataFrame, **kwargs):
-        """Make predictions for time series in data that are not cached yet."""
-        # TODO: Improve prediction caching logic -> save predictions to a separate file, like in Tabular?
-        from statsforecast import StatsForecast
-        from statsforecast.models import SeasonalNaive
-
-        data_hash = hash_ts_dataframe_items(data)
-        items_to_fit = [item_id for item_id, ts_hash in data_hash.items() if ts_hash not in self._cached_predictions]
-        if len(items_to_fit) > 0:
-            logger.debug(f"{self.name} received {len(items_to_fit)} new items to predict, generating predictions")
-            data_to_fit = pd.DataFrame(data).query("item_id in @items_to_fit")
-
-            model_type = self.get_model_type()
-            model = model_type(**self._local_model_args)
-
-            sf = StatsForecast(
-                models=[model],
-                fallback_model=SeasonalNaive(season_length=self._local_model_args["season_length"]),
-                sort_df=False,
-                freq=self.freq,
-                n_jobs=self.n_jobs,
-            )
-
-            # StatsForecast generates probabilistic forecasts in lo/hi confidence region boundaries
-            # We chose the columns that correspond to the desired quantile_levels
-            model_name = str(model)
-            new_column_names = {"unique_id": ITEMID, "ds": TIMESTAMP, model_name: "mean"}
-            levels = []
-            for q in self.quantile_levels:
-                level = round(abs(q - 0.5) * 200, 1)
-                suffix = "lo" if q < 0.5 else "hi"
-                levels.append(level)
-                new_column_names[f"{model_name}-{suffix}-{level}"] = str(q)
-            levels = sorted(list(set(levels)))
-            chosen_columns = list(new_column_names.values())
-
-            with statsmodels_warning_filter(), statsmodels_joblib_warning_filter():
-                raw_predictions = sf.forecast(
-                    df=self._to_statsforecast_dataframe(data_to_fit),
-                    h=self.prediction_length,
-                    level=levels,
-                ).reset_index()
-            predictions = raw_predictions.rename(new_column_names, axis=1)[chosen_columns].set_index(TIMESTAMP)
-            item_ids = predictions.pop(ITEMID)
-
-            for item_id, preds in predictions.groupby(item_ids, sort=False):
-                self._cached_predictions[data_hash.loc[item_id]] = preds
-            # Make sure cached predictions can be reused by other models
-            self.save()
-
-    def hyperparameter_tune(self, **kwargs):
-        # FIXME: multiprocessing.pool.ApplyResult.get() hangs inside StatsForecast.forecast if HPO enabled - needs investigation
-        if self.n_jobs != 1:
-            raise NotImplementedError(f"{self.__class__.__name__} does not support hyperparameter tuning.")
+    def _predict_with_local_model(
+        self,
+        time_series: pd.Series,
+        local_model_args: dict,
+    ) -> pd.DataFrame:
+        model_type = self._get_model_type()
+        model = model_type(**local_model_args)
+
+        # Code does conversion between confidence levels and quantiles
+        levels = []
+        quantile_to_key = {}
+        for q in self.quantile_levels:
+            level = round(abs(q - 0.5) * 200, 1)
+            suffix = "lo" if q < 0.5 else "hi"
+            levels.append(level)
+            quantile_to_key[str(q)] = f"{suffix}-{level}"
+        levels = sorted(list(set(levels)))
+
+        forecast = model.forecast(h=self.prediction_length, y=time_series.values.ravel(), level=levels)
+        predictions = {"mean": forecast["mean"]}
+        for q, key in quantile_to_key.items():
+            predictions[q] = forecast[key]
+        return pd.DataFrame(predictions)
 
 
 class AutoARIMAModel(AbstractStatsForecastModel):
     """Automatically tuned ARIMA model.
 
     Automatically selects the best (p,d,q,P,D,Q) model parameters using an information criterion
 
@@ -176,30 +113,31 @@
         "max_D",
         "start_p",
         "start_q",
         "start_P",
         "start_Q",
         "stationary",
         "seasonal",
-        "approximatio",
+        "approximation",
         "allowdrift",
         "allowmean",
         "seasonal_period",
     ]
     MAX_TS_LENGTH = 3000
 
-    def _update_local_model_args(self, local_model_args: dict, data: TimeSeriesDataFrame) -> dict:
+    def _update_local_model_args(self, local_model_args: dict) -> dict:
+        local_model_args = super()._update_local_model_args(local_model_args)
         local_model_args.setdefault("approximation", True)
         local_model_args.setdefault("allowmean", True)
         return local_model_args
 
-    def get_model_type(self):
-        from statsforecast.models import AutoARIMA as AutoARIMA_
+    def _get_model_type(self):
+        from statsforecast.models import AutoARIMA
 
-        return AutoARIMA_
+        return AutoARIMA
 
 
 class AutoETSModel(AbstractStatsForecastModel):
     """Automatically tuned exponential smoothing with trend and seasonality.
 
     Automatically selects the best ETS (Error, Trend, Seasonality) model using an information criterion
 
@@ -225,18 +163,18 @@
     """
 
     allowed_local_model_args = [
         "model",
         "seasonal_period",
     ]
 
-    def get_model_type(self):
-        from statsforecast.models import AutoETS as AutoETS_
+    def _get_model_type(self):
+        from statsforecast.models import AutoETS
 
-        return AutoETS_
+        return AutoETS
 
 
 class DynamicOptimizedThetaModel(AbstractStatsForecastModel):
     """Optimized Theta forecasting model from Fiorucci et al. (2016).
 
     Based on `statsforecast.models.DynamicOptimizedTheta <https://nixtla.github.io/statsforecast/models.html#dynamic-optimized-theta-method>`_.
 
@@ -254,23 +192,64 @@
         Seasonal decomposition type.
     seasonal_period : int or None, default = None
         Number of time steps in a complete seasonal cycle for seasonal models. For example, 7 for daily data with a
         weekly cycle or 12 for monthly data with an annual cycle.
         When set to None, seasonal_period will be inferred from the frequency of the training data. Can also be
         specified manually by providing an integer > 1.
         If seasonal_period (inferred or provided) is equal to 1, seasonality will be disabled.
-    n_jobs : int or float, default = 0.5
+    n_jobs : int or float, default = -1
         Number of CPU cores used to fit the models in parallel.
         When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
         When set to a positive integer, that many cores are used.
         When set to -1, all CPU cores are used.
     """
 
     allowed_local_model_args = [
         "decomposition_type",
         "seasonal_period",
     ]
 
-    def get_model_type(self):
+    def _get_model_type(self):
         from statsforecast.models import DynamicOptimizedTheta
 
         return DynamicOptimizedTheta
+
+
+class ThetaModel(AbstractStatsForecastModel):
+    """Theta forecasting model from Assimakopoulos and Nikolopoulos (2000).
+
+    Based on `statsforecast.models.Theta <https://nixtla.github.io/statsforecast/models.html#theta>`_.
+
+
+    References
+    ----------
+    Assimakopoulos, Vassilis, and Konstantinos Nikolopoulos.
+    "The theta model: a decomposition approach to forecasting."
+    International journal of forecasting 16.4 (2000): 521-530.
+
+
+    Other Parameters
+    ----------------
+    decomposition_type : {"multiplicative", "additive"}, default = "multiplicative"
+        Seasonal decomposition type.
+    seasonal_period : int or None, default = None
+        Number of time steps in a complete seasonal cycle for seasonal models. For example, 7 for daily data with a
+        weekly cycle or 12 for monthly data with an annual cycle.
+        When set to None, seasonal_period will be inferred from the frequency of the training data. Can also be
+        specified manually by providing an integer > 1.
+        If seasonal_period (inferred or provided) is equal to 1, seasonality will be disabled.
+    n_jobs : int or float, default = -1
+        Number of CPU cores used to fit the models in parallel.
+        When set to a float between 0.0 and 1.0, that fraction of available CPU cores is used.
+        When set to a positive integer, that many cores are used.
+        When set to -1, all CPU cores are used.
+    """
+
+    allowed_local_model_args = [
+        "decomposition_type",
+        "seasonal_period",
+    ]
+
+    def _get_model_type(self):
+        from statsforecast.models import Theta
+
+        return Theta
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import warnings
 from typing import Any, Callable, Dict, List
 
 import pandas as pd
 from statsmodels.tools.sm_exceptions import ConvergenceWarning, ModelWarning, ValueWarning
 
-from autogluon.timeseries.dataset.ts_dataframe import TimeSeriesDataFrame
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_single_time_series
 from autogluon.timeseries.utils.warning_filters import statsmodels_warning_filter
 
 from .abstract_local_model import AbstractLocalModel
 
 logger = logging.getLogger(__name__)
 
 warnings.simplefilter("ignore", ModelWarning)
 warnings.simplefilter("ignore", ConvergenceWarning)
 warnings.simplefilter("ignore", ValueWarning)
 
+from .abstract_local_model import AbstractLocalModel
+
 
 def get_quantiles_from_statsmodels(coverage_fn: Callable, quantile_levels: List[float]) -> List[pd.Series]:
     """Obtain quantile forecasts using a fitted Statsmodels model.
 
     The method for computing quantiles is different for all models in Statsmodels, this method unifies the interface.
 
     Parameters
@@ -93,17 +94,15 @@
         "trend",
         "damped_trend",
         "seasonal",
         "seasonal_period",
         "maxiter",
     ]
 
-    def _update_local_model_args(
-        self, local_model_args: Dict[str, Any], data: TimeSeriesDataFrame, **kwargs
-    ) -> Dict[str, Any]:
+    def _update_local_model_args(self, local_model_args: Dict[str, Any]) -> Dict[str, Any]:
         local_model_args.setdefault("trend", "add")
         local_model_args.setdefault("maxiter", 1000)
 
         seasonal_period = local_model_args.pop("seasonal_period")
         seasonal = local_model_args.setdefault("seasonal", "add")
         if seasonal is not None and seasonal_period <= 1:
             logger.warning(
@@ -113,38 +112,34 @@
             local_model_args["seasonal"] = None
             local_model_args["seasonal_periods"] = 1
         else:
             local_model_args["seasonal_periods"] = seasonal_period
 
         return local_model_args
 
-    @staticmethod
     def _predict_with_local_model(
+        self,
         time_series: pd.Series,
-        freq: str,
-        prediction_length: int,
-        quantile_levels: List[float],
         local_model_args: dict,
-        **kwargs,
     ) -> pd.DataFrame:
         forecast_timestamps = get_forecast_horizon_index_single_time_series(
-            past_timestamps=time_series.index, freq=freq, prediction_length=prediction_length
+            past_timestamps=time_series.index, freq=self.freq, prediction_length=self.prediction_length
         )
         from statsmodels.tsa.exponential_smoothing.ets import ETSModel
 
         maxiter = local_model_args.pop("maxiter")
 
         # Disable seasonality if timeseries is too short for given seasonal_period
         if local_model_args["seasonal"] is not None and len(time_series) < 2 * local_model_args["seasonal_periods"]:
             local_model_args["seasonal"] = None
 
         with statsmodels_warning_filter():
             model = ETSModel(
                 endog=time_series,
-                freq=freq,
+                freq=self.freq,
                 **local_model_args,
             )
             fit_result = model.fit(disp=False, maxiter=maxiter)
             predictions = fit_result.get_prediction(start=forecast_timestamps[0], end=forecast_timestamps[-1])
 
         results = [predictions.predicted_mean.rename("mean")]
         coverage_fn = lambda alpha: predictions.pred_int(alpha=alpha)
@@ -198,17 +193,15 @@
         "trend",
         "enforce_stationarity",
         "enforce_invertibility",
         "maxiter",
     ]
     MAX_TS_LENGTH = 3000
 
-    def _update_local_model_args(
-        self, local_model_args: Dict[str, Any], data: TimeSeriesDataFrame, **kwargs
-    ) -> Dict[str, Any]:
+    def _update_local_model_args(self, local_model_args: Dict[str, Any]) -> Dict[str, Any]:
         local_model_args.setdefault("trend", "c")
         local_model_args.setdefault("order", (1, 1, 1))
         local_model_args.setdefault("maxiter", 50)
 
         seasonal_period = local_model_args.pop("seasonal_period")
         seasonal_order = local_model_args.pop("seasonal_order", (0, 0, 0))
 
@@ -223,46 +216,42 @@
         if seasonal_period <= 1:
             local_model_args["seasonal_order"] = (0, 0, 0, 0)
         else:
             local_model_args["seasonal_order"] = tuple(seasonal_order) + (seasonal_period,)
 
         return local_model_args
 
-    @staticmethod
     def _predict_with_local_model(
+        self,
         time_series: pd.Series,
-        freq: str,
-        prediction_length: int,
-        quantile_levels: List[float],
         local_model_args: dict,
-        **kwargs,
     ) -> pd.DataFrame:
         forecast_timestamps = get_forecast_horizon_index_single_time_series(
-            past_timestamps=time_series.index, freq=freq, prediction_length=prediction_length
+            past_timestamps=time_series.index, freq=self.freq, prediction_length=self.prediction_length
         )
         from statsmodels.tsa.statespace.sarimax import SARIMAX as StatsmodelSARIMAX
 
         maxiter = local_model_args.pop("maxiter")
 
         with statsmodels_warning_filter():
             model = StatsmodelSARIMAX(
                 endog=time_series,
-                freq=freq,
+                freq=self.freq,
                 **local_model_args,
             )
             fit_result = model.fit(disp=False, maxiter=maxiter)
             predictions = fit_result.get_prediction(start=forecast_timestamps[0], end=forecast_timestamps[-1])
 
         results = [predictions.predicted_mean.rename("mean")]
         coverage_fn = lambda alpha: predictions.conf_int(alpha=alpha)
-        results += get_quantiles_from_statsmodels(coverage_fn=coverage_fn, quantile_levels=quantile_levels)
+        results += get_quantiles_from_statsmodels(coverage_fn=coverage_fn, quantile_levels=self.quantile_levels)
         return pd.concat(results, axis=1)
 
 
-class ThetaModel(AbstractLocalModel):
+class ThetaStatsmodelsModel(AbstractLocalModel):
     """The Theta forecasting model of Assimakopoulos and Nikolopoulos (2000).
 
     Based on `statsmodels.tsa.forecasting.theta.ThetaModel <https://www.statsmodels.org/stable/generated/statsmodels.tsa.forecasting.theta.ThetaModel.html>`_.
 
     Our implementation contains several improvements over the Statsmodels version, such
     as multi-CPU training and reducing the disk usage when saving models.
 
@@ -305,45 +294,39 @@
         "deseasonalize",
         "seasonal_period",
         "use_test",
         "method",
         "difference",
     ]
 
-    def _update_local_model_args(
-        self, local_model_args: Dict[str, Any], data: TimeSeriesDataFrame, **kwargs
-    ) -> Dict[str, Any]:
+    def _update_local_model_args(self, local_model_args: Dict[str, Any]) -> Dict[str, Any]:
         local_model_args.setdefault("deseasonalize", True)
 
         seasonal_period = local_model_args.pop("seasonal_period")
         local_model_args["period"] = seasonal_period
 
         return local_model_args
 
-    @staticmethod
     def _predict_with_local_model(
+        self,
         time_series: pd.Series,
-        freq: str,
-        prediction_length: int,
-        quantile_levels: List[float],
         local_model_args: dict,
-        **kwargs,
     ) -> pd.DataFrame:
         from statsmodels.tsa.forecasting.theta import ThetaModel as StatsmodelsTheta
 
         # Disable seasonality if timeseries is too short for given seasonal_period
         if local_model_args["deseasonalize"] and len(time_series) < 2 * local_model_args["period"]:
             local_model_args["deseasonalize"] = False
 
-        time_series.index.freq = freq
+        time_series.index.freq = self.freq
 
         with statsmodels_warning_filter():
             model = StatsmodelsTheta(
                 endog=time_series,
                 **local_model_args,
             )
             fit_result = model.fit(disp=False)
 
-        results = [fit_result.forecast(prediction_length).rename("mean")]
-        coverage_fn = lambda alpha: fit_result.prediction_intervals(steps=prediction_length, alpha=alpha)
-        results += get_quantiles_from_statsmodels(coverage_fn=coverage_fn, quantile_levels=quantile_levels)
+        results = [fit_result.forecast(self.prediction_length).rename("mean")]
+        coverage_fn = lambda alpha: fit_result.prediction_intervals(steps=self.prediction_length, alpha=alpha)
+        results += get_quantiles_from_statsmodels(coverage_fn=coverage_fn, quantile_levels=self.quantile_levels)
         return pd.concat(results, axis=1)
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,37 @@
     ETSModel,
     NaiveModel,
     RecursiveTabularModel,
     SeasonalNaiveModel,
     SimpleFeedForwardModel,
     TemporalFusionTransformerModel,
     ThetaModel,
+    ThetaStatsmodelsModel,
 )
 from .abstract import AbstractTimeSeriesModel, AbstractTimeSeriesModelFactory
 from .multi_window.multi_window_model import MultiWindowBacktestingModel
 
 logger = logging.getLogger(__name__)
 
 # define the model zoo with their aliases
 MODEL_TYPES = dict(
     SimpleFeedForward=SimpleFeedForwardModel,
     DeepAR=DeepARModel,
     TemporalFusionTransformer=TemporalFusionTransformerModel,
-    ETS=ETSModel,
-    ARIMA=ARIMAModel,
-    Theta=ThetaModel,
     AutoGluonTabular=AutoGluonTabularModel,
     RecursiveTabular=RecursiveTabularModel,
     Naive=NaiveModel,
     SeasonalNaive=SeasonalNaiveModel,
     AutoETS=AutoETSModel,
     AutoARIMA=AutoARIMAModel,
     DynamicOptimizedTheta=DynamicOptimizedThetaModel,
+    Theta=ThetaModel,
+    ARIMA=ARIMAModel,
+    ETS=ETSModel,
+    ThetaStatsmodels=ThetaStatsmodelsModel,
 )
 if agts.MXNET_INSTALLED:
     from .gluonts.mx import (
         DeepARMXNetModel,
         MQCNNMXNetModel,
         MQRNNMXNetModel,
         SimpleFeedForwardMXNetModel,
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import networkx as nx
 import pandas as pd
 from tqdm import tqdm
 
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.core.models import AbstractModel
+from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.core.utils.loaders import load_pkl
 from autogluon.core.utils.savers import save_json, save_pkl
 from autogluon.timeseries import TimeSeriesDataFrame, TimeSeriesEvaluator
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 from autogluon.timeseries.models.ensemble import AbstractTimeSeriesEnsembleModel, TimeSeriesGreedyEnsemble
 from autogluon.timeseries.models.presets import contains_searchspace
 from autogluon.timeseries.utils.features import CovariateMetadata
@@ -506,14 +507,16 @@
 
             if val_data is not None:
                 model.score_and_cache_oof(val_data, store_val_score=True, store_predict_time=True)
 
             self._log_scores_and_times(model.val_score, model.fit_time, model.predict_time)
 
             self.save_model(model=model)
+        except TimeLimitExceeded:
+            logger.error(f"\tTime limit exceeded... Skipping {model.name}.")
         except (Exception, MemoryError) as err:
             logger.error(f"\tWarning: Exception caused {model.name} to fail during training... Skipping this model.")
             logger.error(f"\t{err}")
             logger.debug(traceback.format_exc())
         else:
             self._add_model(model=model)  # noqa: F821
             model_names_trained.append(model.name)  # noqa: F821
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,18 +41,16 @@
         finally:
             pass
 
 
 @contextlib.contextmanager
 def statsmodels_joblib_warning_filter():
     env_py_warnings = os.environ.get("PYTHONWARNINGS", "")
-    warning_categories = [RuntimeWarning, UserWarning, FutureWarning]  # ignore these
     try:
-        # required to suppress gluonts evaluation warnings as the module uses multiprocessing
-        os.environ["PYTHONWARNINGS"] = ",".join([f"ignore::{c.__name__}" for c in warning_categories])
+        os.environ["PYTHONWARNINGS"] = "ignore"
         yield
     finally:
         os.environ["PYTHONWARNINGS"] = env_py_warnings
 
 
 @contextlib.contextmanager
 def disable_root_logger():
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230522
+Version: 0.7.1b20230523
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230522/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

