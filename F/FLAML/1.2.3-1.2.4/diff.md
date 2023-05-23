# Comparing `tmp/FLAML-1.2.3.tar.gz` & `tmp/FLAML-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-1.2.3.tar", last modified: Fri May  5 20:04:35 2023, max compression
+gzip compressed data, was "FLAML-1.2.4.tar", last modified: Tue May 23 16:02:59 2023, max compression
```

## Comparing `FLAML-1.2.3.tar` & `FLAML-1.2.4.tar`

### file list

```diff
@@ -1,132 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.513713 FLAML-1.2.3/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-05 20:03:33.000000 FLAML-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-05 20:03:33.000000 FLAML-1.2.3/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-05 20:04:35.525714 FLAML-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-05 20:03:33.000000 FLAML-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.513713 FLAML-1.2.3/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.513713 FLAML-1.2.3/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/autogen/agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/coding_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/execution_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/code_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/autogen/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44488 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/oai/completion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130309 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)   104984 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    37002 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-05 20:03:33.000000 FLAML-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:04:35.525714 FLAML-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-05 20:03:33.000000 FLAML-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 16:02:59.000000 FLAML-1.2.4/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-23 16:01:44.000000 FLAML-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-23 16:01:44.000000 FLAML-1.2.4/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-23 16:02:59.628680 FLAML-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-23 16:01:44.000000 FLAML-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/chat_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/coding_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/agent/user_proxy_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.612680 FLAML-1.2.4/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45993 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/oai/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/autogen/oai/openai_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130309 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104984 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.616680 FLAML-1.2.4/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.620680 FLAML-1.2.4/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.624680 FLAML-1.2.4/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23100 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37002 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 16:01:44.000000 FLAML-1.2.4/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 16:01:44.000000 FLAML-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:02:59.628680 FLAML-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-23 16:01:44.000000 FLAML-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:02:59.628680 FLAML-1.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 16:01:44.000000 FLAML-1.2.4/test/test_version.py
```

### Comparing `FLAML-1.2.3/FLAML.egg-info/PKG-INFO` & `FLAML-1.2.4/FLAML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.3
+Version: 1.2.4
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FLAML-1.2.3/FLAML.egg-info/SOURCES.txt` & `FLAML-1.2.4/FLAML.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 flaml/model.py
 flaml/version.py
 flaml/autogen/__init__.py
 flaml/autogen/code_utils.py
 flaml/autogen/math_utils.py
 flaml/autogen/agent/__init__.py
 flaml/autogen/agent/agent.py
+flaml/autogen/agent/chat_agent.py
 flaml/autogen/agent/coding_agent.py
-flaml/autogen/agent/execution_agent.py
+flaml/autogen/agent/user_proxy_agent.py
 flaml/autogen/extensions/__init__.py
 flaml/autogen/oai/__init__.py
 flaml/autogen/oai/completion.py
+flaml/autogen/oai/openai_utils.py
 flaml/automl/__init__.py
 flaml/automl/automl.py
 flaml/automl/data.py
 flaml/automl/logger.py
 flaml/automl/ml.py
 flaml/automl/model.py
 flaml/automl/state.py
```

### Comparing `FLAML-1.2.3/FLAML.egg-info/requires.txt` & `FLAML-1.2.4/FLAML.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/LICENSE` & `FLAML-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/NOTICE.md` & `FLAML-1.2.4/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/PKG-INFO` & `FLAML-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.3
+Version: 1.2.4
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FLAML-1.2.3/README.md` & `FLAML-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/autogen/agent/agent.py` & `FLAML-1.2.4/flaml/autogen/agent/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from collections import defaultdict
 
 
 class Agent:
     """(Experimental) An abstract class for AI agent.
-    An agent can communicate with other agents, human and perform actions.
-    Different agents can differ in how and who they communicate with, and what actions they can perform. For example, an autonomous agent can communicate with human and other agents, and perform actions by creating agents and sending messages to other agents. A planning agent can communicate with other agents to make a plan and keep track of tasks. An execution agent can only communicate with other agents, and perform actions such as executing a command or code.
+    An agent can communicate with other agents and perform actions.
+    Different agents can differ in what actions they perform in the `receive` method.
+
     """
 
     def __init__(self, name, system_message=""):
+        """
+        Args:
+            name (str): name of the agent
+            system_message (str): system message to be sent to the agent
+        """
         # empty memory
         self._memory = []
         # a dictionary of conversations, default value is list
         self._conversations = defaultdict(list)
         self._name = name
         self._system_message = system_message
 
@@ -27,15 +33,16 @@
     def _send(self, message, recipient):
         """Send a message to another agent."""
         self._conversations[recipient.name].append({"content": message, "role": "assistant"})
         recipient.receive(message, self)
 
     def _receive(self, message, sender):
         """Receive a message from another agent."""
-        # print(self.name, "received message from", sender.name, ":", message)
+        print("\n****", self.name, "received message from", sender.name, "****\n")
+        print(message)
         self._conversations[sender.name].append({"content": message, "role": "user"})
 
     def receive(self, message, sender):
         """Receive a message from another agent.
         This method is called by the sender.
         It needs to be overriden by the subclass to perform followup actions.
         """
```

### Comparing `FLAML-1.2.3/flaml/autogen/code_utils.py` & `FLAML-1.2.4/flaml/autogen/code_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,38 +33,36 @@
         config (Optional, dict): The configuration for the API call.
 
     Returns:
         str: The generated code.
         float: The cost of the generation.
     """
     response = oai.Completion.create(**config)
-    cost = oai.Completion.cost(response)
-    return extract_code(oai.Completion.extract_text(response)[0], pattern), cost
+    return extract_code(oai.Completion.extract_text(response)[0], pattern), response["cost"]
 
 
 _IMPROVE_FUNCTION_CONFIG = {
     "prompt": """Improve the function '{func_name}' to achieve the objective '{objective}'.
 The current implementation of the function is as follows:
 {file_string}""",
     "model": DEFAULT_MODEL,
-    "request_timeout": 300,
+    "request_timeout": 600,
 }
 
 
 def improve_function(file_name, func_name, objective, **config):
     """(work in progress) Improve the function to achieve the objective."""
     params = {**_IMPROVE_FUNCTION_CONFIG, **config}
     # read the entire file into a str
     with open(file_name, "r") as f:
         file_string = f.read()
     response = oai.Completion.create(
         {"func_name": func_name, "objective": objective, "file_string": file_string}, **params
     )
-    cost = oai.Completion.cost(response)
-    return oai.Completion.extract_text(response)[0], cost
+    return oai.Completion.extract_text(response)[0], response["cost"]
 
 
 _IMPROVE_CODE_CONFIG = {
     "prompt": """Analyze the code in the following files and return a list of suggestions for improvement{followup}, to achieve the objective of '{objective}'.
 {code}
 """,
     "model": DEFAULT_MODEL,
@@ -93,16 +91,15 @@
         code += f"""{file_name}:
 {file_string}
 
 """
     params = {**_IMPROVE_CODE_CONFIG, **config}
     followup = "" if suggest_only else " followed by the improved code"
     response = oai.Completion.create({"objective": objective, "code": code, "followup": followup}, **params)
-    cost = oai.Completion.cost(response)
-    return oai.Completion.extract_text(response)[0], cost
+    return oai.Completion.extract_text(response)[0], response["cost"]
 
 
 def timeout_handler(signum, frame):
     raise TimeoutError("Timed out!")
 
 
 def execute_code(
@@ -277,17 +274,16 @@
         float: The cost of the generation.
     """
     params = {**_GENERATE_ASSERTIONS_CONFIG, **config}
     response = oai.Completion.create(
         {"definition": definition},
         **params,
     )
-    cost = oai.Completion.cost(response)
     assertions = oai.Completion.extract_text(response)[0]
-    return assertions, cost
+    return assertions, response["cost"]
 
 
 def _remove_check(response):
     """Remove the check function from the response."""
     # find the position of the check function
     pos = response.find("def check(")
     if pos == -1:
@@ -383,14 +379,31 @@
     {"model": FAST_MODEL, "prompt": _FUNC_COMPLETION_PROMPT, "stop": _FUNC_COMPLETION_STOP, "n": 7, "seed": 0},
     {"model": DEFAULT_MODEL, "prompt": _FUNC_COMPLETION_PROMPT, "temperature": 0, "seed": 1},
     {"model": DEFAULT_MODEL, "prompt": _FUNC_COMPLETION_PROMPT, "stop": _FUNC_COMPLETION_STOP, "n": 2, "seed": 2},
     {"model": DEFAULT_MODEL, "prompt": _FUNC_COMPLETION_PROMPT, "stop": _FUNC_COMPLETION_STOP, "n": 1, "seed": 2},
 ]
 
 
+class PassAssertionFilter:
+    def __init__(self, assertions):
+        self._assertions = assertions
+        self.cost = 0
+        self.metrics = self.responses = None
+
+    def pass_assertions(self, context, response, **_):
+        """Check if the response passes the assertions."""
+        responses = oai.Completion.extract_text(response)
+        metrics = eval_function_completions(responses, context["definition"], assertions=self._assertions)
+        self._assertions = metrics["assertions"]
+        self.cost += metrics["gen_cost"]
+        self.metrics = metrics
+        self.responses = responses
+        return metrics["succeed_assertions"]
+
+
 def implement(
     definition: str,
     configs: Optional[List[Dict]] = None,
     assertions: Optional[Union[str, Callable[[str], Tuple[str, float]]]] = generate_assertions,
 ) -> Tuple[str, float]:
     """Implement a function from a definition.
 
@@ -404,16 +417,23 @@
         float: The cost of the implementation.
         int: The index of the configuration which generates the implementation.
     """
     cost = 0
     configs = configs or _IMPLEMENT_CONFIGS
     if len(configs) > 1 and callable(assertions):
         assertions, cost = assertions(definition)
-    for i, config in enumerate(configs):
-        response = oai.Completion.create({"definition": definition}, **config)
-        cost += oai.Completion.cost(response)
-        responses = oai.Completion.extract_text(response)
-        metrics = eval_function_completions(responses, definition, assertions=assertions)
-        assertions = metrics["assertions"]
-        cost += metrics["gen_cost"]
-        if metrics["succeed_assertions"] or i == len(configs) - 1:
-            return responses[metrics["index_selected"]], cost, i
+    assertion_filter = PassAssertionFilter(assertions)
+    response = oai.Completion.create(
+        {"definition": definition}, config_list=configs, filter_func=assertion_filter.pass_assertions
+    )
+    cost += assertion_filter.cost + response["cost"]
+    return assertion_filter.responses[assertion_filter.metrics["index_selected"]], cost, response["config_id"]
+
+    # for i, config in enumerate(configs):
+    #     response = oai.Completion.create({"definition": definition}, **config)
+    #     cost += oai.Completion.cost(response)
+    #     responses = oai.Completion.extract_text(response)
+    #     metrics = eval_function_completions(responses, definition, assertions=assertions)
+    #     assertions = metrics["assertions"]
+    #     cost += metrics["gen_cost"]
+    #     if metrics["succeed_assertions"] or i == len(configs) - 1:
+    #         return responses[metrics["index_selected"]], cost, i
```

### Comparing `FLAML-1.2.3/flaml/autogen/math_utils.py` & `FLAML-1.2.4/flaml/autogen/math_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
         config (Optional, dict): The configuration for the API call.
 
     Returns:
         str: The solution to the problem.
     """
     params = {**_MATH_CONFIG, **config}
     response = oai.Completion.create({"problem": problem}, **params)
-    cost = oai.Completion.cost(response)
     results = eval_math_responses(oai.Completion.extract_text(response))
-    return results.get("voted_answer"), cost
+    return results.get("voted_answer"), response["cost"]
 
 
 def remove_boxed(string: str) -> Optional[str]:
     """Source: https://github.com/hendrycks/math
     Extract the text within a \\boxed{...} environment.
     Example:
     >>> remove_boxed(\\boxed{\\frac{2}{3}})
```

### Comparing `FLAML-1.2.3/flaml/autogen/oai/completion.py` & `FLAML-1.2.4/flaml/autogen/oai/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from time import sleep
 import logging
 import numpy as np
 import time
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Callable, Any
 import sys
-import json
+import shutil
 from flaml import tune, BlendSearch
+from flaml.tune.space import is_constant
 from flaml.automl.logger import logger_formatter
+from .openai_utils import get_key
 
 try:
     import openai
     from openai.error import (
         ServiceUnavailableError,
         RateLimitError,
         APIError,
         InvalidRequestError,
         APIConnectionError,
         Timeout,
+        AuthenticationError,
     )
     from openai import Completion as openai_Completion
     import diskcache
 
     ERROR = None
 except ImportError:
     ERROR = ImportError("please install flaml[openai] option to use the flaml.oai subpackage.")
@@ -29,31 +32,14 @@
 if not logger.handlers:
     # Add the console handler.
     _ch = logging.StreamHandler(stream=sys.stdout)
     _ch.setFormatter(logger_formatter)
     logger.addHandler(_ch)
 
 
-def get_key(config):
-    """Get a unique identifier of a configuration.
-
-    Args:
-        config (dict or list): A configuration.
-
-    Returns:
-        tuple: A unique identifier which can be used as a key for a dict.
-    """
-    # if isinstance(config, dict):
-    #     return tuple(get_key(x) for x in sorted(config.items()))
-    # if isinstance(config, list):
-    #     return tuple(get_key(x) for x in config)
-    # return config
-    return json.dumps(config, sort_keys=True)
-
-
 class Completion(openai_Completion):
     """A class for OpenAI completion API.
 
     It also supports: ChatCompletion, Azure OpenAI API.
     """
 
     # set of models that support chat completion
@@ -93,15 +79,15 @@
                 "text-davinci-003",
                 "gpt-3.5-turbo",
                 "gpt-4",
             ]
         ),
         "temperature_or_top_p": tune.choice(
             [
-                {"temperature": tune.uniform(0, 1)},
+                {"temperature": tune.uniform(0, 2)},
                 {"top_p": tune.uniform(0, 1)},
             ]
         ),
         "max_tokens": tune.lograndint(50, 1000),
         "n": tune.randint(1, 100),
         "prompt": "{prompt}",
     }
@@ -118,29 +104,47 @@
     openai_completion_class = not ERROR and openai.Completion
     _total_cost = 0
     optimization_budget = None
 
     _history_dict = _count_create = None
 
     @classmethod
-    def set_cache(cls, seed=41, cache_path=".cache"):
+    def set_cache(cls, seed: Optional[int] = 41, cache_path_root: Optional[str] = ".cache"):
         """Set cache path.
 
         Args:
             seed (int, Optional): The integer identifier for the pseudo seed.
                 Results corresponding to different seeds will be cached in different places.
             cache_path (str, Optional): The root path for the cache.
                 The complete cache path will be {cache_path}/{seed}.
         """
         cls.seed = seed
-        cls.cache_path = f"{cache_path}/{seed}"
+        cls.cache_path = f"{cache_path_root}/{seed}"
+
+    @classmethod
+    def clear_cache(cls, seed: Optional[int] = None, cache_path_root: Optional[str] = ".cache"):
+        """Clear cache.
+
+        Args:
+            seed (int, Optional): The integer identifier for the pseudo seed.
+                If omitted, all caches under cache_path_root will be cleared.
+            cache_path (str, Optional): The root path for the cache.
+                The complete cache path will be {cache_path}/{seed}.
+        """
+        if seed is None:
+            shutil.rmtree(cache_path_root, ignore_errors=True)
+            return
+        with diskcache.Cache(f"{cache_path_root}/{seed}") as cache:
+            cache.clear()
 
     @classmethod
     def _book_keeping(cls, config: Dict, response):
         """Book keeping for the created completions."""
+        if response != -1 and "cost" not in response:
+            response["cost"] = cls.cost(response)
         if cls._history_dict is None:
             return
         if cls._history_compact:
             value = {
                 "created_at": [],
                 "cost": [],
             }
@@ -149,104 +153,103 @@
                 if len(messages) > 1 and messages[-1]["role"] != "assistant":
                     existing_key = get_key(messages[:-1])
                     value = cls._history_dict.pop(existing_key, value)
                 key = get_key(messages + [choice["message"] for choice in response["choices"]])
             else:
                 key = get_key([config["prompt"]] + [choice.get("text") for choice in response["choices"]])
             value["created_at"].append(cls._count_create)
-            value["cost"].append(cls.cost(response))
+            value["cost"].append(response["cost"])
             cls._history_dict[key] = value
             cls._count_create += 1
             return
         cls._history_dict[cls._count_create] = {
             "request": config,
             "response": response.to_dict_recursive(),
         }
         cls._count_create += 1
 
     @classmethod
-    def _get_response(cls, config: Dict, eval_only=False, use_cache=True):
+    def _get_response(cls, config: Dict, raise_error=False, use_cache=True):
         """Get the response from the openai api call.
 
         Try cache first. If not found, call the openai api. If the api call fails, retry after retry_time.
         """
         config = config.copy()
-        openai.api_key = config.pop("api_key", openai.api_key)
-        openai.api_base = config.pop("api_base", openai.api_base)
         openai.api_key_path = config.pop("api_key_path", openai.api_key_path)
-        openai.api_type = config.pop("api_type", openai.api_type)
-        openai.api_version = config.pop("api_version", openai.api_version)
         key = get_key(config)
         if use_cache:
             response = cls._cache.get(key, None)
-            if response is not None and (response != -1 or not eval_only):
+            if response is not None and (response != -1 or not raise_error):
                 # print("using cached response")
                 cls._book_keeping(config, response)
                 return response
-        openai_completion = openai.ChatCompletion if config["model"] in cls.chat_models else openai.Completion
+        openai_completion = (
+            openai.ChatCompletion
+            if config["model"] in cls.chat_models or issubclass(cls, ChatCompletion)
+            else openai.Completion
+        )
         start_time = time.time()
         request_timeout = cls.request_timeout
         while True:
             try:
                 if "request_timeout" in config:
                     response = openai_completion.create(**config)
                 else:
                     response = openai_completion.create(request_timeout=request_timeout, **config)
             except (
                 ServiceUnavailableError,
                 APIConnectionError,
             ):
                 # transient error
-                logger.warning(f"retrying in {cls.retry_time} seconds...", exc_info=1)
+                logger.info(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 sleep(cls.retry_time)
             except APIError as err:
                 error_code = err and err.json_body and err.json_body.get("error")
                 error_code = error_code and error_code.get("code")
                 if error_code == "content_filter":
                     raise
                 # transient error
-                logger.warning(f"retrying in {cls.retry_time} seconds...", exc_info=1)
+                logger.info(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 sleep(cls.retry_time)
             except (RateLimitError, Timeout) as err:
                 time_left = cls.retry_timeout - (time.time() - start_time + cls.retry_time)
                 if (
                     time_left > 0
                     and isinstance(err, RateLimitError)
                     or time_left > request_timeout
                     and isinstance(err, Timeout)
                 ):
                     logger.info(f"retrying in {cls.retry_time} seconds...", exc_info=1)
-                elif eval_only:
+                elif raise_error:
                     raise
                 else:
-                    break
+                    response = -1
+                    if use_cache and isinstance(err, Timeout):
+                        cls._cache.set(key, response)
+                    logger.warning(
+                        f"Failed to get response from openai api due to getting RateLimitError or Timeout for {cls.retry_timeout} seconds."
+                    )
+                    return response
                 if isinstance(err, Timeout):
                     if "request_timeout" in config:
                         raise
                     request_timeout <<= 1
                 request_timeout = min(request_timeout, time_left)
                 sleep(cls.retry_time)
             except InvalidRequestError:
-                if "azure" == openai.api_type and "model" in config:
+                if "azure" == config.get("api_type", openai.api_type) and "model" in config:
                     # azure api uses "engine" instead of "model"
                     config["engine"] = config.pop("model").replace("gpt-3.5-turbo", "gpt-35-turbo")
                 else:
                     raise
             else:
                 if use_cache:
                     cls._cache.set(key, response)
                 cls._book_keeping(config, response)
                 return response
-        logger.warning(
-            f"Failed to get response from openai api due to getting RateLimitError or Timeout for {cls.retry_timeout} seconds."
-        )
-        response = -1
-        if use_cache:
-            cls._cache.set(key, response)
-        return response
 
     @classmethod
     def _get_max_valid_n(cls, key, max_tokens):
         # find the max value in max_valid_n_per_max_tokens
         # whose key is equal or larger than max_tokens
         return max(
             (value for k, value in cls._max_valid_n_per_max_tokens.get(key, {}).items() if k >= max_tokens),
@@ -261,14 +264,15 @@
             (value for k, value in cls._min_invalid_n_per_max_tokens.get(key, {}).items() if k <= max_tokens),
             default=None,
         )
 
     @classmethod
     def _get_region_key(cls, config):
         # get a key for the valid/invalid region corresponding to the given config
+        config = cls._pop_subspace(config, always_copy=False)
         return (
             config["model"],
             config.get("prompt", config.get("messages")),
             config.get("stop"),
         )
 
     @classmethod
@@ -277,67 +281,65 @@
             # update invalid n and prune this config
             cls._min_invalid_n_per_max_tokens[region_key] = invalid_n = cls._min_invalid_n_per_max_tokens.get(
                 region_key, {}
             )
             invalid_n[max_tokens] = min(num_completions, invalid_n.get(max_tokens, np.inf))
 
     @classmethod
-    def _pop_subspace(cls, config):
+    def _pop_subspace(cls, config, always_copy=True):
         if "subspace" in config:
             config = config.copy()
             config.update(config.pop("subspace"))
-        return config
+        return config.copy() if always_copy else config
 
     @classmethod
-    def _get_prompt_messages_from_config(cls, model, config):
-        prompt, messages = None, None
-        if model in cls.chat_models:
-            # either "prompt" should be in config (for being compatible with non-chat models)
-            # or "messages" should be in config (for tuning chat models only)
-            prompt = config.get("prompt")
-            messages = config.get("messages")
-            # either prompt or messages should be in config, but not both
-            assert (prompt is None) != (
-                messages is None
-            ), "Either prompt or messages should be in config for chat models."
-            if prompt is None:
-                messages = cls._messages[messages]
-            else:
-                prompt = cls._prompts[prompt]
+    def _get_params_for_create(cls, config: Dict) -> Dict:
+        """Get the params for the openai api call from a config in the search space."""
+        params = cls._pop_subspace(config)
+        if cls._prompts:
+            params["prompt"] = cls._prompts[config["prompt"]]
         else:
-            prompt = cls._prompts[config["prompt"]]
-        return prompt, messages
+            params["messages"] = cls._messages[config["messages"]]
+        if "stop" in params:
+            params["stop"] = cls._stops and cls._stops[params["stop"]]
+        temperature_or_top_p = params.pop("temperature_or_top_p", None)
+        if temperature_or_top_p:
+            params.update(temperature_or_top_p)
+        if cls._config_list and "config_list" not in params:
+            params["config_list"] = cls._config_list
+        return params
 
     @classmethod
     def _eval(cls, config: dict, prune=True, eval_only=False):
         """Evaluate the given config as the hyperparameter setting for the openai api call.
 
         Args:
             config (dict): Hyperparameter setting for the openai api call.
             prune (bool, optional): Whether to enable pruning. Defaults to True.
-            eval_only (bool, optional): Whether to evaluate only (ignore the inference budget and no timeout).
+            eval_only (bool, optional): Whether to evaluate only
+              (ignore the inference budget and do not rasie error when a request fails).
               Defaults to False.
 
         Returns:
             dict: Evaluation results.
         """
         cost = 0
         data = cls.data
-        config = cls._pop_subspace(config)
-        model = config["model"]
+        params = cls._get_params_for_create(config)
+        model = params["model"]
         data_length = len(data)
         price = cls.price1K.get(model)
         price_input, price_output = price if isinstance(price, tuple) else (price, price)
         inference_budget = getattr(cls, "inference_budget", None)
         prune_hp = getattr(cls, "_prune_hp", "n")
         metric = cls._metric
-        config_n = config.get(prune_hp, 1)  # default value in OpenAI is 1
-        max_tokens = config.get("max_tokens", np.inf if model in cls.chat_models else 16)
-        prompt, messages = cls._get_prompt_messages_from_config(model, config)
-        stop = cls._stops and cls._stops[config["stop"]]
+        config_n = params.get(prune_hp, 1)  # default value in OpenAI is 1
+        max_tokens = params.get(
+            "max_tokens", np.inf if model in cls.chat_models or issubclass(cls, ChatCompletion) else 16
+        )
         target_output_tokens = None
         if not cls.avg_input_tokens:
             input_tokens = [None] * data_length
         prune = prune and inference_budget and not eval_only
         if prune:
             region_key = cls._get_region_key(config)
             max_valid_n = cls._get_max_valid_n(region_key, max_tokens)
@@ -360,48 +362,42 @@
                         metric: np.inf if cls._mode == "min" else -np.inf,
                         "cost": cost,
                     }
                 start_n = max_valid_n + 1
         else:
             start_n = config_n
             region_key = None
-        params = config.copy()
-        if "stop" in config:
-            params["stop"] = stop
-        temperature_or_top_p = params.pop("temperature_or_top_p", None)
-        if temperature_or_top_p:
-            params.update(temperature_or_top_p)
         num_completions, previous_num_completions = start_n, 0
         n_tokens_list, result, responses_list = [], {}, []
         while True:  # n <= config_n
             params[prune_hp] = num_completions - previous_num_completions
             data_limit = 1 if prune else data_length
             prev_data_limit = 0
             data_early_stop = False  # whether data early stop happens for this n
             while True:  # data_limit <= data_length
                 # limit the number of data points to avoid rate limit
                 for i in range(prev_data_limit, data_limit):
                     logger.debug(f"num_completions={num_completions}, data instance={i}")
                     data_i = data[i]
-                    params = cls._construct_params(data_i, params, prompt, messages)
-                    response = cls._get_response(params, eval_only)
-                    if response == -1:  # rate limit error, treat as invalid
+                    # params = cls._construct_params(data_i, params, prompt, messages)
+                    response = cls.create(data_i, raise_error=eval_only, **params)
+                    if response == -1:  # rate limit/timeout error, treat as invalid
                         cls._update_invalid_n(prune, region_key, max_tokens, num_completions)
                         result[metric] = 0
                         result["cost"] = cost
                         return result
                     # evaluate the quality of the responses
                     responses = cls.extract_text(response)
                     usage = response["usage"]
                     n_input_tokens = usage["prompt_tokens"]
                     n_output_tokens = usage.get("completion_tokens", 0)
                     if not cls.avg_input_tokens and not input_tokens[i]:
                         # store the # input tokens
                         input_tokens[i] = n_input_tokens
-                    query_cost = (price_input * n_input_tokens + price_output * n_output_tokens) / 1000
+                    query_cost = response["cost"]
                     cls._total_cost += query_cost
                     cost += query_cost
                     if cls.optimization_budget and cls._total_cost >= cls.optimization_budget and not eval_only:
                         # limit the total tuning cost
                         return {
                             metric: 0,
                             "total_cost": cls._total_cost,
@@ -484,23 +480,23 @@
                     previous_num_completions = num_completions
                 num_completions = min(num_completions << 1, config_n)
         return result
 
     @classmethod
     def tune(
         cls,
-        data,
-        metric,
-        mode,
-        eval_func,
-        log_file_name=None,
-        inference_budget=None,
-        optimization_budget=None,
-        num_samples=1,
-        logging_level=logging.WARNING,
+        data: List[Dict],
+        metric: str,
+        mode: str,
+        eval_func: Callable,
+        log_file_name: Optional[str] = None,
+        inference_budget: Optional[float] = None,
+        optimization_budget: Optional[float] = None,
+        num_samples: Optional[int] = 1,
+        logging_level: Optional[int] = logging.WARNING,
         **config,
     ):
         """Tune the parameters for the OpenAI API call.
 
         TODO: support parallel tuning with ray or spark.
         TODO: support agg_method as in test
 
@@ -592,14 +588,19 @@
         if cls._stops:
             assert isinstance(
                 cls._stops, (str, list)
             ), "stop must be a string, a list of strings, or a list of lists of strings."
             if not (isinstance(cls._stops, list) and isinstance(cls._stops[0], list)):
                 cls._stops = [cls._stops]
             space["stop"] = tune.choice(list(range(len(cls._stops))))
+        cls._config_list = space.get("config_list")
+        if cls._config_list is not None:
+            is_const = is_constant(cls._config_list)
+            if is_const:
+                space.pop("config_list")
         cls._metric, cls._mode = metric, mode
         cls._total_cost = 0  # total optimization cost
         cls._eval_func = eval_func
         cls.data = data
         cls.avg_input_tokens = None
 
         space_model = space["model"]
@@ -658,40 +659,35 @@
                 cls._eval,
                 search_alg=search_alg,
                 num_samples=num_samples,
                 log_file_name=log_file_name,
                 verbose=3,
             )
         config = analysis.best_config
-        params = cls._pop_subspace(config)
-        if cls._prompts:
-            params["prompt"] = cls._prompts[config["prompt"]]
-        else:
-            params["messages"] = cls._messages[config["messages"]]
-        stop = cls._stops and cls._stops[config["stop"]]
-        params["stop"] = stop
-        temperature_or_top_p = params.pop("temperature_or_top_p", None)
-        if temperature_or_top_p:
-            params.update(temperature_or_top_p)
+        params = cls._get_params_for_create(config)
+        if cls._config_list is not None and is_const:
+            params.pop("config_list")
         logger.setLevel(old_level)
         return params, analysis
 
     @classmethod
     def create(
         cls,
         context: Optional[Dict] = None,
         use_cache: Optional[bool] = True,
-        config_list: Optional[List] = None,
+        config_list: Optional[List[Dict]] = None,
+        filter_func: Optional[Callable[[Dict, Dict, Dict], bool]] = None,
+        raise_error: Optional[bool] = True,
         **config,
     ):
         """Make a completion for a given context.
 
         Args:
             context (Dict, Optional): The context to instantiate the prompt.
-                It needs to contain keys that are used by the prompt template.
+                It needs to contain keys that are used by the prompt template or the filter function.
                 E.g., `prompt="Complete the following sentence: {prefix}, context={"prefix": "Today I feel"}`.
                 The actual prompt will be:
                 "Complete the following sentence: Today I feel".
                 More examples can be found at [templating](/docs/Use-Cases/Auto-Generation#templating).
             use_cache (bool, Optional): Whether to use cached responses.
             config_list (List, Optional): List of configurations for the completion to try.
                 The first one that does not raise an error will be used.
@@ -709,61 +705,81 @@
                     "api_version": "2023-03-15-preview",
                 },
                 {
                     "model": "gpt-3.5-turbo",
                     "api_key": os.environ.get("OPENAI_API_KEY"),
                     "api_type": "open_ai",
                     "api_base": "https://api.openai.com/v1",
-                    "api_version": None,
                 },
                 {
                     "model": "llama-7B",
                     "api_base": "http://127.0.0.1:8080",
                     "api_type": "open_ai",
-                    "api_version": None,
                 }
             ],
             prompt="Hi",
         )
         ```
 
+            filter_func (Callable, Optional): A function that takes in the context, the config and the response and returns a boolean to indicate whether the response is valid. E.g.,
+
+        ```python
+        def yes_or_no_filter(context, config, response):
+            return context.get("yes_or_no_choice", False) is False or any(
+                text in ["Yes.", "No."] for text in oai.Completion.extract_text(response)
+            )
+        ```
+
+            raise_error (bool, Optional): Whether to raise error when all configs fail.
+                When set to False, -1 will be returned when all configs fail.
             **config: Configuration for the completion.
                 Besides the parameters for the openai API call, it can also contain a seed (int) for the cache.
                 This is useful when implementing "controlled randomness" for the completion.
                 Also, the "prompt" or "messages" parameter can contain a template (str or Callable) which will be instantiated with the context.
 
         Returns:
             Responses from OpenAI API.
         """
         if ERROR:
             raise ERROR
         if config_list:
             retry_timeout = cls.retry_timeout
+            last = len(config_list) - 1
+            cost = 0
             for i, each_config in enumerate(config_list):
                 base_config = config.copy()
                 base_config.update(each_config)
                 try:
-                    cls.retry_timeout = 0 if i < len(config_list) - 1 else retry_timeout
-                    # retry_timeout = 0 to avoid retrying
-                    return cls.create(context, use_cache, **base_config)
-                except (RateLimitError, Timeout):
-                    logger.info(f"failed with config {i}", exc_info=1)
-                    if i == len(config_list) - 1:
+                    cls.retry_timeout = 0 if i < last and filter_func is None else retry_timeout
+                    # retry_timeout = 0 to avoid retrying when no filter is given
+                    response = cls.create(context, use_cache, **base_config)
+                    pass_filter = filter_func is None or filter_func(
+                        context=context, base_config=config, response=response
+                    )
+                    if pass_filter or i == last:
+                        response["cost"] = cost + response["cost"]
+                        response["config_id"] = i
+                        response["pass_filter"] = pass_filter
+                        return response
+                    cost += response["cost"]
+                except (AuthenticationError, RateLimitError, Timeout):
+                    logger.debug(f"failed with config {i}", exc_info=1)
+                    if i == last:
                         raise
                 finally:
                     cls.retry_timeout = retry_timeout
         params = cls._construct_params(context, config)
         if not use_cache:
-            return cls._get_response(params, eval_only=True, use_cache=False)
+            return cls._get_response(params, raise_error=raise_error, use_cache=False)
         seed = cls.seed
         if "seed" in params:
             cls.set_cache(params.pop("seed"))
         with diskcache.Cache(cls.cache_path) as cls._cache:
             cls.set_cache(seed)
-            return cls._get_response(params, eval_only=True)
+            return cls._get_response(params, raise_error=raise_error)
 
     @classmethod
     def _instantiate(cls, template: str, context: Optional[Dict] = None):
         if not context:
             return template
         if isinstance(template, str):
             return template.format(**context)
@@ -773,30 +789,30 @@
     def _construct_params(cls, data_instance, config, prompt=None, messages=None):
         params = config.copy()
         model = config["model"]
         prompt = config.get("prompt") if prompt is None else prompt
         messages = config.get("messages") if messages is None else messages
         # either "prompt" should be in config (for being compatible with non-chat models)
         # or "messages" should be in config (for tuning chat models only)
-        if prompt is None and model in cls.chat_models:
+        if prompt is None and (model in cls.chat_models or issubclass(cls, ChatCompletion)):
             if messages is None:
                 raise ValueError("Either prompt or messages should be in config for chat models.")
         if prompt is None:
             params["messages"] = (
                 [
                     {
                         "role": m["role"],
                         "content": cls._instantiate(m["content"], data_instance),
                     }
                     for m in messages
                 ]
                 if data_instance
                 else messages
             )
-        elif model in cls.chat_models:
+        elif model in cls.chat_models or issubclass(cls, ChatCompletion):
             # convert prompt to messages
             params["messages"] = [
                 {
                     "role": "user",
                     "content": cls._instantiate(prompt, data_instance),
                 },
             ]
@@ -805,26 +821,25 @@
             params["prompt"] = cls._instantiate(prompt, data_instance)
         return params
 
     @classmethod
     def test(
         cls,
         data,
-        config,
         eval_func=None,
         use_cache=True,
         agg_method="avg",
         return_responses_and_per_instance_result=False,
         logging_level=logging.WARNING,
+        **config,
     ):
         """Evaluate the responses created with the config for the OpenAI API call.
 
         Args:
             data (list): The list of test data points.
-            config (dict): Hyperparameter setting for the openai api call.
             eval_func (Callable): The evaluation function for responses per data instance.
                 The function should take a list of responses and a data point as input,
                 and return a dict of metrics. You need to either provide a valid callable
                 eval_func; or do not provide one (set None) but call the test function after
                 calling the tune function in which a eval_func is provided.
                 In the latter case we will use the eval_func provided via tune function.
                 Defaults to None.
@@ -862,29 +877,30 @@
         ```python
         agg_method={'median_success': np.median, 'avg_success': np.mean}
         ```
 
             return_responses_and_per_instance_result (bool): Whether to also return responses
                 and per instance results in addition to the aggregated results.
             logging_level (optional): logging level. Defaults to logging.WARNING.
+            **config (dict): parametes passed to the openai api call `create()`.
 
         Returns:
             None when no valid eval_func is provided in either test or tune;
             Otherwise, a dict of aggregated results, responses and per instance results if `return_responses_and_per_instance_result` is True;
             Otherwise, a dict of aggregated results (responses and per instance results are not returned).
         """
         result_agg, responses_list, result_list = {}, [], []
         metric_keys = None
         cost = 0
         old_level = logger.getEffectiveLevel()
         logger.setLevel(logging_level)
         for i, data_i in enumerate(data):
             logger.info(f"evaluating data instance {i}")
             response = cls.create(data_i, use_cache, **config)
-            cost += cls.cost(response)
+            cost += response["cost"]
             # evaluate the quality of the responses
             responses = cls.extract_text(response)
             if eval_func is not None:
                 metrics = eval_func(responses, **data_i)
             elif hasattr(cls, "_eval_func"):
                 metrics = cls._eval_func(responses, **data_i)
             else:
@@ -942,19 +958,20 @@
     def cost(cls, response: dict):
         """Compute the cost of an API call.
 
         Args:
             response (dict): The response from OpenAI API.
 
         Returns:
-            The cost in USD.
+            The cost in USD. 0 if the model is not supported.
         """
         model = response["model"]
         if model not in cls.price1K:
-            raise ValueError(f"Unknown model: {model}")
+            return 0
+            # raise ValueError(f"Unknown model: {model}")
         usage = response["usage"]
         n_input_tokens = usage["prompt_tokens"]
         n_output_tokens = usage.get("completion_tokens", 0)
         price1K = cls.price1K[model]
         if isinstance(price1K, tuple):
             return (price1K[0] * n_input_tokens + price1K[1] * n_output_tokens) / 1000
         return price1K * (n_input_tokens + n_output_tokens) / 1000
```

### Comparing `FLAML-1.2.3/flaml/automl/automl.py` & `FLAML-1.2.4/flaml/automl/automl.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/data.py` & `FLAML-1.2.4/flaml/automl/data.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/ml.py` & `FLAML-1.2.4/flaml/automl/ml.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/model.py` & `FLAML-1.2.4/flaml/automl/model.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-1.2.4/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-1.2.4/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-1.2.4/flaml/automl/nlp/huggingface/training_args.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/nlp/huggingface/utils.py` & `FLAML-1.2.4/flaml/automl/nlp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/nlp/utils.py` & `FLAML-1.2.4/flaml/automl/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/spark/configs.py` & `FLAML-1.2.4/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/spark/metrics.py` & `FLAML-1.2.4/flaml/automl/spark/metrics.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/spark/utils.py` & `FLAML-1.2.4/flaml/automl/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/state.py` & `FLAML-1.2.4/flaml/automl/state.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/task/generic_task.py` & `FLAML-1.2.4/flaml/automl/task/generic_task.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/task/task.py` & `FLAML-1.2.4/flaml/automl/task/task.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/training_log.py` & `FLAML-1.2.4/flaml/automl/training_log.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/automl/utils.py` & `FLAML-1.2.4/flaml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/all/binary.json` & `FLAML-1.2.4/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/all/multiclass.json` & `FLAML-1.2.4/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/all/regression.json` & `FLAML-1.2.4/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/estimator.py` & `FLAML-1.2.4/flaml/default/estimator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/extra_tree/binary.json` & `FLAML-1.2.4/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/extra_tree/multiclass.json` & `FLAML-1.2.4/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/extra_tree/regression.json` & `FLAML-1.2.4/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/greedy.py` & `FLAML-1.2.4/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/lgbm/binary.json` & `FLAML-1.2.4/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/lgbm/multiclass.json` & `FLAML-1.2.4/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/lgbm/regression.json` & `FLAML-1.2.4/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/portfolio.py` & `FLAML-1.2.4/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/regret.py` & `FLAML-1.2.4/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/rf/binary.json` & `FLAML-1.2.4/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/rf/multiclass.json` & `FLAML-1.2.4/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/rf/regression.json` & `FLAML-1.2.4/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/suggest.py` & `FLAML-1.2.4/flaml/default/suggest.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/xgb_limitdepth/binary.json` & `FLAML-1.2.4/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-1.2.4/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/xgb_limitdepth/regression.json` & `FLAML-1.2.4/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/xgboost/binary.json` & `FLAML-1.2.4/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/xgboost/multiclass.json` & `FLAML-1.2.4/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/default/xgboost/regression.json` & `FLAML-1.2.4/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/onlineml/autovw.py` & `FLAML-1.2.4/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/onlineml/trial.py` & `FLAML-1.2.4/flaml/onlineml/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/onlineml/trial_runner.py` & `FLAML-1.2.4/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/__init__.py` & `FLAML-1.2.4/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/analysis.py` & `FLAML-1.2.4/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/result.py` & `FLAML-1.2.4/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/sample.py` & `FLAML-1.2.4/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/scheduler/online_scheduler.py` & `FLAML-1.2.4/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-1.2.4/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/blendsearch.py` & `FLAML-1.2.4/flaml/tune/searcher/blendsearch.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/cfo_cat.py` & `FLAML-1.2.4/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/flow2.py` & `FLAML-1.2.4/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/online_searcher.py` & `FLAML-1.2.4/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/search_thread.py` & `FLAML-1.2.4/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/suggestion.py` & `FLAML-1.2.4/flaml/tune/searcher/suggestion.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/searcher/variant_generator.py` & `FLAML-1.2.4/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/space.py` & `FLAML-1.2.4/flaml/tune/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         from ray.tune.suggest.variant_generator import generate_variants
     else:
         from ray.tune.search import sample
         from ray.tune.search.variant_generator import generate_variants
 except (ImportError, AssertionError):
     from . import sample
     from .searcher.variant_generator import generate_variants
-from typing import Dict, Optional, Any, Tuple, Generator
+from typing import Dict, Optional, Any, Tuple, Generator, List, Union
 import numpy as np
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def generate_variants_compatible(
@@ -23,14 +23,37 @@
 ) -> Generator[Tuple[Dict, Dict], None, None]:
     try:
         return generate_variants(unresolved_spec, constant_grid_search, random_state)
     except TypeError:
         return generate_variants(unresolved_spec, constant_grid_search)
 
 
+def is_constant(space: Union[Dict, List]) -> bool:
+    """Whether the search space is all constant.
+
+    Returns:
+        A bool of whether the search space is all constant.
+    """
+    if isinstance(space, dict):
+        for domain in space.values():
+            if isinstance(domain, (dict, list)):
+                if not is_constant(domain):
+                    return False
+                continue
+            if isinstance(domain, sample.Domain):
+                return False
+        return True
+    elif isinstance(space, list):
+        for item in space:
+            if not is_constant(item):
+                return False
+        return True
+    return not isinstance(space, sample.Domain)
+
+
 def define_by_run_func(trial, space: Dict, path: str = "") -> Optional[Dict[str, Any]]:
     """Define-by-run function to create the search space.
 
     Returns:
         A dict with constant values.
     """
     config = {}
```

### Comparing `FLAML-1.2.3/flaml/tune/spark/utils.py` & `FLAML-1.2.4/flaml/tune/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/trial.py` & `FLAML-1.2.4/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/trial_runner.py` & `FLAML-1.2.4/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/tune.py` & `FLAML-1.2.4/flaml/tune/tune.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/flaml/tune/utils.py` & `FLAML-1.2.4/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/pyproject.toml` & `FLAML-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/setup.py` & `FLAML-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/test/test_autovw.py` & `FLAML-1.2.4/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/test/test_conda_distribution.py` & `FLAML-1.2.4/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/test/test_gpu.py` & `FLAML-1.2.4/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.3/test/test_model.py` & `FLAML-1.2.4/test/test_model.py`

 * *Files identical despite different names*

