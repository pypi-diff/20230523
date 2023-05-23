# Comparing `tmp/heron-ravenframework-0.2rc1.tar.gz` & `tmp/heron-ravenframework-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jjc/raven/setup/heron_package/dist/tmpd_tzbyxl/heron-ravenframework-0.2rc1.tar", last modified: Thu Oct 27 15:33:27 2022, max compression
+gzip compressed data, was "heron-ravenframework-0.3.tar", last modified: Mon May 22 17:56:53 2023, max compression
```

## Comparing `heron-ravenframework-0.2rc1.tar` & `heron-ravenframework-0.3.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/
--rw-r--r--   0 jjc       (1000) jjc       (1000)    11357 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/LICENSE
--rw-r--r--   0 jjc       (1000) jjc       (1000)     1762 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/NOTICE.txt
--rw-r--r--   0 jjc       (1000) jjc       (1000)     2768 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/README.md
--rw-r--r--   0 jjc       (1000) jjc       (1000)      144 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/__init__.py
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/src/
--rw-r--r--   0 jjc       (1000) jjc       (1000)      674 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ArmaBypass.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    46477 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/Cases.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     2723 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/CashFlowUser.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    50758 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/Components.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)      502 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/DispatchBypass.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    32943 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/DispatchManager.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     8547 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/DispatchPlot.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    21199 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/Economics.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    45489 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/Herd.py
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/src/Hybrid2Heron/
--rw-r--r--   0 jjc       (1000) jjc       (1000)     4494 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/Hybrid2Heron/HYBRID_HERON_keywords.csv
--rw-r--r--   0 jjc       (1000) jjc       (1000)    16415 2022-10-27 15:29:11.000000 heron-ravenframework-0.2rc1/HERON/src/Hybrid2Heron/hybrid2heron_economic.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    49471 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/Moped.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    18996 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/Placeholders.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     1099 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/SerializationManager.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     7924 2022-10-27 15:29:07.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParamHandler.py
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/
--rw-r--r--   0 jjc       (1000) jjc       (1000)     5249 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Activity.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3420 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Factory.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3007 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Function.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3375 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Linear.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     5060 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Parametric.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     5602 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/ROM.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3870 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/StaticHistory.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3947 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/SyntheticHistory.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     4441 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/ValuedParam.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     2635 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Variable.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)      508 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/ValuedParams/__init__.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/__init__.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     7300 2022-10-20 20:28:10.000000 heron-ravenframework-0.2rc1/HERON/src/_utils.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     1167 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/base.py
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/
--rw-r--r--   0 jjc       (1000) jjc       (1000)     4001 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/CustomDispatcher.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     8972 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/DispatchState.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     5728 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/Dispatcher.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)      393 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/Factory.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/__init__.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    45525 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/pyomo_dispatch.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    10052 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/twin_pyomo_test.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    10465 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/twin_pyomo_test_ch_disch.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)    12207 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/dispatch/twin_pyomo_test_rte.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3639 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/input_loader.py
--rwxr-xr-x   0 jjc       (1000) jjc       (1000)     5055 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/main.py
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/src/validators/
--rw-r--r--   0 jjc       (1000) jjc       (1000)     3489 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/validators/ExampleValidator.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     1331 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/src/validators/Factory.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)     2972 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/validators/Validator.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)        0 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/src/validators/__init__.py
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/HERON/templates/
--rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/templates/__init__.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)      208 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/templates/cash.xml
--rw-r--r--   0 jjc       (1000) jjc       (1000)     4977 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/templates/inner.xml
--rw-r--r--   0 jjc       (1000) jjc       (1000)     4121 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/templates/outer.xml
--rw-r--r--   0 jjc       (1000) jjc       (1000)    75982 2022-10-13 21:14:52.000000 heron-ravenframework-0.2rc1/HERON/templates/template_driver.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)      917 2022-10-11 14:25:39.000000 heron-ravenframework-0.2rc1/HERON/templates/write_inner.py
--rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-13 14:54:16.000000 heron-ravenframework-0.2rc1/MANIFEST.in
--rw-r--r--   0 jjc       (1000) jjc       (1000)     2944 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/PKG-INFO
-drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/
--rw-r--r--   0 jjc       (1000) jjc       (1000)     2944 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/PKG-INFO
--rw-r--r--   0 jjc       (1000) jjc       (1000)     1935 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/SOURCES.txt
--rw-r--r--   0 jjc       (1000) jjc       (1000)        1 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/dependency_links.txt
--rw-r--r--   0 jjc       (1000) jjc       (1000)       46 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/entry_points.txt
--rw-r--r--   0 jjc       (1000) jjc       (1000)       80 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/requires.txt
--rw-r--r--   0 jjc       (1000) jjc       (1000)      118 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/top_level.txt
--rw-r--r--   0 jjc       (1000) jjc       (1000)       85 2022-10-11 14:31:56.000000 heron-ravenframework-0.2rc1/pyproject.toml
--rw-r--r--   0 jjc       (1000) jjc       (1000)      704 2022-10-27 15:33:27.000000 heron-ravenframework-0.2rc1/setup.cfg
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.760157 heron-ravenframework-0.3/
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.739158 heron-ravenframework-0.3/HERON/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    11357 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/LICENSE
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1762 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/NOTICE.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     2809 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/README.md
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      144 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/__init__.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.745158 heron-ravenframework-0.3/HERON/src/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      674 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ArmaBypass.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    46896 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/Cases.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     2723 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/CashFlowUser.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    51939 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/Components.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      502 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/DispatchBypass.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    35364 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/DispatchManager.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    12564 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/DispatchPlot.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    21342 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/Economics.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    54192 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/Herd.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.745158 heron-ravenframework-0.3/HERON/src/Hybrid2Heron/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     4494 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/Hybrid2Heron/HYBRID_HERON_keywords.csv
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    16511 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/Hybrid2Heron/hybrid2heron_economic.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    50639 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/Moped.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3590 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/NetworkPlot.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    18996 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/Placeholders.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1099 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/SerializationManager.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     7924 2022-10-27 15:29:07.000000 heron-ravenframework-0.3/HERON/src/ValuedParamHandler.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.750157 heron-ravenframework-0.3/HERON/src/ValuedParams/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     5249 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/Activity.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3420 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/Factory.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3007 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/Function.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3375 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/Linear.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     5060 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/Parametric.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     5602 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/ROM.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3870 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/StaticHistory.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3947 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/SyntheticHistory.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     4441 2022-10-13 21:14:52.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/ValuedParam.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     2635 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/Variable.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      508 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/ValuedParams/__init__.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/__init__.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     7544 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/_utils.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1167 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/base.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.754157 heron-ravenframework-0.3/HERON/src/dispatch/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     4001 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/CustomDispatcher.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     8972 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/dispatch/DispatchState.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     5728 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/Dispatcher.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      393 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/Factory.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/__init__.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    45858 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/dispatch/pyomo_dispatch.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    10052 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/twin_pyomo_test.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    10465 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/twin_pyomo_test_ch_disch.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    12207 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/dispatch/twin_pyomo_test_rte.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     6082 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/input_definition.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3639 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/src/input_loader.py
+-rwxr-xr-x   0 jjc       (1000) jjc       (1000)     6350 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/src/main.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.754157 heron-ravenframework-0.3/HERON/src/validators/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     3489 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/validators/ExampleValidator.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1331 2022-10-13 21:14:52.000000 heron-ravenframework-0.3/HERON/src/validators/Factory.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     2972 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/validators/Validator.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)        0 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/src/validators/__init__.py
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.757157 heron-ravenframework-0.3/HERON/templates/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/templates/__init__.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      208 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/templates/cash.xml
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     5082 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/templates/inner.xml
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     4248 2023-05-22 16:57:07.000000 heron-ravenframework-0.3/HERON/templates/outer.xml
+-rw-r--r--   0 jjc       (1000) jjc       (1000)    73324 2023-05-22 17:28:47.000000 heron-ravenframework-0.3/HERON/templates/template_driver.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      917 2022-10-11 14:25:39.000000 heron-ravenframework-0.3/HERON/templates/write_inner.py
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       71 2022-10-13 14:54:16.000000 heron-ravenframework-0.3/MANIFEST.in
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     2982 2023-05-22 17:56:53.760157 heron-ravenframework-0.3/PKG-INFO
+drwxr-xr-x   0 jjc       (1000) jjc       (1000)        0 2023-05-22 17:56:53.759157 heron-ravenframework-0.3/heron_ravenframework.egg-info/
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     2982 2023-05-22 17:56:53.000000 heron-ravenframework-0.3/heron_ravenframework.egg-info/PKG-INFO
+-rw-r--r--   0 jjc       (1000) jjc       (1000)     1990 2023-05-22 17:56:53.000000 heron-ravenframework-0.3/heron_ravenframework.egg-info/SOURCES.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)        1 2023-05-22 17:56:53.000000 heron-ravenframework-0.3/heron_ravenframework.egg-info/dependency_links.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       46 2023-05-22 17:56:53.000000 heron-ravenframework-0.3/heron_ravenframework.egg-info/entry_points.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       82 2023-05-22 17:56:53.000000 heron-ravenframework-0.3/heron_ravenframework.egg-info/requires.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      118 2023-05-22 17:56:53.000000 heron-ravenframework-0.3/heron_ravenframework.egg-info/top_level.txt
+-rw-r--r--   0 jjc       (1000) jjc       (1000)       85 2022-10-11 14:31:56.000000 heron-ravenframework-0.3/pyproject.toml
+-rw-r--r--   0 jjc       (1000) jjc       (1000)      703 2023-05-22 17:56:53.761157 heron-ravenframework-0.3/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `heron-ravenframework-0.2rc1/HERON/LICENSE` & `heron-ravenframework-0.3/HERON/LICENSE`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/NOTICE.txt` & `heron-ravenframework-0.3/HERON/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/README.md` & `heron-ravenframework-0.3/HERON/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 It leverages probabalistic analysis tool [raven](https://github.com/idaholab/raven)
 to run constructed workflows. HERON is a plugin for RAVEN.
 
 Instructions for
 installing RAVEN plugins (including HERON) can be found [on RAVEN's website](https://github.com/idaholab/raven/wiki/Plugins).
 
-See more on the [HERON wiki](https://github.com/idaholab/HERON/wiki)
+See more on the [HERON wiki](https://github.com/idaholab/HERON/wiki) for installation, examples, and documentation.
 
 ## Publications
 The following are a selection of technical reports, conference proceedings, and journal articles that may be of interest to users and developers of HERON, loosely in order of work performed.
 
 ### Technoeconomic Assessments
 - [A Technical and Economic Assessment of LWR Flexible Operation for Generation and Demand Balancing to Optimize Plant Revenue](https://www.osti.gov/biblio/1844211-technical-economic-assessment-lwr-flexible-operation-generation-demand-balancing-optimize-plant-revenue)
 - [Evaluation of Hybrid FPOG Applications in Regulated and Deregulated Markets Using HERON](https://www.osti.gov/biblio/1755894-evaluation-hybrid-fpog-applications-regulated-deregulated-markets-using-heron)
-- [HERON as a Tool for LWR Market Interaction in a Deregulated Market](https://www.osti.gov/biblio/1581179-heron-tool-lwr-market-interaction-deregulated-market) 
-- [Evaluation of Hydrogen Production Feasibility for a Light Water Reactor in the Midwest](https://www.osti.gov/biblio/1569271-evaluation-hydrogen-production-feasibility-light-water-reactor-midwest) 
-- [Economic Assessment of Nuclear Hybrid Energy Systems: Nuclear-Renewable-Water Integration in Arizona](https://www.osti.gov/biblio/1634115-economic-assessment-nuclear-hybrid-energy-systems-nuclear-renewable-water-integration-arizona) 
-- [Economic analysis of a nuclear hybrid energy system in a stochastic environment including wind turbines in an electricity grid](https://www.osti.gov/biblio/1593858-economic-analysis-nuclear-hybrid-energy-system-stochastic-environment-including-wind-turbines-electricity-grid) 
+- [HERON as a Tool for LWR Market Interaction in a Deregulated Market](https://www.osti.gov/biblio/1581179-heron-tool-lwr-market-interaction-deregulated-market)
+- [Evaluation of Hydrogen Production Feasibility for a Light Water Reactor in the Midwest](https://www.osti.gov/biblio/1569271-evaluation-hydrogen-production-feasibility-light-water-reactor-midwest)
+- [Economic Assessment of Nuclear Hybrid Energy Systems: Nuclear-Renewable-Water Integration in Arizona](https://www.osti.gov/biblio/1634115-economic-assessment-nuclear-hybrid-energy-systems-nuclear-renewable-water-integration-arizona)
+- [Economic analysis of a nuclear hybrid energy system in a stochastic environment including wind turbines in an electricity grid](https://www.osti.gov/biblio/1593858-economic-analysis-nuclear-hybrid-energy-system-stochastic-environment-including-wind-turbines-electricity-grid)
 
 ### Synthetic History Generation
-- [Correlated synthetic time series generation for energy system simulations using Fourier and ARMA signal processing](https://www.osti.gov/biblio/1603186-correlated-synthetic-time-series-generation-energy-system-simulations-using-fourier-arma-signal-processing) 
-- [Synthetic wind speed scenarios generation for probabilistic analysis of hybrid energy systems](https://www.osti.gov/biblio/1361550-synthetic-wind-speed-scenarios-generation-probabilistic-analysis-hybrid-energy-systems) 
+- [Correlated synthetic time series generation for energy system simulations using Fourier and ARMA signal processing](https://www.osti.gov/biblio/1603186-correlated-synthetic-time-series-generation-energy-system-simulations-using-fourier-arma-signal-processing)
+- [Synthetic wind speed scenarios generation for probabilistic analysis of hybrid energy systems](https://www.osti.gov/biblio/1361550-synthetic-wind-speed-scenarios-generation-probabilistic-analysis-hybrid-energy-systems)
 
 ### See More
 - [Integrated Energy Systems](https://ies.inl.gov/SitePages/Home.aspx)
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ArmaBypass.py` & `heron-ravenframework-0.3/HERON/src/ArmaBypass.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Cases.py` & `heron-ravenframework-0.3/HERON/src/Cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,18 @@
     debug.addSub(InputData.parameterInputFactory('macro_steps', contentType=InputTypes.IntegerType,
         descr=r"""sets the number of macro steps (e.g. years) the stochastic synthetic histories and dispatch
               optimization should include. \default{1}"""))
     debug.addSub(InputData.parameterInputFactory('dispatch_plot', contentType=InputTypes.BoolType,
         descr=r"""provides a dispatch plot after running through \xmlNode{inner_samples} and
               \xmlNode{macro_steps} provided. To prevent plotting output during debug mode set to "False".
               \default{True}"""))
+    debug.addSub(InputData.parameterInputFactory('cashflow_plot', contentType=InputTypes.BoolType,
+        descr=r"""provides a cashflow plot after running through \xmlNode{inner_samples} and
+              \xmlNode{macro_steps} provided. To prevent plotting output during debug mode set to "False".
+              \default{True}"""))
     input_specs.addSub(debug)
 
     parallel = InputData.parameterInputFactory('parallel', descr=r"""Describes how to parallelize this run. If not present defaults to no parallelization (1 outer, 1 inner)""")
     parallel.addSub(InputData.parameterInputFactory('outer', contentType=InputTypes.IntegerType,
         descr=r"""the number of parallel runs to use for the outer optimization run. The product of this
               number and \xmlNode{inner} should be at most the number of parallel process available on
               your computing device. This should also be at most the number of samples needed per outer iteration;
@@ -405,15 +409,16 @@
     self._time_varname = 'time'        # name of the time-variable throughout simulation
     self._year_varname = 'Year'        # name of the year-variable throughout simulation
     self._labels = {}                  # extra information pertaining to current case
     self.debug = {                     # debug options, as enabled by the user (defaults included)
         'enabled': False,              # whether to enable debug mode
         'inner_samples': 1,            # how many inner realizations to sample
         'macro_steps': 1,              # how many "years" for inner realizations
-        'dispatch_plot': True          # whether to output a plot in debug mode
+        'dispatch_plot': True,         # whether to output a dispatch plot in debug mode
+        'cashflow_plot': True          # whether to output a cashflow plot in debug mode
     }
 
     self.data_handling = {             # data handling options
       'inner_to_outer': 'netcdf',      # how to pass inner data to outer (csv, netcdf)
     }
 
     self._time_discretization = None   # (start, end, number) for constructing time discretization, same as argument to np.linspace
@@ -872,17 +877,17 @@
       @ In, components, HERON components, components for the simulation
       @ In, sources, HERON sources, sources for the simulation
       @ In, loc, str, location in which to write files
       @ Out, None
     """
     # load templates
     template_class = self._load_template()
-    inner, outer, cash = template_class.createWorkflow(self, components, sources)
+    inner, outer = template_class.createWorkflow(self, components, sources)
 
-    template_class.writeWorkflow((inner, outer, cash), loc)
+    template_class.writeWorkflow((inner, outer), loc)
 
   #### UTILITIES ####
   def _load_template(self):
     """
       Loads template files for modification
       @ In, None
       @ Out, template_class, RAVEN Template, instantiated Template class
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/CashFlowUser.py` & `heron-ravenframework-0.3/HERON/src/CashFlowUser.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Components.py` & `heron-ravenframework-0.3/HERON/src/Components.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,20 @@
         descr=r"""indicates the resource that defines the capacity of this component's operation. For example,
               if a component consumes steam and electricity to produce hydrogen, the capacity of the component
               can be defined by the maximum steam consumable, maximum electricity consumable, or maximum
               hydrogen producable. Any choice should be nominally equivalent, but determines the units
               of the value of this node.""")
     specs.addSub(cap)
 
+    descr = r"""the actual value at which this component can act, as a unitless fraction of total rated capacity.
+            Note that these factors are applied within the dispatch optimization; we assume that the capacity factor
+            is not a variable in the outer optimization."""
+    capfactor = vp_factory.make_input_specs('capacity_factor', descr=descr, allowed=['ARMA', 'CSV'])
+    specs.addSub(capfactor)
+
     descr = r"""provides the minimum value at which this component can act, in units of the indicated resource. """
     minn = vp_factory.make_input_specs('minimum', descr=descr)
     minn.addParam('resource', param_type=InputTypes.StringType,
         descr=r"""indicates the resource that defines the minimum activity level for this component,
               as with the component's capacity.""")
     specs.addSub(minn)
 
@@ -412,14 +418,15 @@
       Constructor
       @ In, kwargs, dict, arbitrary pass-through arguments
       @ Out, None
     """
     Base.__init__(self, **kwargs)
     self._capacity = None               # upper limit of this interaction
     self._capacity_var = None           # which variable limits the capacity (could be produced or consumed?)
+    self._capacity_factor = None        # ratio of actual output as fraction of _capacity
     self._signals = set()               # dependent signals for this interaction
     self._crossrefs = defaultdict(dict) # crossrefs objects needed (e.g. armas, etc), as {attr: {tag, name, obj})
     self._dispatchable = None           # independent, dependent, or fixed?
     self._minimum = None                # lowest interaction level, if dispatchable
     self._minimum_var = None            # limiting variable for minimum
     self._function_method_map = {}      # maps things that call functions to the method within the function that needs calling
     self._transfer = None               # the production rate (if any), in produces per consumes
@@ -435,15 +442,15 @@
       @ In, comp_name, string, name of component this Interaction belongs to
       @ Out, None
     """
     self.raiseADebug(' ... loading interaction "{}"'.format(self.tag))
     self._dispatchable = specs.parameterValues['dispatch']
     for item in specs.subparts:
       name = '_' + item.getName()
-      if name in ['_capacity', '_minimum']:
+      if name in ['_capacity', '_capacity_factor', '_minimum']:
         # common reading for valued params
         self._set_valued_param(name, comp_name, item, mode)
         if name == '_capacity':
           self._capacity_var = item.parameterValues.get('resource', None)
         elif item.getName() == 'minimum':
           self._minimum_var = item.parameterValues.get('resource', None)
     # finalize some values
@@ -482,17 +489,22 @@
       Returns an evaluated value unless "raw" is True, then gives ValuedParam
       @ In, meta, dict, additional variables to pass through
       @ In, raw, bool, optional, if True then provide ValuedParam instead of evaluation
       @ Out, evaluated, float or ValuedParam, requested value
       @ Out, meta, dict, additional variable passthrough
     """
     if raw:
+      #NOTE: not returing capacity_factor since it will not be used as a variable
       return self._capacity
     meta['request'] = {self._capacity_var: None}
     evaluated, meta = self._capacity.evaluate(meta, target_var=self._capacity_var)
+    # apply capacity factor to get actual capacity for given timestep
+    if self._capacity_factor is not None:
+      capacity_factor = self._capacity_factor.evaluate(meta, target_var=self._capacity_var)[0]
+      evaluated[self._capacity_var] *= capacity_factor[self._capacity_var]
     return evaluated, meta
 
   def get_capacity_var(self):
     """
       Returns the resource variable that is used to define the capacity limits of this interaction.
       @ In, None
       @ Out, capacity_var, string, name of capacity-limiting resource
@@ -892,17 +904,18 @@
       @ In, None
       @ Out, input_specs, InputData, specs
     """
     specs = super().get_input_specs()
     # TODO unused, please implement ... :
     # descr = r"""the limiting charge/discharge rate of this storage. """
     # specs.addSub(ValuedParam.get_input_specs('rate'))
-    descr=r"""initial quantity of resource assumed to be present in the storage unit at the beginning
-          of a given calculation, in units of quantity (not rate). \default{0}. """
-    specs.addSub(vp_factory.make_input_specs('initial_stored', descr=descr))
+    descr=r"""indicates what percent of the storage unit is full at the start of each optimization sequence,
+              from 0 to 1. \default{0.0}. """
+    sub = vp_factory.make_input_specs('initial_stored', descr=descr)
+    specs.addSub(sub)
     descr=r"""control strategy for operating the storage. If not specified, uses a perfect foresight strategy. """
     specs.addSub(vp_factory.make_input_specs('strategy', allowed=['Function'], descr=descr))
     descr = r"""round-trip efficiency for this component as a scalar multiplier. \default{1.0}"""
     specs.addSub(InputData.parameterInputFactory('RTE', contentType=InputTypes.FloatType, descr=descr))
     return specs
 
   def __init__(self, **kwargs):
@@ -934,19 +947,19 @@
         self._set_valued_param('_rate', comp_name, item, mode)
       elif item.getName() == 'initial_stored':
         self._set_valued_param('_initial_stored', comp_name, item, mode)
       elif item.getName() == 'strategy':
         self._set_valued_param('_strategy', comp_name, item, mode)
       elif item.getName() == 'RTE':
         self._sqrt_rte = np.sqrt(item.value)
-    assert len(self._stores) == 1, 'Multiple storage resources given for component "{}"'.format(comp_name)
+    assert len(self._stores) == 1, f'Multiple storage resources given for component "{comp_name}"'
     self._stores = self._stores[0]
     # checks and defaults
     if self._initial_stored is None:
-      self.raiseAWarning('Initial storage level for "{}" was not provided! Defaulting to 0.'.format(comp_name))
+      self.raiseAWarning(f'Initial storage level for "{comp_name}" was not provided! Defaulting to 0%.')
       # make a fake reader node for a 0 value
       vp = ValuedParamHandler('initial_stored')
       vp.set_const_VP(0.0)
       self._initial_stored = vp
     # the capacity is limited by the stored resource.
     self._capacity_var = self._stores
 
@@ -1099,15 +1112,21 @@
       Find initial level of the storage
       @ In, meta, dict, additional variable passthrough
       @ Out, initial, float, initial level
     """
     res = self.get_resource()
     request = {res: None}
     meta['request'] = request
-    return self._initial_stored.evaluate(meta, target_var=res)[0][res]
+    pct = self._initial_stored.evaluate(meta, target_var=res)[0][res]
+    if not (0 <= pct <= 1):
+      self.raiseAnError(ValueError, f'While calculating initial storage level for storage "{self.tag}", ' +
+          f'an invalid percent was provided/calculated ({pct}). Initial levels should be between 0 and 1, inclusive.')
+    amt = pct * self.get_capacity(meta)[0][res]
+    return amt
+
 
 
 
 class Demand(Interaction):
   """
     Explains a particular interaction, where a resource is demanded
   """
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/DispatchManager.py` & `heron-ravenframework-0.3/HERON/src/DispatchManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,14 @@
   sys.path.append(raven_path)
   from ravenframework.PluginBaseClasses.ExternalModelPluginBase import ExternalModelPluginBase
   sys.path.pop()
 
   cashflow_path = os.path.abspath(os.path.join(hutils.get_cashflow_loc(raven_path=raven_path), '..'))
   sys.path.append(cashflow_path)
   import TEAL
-from TEAL.src import CashFlows
-from TEAL.src.main import run as CashFlow_run
 
 # make functions findable
 sys.path.append(os.getcwd())
 
 class DispatchRunner:
   """
     Manages the interface between RAVEN and running the dispatch
@@ -242,16 +240,34 @@
         for var_name, data in dispatches.items():
           # if first time, initialize data structure
           if y == c == 0:
             shape = (n_year, n_clst, n_time)
             setattr(raven, var_name, np.empty(shape)) # NOTE could use np.zeros, but slower?
           getattr(raven, var_name)[y, c] = data
           getattr(raven, '_indexMap')[0][var_name] = [year_name, clst_name, time_name]
+    cfYears = None
     for metric, value in metrics.items():
-      setattr(raven, metric, np.atleast_1d(value))
+      if metric not in ['outputType', 'all_data']:
+        setattr(raven, metric, np.atleast_1d(value))
+      elif metric == 'all_data':
+        # store the cashflow years index cfYears
+        ## implicitly assume the first cashflow has representative years
+        # store each of the cashflows
+        for comp, comp_data in value.items():
+          for cf, cf_values in comp_data.items():
+            if cfYears is None:
+              cfYears = len(cf_values)
+            if cf.endswith(('depreciation_tax_credit', 'depreciation')):
+              name = cf
+            else:
+              name = f'{comp}_{cf}_CashFlow'
+            setattr(raven, name, np.atleast_1d(cf_values))
+    if cfYears is not None:
+      setattr(raven, 'cfYears', np.arange(cfYears))
+
     # if component capacities weren't given by Outer, save them as part of Inner
     for comp in self._components:
       cap_name = self.naming_template['comp capacity'].format(comp=comp.name)
       if cap_name not in dir(raven):
         # TODO what value should actually be used?
         setattr(raven, cap_name, -42)
 
@@ -266,14 +282,17 @@
       @ In, segs, list(int), segments/clusters/divisions
       @ In, seg_type, str, "segment" or "cluster" if segmented or clustered
       @ Out, dispatch_results, list(DispatchState), results of dispatch for each segment/cluster and year
     """
     structure = all_structure['summary']
     ## FINAL settings/components/cashflows use the multiplicity of divisions for aggregated evaluation
     final_settings, final_components = self._build_econ_objects(self._case, self._components, project_life)
+    # enable additional cashflow outputs if in debug mode
+    if self._case.debug['enabled']:
+      final_settings.setParams({'Output': True})
     active_index = {}
     dispatch_results = {}
     yearly_cluster_data = next(iter(all_structure['details'].values()))['clusters']
     for year in range(project_life):
       interp_year = interp_years[year] if len(interp_years) > 1 else (interp_years[0] + year)
       if self._save_dispatch:
         dispatch_results[interp_year] = {}
@@ -300,61 +319,81 @@
       Note the only reason there's a difference is because HERON needs to retain some level of
       flexibility in the parameter values until this method is called, whereas CashFlow expects
       them to be evaluated.
       @ In, heron_case, HERON Case instance, global HERON settings for this analysis
       @ In, heron_components, list, HERON component instances
       @ In, project_life, int, number of years to evaluate project
       @ Out, global_settings, CashFlow.GlobalSettings instance, settings for CashFlow analysis
-      @ Out, cf_components, dict, CashFlow component instances
+      @ Out, teal_components, dict, CashFlow component instances
     """
     heron_econs = list(comp.get_economics() for comp in heron_components)
     # build global econ settings for CashFlow
     global_params = heron_case.get_econ(heron_econs)
-    global_settings = CashFlows.GlobalSettings()
+    global_settings = TEAL.src.CashFlows.GlobalSettings()
     global_settings.setParams(global_params)
     global_settings._verbosity = 0 # FIXME direct access, also make user option?
-    # build CashFlow component instances
-    cf_components = {}
+    # build TEAL CashFlow component instances
+    teal_components = {}
     for c, cfg in enumerate(heron_econs):
       # cfg is the cashflowgroup connected to the heron component
       # get the associated heron component
       heron_comp = heron_components[c]
       comp_name = heron_comp.name
-      # build CashFlow equivalent component
-      cf_comp = CashFlows.Component()
-      cf_comp_params = {'name': comp_name,
+      # build TEAL equivalent component
+      teal_comp = TEAL.src.CashFlows.Component()
+      teal_comp_params = {'name': comp_name,
                         'Life_time': cfg.get_lifetime(),
-                        # TODO StartTime, Repetitions, tax, inflation
+                        # TODO StartTime, Repetitions, custom tax/inflation rate
                        }
-      cf_comp.setParams(cf_comp_params)
-      cf_components[comp_name] = cf_comp
-      # create all the CashFlow.CashFlows (cf_cf) for the CashFlow.Component
-      cf_cfs = []
+      teal_comp.setParams(teal_comp_params)
+      teal_components[comp_name] = teal_comp
+      # create all the TEAL.CashFlows (teal_cf) for the TEAL.Component
+      teal_cfs = []
       for heron_cf in cfg.get_cashflows():
         cf_name = heron_cf.name
         # the way to build it slightly changes depending on the CashFlow type
         if heron_cf._type == 'repeating': # FIXME protected access
-          cf_cf = CashFlows.Recurring()
-          cf_cf_params = {'name': cf_name,
+          teal_cf = TEAL.src.CashFlows.Recurring()
+          # NOTE: the params are listed in order of how they're read in TEAL.CashFlows.CashFlow.setParams
+          teal_cf_params = {'name': cf_name,
+                          # driver: comes later
+                          'tax': heron_cf._taxable,
+                          'inflation': heron_cf._inflation,
+                          'mult_target': heron_cf._mult_target,
+                          # multiply: do we ever use this?
+                          # alpha: comes later
+                          # reference: not relevant for recurring
                           'X': 1.0,
-                          'mult_target': heron_cf._mult_target, # FIXME protected access
+                          # depreciate: not relevant for recurring
                           }
-          cf_cf.setParams(cf_cf_params)
-          cf_cf.initParams(project_life)
-        elif heron_cf._type == 'one-time': # FIXME protected access
-          cf_cf = CashFlows.Capex()
-          cf_cf.name = cf_name
-          cf_cf.initParams(cf_comp.getLifetime())
+          teal_cf.setParams(teal_cf_params)
+          teal_cf.initParams(project_life)
+        elif heron_cf._type == 'one-time':
+          teal_cf = TEAL.src.CashFlows.Capex()
+          teal_cf.name = cf_name
+          teal_cf_params = {'name': cf_name,
+                            'driver': 1.0, # handled in segment_cashflow
+                            'tax': heron_cf._taxable,
+                            'inflation': heron_cf._inflation,
+                            'mult_target': heron_cf._mult_target,
+                            # multiply: do we ever use this?
+                            'alpha': 1.0, # handled in segment_cashflow
+                            'reference': 1.0, # actually handled in segment_cashflow
+                            'X': 1.0,
+                            # depreciate: handled in segment_cashflow
+                           }
+          teal_cf.setParams(teal_cf_params)
+          teal_cf.initParams(teal_comp.getLifetime())
           # alpha, driver aren't known yet, so set those later
         else:
           raise NotImplementedError(f'Unknown HERON CashFlow Type: {heron_cf._type}')
         # store new object
-        cf_cfs.append(cf_cf)
-      cf_comp.addCashflows(cf_cfs)
-    return global_settings, cf_components
+        teal_cfs.append(teal_cf)
+      teal_comp.addCashflows(teal_cfs)
+    return global_settings, teal_components
 
   def _update_meta_for_segment(self, meta, seg, interp_year, yearly_cluster_data,
                                interp_years, active_index, all_structure) -> int:
     """
       Updates the "meta" auxiliary information variable to use info specific to the segment
       @ In, meta, dict, auxiliary information
       @ In, seg, int, id for current segment (or cluster)
@@ -400,69 +439,74 @@
     meta['HERON']['RAVEN_vars'] = self._slice_signals(all_structure, meta['HERON'])
     pivot_var = meta['HERON']['Case'].get_time_name()
     times = meta['HERON']['RAVEN_vars'][pivot_var]
     specific_meta = dict(meta) # TODO more deepcopy needed?
     resource_indexer = meta['HERON']['resource_indexer']
     for comp in self._components:
       # get corresponding current and final CashFlow.Component
-      cf_comp = local_comps[comp.name]
+      teal_comp = local_comps[comp.name]
       final_comp = final_components[comp.name]
       # sanity check
-      if comp.name != cf_comp.name: raise RuntimeError
+      if comp.name != teal_comp.name: raise RuntimeError
       specific_meta['HERON']['component'] = comp
       specific_meta['HERON']['all_activity'] = dispatch
       specific_activity = {}
       final_cashflows = final_comp.getCashflows()
       for f, heron_cf in enumerate(comp.get_cashflows()):
-        # get the corresponding CashFlow.CashFlow
-        cf_cf = cf_comp.getCashflows()[f]
+        # get the corresponding TEAL.CashFlow
+        teal_cf = teal_comp.getCashflows()[f]
         final_cf = final_cashflows[f]
         # sanity continued
-        if not (cf_cf.name == final_cf.name == heron_cf.name):
+        if not (teal_cf.name == final_cf.name == heron_cf.name):
             raise RuntimeError
 
         ## FIXME time then cashflow, or cashflow then time?
         ## "activity" is the same for every cashflow at a point in
         ## time, but many cashflows only need to be evaluated once
         ## and we can vectorize ...
 
         ## FIXME maybe "if activity is None" approach, so it gets
         ## filled on the first cashflow when looping through time.
 
         ## TODO we assume Capex and Recurring Year do not depend
         ## on the Activity
 
-        if cf_cf.type == 'Capex':
+        if teal_cf.type == 'Capex':
           # Capex cfs should only be constructed in the first  of the project life
           # FIXME is this doing capex once per segment, or once per life?
           if year == 0 and s == 0:
             params = heron_cf.calculate_params(specific_meta) # a, D, Dp, x, cost
-            cf_params = {'name': cf_cf.name,
-                          'mult_target': heron_cf._mult_target,
-                          'depreciate': heron_cf._depreciate,
-                          'alpha': params['alpha'],
-                          'driver': params['driver'],
-                          'reference': params['ref_driver'],
-                          'X': params['scaling'],}
-            cf_cf.setParams(cf_params)
+            # NOTE: listing params in order of TEAL.CashFlows.CashFlow.setParams
+            cf_params = {'name': teal_cf.name,
+                         'driver': params['driver'],
+                         'tax': heron_cf._taxable,
+                         'inflation': heron_cf._inflation,
+                         'mult_target': heron_cf._mult_target,
+                         # TODO "multiply" needed? Can't think of an application right now.
+                         'alpha': params['alpha'],
+                         'reference': params['ref_driver'],
+                         'X': params['scaling'],
+                         'depreciate': heron_cf._depreciate,
+                        }
+            teal_cf.setParams(cf_params)
 
             ## Because alpha, driver, etc are only set once for capex cash flows,
             ## we can just hot swap this cashflow into the final_comp, I think ...
 
             ## I believe we can do this because Capex are division-independent?
             ## Can we just do it once instead of once per division?
 
-            final_comp._cashFlows[f] = cf_cf
+            final_comp._cashFlows[f] = teal_cf
             # depreciators
             # FIXME do we need to know alpha, drivers first??
-            if heron_cf._depreciate and cf_cf.getAmortization() is None:
-              cf_cf.setAmortization('MACRS', heron_cf._depreciate)
-              deprs = cf_comp._createDepreciation(cf_cf)
+            if heron_cf._depreciate and teal_cf.getAmortization() is None:
+              teal_cf.setAmortization('MACRS', heron_cf._depreciate)
+              deprs = teal_comp._createDepreciation(teal_cf)
               final_comp._cashFlows.extend(deprs)
-        elif cf_cf.type == 'Recurring':
+        elif teal_cf.type == 'Recurring':
           # yearly recurring only need setting up once per year
           if heron_cf.get_period() == 'year':
             if s == 0:
               params = heron_cf.calculate_params(specific_meta) # a, D, Dp, x, cost
               contrib = params['cost']
               final_cf._yearlyCashflow[year + 1] += contrib
           # hourly recurring need iteration over time
@@ -484,15 +528,15 @@
               final_cf._yearlyCashflow[year+1] += contrib
           else:
             raise NotImplementedError(
                 f'Unrecognized Recurring period for "{comp.name}" cashflow "{heron_cf.name}": {heron_cf.get_period()}'
             )
         else:
             raise NotImplementedError(
-                f'Unrecognized CashFlow type for "{comp.name}" cashflow "{heron_cf.name}": {cf_cf.type}'
+                f'Unrecognized CashFlow type for "{comp.name}" cashflow "{heron_cf.name}": {teal_cf.type}'
             )
         # end CashFlow type if
       # end CashFlow per Component loop
     # end Component loop
 
   def _final_cashflow(self, meta, final_components, final_settings) -> dict:
     """
@@ -515,20 +559,21 @@
         print(f' ... ... ... D', cf._driver)
         print(f' ... ... ... a', cf._alpha)
         print(f' ... ... ... Dp', cf._reference)
         print(f' ... ... ... x', cf._scale)
         if hasattr(cf, '_yearlyCashflow'):
           print(f' ... ... ... hourly', cf._yearlyCashflow)
     # END DEBUGG
-    cf_metrics = CashFlow_run(final_settings, list(final_components.values()), raven_vars)
+    cf_metrics = TEAL.src.main.run(final_settings, list(final_components.values()), raven_vars)
     # DEBUGG
     print('****************************************')
     print('DEBUGG final cashflow metrics:')
     for k, v in cf_metrics.items():
-      print('  ', k, v)
+      if k not in ['outputType', 'all_data']:
+        print('  ', k, v)
     print('****************************************')
     # END DEBUGG
     return cf_metrics
 
   def _get_structure(self, raven_vars):
     """
       interpret the clustering information from the ROM
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/DispatchPlot.py` & `heron-ravenframework-0.3/HERON/src/DispatchPlot.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,16 @@
   Date: 2021-05-18
 """
 import itertools as it
 import matplotlib as mpl
 mpl.use('Agg') # Prevents the script from blocking while plotting
 import matplotlib.pyplot as plt
 from typing import List, Dict
+import random
+import numpy as np
 
 try:
   from ravenframework.PluginBaseClasses.OutStreamPlotPlugin import PlotPlugin, InputTypes, InputData
 except ModuleNotFoundError:
   import sys
   from . import _utils
   sys.path.append(_utils.get_raven_loc())
@@ -100,57 +102,88 @@
       key = var.split('__')[idx]
       if key in gr.keys():
         gr[key].append(var)
       else:
         gr[key] = [var]
     return gr
 
-  def plot_component(self, fig, axes, df, grp_vars, comp_idx, sid, mstep, cid) -> None:
+  def plot_component(self, fig, axes, df, grp_vars, comp_idx, sid, mstep, cid, cdict) -> None:
     """
       Plot and output the optimized dispatch for a specific sample, year, and cluster.
       @ In, fig, matplotlib.figure.Figure, current figure used for plotting.
       @ In, axes, List[List[matplotlib.Axes]], a list of axes to plot each variable.
       @ In, df, pandas.DataFrame, a dataframe containing data to plot.
       @ In, grp_vars, Dict[str, List[str]], a dictionary mapping components to variables.
       @ In, comp_idx, Dict[str, int], a dictionary mapping components to numbers.
       @ In, sid, int, the sample ID.
       @ In, mstep, int, the macro step.
       @ In, cid, int, the cluster ID.
+      @ In, cdict, Dict[str, str], a dictionary contains color code to variables
       @ Out, None
     """
+    # Pre-define color codes and transparency
+    Gray, Dark = ('#dcddde','#1a2b3c')
+    alpha = '70'
     for (key, group), ax in zip(grp_vars.items(), axes.flat):
-      lines = []
+      # Define list for data, label, and color. Seperate 'level'(line plot) with other variables (stack plot)
+      positive_dat = []
+      positive_label = []
+      positive_color = []
+      negative_dat = []
+      negative_label = []
+      negative_color = []
+      level_dat = []
+      level_label = []
+      level_color = []
+
+      # Secondary y axis for levels
+      ax2 = ax.twinx()
+      # Fill the lists
       for var in group:
         _, comp_name, tracker, _ = var.split('__')
         comp_label = comp_name.replace('_', ' ').title()
-        cidx = comp_idx[comp_name]
-
-        # NOTE custom behavior based on production/storage labels
-        plot_ax = ax
         var_label = f'{comp_label}, {tracker.title()}'
         ls = '-'
-        mk = '1'
-        if tracker == 'production':
-          var_label = comp_label
-        elif tracker == 'level':
-          plot_ax = ax.twinx()
-          ls = ':'
-          mk = '.'
-        elif tracker == 'charge':
-          mk = '^'
-        elif tracker == 'discharge':
-          mk = 'v'
-
-        # Plot the micro-step variable on the x-axis (i.e Time)
-        ln = plot_ax.plot(df[self._microName], df[var], marker=mk, linestyle=ls, label=var_label, color=f"C{cidx}")
-        lines.extend(ln)
-        ax.set_title(key.title())
-        ax.set_xlabel(self._microName)
-        ax.legend(lines, [l.get_label() for l in lines], loc='center left', bbox_to_anchor=(1.03, 0.5))
-
+        # Fill the positive, negative, and level lists
+        cindex = key + "," + comp_name # key for cdict dictionary
+        if (df[var] != 0).any(): # no plotting variables that have all zeros values
+          if tracker == 'level':
+            level_dat.append(var)
+            level_label.append(var_label)
+            level_color.append(cdict.get(cindex))
+          else:
+            if (df[var] > 0).any():
+                positive_dat.append(var)
+                positive_label.append(var_label)
+                positive_color.append(cdict.get(cindex))
+            else:
+                negative_dat.append(var)
+                negative_label.append(var_label)
+                negative_color.append(cdict.get(cindex))
+      # Plot the micro-step variable on the x-axis (i.e Time)
+      # Stackplot
+      ax.stackplot(df[self._microName],*[df[key] for key in positive_dat],labels= positive_label, baseline='zero', colors= [color+alpha for color in positive_color[:len(negative_dat)]]+[Gray])
+      ax.stackplot(df[self._microName],*[df[key] for key in negative_dat], labels= negative_label, baseline='zero', colors= [color+alpha for color in negative_color[:len(negative_dat)]] +[Gray])
+      # Lineplot
+      for key, c, llabel in zip(level_dat, level_color[:len(level_dat)] + [Dark], level_label[:len(level_dat)]):
+        ax2.plot(df[self._microName], df[key], linestyle=ls, label=llabel, color=c )
+      # Set figure title, legend, and grid
+      ax.set_title(key.title().split('_')[-1])
+      ax.set_xlabel(self._microName)
+      if(len(positive_label) > 0 or len(negative_label) > 0):
+        ax.legend(loc='upper left', bbox_to_anchor=(1.1, 0.6), fontsize = 10)
+      if(len(level_label) > 0):
+        ax2.legend(loc='lower left', bbox_to_anchor=(1.1, 0.6), fontsize = 10)
+      # Add the label and adjust location
+      ax.set_ylabel('Activity', fontsize=10, rotation=0)
+      ax2.set_ylabel('Level', fontsize=10, rotation=0)
+      ax.yaxis.set_label_coords(-0.01,1.02)
+      ax2.yaxis.set_label_coords(1,1.07)
+      ax.grid(None)
+      ax2.grid(None)
     # Output and save the image
     file_name = f"dispatch_id{sid}_y{mstep}_c{cid}.png"
     fig.tight_layout()
     fig.savefig(file_name)
     self.raiseAMessage(f'Saved figure to "{file_name}"')
     plt.clf()
 
@@ -175,14 +208,60 @@
 
     signal_file_name = f"dispatch_id{sid}_y{mstep}_c{cid}_SIGNAL.png"
     fig.tight_layout()
     fig.savefig(signal_file_name)
     self.raiseAMessage(f'Saved figure to "{signal_file_name}"')
     plt.clf()
 
+  def color_style(self, grp_vars):
+    """
+      @ In, grp_vars, Dict[str, List[str]], a dictionary mapping components to variables.
+      @ Out, colors, Dict[str, str], contains color code for variables
+    """
+    resources = [] # Determine the number of colormaps
+    technologis = [] # Determine the number of colors obtained from a colormap
+    for key, group in grp_vars.items():
+      resources.append(key)
+      for var in group:
+        _, comp_name, tracker, _ = var.split('__')
+        technologis.append(key + ',' + comp_name)
+    # remve duplicates
+    resources = list(dict.fromkeys(resources))
+    technologis = list(dict.fromkeys(technologis))
+    # colormap codes - can be changed to preferred colormaps - 17 in total 'Sequential' series
+    cm_codes = ['Purples', 'Blues', 'Greens', 'Oranges', 'Reds','YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu','GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn']
+    sample_cm = random.sample(cm_codes, len(resources))
+    resource_cm = {} # E.g. {'heat': 'OrRd', 'electricity': 'GnBu'} all string
+    i = 0
+    for s in resources:
+      resource_cm[s] = sample_cm[i] + '_r' #reverse colormap so it won't pick the lightest color that is almost invisible
+      i = i + 1
+    # Get the number of colors needed
+    resource_count = {} # E.g. {'heat': 5, 'electricity': 5}
+    for s in resources:
+      count = 0
+      for t in technologis:
+        if s in t:
+          count = count + 1
+      resource_count[s] = count
+    # Assign colors
+    colors = {}
+    for s in resources:
+      cm = mpl.cm.get_cmap(name= resource_cm[s])
+      # Get a subset of color map from 0 - 0.8 to avoid invisble light colors
+      cm = mpl.colors.LinearSegmentedColormap.from_list('trunc({n},{a:.2f},{b:.2f})'.format(n=cm.name, a=0, b=0.8),cm(np.linspace(0, 0.8)))
+      j = 0
+      for t in technologis:
+        clist = [cm(1.*i/resource_count[s]) for i in range(resource_count[s])] #color list
+        clist.reverse()
+        if s in t:
+          colors[t] = mpl.colors.rgb2hex(clist[j])
+          j = j + 1
+    return colors
+
   def run(self):
     """
       Generate the plot
       @ In, None
       @ Out, None
     """
     assert self._source is not None
@@ -191,20 +270,20 @@
       self.raiseAWarning(f'No data in "{self._source.name}" data object; nothing to plot!')
       return
     df = ds.to_dataframe().reset_index()
     dispatch_vars = list(filter(lambda x: "Dispatch__" in x, df.columns))
     grouped_vars = self._group_by(dispatch_vars, -1)
     grouped_comp = self._group_by(dispatch_vars, 1)
     comp_idx = {comp: i for i, comp in enumerate(grouped_comp.keys())}
-
     # Dimension variables to plot
     sample_ids = df[self._source.sampleTag].unique()
     cluster_ids = df['_ROM_Cluster'].unique()  # TODO: find way to not hardcode name
     macro_steps = df[self._macroName].unique()
-
+    # Assign colors
+    cdict = self.color_style(grouped_vars)
     for sample_id, macro_step, cluster_id in it.product(sample_ids, macro_steps, cluster_ids):
       # Filter data to plot correct values for current dimension
       dat = df[
         (df[self._source.sampleTag] == sample_id) &
         (df[self._macroName] == macro_step) &
         (df['_ROM_Cluster'] == cluster_id)
       ]
@@ -212,12 +291,12 @@
       # TODO: find a way to combine both plots into one output.
       # Currently, this is difficult to do because of the nested
       # nature of the subplots, as well as the dynamic number of
       # components and signals to plot (i.e. dynamically nested subplots)
 
       # Output optimized component dispatch for current dimension.
       fig0, axs0 = plt.subplots(len(grouped_vars), 1, sharex=True, squeeze=False)
-      self.plot_component(fig0, axs0, dat, grouped_vars, comp_idx, sample_id, macro_step, cluster_id)
+      self.plot_component(fig0, axs0, dat, grouped_vars, comp_idx, sample_id, macro_step, cluster_id, cdict)
 
       # Output synthetic time series signal for current dimension.
       fig1, axs1 = plt.subplots(len(self._addSignals), 1, sharex=True, squeeze=False)
       self.plot_signal(fig1, axs1, dat, sample_id, macro_step, cluster_id)
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Economics.py` & `heron-ravenframework-0.3/HERON/src/Economics.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,14 +440,16 @@
     """
     vp = ValuedParamHandler(name)
     signal = vp.read('CashFlow \'{}\''.format(self.name), spec, None) # TODO what "mode" to use?
     self._signals.update(signal)
     self._crossrefs[name] = vp
     # standard alias: redirect "capacity" variable
     if isinstance(vp, ValuedParams.factory.returnClass('variable')) and vp._raven_var == 'capacity':
+      #NOTE: we are assuming here that capacity_factors are only applied in dispatch and
+      # are not a variable in the outer optimization.
       vp = self._component.get_capacity_param()
     setattr(self, name, vp)
 
   def get_alpha_extension(self):
     """
       creates multiplier for the valued shape the alpha cashflow parameter should be in
       @ In, None,
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Herd.py` & `heron-ravenframework-0.3/HERON/src/Herd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # Copyright 2022, Battelle Energy Alliance, LLC
 # ALL RIGHTS RESERVED
 """
   New HERON workflow for setting up and running DISPATCHES cases
   (HE)RON (R)uns (D)ISPATCHES (HERD)
 """
 import os.path as path
-import json
 import sys
+import time
 import copy
 import operator
 import pandas as pd
 from itertools import compress
 import pyomo.environ as pyo
 from pyomo.opt import SolverFactory
 import numpy as np
 import _utils as hutils
+from functools import partial
+import logging
 try:
   import ravenframework
 except ModuleNotFoundError:
   path_to_raven = hutils.get_raven_loc()
   sys.path.append(path.abspath(path.join(path_to_raven, 'plugins')))
   sys.path.append(path_to_raven)
 from ravenframework.utils import xmlUtils
 from ravenframework.ROMExternal import ROMLoader
 
-# Nuclear flowsheet function imports
 # NOTE: these paths will change for next DISPATCHES release
-from dispatches.models.nuclear_case.flowsheets.nuclear_flowsheet import build_ne_flowsheet
-from dispatches.models.nuclear_case.flowsheets.nuclear_flowsheet import fix_dof_and_initialize
-
-# Import function for the construction of the multiperiod model
-from dispatches.models.nuclear_case.flowsheets.multiperiod import build_multiperiod_design
-
-from idaes.core.solvers import get_solver
+try:
+  # Nuclear flowsheet function imports
+  from dispatches.case_studies.nuclear_case.nuclear_flowsheet import (build_ne_flowsheet,
+                                                                      fix_dof_and_initialize)
+  # Import function for the construction of the multiperiod model
+  from idaes.apps.grid_integration import MultiPeriodModel
+  from idaes.core.solvers import get_solver
+except ModuleNotFoundError:
+  print("DISPATCHES has not been found in current conda environment. This is only needed when "+
+        "running the DISPATCHES workflow through HERD.")
 
 # append path with RAVEN location
 path_to_raven = hutils.get_raven_loc()
 sys.path.append(path.abspath(path.join(path_to_raven, 'scripts')))
 sys.path.append(path.abspath(path.join(path_to_raven, 'plugins')))
 sys.path.append(path_to_raven)
 
@@ -72,29 +76,27 @@
       "Produces": 'electricity',
       "Consumes": 'hydrogen',
       "Cashflows":{
         "Capacity":{
           "Expressions": 'h2_turbine_capacity',
         },
         "Dispatch":{
-          "Expressions": ['fs.h2_turbine.turbine.work_mechanical',
-            'fs.h2_turbine.compressor.work_mechanical'],
-          "Multiplier":  [-1, -1] # extra multiplier to ensure correct sign
+          "Expressions": ['fs.h2_turbine.work_mechanical'],
+          "Multiplier":  [-1] # extra multiplier to ensure correct sign
         },
       },
     },
     "electricity_market":{
       "Demands":  'electricity',
       "Consumes": {},
       "Cashflows":{
         "Dispatch":{
           "Expressions": ['fs.np_power_split.np_to_grid_port.electricity',
-            'fs.h2_turbine.turbine.work_mechanical',
-            'fs.h2_turbine.compressor.work_mechanical'],
-          "Multiplier":  [1e-3, -1e-6, -1e-6] # NOTE: h2 turbine is in W, convert to kW
+            'fs.h2_turbine.work_mechanical'],
+          "Multiplier":  [1e-3, -1e-6] # NOTE: h2 turbine is in W, convert to kW
         },
       },
     },
     "h2_market":{
       "Demands":  'hydrogen',
       "Consumes": {},
       "Cashflows":{
@@ -121,22 +123,25 @@
       @ Out, None
     """
     # running the init for MOPED first to initialize empty params
     super().__init__()
 
     # extra parameters for HERD
     self._dmdl = None # Pyomo model specific to DISPATCHES (different from _m)
+    self._dispatches_model_name = ''
     self._dispatches_model_template = None # Template of DISPATCHES Model for HERON comparison
     self._dispatches_model_comp_names = None # keys of the dispatches_model_template
     self._time_index_map = ['years', 'days', 'hours'] # index map to save time sets to dict later
     self._metrics = []     # TEAL metrics, summed expressions
     self._results = None   # results from Dispatch solve
     self._num_samples = 0  # number of samples/scenarios/realizations for easier retrievability
     self._demand_meta = {} # saving demand data to separate dict (in case it is also sampled)
-    self._synth_histories = {}  # nested dict of all synthetic histories
+    self._synth_histories = {}  # nested dict of all generated synthetic histories
+    self._time_sets = {}
+    self._multiperiod_options = {}
 
     # Testing - using LMP signals from JSON script as used in example Jupyter notebook
     #    intended years to test out (2022-2031, use same data. 2032-2041, use same data)
     self._test_mode = False
     self._test_synth_years = []  # the actual years to test out, [2022, 2032]
     self._test_proj_life = 0     # intended length of project, regardless of synth_years
     self._test_project_year_range = [] # actual years of project [2022, 2023, 2024, ...]
@@ -144,25 +149,28 @@
 
   def _set_test_time_sets(self):
     """
       Sets object attributes for time sets specifically for JSON test.
       @ In, None
       @ Out, None
     """
-    self._test_synth_years = [2022]
+    self._test_synth_years = [2022, ]
     self._test_proj_life = 20
     # range of years through intended project life (_test_synth_years contained within this set)
     #   year[0]-1 is the construction year
     self._test_project_year_range =  np.arange(self._test_synth_years[0],
                                             self._test_synth_years[0] + self._test_proj_life)
     # array map, same length as project year range but with entries in _test_synth_years
     test_synth_years = self._test_synth_years
     self._test_map_synth_to_proj = np.array([test_synth_years[sum(y>=test_synth_years) - 1]
                                             for y in self._test_project_year_range])
 
+  # ===================
+  # COLLECT METADATA
+  # ===================
   def buildEconSettings(self, verbosity=0):
     """
       Builds TEAL economic settings for running cashflows
       @ In, verbosity, int or string, verbosity settings for TEAL
       @ Out, None
     """
     # checking for a specific case - testing the DISPATCHES base Nuclear Case
@@ -252,45 +260,106 @@
 
     # sample synthetic histories
     elif mode == 'SyntheticHistory':
       self.raiseADebug(f'|Building pyomo parameter with synthetic histories for {comp.name}|')
       synth_hist = self.loadSyntheticHistory( getattr(value, "_var_name"), capacity_mult ) # runs external ROM load
       self._component_meta[comp.name][mode] = synth_hist
 
+    # sample static histories
+    elif mode == 'StaticHistory':
+      self.raiseADebug(f'|Building pyomo parameter with static histories for {comp.name}|')
+      synth_hist = self.loadStaticHistory( getattr(value, "_var_name"), capacity_mult ) # runs external ROM load
+      self._component_meta[comp.name][mode] = synth_hist
+
     # cannot do sweep values yet
     elif mode == 'SweepValues': # TODO Add capability to handle sweepvalues
       raise IOError('HERD does not currently support sweep values option')
 
     # NOTE not all producers consume
     # TODO should we handle transfer functions here?
     if consumes:
       for con in getattr(action, "_consumes"):
         self._component_meta[comp.name]['Consumes'][con] = getattr(action, "_transfer")
 
-  def sample_from_ROM(self, signal, multiplier):
+  def loadSyntheticHistory(self, signal, multiplier):
     """
-      Loads synthetic history for a specified signal, from given ROM.
+      Loads synthetic history for a specified signal, also sets yearly hours.
+      Calls the parent method and restructures dictionary to match DISPATCHES format.
       @ In, signal, string, name of signal to sample
-      @ In, multiplier, int/float, value to multiply synthetic history evaluations by
-      @ Out, synthetic_data, dict, contains data from evaluated ROM
+      @ Out, synthetic_histories, dict, contains data from evaluated ROM
     """
+    if signal == 'Signal' and multiplier == -1:
+      multiplier *= -1 # undoing negative multiplier from one step above, price != demand
+
     # NOTE self._sources[0]._var_names are the user assigned signal names in DataGenerators
     source = getattr(self, "_sources")[0]
     source_var_names = getattr(source, "_var_names")
 
     # check that signal name is available within data generator
     if signal not in source_var_names:
       raise IOError('The requested signal name is not available'
                     'from the synthetic history, check DataGenerators node in input')
 
     # Initializing ravenROMexternal object gives PATH access to xmlUtils
     target_file = getattr(source, "_target_file")
     runner = ROMLoader( binaryFileName=target_file)
 
     # TODO expand to change other pickledROM settings withing this method
+    synthetic_data = self._generate_synthetic_histories(runner, signal, multiplier)
+
+    # check that evaluation mode is either clustered or full
+    if self._eval_mode not in ['clustered', 'full']:
+      raise IOError('Improper ROM evaluation mode detected, try "clustered" or "full".')
+
+    # extracting cluster info from ROM - how many days of year per cluster?
+    synthetic_data = self._get_cluster_info_from_synth_histories(runner, synthetic_data)
+
+    synth_years, synth_days, synth_hours = [synthetic_data[ind] for ind in self._time_index_map]
+    synth_scenarios  = range(self._num_samples)
+    proj_years_range = self._test_project_year_range
+    map_synth2proj   = self._test_map_synth_to_proj
+
+    # restructure the synthetic history dictionary to match DISPATCHES
+    synth_histories = {}
+    synth_histories['signals'] = {}
+    # converting to dictionary that plays nice with DISPATCHES/IDAES
+    for key, data in synthetic_data.items():
+      # assuming the keys are in format "Realization_i"
+      if "Realization" in key:
+        # realizations (known as scenarios in DISPATCHES) index starting at 0
+        k = int( key.split('_')[-1] )
+        # years indexed by integer year (2020, etc.)
+        # clusters and hours indexed starting at 1
+        synth_histories['signals'][synth_scenarios[k-1]] = {year: {day: {hour: data[y, day-1, hour-1]
+                                                                  for hour in synth_hours}
+                                                        for day in synth_days}
+                                                  for y, year in enumerate(synth_years)}
+    # save set time data for use within DISPATCHES
+    synth_histories["sets"] = {}
+    synth_histories["sets"]["synth_scenarios"] = list(synth_scenarios) # DISPATCHES wants this as a list
+    synth_histories["sets"]["synth_years"]  = np.unique(synth_years) # DISPATCHES wants this as a list
+    synth_histories["sets"]["synth_days"]   = np.unique(synth_days)  # DISPATCHES wants this as a range
+    synth_histories["sets"]["synth_hours"]  = np.unique(synth_hours) # DISPATCHES wants this as a range
+    synth_histories["sets"]["map_synth2proj"] = map_synth2proj # used only for tests
+    synth_histories["sets"]["proj_years_range"] = proj_years_range # used only for tests
+    # getting weights_days - how many days does each cluster represent?
+    synth_histories["weights_days"] = synthetic_data['weights_days']
+
+    # saving a copy to self, referred to later when adding timesets to Pyomo model
+    self._synth_histories[signal] = copy.deepcopy(synth_histories)
+    return synth_histories
+
+  def _generate_synthetic_histories(self, runner, signal, multiplier):
+    """
+      Samples from external ROM given a signal and multiplier for said signal
+      @ In, runner, ROM loader, external ROM loader object
+      @ In, signal, str, name of signal to sample
+      @ In, multiplier, float or int, multiplier for given signal
+      @ Out, synthetic_data, dict, dictionary of samples from ROM
+    """
     inp = {'scaling': [1]}
     nodes = []
     node = xmlUtils.newNode('ROM', attrib={'name': 'SyntheticHistory', 'subType': 'pickledRom'})
     node.append(xmlUtils.newNode('clusterEvalMode', text=self._eval_mode))
     nodes.append(node)
     runner.setAdditionalParams(nodes)
 
@@ -306,159 +375,177 @@
         # reshape so that a filler cluster index is made
         current_realization[signal] = np.expand_dims(current_realization[signal], axis=1)
       synthetic_data[name] = current_realization[signal]
 
     # saving index map, often looks like ["Year", "ROM Cluster", "Hour"]
     synthetic_data['indexMap'] = current_realization['_indexMap'][0][signal]
 
-    # get time set data from ROM realizations
+    # set time set data
     years, days, hours = self._time_index_map # defined in __init__, order matters
     for ind in synthetic_data['indexMap']:
       # for year set, we truncate based on desired Project Time (28 yrs available)
       if ind.lower() in 'years':
         projLife = int( getattr(self._case, '_global_econ')['ProjectTime'] )
         synthetic_data[years] = np.array(current_realization[ind][0:projLife], dtype=int)
       elif ind.lower() in '_rom_cluster_days':
         synthetic_data[days]  = np.array(current_realization[ind] + 1, dtype=int)
       elif ind.lower() in 'timehours':
         synthetic_data[hours] = np.array(current_realization[ind] + 1, dtype=int)
 
+    return synthetic_data
+
+  def _get_cluster_info_from_synth_histories(self, runner, synthetic_data):
+    """
+      Extracts cluster information and sets to synthetic data dictionary
+      as weights for number of days simulated per year
+      @ In, runner, ROM loader, external ROM loader object
+      @ In, synthetic_data, dict, dictionary of samples from ROM
+      @ Out, synthetic_data, dict, dictionary of samples from ROM
+    """
+    years, days, __ = self._time_index_map # defined in __init__, order matters
+
     # extracting cluster info from ROM - how many days of year per cluster?
     #    location: runner.rom._segmentROM._macroSteps[2018]._clusterInfo['map']
     #    using attrgetter to get rid of "access to protected member" warning
     cluster_steps = operator.attrgetter('_segmentROM._macroSteps')(runner.rom)
     synthetic_data['weights_days'] = {}
     for year in synthetic_data[years]:
       synthetic_data['weights_days'][year] = {}
       for cluster in synthetic_data[days]:
         cluster_map = operator.attrgetter('_clusterInfo')(cluster_steps[year])['map']
         index = int(cluster-1)
         synthetic_data['weights_days'][year][cluster] = len(cluster_map[index])
 
-    # check that evaluation mode is either clustered or full
-    if self._eval_mode not in ['clustered', 'full']:
-      raise IOError('Improper ROM evaluation mode detected, try "clustered" or "full".')
     return synthetic_data
 
-  def load_synthetic_history_from_JSON(self):
+  def loadStaticHistory(self, signal, multiplier):
     """
-      Load synthetic history data specifically from a JSON file (very specific for testing)
-      @ In, None
-      @ Out, fullHist, dict, synthetic history with set data
+      Loads static history for a specified signal,
+      also sets yearly hours and pyomo indexing sets
+      @ In, signal, string, name of signal to sample
+      @ In, multiplier, int/float, value to multiply synthetic history evaluations by
+      @ Out, synthetic_data, dict, contains data from evaluated ROM
+    """
+    if signal == 'Signal' and multiplier == -1:
+      multiplier *= -1 # undoing negative multiplier from one step above, price != demand
+
+    # NOTE self._sources[0]._var_names are the user assigned signal names in DataGenerators
+    source = getattr(self, "_sources")[0]
+    source_var_names = getattr(source, "_var_names")
+
+    # check that signal name is available within data generator
+    if signal not in source_var_names:
+      raise IOError('The requested signal name is not available'
+                    'from the static history, check DataGenerators node in input')
+
+    # paths to LMP signal data in CSV (reformatted from DISPATCHES JSON file)
+    lmp_path  = getattr(source, "_target_file")
+    data_frame = pd.read_csv(lmp_path) # loading csv data
+    synthetic_data = self._get_synthetic_histories_from_dataframe( data_frame, signal, multiplier)
+
+    # saving a copy to self, referred to later when adding timesets to Pyomo model
+    self._synth_histories[signal] = copy.deepcopy(synthetic_data)
+    return synthetic_data
+
+  def _get_synthetic_histories_from_dataframe(self, data_frame, signal, multiplier):
     """
-    # paths to LMP signal JSON within DISPATCHES
-    # TODO: move a copy of this file to HERD? or convert to static history
-    disp_nuc_path = path.dirname( build_multiperiod_design.__code__.co_filename )
-    lmp_path  = path.abspath( path.join(disp_nuc_path, "lmp_signal.json") )
-
-    # loading JSON data
-    with open(lmp_path, encoding='utf-8') as fp:
-      synth_hist = json.load(fp)
+      Samples from external ROM given a signal and multiplier for said signal
+      @ In, data_frame, Pandas DataFrame object, dataframe with imported csv signals
+      @ In, signal, str, name of signal to sample
+      @ In, multiplier, float or int, multiplier for given signal
+      @ Out, synthetic_data, dict, dictionary of samples from ROM
+    """
+    macro_var_name = self._case.get_year_name() # e.g., Year
+    micro_var_name = self._case.get_time_name() # e.g., Time
+
+    # check that all required columns are present in dataframe
+    required_columns = ['RAVEN_sample_ID', macro_var_name, micro_var_name, signal]
+    assert np.all([rcol in data_frame.columns for rcol in required_columns])
 
     # data is the same for 2022-2031, and 2032-2041
     #   to save on # of variables, just duplicate LMP values
-    synth_years = self._test_synth_years # actual years to gather data from e.g., [2022, 2032]
+    assert len(self._test_synth_years) <= self._test_proj_life
 
     # building array of simulation years
-    proj_life_range = self._test_project_year_range # actual year range for full project [2022->2041]
-    set_years_map = self._test_map_synth_to_proj # array looks like [2022, 2022, ...., 2032, 2032, ...]
+    years_range = self._test_project_year_range # actual year range for project [2022->2041]
+    years_map   = self._test_map_synth_to_proj # array => [2022, 2022, ...., 2032, 2032, ...]
 
-    # creating set of scenarios/realizations/samples
-    n_scenarios = self._num_samples
-    set_scenarios = list( range(n_scenarios) )
-
-    # we have to rebuild the LMP signal, using set_years as a map for when to duplicate data
-    if len(synth_years) < self._test_proj_life:
-      full_hist = {}
-      # looping through scenarios, re-building LMP signal if necessary
-      for r in set_scenarios:
-        # output dict key is actual year, input dict key is mapped year with duplicates
-        full_hist[str(r)] = {str(y): synth_hist[str(r)][str(i)]
-                                for i,y in zip(set_years_map, proj_life_range)}
-    else:
-      # same dictionary
-      full_hist = synth_hist
+    # calculating time set lengths from full CSV
+    n_columns = len(data_frame.columns)
+    n_pts     = len( data_frame )
+    n_scenarios  = len( np.unique( getattr(data_frame, 'RAVEN_sample_ID') ) )
+    n_years_data = len( np.unique( getattr(data_frame, macro_var_name) ) )
+    n_time       = len( np.unique( getattr(data_frame, micro_var_name) ) )
+    n_clusters   = int( n_pts / n_scenarios / n_years_data / n_time ) # if == 1, full year data
+
+    if 'Cluster_weight' not in data_frame.columns:
+      ones = np.ones(n_pts, dtype=int)
+      data_frame.insert(loc=n_columns, column="Cluster_weight", value=ones)
+
+    # creating set data for time series
+    set_scenarios  = range(self._num_samples)
+    set_days = range(1, int(n_clusters+1) ) if n_clusters != 1 else [1]
+    set_time = range(1, int(n_time+1) )
 
-    n_days = len(synth_hist['0']['2020'].keys())
-    n_time = len(synth_hist['0']['2020']['1'].keys()) - 1
-    full_hist['years'] = synth_years
-    full_hist['days']  = range(1, int(n_days + 1) )
-    full_hist['hours'] = range(1, int(n_time + 1) )
-
-    return full_hist
-
-  def loadSyntheticHistory(self, signal, multiplier):
-    """
-      Loads synthetic history for a specified signal, also sets yearly hours.
-      Calls the parent method and restructures dictionary to match DISPATCHES format.
-      @ In, signal, string, name of signal to sample
-      @ Out, new_ist, dict, contains data from evaluated ROM
-    """
-    if signal == 'price' and multiplier == -1:
-      multiplier *= -1 # undoing negative multiplier from one step above, price != demand
+    # create empty data dictionary
+    synthetic_data = {}
+    synthetic_data['signals'] = {}
+    synthetic_data['weights_days'] = {}
+    synthetic_data['sets'] = {}
 
-    # calling parent method for loading synthetic history
-    test_JSON = (signal == 'dispatches-test' and self._test_mode)
+    # sample realizations/scenarios from CSV
+    for real in set_scenarios:
+      synthetic_data['signals'][real] = {}  # empty dict for this scenario signals
+      df_realization = data_frame.loc[data_frame['RAVEN_sample_ID'] == real] # subset of dataframe
 
-    if test_JSON:
-      synth_hist = self.load_synthetic_history_from_JSON()
-    else: # normal extraction
-      synth_hist = self.sample_from_ROM(signal, multiplier)
+      # loop through the year map + actual continuous project year range
+      for y_map, y_actual in zip(years_map, years_range):
+        synthetic_data['signals'][real][y_actual] = {}  # empty dict for this year signals
+        synthetic_data['weights_days'][y_actual]  = {}
+
+        assert np.sum(df_realization[macro_var_name] == y_map) > 0
+        df_year = df_realization.loc[df_realization[macro_var_name] == y_map] # subset of dataframe
+
+        # loop through all clusters/days per year
+        for cluster in set_days:
+          # number of days represented by first 24 hrs
+          cluster_num = df_year['Cluster_weight'].head(1).to_list()[0]
+          synthetic_data["weights_days"][y_actual][cluster] = cluster_num
+
+          # subset of dataframe for given cluster
+          df_cluster = df_year.loc[df_year['Cluster_weight'] == cluster_num]
+
+          # get signal for given cluster, set to dict indexed by Time
+          signal_data = df_cluster.head(n_time)[signal].to_numpy()
+          signal_data *= multiplier
+          synthetic_data['signals'][real][y_actual][cluster] = dict( zip(set_time, signal_data) )
+
+          # remove data points that have already been used
+          df_year = df_year.drop(df_cluster.index[:n_time])
+          # delete temporary dataframe subsets
+          del df_cluster
+        del df_year
+      del df_realization
 
-    synth_years, synth_days, synth_hours = [synth_hist[ind] for ind in self._time_index_map]
-    synth_scenarios = range(self._num_samples)
-    proj_years_range = self._test_project_year_range
-    map_synth2proj = self._test_map_synth_to_proj
-    # restructure the synthetic history dictionary to match DISPATCHES
-    new_hist = {}
-    new_hist['signals'] = {}
-    # converting to dictionary that plays nice with DISPATCHES/IDAES
-    if test_JSON:
-      for scenario in synth_scenarios:
-        new_hist['signals'][scenario] = {year: {day: {hour:
-                                        synth_hist[str(scenario)][str(year)][str(day)][str(hour)]
-                                                      for hour in synth_hours}
-                                              for day in synth_days}
-                                      for year in proj_years_range}
-    else:
-      for key, data in synth_hist.items():
-        # assuming the keys are in format "Realization_i"
-        if "Realization" in key:
-          # realizations known as scenarios in DISPATCHES, index starting at 0
-          k = int( key.split('_')[-1] )
-          # years indexed by integer year (2020, etc.)
-          # clusters and hours indexed starting at 1
-          new_hist['signals'][synth_scenarios[k-1]] = {year: {day: {hour: data[y, day-1, hour-1]
-                                                                    for hour in synth_hours}
-                                                          for day in synth_days}
-                                                    for y, year in enumerate(synth_years)}
     # save set time data for use within DISPATCHES
-    new_hist["sets"] = {}
-    new_hist["sets"]["synth_scenarios"] = list(synth_scenarios) # DISPATCHES wants this as a list
-    new_hist["sets"]["synth_years"]  = np.unique(synth_years) # DISPATCHES wants this as a list
-    new_hist["sets"]["synth_days"]   = np.unique(synth_days)  # DISPATCHES wants this as a range
-    new_hist["sets"]["synth_hours"]  = np.unique(synth_hours) # DISPATCHES wants this as a range
-    new_hist["sets"]["map_synth2proj"] = map_synth2proj # used only for tests
-    new_hist["sets"]["proj_years_range"] = proj_years_range # used only for tests
-    # getting weights_days - how many days does each cluster represent?
-    if test_JSON:
-      new_hist["weights_days"] = {yr: {cl: synth_hist[str(0)][str(yr)][str(cl)]["num_days"]
-                                      for cl in synth_days}
-                                for yr in synth_years}
-    else:
-      new_hist["weights_days"] = synth_hist['weights_days']
+    synthetic_data["sets"]["synth_scenarios"] = list(set_scenarios) # DISPATCHES wants this as a list
+    synthetic_data["sets"]["synth_years"]  = self._test_synth_years # DISPATCHES wants this as a list
+    synthetic_data["sets"]["synth_days"]   = set_days  # DISPATCHES wants this as a range
+    synthetic_data["sets"]["synth_hours"]  = set_time # DISPATCHES wants this as a range
+    synthetic_data["sets"]["map_synth2proj"]   = years_map # used only for tests
+    synthetic_data["sets"]["proj_years_range"] = years_range # used only for tests
 
-    # saving a copy to self, referred to later when adding timesets to Pyomo model
-    self._synth_histories[signal] = copy.deepcopy(new_hist)
-    return new_hist
+    return synthetic_data
 
+  # ===========================
+  # DISPATCHES COMPATIBILITY
+  # ===========================
   def _check_dispatches_compatibility(self):
     """
-      Checks HERON components to match compatibility with available
-      DISPATCHES flowsheets.
+      Checks HERON components to match compatibility with available DISPATCHES flowsheets.
       @ In, None
       @ Out, None
     """
     # TODO: check for financial params/inputs?
     heron_comp_list = list( self._component_meta.keys() ) # current list of HERON components
     self.raiseADebug('|Checking compatibility between HERON and available DISPATCHES cases|')
 
@@ -508,97 +595,71 @@
         if sum(mismatched_actions) > 0:
           message = f'Attributes of HERON Component {dComp} do not match DISPATCHES case: '
           message += ', '.join( list(compress(dispatches_actions_list, mismatched_actions)) )
           raise IOError(message)
       break
 
     self.raiseADebug(f'|HERON Case is compatible with {dName} DISPATCHES Model|')
+    self._dispatches_model_name = dName
     self._dispatches_model_template = DISPATCHES_MODEL_COMPONENT_META[dName] # NOTE: NOT using copy
     self._dispatches_model_comp_names = list(self._dispatches_model_template.keys())
 
-  def _add_sets_to_pyomo(self):
-    """
-      Create new DISPATCHES Pyomo Model with available data
-      @ In, None
-      @ Out, None
-    """
-    signals = list( self._synth_histories.keys() )
-
-    if 'dispatches-test' in signals:
-      market_synthetic_history = self._synth_histories['dispatches-test']
-    elif 'price' in signals:
-      market_synthetic_history = self._synth_histories['price']
-    elif 'Signal' in signals:
-      market_synthetic_history = self._synth_histories['Signal']
-    else:
-      raise IOError('Signal name not found in generated synthetic history dictionary')
-
-    # transferring information on Sets
-    sets = market_synthetic_history['sets']
-    self._dmdl.set_time  = np.unique(sets['synth_hours'])
-    self._dmdl.set_days  = np.unique(sets['synth_days'])
-    self._dmdl.set_years = np.unique(sets['synth_years'])
-    self._dmdl.set_years_map = sets['map_synth2proj'] if self._test_mode else sets['synth_years']
-    self._dmdl.set_scenarios = sets['synth_scenarios']
-
-    # transferring information on LMP Synthetic History signal
-    self._dmdl.LMP = market_synthetic_history['signals']
-
-    # transferring information on weightings
-    self._dmdl.weights_days = market_synthetic_history['weights_days']
-
-    # NOTE: equal probability for all scenarios
-    self._dmdl.weights_scenarios = {s:1/self._num_samples for s in range(self._num_samples)}
-
-  def _add_additional_constraints(self, mdl):
-    """
-      Method to add additional constraints not included in DISPATCHES flowsheet
-      @ In, mdl, Pyomo model
-      @ Out, None
-    """
-    @mdl.Constraint(self._dmdl.set_time, self._dmdl.set_days, self._dmdl.set_years)
-    def hydrogen_demand_constraint(blk, t, d, y):
-      return blk.period[t, d, y].fs.h2_tank.outlet_to_pipeline.flow_mol[0] \
-                <= self._demand_meta['h2_market']["Demand"] / 2.016e-3 # convert from kg to mol
-
+  # ==============
+  # BUILD MODEL
+  # ==============
   def _build_dispatches_model(self):
     """
       Builds full DISPATCHES Pyomo model
       @ In, None
       @ Out, None
     """
     # add time sets to Pyomo model from given synthetic history and desired project lifetime
-    self._add_sets_to_pyomo()
-
-    # pointing to necessary IDAES/DISPATCHES Physics models
-    mdl_flowsheet = build_ne_flowsheet # pointing to the imported DISPATCHES nuclear flowsheet
-    mdl_init  = fix_dof_and_initialize # pointing to the imported DISPATCHES fix/init method
-    mdl_unfix = self.unfixDof # we add a method to unfix certain DoFs based on DISPATCHES jupyter notebooks
+    self._time_sets = self._get_time_sets()
+    set_days      = self._time_sets['set_days']
+    set_years     = self._time_sets['set_years']
+    set_scenarios = self._time_sets['set_scenarios']
+    n_time_points = self._time_sets['n_time_points']
+
+    # get extra arguments/options to pass into Multiperiod model for flowsheet
+    self._multiperiod_options = self._get_multiperiod_flowsheet_options()
+    init_options      = self._multiperiod_options['initialization_options']
+    unfix_dof_options = self._multiperiod_options['unfix_dof_options']
+
+    # wrapping fs options in a dict allow extraction downstream and keep staging_params intact
+    flowsheet_options = {'fs_options':self._multiperiod_options['flowsheet_options']}
+
+    # using partial to sneak in an extra dictionary input to the call
+    staging_params = self._multiperiod_options['staging_params']
+    process_func   = partial(self.flowsheet_block, staging_params=staging_params)
 
     # NOTE: within the build process, a tmp JSON file is created in wdir...
-    build_multiperiod_design(self._dmdl,
-                         flowsheet=mdl_flowsheet,
-                         initialization=mdl_init,
-                         unfix_dof=mdl_unfix,
-                         unfix_dof_options={},
-                         multiple_days=True,
-                         multiyear=True,
-                         stochastic=True,
-                         verbose=False)
+    self._dmdl = MultiPeriodModel(
+                    n_time_points=n_time_points,
+                    set_days=set_days,
+                    set_years=set_years,
+                    set_scenarios=set_scenarios,
+                    process_model_func=process_func,
+                    initialization_func=fix_dof_and_initialize,
+                    unfix_dof_func=self.unfixDof,
+                    linking_variable_func=self._get_linking_variable_pairs,
+                    flowsheet_options=flowsheet_options,
+                    initialization_options=init_options,
+                    unfix_dof_options=unfix_dof_options,
+                    use_stochastic_build=True,
+                    outlvl=logging.INFO,
+                  )
 
     # list of initialized TEAL components; filters out HERON components that don't have cash flows
     teal_components, heron_components = self._initialize_cash_flows()
 
     # looping through all sampled scenarios
-    for s in self._dmdl.set_scenarios:
-      # Build the connecting constraints
-      self.build_connecting_constraints(self._dmdl.scenario[s],
-                                  set_time=self._dmdl.set_time,
-                                  set_days=self._dmdl.set_days,
-                                  set_years=self._dmdl.set_years)
+    for s in self._time_sets['set_scenarios']:
+
+      # Add first-stage variables
+      self._add_capacity_variables(self._dmdl.scenario[s])
 
       # Hydrogen demand constraint (Divide the RHS by the molecular mass to convert kg/s to mol/s)
       self._add_additional_constraints(self._dmdl.scenario[s])
 
       # Append cash flow expressions
       for hComp, tComp in zip(heron_components, teal_components): #this zip might be danger
         # skip components within HERON that are NOT defined in DISPATCHES template
@@ -608,14 +669,247 @@
         self._create_cash_flows_for_dispatches(self._dmdl.scenario[s], hComp, tComp, s)
 
       # compute desired metric using TEAL and storing it
       scenario_metric = RunCashFlow.run(self._econ_settings, teal_components, {}, pyomoVar=True)
       self._metrics.append( scenario_metric )
       del scenario_metric
 
+  def _get_time_sets(self):
+    """
+      Getting time set data from a saved synthetic history
+      @ In, None
+      @ Out, time_sets, dict, time set information for simulation
+    """
+    # NOTE: assuming here that we're not importing both static histories and synthetic histories
+    #       therefore all time sets are presumably the same (generated through the same method)
+    signal_name = list(self._synth_histories.keys())[0] # from our assumption, any signal will do
+    market_synthetic_history = self._synth_histories[signal_name]
+
+    # transferring information on Sets
+    sets = market_synthetic_history['sets']
+    time_sets = {}
+    time_sets['set_time']  = np.unique(sets['synth_hours'])
+    time_sets['set_days']  = np.unique(sets['synth_days'])
+    time_sets['set_years'] = np.unique(sets['synth_years'])
+    time_sets['set_years_map'] = sets['map_synth2proj'] if self._test_mode \
+                                                     else sets['synth_years']
+    time_sets['set_scenarios'] = sets['synth_scenarios']
+    time_sets['n_time_points'] = len(time_sets['set_time'])
+
+    # transferring information on weightings
+    time_sets['weights_days'] = market_synthetic_history['weights_days']
+    # NOTE: equal probability for all scenarios
+    time_sets['weights_scenarios'] = {s:1/self._num_samples for s in range(self._num_samples)}
+    return time_sets
+
+  def _get_multiperiod_flowsheet_options(self):
+    """
+      Getting extra arguments/options for flowsheet, initialization, and unfix_DOF methods
+      To be used within MultiPeriodModel init.
+      @ In, None
+      @ Out, multiperiod_options, dict, extra arguments for flowsheet and ancilliary methods
+    """
+    multiperiod_options = {}
+    multiperiod_options['flowsheet_options'] = {"np_capacity": 1000}
+    multiperiod_options['initialization_options'] = {
+                                "split_frac_grid": 0.8,
+                                "tank_holdup_previous": 0,
+                                "flow_mol_to_pipeline": 10,
+                                "flow_mol_to_turbine": 10,
+                              }
+    multiperiod_options['unfix_dof_options'] = {}
+    multiperiod_options['staging_params'] = {}
+
+    return multiperiod_options
+
+  #==== METHODS CALLED THROUGH IDAES ====#
+  def flowsheet_block(self, mdl, fs_options, staging_params):
+    """
+      Staging area for flowsheet call through the IDAES MultiPeriodModel class.
+      Note that the `staging_params` input is not part of the MultiPeriodModel call; it is
+      snuck in using `functools.partial` from the HERD call.
+
+      This is partially taken from
+      `dispatches.dispatches.case_studies.renewables_case.wind_battery_LMP.py`,
+      from the `wind_battery_mp_block( )` method.
+      @ In, mdl, Pyomo ConcreteModel or Pyomo BlockData object
+      @ In, fs_options, dict, arguments for flowsheet
+      @ In, staging_params, dict, extra arguments not intended for flowsheet
+      @ Out, None
+    """
+    if isinstance(mdl, pyo.ConcreteModel):
+      # building a simple model for the initialization method
+      mdl = build_ne_flowsheet(mdl, **fs_options)
+    else:
+      # this means mdl is a _BlockData object, being called from `build_stochastic_multi_period` for
+      # a given period (e.g., hr:10, d:2, yr:2022)
+      if 'pyo_model' not in staging_params.keys():
+        # if this is the first call, creates a Pyomo model with flowsheet attributes
+        # then saves it to the staging_params dictionary.
+        staging_params['pyo_model'] = build_ne_flowsheet(**fs_options)
+      # on subsequent calls, it just pulls the saved model, clones it, and transfers
+      # attributes to current period model
+      mdl.transfer_attributes_from(staging_params['pyo_model'].clone())
+
+  def unfixDof(self, ps, **kwargs):
+    """
+      This function unfixes a few degrees of freedom for optimization.
+
+      This is taken from `multiperiod_design_pricetaker.ipynb` in the DISPATCHES repository
+      found in `dispatches/dispatches/case_studies/nuclear_case/`
+      (currently not callable, so replicated here).
+      @In, ps, Pyomo model for period within a given scenario
+      @In, kwargs, extra arguments for flowsheet parameters
+      @ Out, None
+    """
+    # Set defaults in case options are not passed to the function
+    options = kwargs.get("options", {})
+    air_h2_ratio = options.get("air_h2_ratio", 10.76)
+
+    # Unfix the electricity split in the electrical splitter
+    ps.fs.np_power_split.split_fraction["np_to_grid", 0].unfix()
+
+    # Unfix the holdup_previous and outflow variables
+    ps.fs.h2_tank.tank_holdup_previous.unfix()
+    ps.fs.h2_tank.outlet_to_turbine.flow_mol.unfix()
+    ps.fs.h2_tank.outlet_to_pipeline.flow_mol.unfix()
+
+    # Unfix the flowrate of air to the mixer
+    ps.fs.mixer.air_feed.flow_mol.unfix()
+
+    # Add a constraint to maintain the air to hydrogen flow ratio
+    ps.fs.mixer.air_h2_ratio = pyo.Constraint(
+                expr=ps.fs.mixer.air_feed.flow_mol[int(0)] ==
+                      air_h2_ratio * ps.fs.mixer.hydrogen_feed.flow_mol[int(0)])
+
+    # Set bounds on variables. A small non-zero value is set as the lower
+    # bound on molar flowrates to avoid convergence issues
+    ps.fs.pem.outlet.flow_mol[0].setlb(0.001)
+
+    ps.fs.h2_tank.inlet.flow_mol[0].setlb(0.001)
+    ps.fs.h2_tank.outlet_to_turbine.flow_mol[0].setlb(0.001)
+    ps.fs.h2_tank.outlet_to_pipeline.flow_mol[0].setlb(0.001)
+
+    ps.fs.translator.inlet.flow_mol[0].setlb(0.001)
+    ps.fs.translator.outlet.flow_mol[0].setlb(0.001)
+
+    ps.fs.mixer.hydrogen_feed.flow_mol[0].setlb(0.001)
+
+  def _get_linking_variable_pairs(self, mdl_start, mdl_end):
+    """
+      Yield pairs of variables that need to be connected across time periods.
+
+      This is taken from `multiperiod_design_pricetaker.ipynb` in the DISPATCHES repository
+      found in `dispatches/dispatches/case_studies/nuclear_case/`
+      (currently not callable, so replicated here).
+      @ In, mdl_start, Pyomo model, current time step
+      @ In, mdl_end, Pyomo model, next time step
+      @ Out, pairs, list, pair of Pyomo expressions to link
+    """
+    pairs = [(mdl_start.fs.h2_tank.tank_holdup[0],
+              mdl_end.fs.h2_tank.tank_holdup_previous[0])]
+    return pairs
+
+  #==== METHODS FOR FLOWSHEET-SPECIFIC PYOMO PROCESSES ====#
+  def _add_capacity_variables(self, mdl):
+    """
+      Setting first-stage capacity variables for model.
+      Also sets upper bound constraints on resource production not exceeding capacity.
+
+      This is taken from `multiperiod_design_pricetaker.ipynb` in the DISPATCHES repository
+      found in `dispatches/dispatches/case_studies/nuclear_case/`
+      (currently not callable, so replicated here).
+      @ In, mdl, Pyomo model
+      @ Out, None
+    """
+    set_period = mdl.parent_block().set_period
+
+    # Declare first-stage variables (Design decisions)
+    mdl.pem_capacity = pyo.Var(within=pyo.NonNegativeReals,
+                                doc="Maximum capacity of the PEM electrolyzer (in kW)" )
+    mdl.tank_capacity = pyo.Var(within=pyo.NonNegativeReals,
+                                 doc="Maximum holdup of the tank (in mol)")
+    mdl.h2_turbine_capacity = pyo.Var(within=pyo.NonNegativeReals,
+                                       doc="Maximum power output from the turbine (in W)")
+
+    # initializing capacity constraints using set period from block
+    mdl.pem_capacity_constraint = pyo.Constraint(set_period)
+    mdl.tank_capacity_constraint = pyo.Constraint(set_period)
+    mdl.turbine_capacity_constraint = pyo.Constraint(set_period)
+
+    for t in set_period:
+      # Ensure that the electricity to the PEM elctrolyzer does not exceed the PEM capacity
+      mdl.pem_capacity_constraint.add(t,
+          mdl.period[t].fs.pem.electricity[0] <= mdl.pem_capacity)
+      # Ensure that the final tank holdup does not exceed the tank capacity
+      mdl.tank_capacity_constraint.add(t,
+          mdl.period[t].fs.h2_tank.tank_holdup[0] <= mdl.tank_capacity)
+      # Ensure that the power generated by the turbine does not exceed the turbine capacity
+      mdl.turbine_capacity_constraint.add(t,
+          -mdl.period[t].fs.h2_turbine.work_mechanical[0] <= mdl.h2_turbine_capacity)
+
+  def _add_additional_constraints(self, mdl):
+    """
+      Method to add additional constraints not included in DISPATCHES flowsheet
+
+      Some content is taken from `multiperiod_design_pricetaker.ipynb` in the DISPATCHES repository
+      found in `dispatches/dispatches/case_studies/nuclear_case/`
+      (currently not callable, so replicated here).
+      @ In, mdl, Pyomo scenario model
+      @ Out, None
+    """
+    set_time  = mdl.parent_block().set_time
+    set_days  = mdl.parent_block().set_days
+    set_years = mdl.parent_block().set_years
+
+    # Set initial holdup for each day (Assumed to be zero at the beginning of each day)
+    for y in set_years:
+      for d in set_days:
+        mdl.period[1, d, y].fs.h2_tank.tank_holdup_previous.fix(0)
+
+    @mdl.Constraint(set_time, set_days, set_years)
+    def hydrogen_demand_constraint(blk, t, d, y):
+      return blk.period[t, d, y].fs.h2_tank.outlet_to_pipeline.flow_mol[0] \
+                <= self._demand_meta['h2_market']["Demand"] / 2.016e-3 # convert from kg to mol
+
+  def _add_non_anticipativity_constraints(self):
+    """
+      Adding non-anticipativity constraints, ensuring that all capacity variables are the same
+      for all scenarios.
+
+      Content is taken from `multiperiod_design_pricetaker.ipynb` in the DISPATCHES repository
+      found in `dispatches/dispatches/case_studies/nuclear_case/`
+      (currently not callable, so replicated here).
+      @ In, None
+      @ Out, None
+    """
+    # temporary object pointing to model
+    dmdl = self._dmdl
+
+    # Add non-anticipativity constraints
+    dmdl.pem_capacity = pyo.Var(within=pyo.NonNegativeReals,
+                                doc="Design PEM capacity (in kW)")
+    dmdl.tank_capacity = pyo.Var(within=pyo.NonNegativeReals,
+                                 doc="Design tank capacity (in mol)")
+    dmdl.h2_turbine_capacity = pyo.Var(within=pyo.NonNegativeReals,
+                                       doc="Design turbine capacity (in W)")
+
+    @dmdl.Constraint(dmdl.set_scenarios)
+    def non_anticipativity_pem(blk, s):
+      return blk.pem_capacity == blk.scenario[s].pem_capacity
+
+    @dmdl.Constraint(dmdl.set_scenarios)
+    def non_anticipativity_tank(blk, s):
+      return blk.tank_capacity == blk.scenario[s].tank_capacity
+
+    @dmdl.Constraint(dmdl.set_scenarios)
+    def non_anticipativity_turbine(blk, s):
+      return blk.h2_turbine_capacity == blk.scenario[s].h2_turbine_capacity
+
+  #==== METHODS CREATING TEAL CASHFLOWS ====#
   def _initialize_cash_flows(self):
     """
       Initialize and populate TEAL cash flows for all components
       @ In, None
       @ Out, None
     """
     teal_components  = []
@@ -746,15 +1040,15 @@
 
     # time indeces for HERON/TEAL
     n_hours = len(self._dmdl.set_time)
     n_days  = len(self._dmdl.set_days)
     n_years = len(self._dmdl.set_years)
     n_hours_per_year = n_hours * n_days # sometimes number of days refers to clusters < 365
 
-    set_years_map = np.hstack([0, self._dmdl.set_years_map])
+    set_years_map = np.hstack([0, self._time_sets['set_years_map'] ])
 
     # template array for holding dispatch Pyomo expressions/objects
     dispatch_array = np.zeros((project_life, n_hours_per_year), dtype=object)
     dispatch_type = self._component_meta[hComp.name]['Dispatch']
 
     # TODO: there should be a more robust check of dispatch type, further upstream
     if dispatch_type == "fixed":
@@ -763,15 +1057,16 @@
 
     # extract Pyomo expressions from DISPATCHES objects
     cashflows_dict = dComp['Cashflows']
     dispatch_dict  = cashflows_dict['Dispatch']
     dispatch_strs  = dispatch_dict['Expressions']
 
     # time indeces for DISPATCHES, as array of tuples
-    indeces = np.array([tuple(i) for i in mdl.period_index], dtype="i,i,i")
+    set_period = mdl.parent_block().set_period
+    indeces = np.array([tuple(i) for i in set_period], dtype="i,i,i")
     time_shape = (n_years, n_hours_per_year) # reshaping the tuples array to match HERON dispatch
     indeces = indeces.reshape(time_shape)
 
     # extra multipliers specific to DISPATCHES (e.g., have to multiply turbine work done by -1)
     dMults = dispatch_dict['Multiplier'] \
                 if 'Multiplier' in dispatch_dict.keys() \
                 else np.ones(len(dispatch_strs)) # defaults to just 1
@@ -789,15 +1084,15 @@
         #   e.g., turbine costs due to work done by turbine + compressor, separate variables
         dispatch_driver = 0
         for ds, dStr in enumerate(dispatch_strs):
           dispatch_driver += operator.attrgetter(dStr)(mdl.period[ind])[0] * dMults[ds]
 
         # getting weights for each day/cluster
         dy, yr = ind[1:]
-        weight = self._dmdl.weights_days[yr][dy]  # extracting weight for year + day
+        weight = self._time_sets['weights_days'][yr][dy]  # extracting weight for year + day
 
         # storing individual Pyomo dispatch
         dispatch_array[p, time] = dispatch_driver * weight
 
     return dispatch_array
 
   def reshapeAlpha(self, alpha):
@@ -831,148 +1126,29 @@
                                       for t in set_time]
                                         for y in set_years] #shape here is [year, hour]
       # first column of 2nd axis is 0 for project year 0
       reshaped_alpha[real,1:,:] = realized_alpha
 
     return reshaped_alpha
 
-  def unfixDof(self, ps, **kwargs):
-    """
-      This function unfixes a few degrees of freedom for optimization.
-      This particular method is taken from the DISPATCHES jupyter notebook
-      found in "dispatches/dispatches/models/nuclear_case/flowsheets"
-      titled "multiperiod_design_pricetaker"
-      @In, ps, Pyomo model for period within a given scenario
-      @In, kwargs, extra arguments for flowsheet parameters
-      @ Out, None
-    """
-    # Set defaults in case options are not passed to the function
-    options = kwargs.get("options", {})
-    air_h2_ratio = options.get("air_h2_ratio", 10.76)
-
-    # Unfix the electricity split in the electrical splitter
-    ps.fs.np_power_split.split_fraction["np_to_grid", 0].unfix()
-
-    # Unfix the holdup_previous and outflow variables
-    ps.fs.h2_tank.tank_holdup_previous.unfix()
-    ps.fs.h2_tank.outlet_to_turbine.flow_mol.unfix()
-    ps.fs.h2_tank.outlet_to_pipeline.flow_mol.unfix()
-
-    # Unfix the flowrate of air to the mixer
-    ps.fs.mixer.air_feed.flow_mol.unfix()
-
-    # Add a constraint to maintain the air to hydrogen flow ratio
-    ps.fs.mixer.air_h2_ratio = pyo.Constraint(
-                expr=ps.fs.mixer.air_feed.flow_mol[int(0)] ==
-                      air_h2_ratio * ps.fs.mixer.hydrogen_feed.flow_mol[int(0)])
-
-    # Set bounds on variables. A small non-zero value is set as the lower
-    # bound on molar flowrates to avoid convergence issues
-    ps.fs.pem.outlet.flow_mol[0].setlb(0.001)
-
-    ps.fs.h2_tank.inlet.flow_mol[0].setlb(0.001)
-    ps.fs.h2_tank.outlet_to_turbine.flow_mol[0].setlb(0.001)
-    ps.fs.h2_tank.outlet_to_pipeline.flow_mol[0].setlb(0.001)
-
-    ps.fs.translator.inlet.flow_mol[0].setlb(0.001)
-    ps.fs.translator.outlet.flow_mol[0].setlb(0.001)
-
-    ps.fs.mixer.hydrogen_feed.flow_mol[0].setlb(0.001)
-
-  def build_connecting_constraints(self, scenario, set_time, set_days, set_years):
-    """
-      This function declares the first-stage variables or design decisions,
-      adds constraints that ensure that the operational variables never exceed their
-      design values, and adds constraints connecting variables at t - 1 and t
-      @ In, scenario, Pyomo model for given scenario
-      @ In, set_time, list of hours in day
-      @ In, set_days, list of days/clusters per year
-      @ In, set_years, list of years per scenario
-      @ Out, None
-    """
-    # Declare first-stage variables (Design decisions)
-    scenario.pem_capacity = pyo.Var(within=pyo.NonNegativeReals,
-                                    doc="Maximum capacity of the PEM electrolyzer (in kW)")
-    scenario.tank_capacity = pyo.Var(within=pyo.NonNegativeReals,
-                                     doc="Maximum holdup of the tank (in mol)")
-    scenario.h2_turbine_capacity = pyo.Var(within=pyo.NonNegativeReals,
-                                           doc="Maximum power output from the turbine (in W)")
-
-    # Ensure that the electricity to the PEM elctrolyzer does not exceed the PEM capacity
-    @scenario.Constraint(set_time, set_days, set_years)
-    def pem_capacity_constraint(blk, t, d, y):
-      return blk.period[t, d, y].fs.pem.electricity[int(0)] <= scenario.pem_capacity
-
-    # Ensure that the final tank holdup does not exceed the tank capacity
-    @scenario.Constraint(set_time, set_days, set_years)
-    def tank_capacity_constraint(blk, t, d, y):
-      return blk.period[t, d, y].fs.h2_tank.tank_holdup[int(0)] <= scenario.tank_capacity
-
-    # Ensure that the power generated by the turbine does not exceed the turbine capacity
-    @scenario.Constraint(set_time, set_days, set_years)
-    def turbine_capacity_constraint(blk, t, d, y):
-      return (
-          - blk.period[t, d, y].fs.h2_turbine.turbine.work_mechanical[int(0)]
-          - blk.period[t, d, y].fs.h2_turbine.compressor.work_mechanical[int(0)] <=
-          scenario.h2_turbine_capacity  )
-
-    # Connect the initial tank holdup at time t with the final tank holdup at time t - 1
-    @scenario.Constraint(set_time, set_days, set_years)
-    def tank_holdup_constraints(blk, t, d, y):
-      if t == 1:
-        # Each day begins with an empty tank
-        return (
-          blk.period[t, d, y].fs.h2_tank.tank_holdup_previous[int(0)] == 0  )
-      else:
-        # Initial holdup at time t = final holdup at time t - 1
-        return (
-          blk.period[t, d, y].fs.h2_tank.tank_holdup_previous[int(0)] ==
-          blk.period[t - 1, d, y].fs.h2_tank.tank_holdup[int(0)]   )
-
-  def _add_non_anticipativity_constraints(self):
-    """
-      Adding non-anticipativity constraints, ensuring that all capacity variables are the same
-      for all scenarios.
-      @ In, None
-      @ Out, None
-    """
-    # temporary object pointing to model
-    dmdl = self._dmdl
-
-    # Add non-anticipativity constraints
-    dmdl.pem_capacity = pyo.Var(within=pyo.NonNegativeReals,
-                                doc="Design PEM capacity (in kW)")
-    dmdl.tank_capacity = pyo.Var(within=pyo.NonNegativeReals,
-                                 doc="Design tank capacity (in mol)")
-    dmdl.h2_turbine_capacity = pyo.Var(within=pyo.NonNegativeReals,
-                                       doc="Design turbine capacity (in W)")
-
-    @dmdl.Constraint(dmdl.set_scenarios)
-    def non_anticipativity_pem(blk, s):
-      return blk.pem_capacity == blk.scenario[s].pem_capacity
-
-    @dmdl.Constraint(dmdl.set_scenarios)
-    def non_anticipativity_tank(blk, s):
-      return blk.tank_capacity == blk.scenario[s].tank_capacity
-
-    @dmdl.Constraint(dmdl.set_scenarios)
-    def non_anticipativity_turbine(blk, s):
-      return blk.h2_turbine_capacity == blk.scenario[s].h2_turbine_capacity
-
+  # =======================
+  # SOLVING OPTIMIZATION
+  # =======================
   def _add_objective(self):
     """
       Adding objective function using TEAL metrics.
       @ In, None
       @ Out, None
     """
-    # scenario probability weights
-    weights = self._dmdl.weights_scenarios
+    ## scenario probability weights
+    # weights = self._time_sets['weights_scenarios'] # TODO: skipping for now
 
     # pyomo expression for full metric wtih scenario weights applied
-    Metric = np.sum( weights[n]*scenario['NPV'] for n, scenario in enumerate(self._metrics) )
+    N = getattr(self, "_num_samples")
+    Metric = self._metrics[-1]['NPV'] / N # TODO: temp fix, things are getting duplicated somewhere
 
     # set objective
     self._dmdl.obj = pyo.Objective(expr=Metric, sense=pyo.maximize)
 
   def _solve_dispatches_model(self):
     """
       Solve the DISPATCHES Pyomo model.
@@ -1014,30 +1190,35 @@
     # optimal capacities
     columns.extend(['PEM Size', 'H2 Tank Size', 'H2 Turbine Size'])
     values.extend([opt_PEM, opt_H2Tank, opt_H2Turb])
     # outputting to csv
     output_data = pd.DataFrame([values], columns=columns)
     output_data.to_csv(f'opt_solution__{case_name}.csv')
 
+  # ================
+  # MAIN WORKFLOW
+  # ================
   def run(self):
     """
       Runs the DISPATCHES workflow
       @ In, None
       @ Out, None
     """
+    time_start = time.time()
     # original workflow from MOPED
     self.buildEconSettings()  # overloaded method
     self.buildComponentMeta() # overloaded method
     self.buildCashflowMeta()  # MOPED method
     self.collectResources()   # MOPED method (TODO: needed?)
 
     # new workflow for DISPATCHES
     self._check_dispatches_compatibility()
     self._get_demand_data()
 
     # building the Pyomo model using DISPATCHES
-    self._dmdl = pyo.ConcreteModel(name=self._case.name)
     self._build_dispatches_model()
     self._add_non_anticipativity_constraints()
     self._add_objective()
     self._solve_dispatches_model()
     self._export_results()
+    time_end = time.time()
+    print(f'Total Elapsed Time: {time_end-time_start} s')
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Hybrid2Heron/HYBRID_HERON_keywords.csv` & `heron-ravenframework-0.3/HERON/src/Hybrid2Heron/HYBRID_HERON_keywords.csv`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Hybrid2Heron/hybrid2heron_economic.py` & `heron-ravenframework-0.3/HERON/src/Hybrid2Heron/hybrid2heron_economic.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 #Note: xm only uses prettify which is in both xmlUtils and convert_utils
 try:
   from ravenframework.utils import xmlUtils as xm
   import HERON.src
   HERON_src_path = HERON.src.__path__[0]
 except ModuleNotFoundError:
   # # Importing XML utility from RAVEN to make the output XML file looks pretty
-  HERON_src_path = os.path.dirname(os.path.abspath(__file__)).split("HERON")[0] + "HERON/src"
+  this_file = os.path.abspath(__file__)
+  #Note, drop everything after last occurence of HERON, then add HERON/src
+  HERON_src_path = "HERON".join(this_file.split("HERON")[:-1])+"HERON/src"
   sys.path.append(HERON_src_path)
   from _utils import get_raven_loc
   sys.path.append(get_raven_loc())
   from scripts.conversionScripts import convert_utils as xm
 
 #####
 # Section 1: HYBRID Information Extraction Function
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Moped.py` & `heron-ravenframework-0.3/HERON/src/Moped.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,27 @@
     if self._eval_mode not in ['clustered', 'full']:
       raise IOError('Improper ROM evaluation mode detected, try "clustered" or "full".')
     # How many dispatch points we will have for each year
     self._yearly_hours = hour_count * cluster_count
     self._m.t = pyo.Set(initialize=np.arange(hour_count))
     return synthetic_data
 
+  def loadStaticHistory(self, signal, multiplier):
+    """
+      Loads static history for a specified signal,
+      also sets yearly hours and pyomo indexing sets
+      @ In, signal, string, name of signal to sample
+      @ In, multiplier, int/float, value to multiply synthetic history evaluations by
+      @ Out, synthetic_data, dict, contains data from evaluated ROM
+    """
+    synthetic_data = {}
+    # TODO: this is being implemented in HERD but makes sense to also add in MOPED
+    raise IOError('Static histories not yet implemented in MOPED.')
+    return synthetic_data
+
   def setCapacityMeta(self, mode, resource, comp, element, kind='produces'):
     """
       Checks the capacity type, dispatch type, and resources involved for each component
       to build component_meta
       @ In, mode, string, type of capacity definition for component
       @ In, resource, string, resource produced or demanded
       @ In, comp, HERON component
@@ -247,14 +260,21 @@
     elif mode == 'SyntheticHistory':
       self.raiseADebug(f'Building capacity with synthetic histories for '
                        f'{comp.name}')
       # This method runs external ROM loader and defines some pyomo sets
       capacity = self.loadSyntheticHistory(element._capacity._vp._var_name, capacity_mult)
       # TODO how to better handle capacities based on Synth Histories
       self._component_meta[comp.name]['Capacity'] = capacity
+    elif mode == 'StaticHistory':
+      self.raiseADebug(f'Building capacity with static histories for '
+                       f'{comp.name}')
+      # This method runs external ROM loader and defines some pyomo sets
+      capacity = self.loadStaticHistory(element._capacity._vp._var_name, capacity_mult)
+      # TODO how to better handle capacities based on Synth Histories
+      self._component_meta[comp.name]['Capacity'] = capacity
     if mode != 'SyntheticHistory':
       # TODO smarter way to do this check?
       self._component_meta[comp.name]['Capacity'] = getattr(self._m, f'{comp.name}')
     if kind == 'produces':
       # TODO should we handle transfer functions here?
       for con in element._consumes:
         transfer_values = element.get_transfer().get_coefficients()
@@ -291,14 +311,17 @@
         # Allows MOPED and default HERON to follow same sign conventions for inputs
         if len(comp._demands) > 0:
           multiplier *= -1
         # Using reference prices for cashflows, considering uncertain market prices
         if cf._alpha.type == 'SyntheticHistory':
           signal = cf._alpha._vp._var_name
           alpha = self.loadSyntheticHistory(signal, multiplier)
+        elif cf._alpha.type == 'StaticHistory':
+          signal = cf._alpha._vp._var_name
+          alpha = self.loadStaticHistory(signal, multiplier)
         else:
           alpha = cf._alpha._vp._parametric * multiplier
         if cf._type == 'one-time':
           # TODO consider other driver types
           if driver_type == 'FixedValue':
             self._cf_meta[comp.name]['Capex Driver'] = cf._driver._vp._parametric
           else:
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/Placeholders.py` & `heron-ravenframework-0.3/HERON/src/Placeholders.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/SerializationManager.py` & `heron-ravenframework-0.3/HERON/src/SerializationManager.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParamHandler.py` & `heron-ravenframework-0.3/HERON/src/ValuedParamHandler.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Activity.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/Activity.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Factory.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/Factory.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Function.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/Function.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Linear.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/Linear.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Parametric.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/Parametric.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/ROM.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/ROM.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/StaticHistory.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/StaticHistory.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/SyntheticHistory.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/SyntheticHistory.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/ValuedParam.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/ValuedParam.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/ValuedParams/Variable.py` & `heron-ravenframework-0.3/HERON/src/ValuedParams/Variable.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/_utils.py` & `heron-ravenframework-0.3/HERON/src/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,14 @@
        use lru_cache for older versions of python
        @ In, user_function, function
        @ Out, user_function, function that caches values
      """
      return lru_cache(maxsize=None)(user_function)
 from os import path
 
-import pandas as pd
-
 
 def get_heron_loc():
   """
     Return HERON location
     @ In, None
     @ Out, loc, string, absolute location of HERON
   """
@@ -38,17 +36,18 @@
     Return RAVEN location
     hopefully this is read from heron/.ravenconfig.xml
     @ In, None
     @ Out, loc, string, absolute location of RAVEN
   """
   try:
     import ravenframework
-    print("WARNING: get_raven_loc deprecated")
-    import traceback
-    traceback.print_stack()
+    # Commented for now -- TODO: address these messages in the future
+    # print("WARNING: get_raven_loc deprecated")
+    # import traceback
+    # traceback.print_stack()
     return path.dirname(ravenframework.__path__[0])
   except ModuleNotFoundError:
     pass
   config = path.abspath(path.join(path.dirname(__file__),'..','.ravenconfig.xml'))
   if not path.isfile(config):
     raise IOError(
         f'HERON config file not found at "{config}"! Has HERON been installed as a plugin in a RAVEN installation?'
@@ -187,14 +186,17 @@
   """
     Returns CSV structure in a way RAVEN & HERON understand
     @ In, fpath, str, file path to CSV file
     @ In, macro_var, str, Macro Variable name - typically 'Year'
     @ In, micro_var, str, Micro Variable name - typically 'Time'
     @ Out, structure, dict, Nested structure of the CSV dataframe.
   """
+  import pandas as pd #Note that this cannot be imported at the start of this
+  # file since _utils.py is used in heron script outside of the raven environment
+  # to find the environment.
   data = pd.read_csv(fpath)
   structure = {}
   if macro_var in data.columns:
     macro_steps = pd.unique(data[macro_var].values)
     structure['macro'] = {
       'id': macro_var,
       'num': len(macro_steps) + 1,
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/base.py` & `heron-ravenframework-0.3/HERON/src/base.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/CustomDispatcher.py` & `heron-ravenframework-0.3/HERON/src/dispatch/CustomDispatcher.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/DispatchState.py` & `heron-ravenframework-0.3/HERON/src/dispatch/DispatchState.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/Dispatcher.py` & `heron-ravenframework-0.3/HERON/src/dispatch/Dispatcher.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/pyomo_dispatch.py` & `heron-ravenframework-0.3/HERON/src/dispatch/pyomo_dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
       else:
         print('DEBUGG ... solve was unsuccessful!')
         print('DEBUGG ... status:', soln.solver.status)
         print('DEBUGG ... termination:', soln.solver.termination_condition)
         self._debug_pyomo_print(m)
         print('Resource Map:')
         pprint.pprint(m.resource_index_map)
-        raise RuntimeError
+        raise RuntimeError(f"Solve was unsuccessful! Status: {soln.solver.status} Termination: {soln.solver.termination_condition}")
       # try validating
       print('DEBUGG ... validating ...')
       validation_errs = self.validate(m.Components, m.Activity, m.Times, meta)
       if validation_errs:
         done_and_checked = False
         print('DEBUGG ... validation concerns raised:')
         for e in validation_errs:
@@ -484,14 +484,17 @@
     indexer = getattr(m, indexer_name, None)
     if indexer is None:
       indexer = pyo.Set(initialize=range(len(m.resource_index_map[comp])))
       setattr(m, indexer_name, indexer)
     prod_name = f'{name}_{tag}'
     caps, mins = self._find_production_limits(m, comp, meta)
     if min(caps) < 0:
+      # quick check that capacities signs are consistent #FIXME: revisit, this is an assumption
+      assert max(caps) < 0, \
+        'Capacities are inconsistent: mix of positive and negative values not currently  supported.'
       # we have a unit that's consuming, so we need to flip the variables to be sensible
       mins, caps = caps, mins
       inits = caps
     else:
       inits = mins
     if add_bounds:
       # create bounds based in min, max operation
```

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/twin_pyomo_test.py` & `heron-ravenframework-0.3/HERON/src/dispatch/twin_pyomo_test.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/twin_pyomo_test_ch_disch.py` & `heron-ravenframework-0.3/HERON/src/dispatch/twin_pyomo_test_ch_disch.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/dispatch/twin_pyomo_test_rte.py` & `heron-ravenframework-0.3/HERON/src/dispatch/twin_pyomo_test_rte.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/input_loader.py` & `heron-ravenframework-0.3/HERON/src/input_loader.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/validators/ExampleValidator.py` & `heron-ravenframework-0.3/HERON/src/validators/ExampleValidator.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/validators/Factory.py` & `heron-ravenframework-0.3/HERON/src/validators/Factory.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/src/validators/Validator.py` & `heron-ravenframework-0.3/HERON/src/validators/Validator.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/HERON/templates/inner.xml` & `heron-ravenframework-0.3/HERON/templates/inner.xml`

 * *Files 5% similar despite different names*

#### Comparing `heron-ravenframework-0.2rc1/HERON/templates/inner.xml` & `heron-ravenframework-0.3/HERON/templates/inner.xml`

```diff
@@ -41,14 +41,15 @@
     <Group name="GRO_armasamples">GRO_armasamples_in, GRO_armasamples_out</Group>
     <Group name="GRO_armasamples_in">GRO_armasamples_in_scalar</Group>
     <Group name="GRO_armasamples_out">GRO_armasamples_out_scalar</Group>
     <Group name="GRO_armasamples_in_scalar">scaling, GRO_capacities</Group>
     <Group name="GRO_armasamples_out_scalar">NPV</Group>
     <Group name="GRO_final_return"/>
     <Group name="GRO_full_dispatch"/>
+    <Group name="GRO_cashflows"/>
     <Group name="GRO_full_dispatch_indices"/>
     <Group name="GRO_interp">stepwise</Group>
     <Group name="GRO_capacities"/>
     <Group name="GRO_init_disp"/>
   </VariableGroups>
   <DataObjects>
     <DataSet name="arma_samples">
@@ -58,18 +59,19 @@
     <PointSet name="arma_metrics">
       <Output>NPV</Output>
     </PointSet>
     <PointSet name="metrics_stats">
       <Output>GRO_final_return</Output>
     </PointSet>
     <DataSet name="disp_full">
-      <Output>GRO_full_dispatch, GRO_dispatch</Output>
+      <Output>GRO_full_dispatch, GRO_dispatch, GRO_cashflows</Output>
       <Index var="Time">GRO_full_dispatch, GRO_dispatch_in_Time</Index>
       <Index var="Year">GRO_full_dispatch, GRO_dispatch_in_Time</Index>
       <Index var="_ROM_Cluster">GRO_full_dispatch, GRO_dispatch_in_Time</Index>
+      <Index var="cfYears">GRO_cashflows</Index>
     </DataSet>
     <DataSet name="dispatch_eval">
       <Input>GRO_dispatch_in</Input>
       <Index var="Time">GRO_dispatch_in_Time</Index>
       <Index var="Year">GRO_dispatch_in_Time</Index>
     </DataSet>
     <PointSet name="dispatch_placeholder">
```

### Comparing `heron-ravenframework-0.2rc1/HERON/templates/outer.xml` & `heron-ravenframework-0.3/HERON/templates/outer.xml`

 * *Files 2% similar despite different names*

#### Comparing `heron-ravenframework-0.2rc1/HERON/templates/outer.xml` & `heron-ravenframework-0.3/HERON/templates/outer.xml`

```diff
@@ -23,21 +23,23 @@
       <Output class="DataObjects" type="PointSet">opt_eval</Output>
       <SolutionExport class="DataObjects" type="PointSet">opt_soln</SolutionExport>
       <Output class="OutStreams" type="Print">opt_soln</Output>
     </MultiRun>
     <IOStep name="plot">
       <Input class="DataObjects" type="PointSet">opt_soln</Input>
       <Output class="OutStreams" type="Plot">opt_path</Output>
+      <Output class="OutStreams" type="Print">opt_soln</Output>
     </IOStep>
   </Steps>
   <VariableGroups>
     <Group name="GRO_capacities"/>
     <Group name="GRO_outer_results"/>
     <Group name="GRO_outer_debug_dispatch"/>
     <Group name="GRO_outer_debug_synthetics"/>
+    <Group name="GRO_outer_debug_cashflows"/>
   </VariableGroups>
   <DataObjects>
     <PointSet name="grid">
       <Input>GRO_capacities</Input>
       <Output>GRO_outer_results</Output>
     </PointSet>
     <PointSet name="opt_eval">
```

### Comparing `heron-ravenframework-0.2rc1/HERON/templates/template_driver.py` & `heron-ravenframework-0.3/HERON/templates/template_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,44 +138,43 @@
     # load a copy of the template
     inner = copy.deepcopy(self._template_inner)
     outer = copy.deepcopy(self._template_outer)
     cash = copy.deepcopy(self._template_cash)
     # modify the templates
     inner = self._modify_inner(inner, case, components, sources)
     outer = self._modify_outer(outer, case, components, sources)
-    cash = self._modify_cash(cash, case, components, sources)
-    return inner, outer, cash
+    return inner, outer
 
   def writeWorkflow(self, templates, destination, run=False):
     """
       Write outer and inner RAVEN workflows.
       @ In, templates, list, modified XML roots
       @ In, destination, str, path to write workflows to
       @ In, run, bool, if True then attempt to run the workflows
       @ Out, None
     """
     # TODO use destination?
     # write templates
-    inner, outer, cash = templates
+    inner, outer = templates
     outer_file = os.path.abspath(os.path.join(destination, 'outer.xml'))
     inner_file = os.path.abspath(os.path.join(destination, 'inner.xml'))
-    cash_file = os.path.abspath(os.path.join(destination, 'cash.xml'))
+
     self.raiseAMessage('========================')
     self.raiseAMessage('HERON: writing files ...')
     self.raiseAMessage('========================')
+
     msg_format = 'Wrote "{1}" to "{0}/"'
     with open(outer_file, 'w') as f:
       f.write(xmlUtils.prettify(outer))
     self.raiseAMessage(msg_format.format(*os.path.split(outer_file)))
+
     with open(inner_file, 'w') as f:
       f.write(xmlUtils.prettify(inner))
     self.raiseAMessage(msg_format.format(*os.path.split(inner_file)))
-    with open(cash_file, 'w') as f:
-      f.write(xmlUtils.prettify(cash))
-    self.raiseAMessage(msg_format.format(*os.path.split(cash_file)))
+
     # write library of info so it can be read in dispatch during inner run
     data = (self.__case, self.__components, self.__sources)
     lib_file = os.path.abspath(os.path.join(destination, self.namingTemplates['lib file']))
     with open(lib_file, 'wb') as lib:
       pk.dump(data, lib)
     self.raiseAMessage(msg_format.format(*os.path.split(lib_file)))
     # copy "write_inner.py", which has the denoising and capacity fixing algorithms
@@ -279,15 +278,15 @@
     # capacities
     caps = var_groups[0]
     var_list = []
 
     # Add component opt vars
     for comp in components:
       comp_cap_type = comp.get_capacity(None, raw=True).type
-      if comp_cap_type  not in ['Function', 'ARMA', 'SyntheticHistory']:
+      if comp_cap_type  not in ['Function', 'ARMA', 'SyntheticHistory', 'StaticHistory']:
         var_list.append(f'{comp.name}_capacity')
 
     # Add dispatch opt vars
     for var in case.dispatch_vars.keys():
       var_list.append(f'{var}_dispatch')
     caps.text = ', '.join(var_list)
 
@@ -313,29 +312,31 @@
           self._updateCommaSeperatedList(group_outer_results, sweep_name)
     # opt mode adds optimization variable if not already there
     if (case.get_mode() == 'opt') and (case._optimization_settings is not None):
       new_metric_outer_results = self._build_opt_metric_out_name(case)
       if (new_metric_outer_results != 'missing') and (new_metric_outer_results not in group_outer_results.text):
         # additional results statistics have been requested, add this metric if not already present
         self._updateCommaSeperatedList(group_outer_results, new_metric_outer_results, position=0)
-
     # labels group
     if case.get_labels():
       case_labels = ET.SubElement(var_groups, 'Group', attrib={'name': 'GRO_case_labels'})
       case_labels.text = ', '.join([f'{key}_label' for key in case.get_labels().keys()])
     if case.debug['enabled']:
       # expected dispatch, ARMA outputs
       # -> dispatch results
       group = var_groups.find(".//Group[@name='GRO_outer_debug_dispatch']")
       for component in components:
         name = component.name
         for tracker in component.get_tracking_vars():
           for resource in component.get_resources():
             var_name = self.namingTemplates['dispatch'].format(component=name, tracker=tracker, resource=resource)
             self._updateCommaSeperatedList(group, var_name)
+      group = var_groups.find(".//Group[@name='GRO_outer_debug_cashflows']")
+      cfs = self._find_cashflows(components)
+      group.text = ', '.join(cfs)
       # -> synthetic histories?
       group = var_groups.find(".//Group[@name='GRO_outer_debug_synthetics']")
       for source in sources:
         if source.is_type('ARMA'):
           synths = source.get_variable()
           for synth in synths:
             if not group.text or synth not in group.text.split(','):
@@ -383,14 +384,18 @@
       deps = {self.__case.get_time_name(): debug_gro,
               self.namingTemplates['cluster_index']: debug_gro,
               self.__case.get_year_name(): debug_gro}
       self._create_dataobject(DOs, 'DataSet', 'dispatch',
                               inputs=['scaling'],
                               outputs=debug_gro,
                               depends=deps)
+      # and similar for debug cashflows
+      debug_gro = ['GRO_outer_debug_cashflows']
+      deps = {'cfYears': debug_gro}
+      self._create_dataobject(DOs, 'HistorySet', 'cashflows', outputs=debug_gro, depends=deps)
 
   def _modify_outer_files(self, template, case, sources):
     """
       Defines modifications to the Files of outer.xml RAVEN input file.
       @ In, template, xml.etree.ElementTree.Element, root of XML to modify
       @ In, case, HERON Case, defining Case instance
       @ In, sources, list, list of HERON Placeholder instances for this run
@@ -486,15 +491,14 @@
     # data handling: inner to outer data format
     if case.data_handling['inner_to_outer'] == 'csv':
       # swap the outputDatabase to outputExportOutStreams
       output_node = template.find('Models').find('Code').find('outputDatabase')
       output_node.tag = 'outputExportOutStreams'
       # no need to change name, as database and outstream have the same name
 
-
   def _modify_outer_outstreams(self, template, case, components, sources):
     """
       Defines modifications to the OutStreams of outer.xml RAVEN input file.
       @ In, template, xml.etree.ElementTree.Element, root of XML to modify
       @ In, case, HERON Case, defining Case instance
       @ In, components, list, list of HERON Component instances for this run
       @ In, sources, list, list of HERON Placeholder instances for this run
@@ -513,30 +517,43 @@
         opt_path_plot_vars.text = opt_path_plot_vars.text.replace(f'mean_{case._metric}', new_opt_objective)
     # debug mode
     if case.debug['enabled']:
       # modify normal metric output
       out = OSs.findall('Print')[0]
       out.attrib['name'] = 'dispatch_print'
       out.find('source').text = 'dispatch'
+      # cashflow output
+      cf_print = ET.SubElement(OSs, 'Print', attrib={'name': 'cashflows'})
+      src = ET.SubElement(cf_print, 'type')
+      src.text = 'csv'
+      src = ET.SubElement(cf_print, 'source')
+      src.text = 'cashflows'
+
       # handle dispatch plots for debug mode
       if case.debug['dispatch_plot']:
+        # dispatch plot
         out_plot = ET.SubElement(OSs, 'Plot', attrib={'name': 'dispatchPlot', 'subType': 'HERON.DispatchPlot'})
         out_plot_source = ET.SubElement(out_plot, 'source')
         out_plot_source.text = 'dispatch'
         out_plot_macro = ET.SubElement(out_plot, 'macro_variable')
         out_plot_macro.text = case.get_year_name()
         out_plot_micro = ET.SubElement(out_plot, 'micro_variable')
         out_plot_micro.text = case.get_time_name()
         out_plot_signals = ET.SubElement(out_plot, 'signals')
         signals = set()
         for source in sources:
           new = source.get_variable()
           if new is not None:
             signals.update(set(new))
         out_plot_signals.text = ', '.join(signals)
+      if case.debug['cashflow_plot']:
+        # cashflow plot
+        cf_plot = ET.SubElement(OSs, 'Plot', attrib={'name': 'cashflow_plot', 'subType': 'TEAL.CashFlowPlot'})
+        cf_plot_source = ET.SubElement(cf_plot, 'source')
+        cf_plot_source.text = 'cashflows'
 
   def _modify_outer_samplers(self, template, case, components):
     """
       Defines modifications to the Samplers/Optimizers of outer.xml RAVEN input file.
       @ In, template, xml.etree.ElementTree.Element, root of XML to modify
       @ In, case, HERON Case, defining Case instance
       @ In, components, list, list of HERON Component instances for this run
@@ -691,23 +708,30 @@
       for output in sweep.findall('Output'):
         if output.text in ['grid', 'sweep']:
           to_remove.append(output)
       for node in to_remove:
         sweep.remove(node)
       # add debug dispatch collector and printer
       sweep.append(self._assemblerNode('Output', 'DataObjects', 'DataSet', 'dispatch'))
+      sweep.append(self._assemblerNode('Output', 'DataObjects', 'HistorySet', 'cashflows'))
       sweep.append(self._assemblerNode('Output', 'Databases', 'NetCDF', 'dispatch'))
       # add an output step to print/plot summaries
       io_step = ET.SubElement(steps, 'IOStep', attrib={'name': 'debug_output'})
-      io_input = ET.SubElement(io_step, 'Input', attrib={'class': 'DataObjects', 'type': 'DataSet'})
-      io_input.text = 'dispatch'
+      io_input_dispatch = ET.SubElement(io_step, 'Input', attrib={'class': 'DataObjects', 'type': 'DataSet'})
+      io_input_dispatch.text = 'dispatch'
+      io_input_cashflow = ET.SubElement(io_step, 'Input', attrib={'class': 'DataObjects', 'type': 'HistorySet'})
+      io_input_cashflow.text = 'cashflows'
       io_step.append(self._assemblerNode('Output', 'OutStreams', 'Print', 'dispatch_print'))
+      io_step.append(self._assemblerNode('Output', 'OutStreams', 'Print', 'cashflows'))
       if case.debug['dispatch_plot']:
-        io_output = ET.SubElement(io_step, 'Output', attrib={'class': 'OutStreams', 'type': 'Plot'})
-        io_output.text = 'dispatchPlot'
+        io_output_dispatch = ET.SubElement(io_step, 'Output', attrib={'class': 'OutStreams', 'type': 'Plot'})
+        io_output_dispatch.text = 'dispatchPlot'
+      if case.debug['cashflow_plot']:
+        io_output_cashflow = ET.SubElement(io_step, 'Output', attrib={'class': 'OutStreams', 'type': 'Plot'})
+        io_output_cashflow.text = 'cashflow_plot'
 
   def _create_new_sweep_capacity(self, comp_name, var_name, capacities, sampler):
     """
       for OUTER, creates new distribution and variable for grid/opt sampling
       @ In, comp_name, str, name of component
       @ In, var_name, str, name of capacity variable
       @ In, capacities, list, float list of capacities to sweep/opt over
@@ -1002,15 +1026,15 @@
         if isinstance(values, list):
           cap_val = 42 # placeholder
         else:
           cap_val = values
         mc.append(xmlUtils.newNode('constant', attrib={'name': cap_name}, text=cap_val))
         # add component to applicable variable groups
         self._updateCommaSeperatedList(groups['capacities'], cap_name)
-      elif capacity.type in ['SyntheticHistory', 'Function', 'Variable']:
+      elif capacity.type in ['StaticHistory', 'SyntheticHistory', 'Function', 'Variable']:
         # capacity is limited by a signal, so it has to be handled in the dispatch; don't include it here.
         # OR capacity is limited by a function, and we also can't handle it here, but in the dispatch.
         pass
       else:
         raise NotImplementedError(f'Capacity from "{capacity}" not implemented yet. Component: {cap_name}')
 
       for tracker in component.get_tracking_vars():
@@ -1030,20 +1054,24 @@
     # RunInfo
     seq = template.find('.//RunInfo/Sequence')
     seq.text = (','.join(seq.text.split(',')[:-2])) # exclude basic stats parts
     # Steps
     for step in template.find('Steps'):
       if step.get('name') == 'arma_sampling':
         step.append(self._assemblerNode('Output', 'DataObjects', 'DataSet', 'disp_full'))
-      # elif step.get('name') == 'write_summary':
-      #   step.find('Output').text = 'disp_full'
+    # Variable Groups
+    grp = template.find('VariableGroups').find(".//Group[@name='GRO_cashflows']")
+    cfs = self._find_cashflows(components)
+    grp.text = ', '.join(cfs)
     # Model
     extmod_vars = template.find('Models').find('ExternalModel').find('variables')
     self._updateCommaSeperatedList(extmod_vars, 'GRO_full_dispatch')
     self._updateCommaSeperatedList(extmod_vars, 'GRO_full_dispatch_indices')
+    self._updateCommaSeperatedList(extmod_vars, 'GRO_cashflows')
+    self._updateCommaSeperatedList(extmod_vars, 'cfYears')
     # DataObject
     datasets = template.find('DataObjects').findall('DataSet')
     for ds in datasets:
       if ds.attrib['name'] == 'dispatch_eval':
         break
     else:
       raise RuntimeError
@@ -1229,108 +1257,14 @@
       print(
       template.find('Steps').find(".//IOStep[@name='database']")
       )
       db = template.find('Steps').find('.//IOStep[@name="database"]').find('.//Output[@class="Databases"]')
       db.attrib.update({'class': 'OutStreams', 'type': 'Print'})
       # the database and outstream print have the same name, so don't need to change text of node
 
-
-  ##### CASHFLOW #####
-  def _modify_cash(self, template, case, components, sources):
-    """
-      Defines modifications to the cash.xml extension to RAVEN input file.
-      @ In, template, xml.etree.ElementTree.Element, root of XML to modify
-      @ In, case, HERON Case, defining Case instance
-      @ In, components, list, list of HERON Component instances for this run
-      @ In, sources, list, list of HERON Placeholder instances for this run
-      @ Out, template, xml.etree.ElementTree.Element, modified template
-    """
-    self._modify_cash_Global(template, case)
-    self._modify_cash_components(template, case, components)
-    return template
-
-  def _modify_cash_Global(self, template, case):
-    """
-      Defines modifications to Global of cash.xml extension to RAVEN input file.
-      @ In, template, xml.etree.ElementTree.Element, root of XML to modify
-      @ In, case, HERON Case, defining Case instance
-      @ Out, None
-    """
-    # load variables
-    tax = case._global_econ['tax']
-    verbosity = case._global_econ['verbosity']
-    inflation = case._global_econ['inflation']
-    indicator = case._global_econ['Indicator']
-    discountRate = case._global_econ['DiscountRate']
-    projectTime = case._global_econ.get('ProjectTime', None)
-    # set variables
-    template.attrib['verbosity'] = str(verbosity)
-    cash_global = template.find('Global')
-    cash_global.find('DiscountRate').text = str(discountRate)
-    cash_global.find('tax').text = str(tax)
-    cash_global.find('inflation').text = str(inflation)
-    cash_global.find('Indicator').attrib['name'] = indicator['name'][0]
-    cash_global.find('Indicator').text = '\n      '.join(indicator['active'][:])
-    if projectTime is not None:
-      cash_global.append(xmlUtils.newNode('ProjectTime', text=str(projectTime)))
-
-  def _modify_cash_components(self, template, case, components):
-    """
-      Defines modifications to Components of cash.xml extension to RAVEN input file.
-      @ In, template, xml.etree.ElementTree.Element, root of XML to modify
-      @ In, case, HERON Case, defining Case instance
-      @ In, components, list, list of HERON Component instances for this run
-      @ Out, template, xml.etree.ElementTree.Element, modified template
-    """
-    for component in components:
-      subComp = xmlUtils.newNode('Component', attrib={'name': component.name}, text='')
-      subEconomics = component.get_economics()
-      Life_time = subEconomics._lifetime
-      subComp.append(xmlUtils.newNode('Life_time', text=str(Life_time)))
-      cfs=xmlUtils.newNode('CashFlows')
-      for subCash in subEconomics._cash_flows:
-        driverName  = self.namingTemplates['cashfname'].format(component=subCash._component.name, cashname=subCash._driver.name)
-        driverType   = subCash._driver.type
-
-        inflation    = subCash._inflation
-        mult_target  = subCash._mult_target
-        name         = subCash.name
-        tax          = subCash._taxable
-        depreciation = subCash._depreciate
-        if subCash._type == 'one-time':
-          cfNode =  xmlUtils.newNode('Capex', text='', attrib={'name': f'{name}',
-                                                                'tax':tax,
-                                                                'inflation': inflation,
-                                                                'mult_target': mult_target
-                                                                })
-          cfNode.append(xmlUtils.newNode('driver',text = driverName))
-          cfNode.append(xmlUtils.newNode('alpha',text = subCash._alpha.get_value()))
-          cfNode.append(xmlUtils.newNode('reference',text = subCash._reference.get_value()))
-          cfNode.append(xmlUtils.newNode('X',text = subCash._scale.get_value()))
-          if depreciation:
-            cfNode.append(xmlUtils.newNode('depreciation',attrib={'scheme':'MACRS'}, text = depreciation))
-          cfs.append(cfNode)
-        else:
-          cfNode =  xmlUtils.newNode('Recurring', text='', attrib={'name': f'{name}',
-                                                                   'tax':tax,
-                                                                   'inflation': inflation,
-                                                                   'mult_target': mult_target
-                                                                    })
-          cfNode.append(xmlUtils.newNode('driver',
-          text = self.namingTemplates['re_cash'].format(period=subCash._period,
-                                                        driverType = driverType,
-                                                        driverName = f'_{component.name}_{name}')))
-
-          cfNode.append(xmlUtils.newNode('alpha',text = '-1.0'))
-          cfs.append(cfNode)
-      subComp.append(cfs)
-      template.append(subComp)
-
-
-
   ##### OTHER UTILS #####
   def _add_arma_to_ensemble(self, template, source):
     """
       Adds an ARMA to EnsembleModel evaluation
       @ In, template, xml.etree.ElementTree.Element, root of XML to modify
       @ In, source, HERON Placeholder, information about ARMA to be used
       @ Out, None
@@ -1370,15 +1304,16 @@
       if group.attrib['name'] == 'GRO_dispatch_in_Time':
         break
     else:
       raise RuntimeError
     for var in out_vars:
       self._updateCommaSeperatedList(group, var)
 
-  def _create_dataobject(self, dataobjects, typ, name, inputs=None, outputs=None, depends=None):
+  @staticmethod
+  def _create_dataobject(dataobjects, typ, name, inputs=None, outputs=None, depends=None):
     """
       Creates a data object candidate to go to base class
       @ In, dataobjects, xml.etree.ElementTreeElement, DataObjects node
       @ In, typ, str, type of data object
       @ In, name, str, name of data object
       @ In, inputs, list(str), optional, input variable names
       @ In, outputs, list(str), optional, output variable names
@@ -1406,14 +1341,33 @@
     elif typ == 'DataSet':
       if depends is not None:
         for index, dep in depends.items():
           assert isinstance(dep, list)
           new.append(xmlUtils.newNode('Index', attrib={'var':index}, text=', '.join(dep)))
     dataobjects.append(new)
 
+  @staticmethod
+  def _find_cashflows(components):
+    """
+      Loop through comps and collect all the full cashflow names
+      @ In, components, list, list of HERON Component instances for this run
+      @ Out, cfs, list, list of cashflow full names e.g. {comp}_{cf}_CashFlow
+    """
+    cfs = []
+    for comp in components:
+      comp_name = comp.name
+      for cashflow in comp.get_cashflows():
+        cf_name = cashflow.name
+        name = f'{comp_name}_{cf_name}_CashFlow'
+        cfs.append(name)
+        if cashflow._depreciate is not None:
+          cfs.append(f'{comp_name}_{cf_name}_depreciation')
+          cfs.append(f'{comp_name}_{cf_name}_depreciation_tax_credit')
+    return cfs
+
   def _iostep_load_rom(self, template, case, components, source):
     """
       for INNER, creates new IOStep for loading a ROM
       @ In, template, xml.etree.ElementTree.Element, root of XML to modify
       @ In, case, HERON Case, defining Case instance
       @ In, components, list, list of HERON Component instances for this run
       @ In, sources, list, list of HERON Placeholder instances for this run
@@ -1483,29 +1437,31 @@
     new_step = xmlUtils.newNode('IOStep', attrib={'name': step_name})
     new_step.append(self._assemblerNode('Input', 'Models', 'ROM', rom_name))
     new_step.append(self._assemblerNode('Output', 'DataObjects', 'PointSet', obj_name))
     new_step.append(self._assemblerNode('Output', 'OutStreams', 'Print', os_name))
     template.find('Steps').append(new_step)
     self._updateCommaSeperatedList(template.find('RunInfo').find('Sequence'), step_name, position=1)
 
-  def _remove_by_name(self, root, removable):
+  @staticmethod
+  def _remove_by_name(root, removable):
     """
       Removes subs of "root" whose "name" attribute is in "removable"
       @ In, root. ET.Element, node whose subs should be searched through
       @ In, removable, list(str), names to remove
       @ Out, None
     """
     to_remove = []
     for node in root:
       if node.get('name', None) in removable:
         to_remove.append(node)
     for node in to_remove:
       root.remove(node)
 
-  def _build_opt_metric_out_name(self, case):
+  @staticmethod
+  def _build_opt_metric_out_name(case):
     """
       Constructs the output name of the metric specified as the optimization objective
       @ In, case, HERON Case, defining Case instance
       @ Out, opt_out_metric_name, str, output metric name for use in inner/outer files
     """
     try:
       # metric name in RAVEN
@@ -1521,15 +1477,16 @@
     except (TypeError, KeyError):
       # <optimization_settings> node not in input file OR
       # 'metric' is missing from _optimization_settings
       opt_out_metric_name = 'missing'
 
     return opt_out_metric_name
 
-  def _build_result_statistic_names(self, case):
+  @staticmethod
+  def _build_result_statistic_names(case):
     """
       Constructs the names of the statistics requested for output
       @ In, case, HERON Case, defining Case instance
       @ Out, names, list, list of names of statistics requested for output
     """
     names = []
     for name in case._result_statistics:
```

### Comparing `heron-ravenframework-0.2rc1/HERON/templates/write_inner.py` & `heron-ravenframework-0.3/HERON/templates/write_inner.py`

 * *Files identical despite different names*

### Comparing `heron-ravenframework-0.2rc1/PKG-INFO` & `heron-ravenframework-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: heron-ravenframework
-Version: 0.2rc1
+Version: 0.3
 Summary: HERON plugin for RAVEN framework
 Home-page: https://github.com/idaholab/HERON
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 
 ![HERON Logo](./logos/HERON_logo_full.png)
 HERON (Holistic Energy Resource Optimization Network) is a project to construct
 workflows solving complex resource allocation problems to meet target economic
 goals.
 
 It leverages probabalistic analysis tool [raven](https://github.com/idaholab/raven)
 to run constructed workflows. HERON is a plugin for RAVEN.
 
 Instructions for
 installing RAVEN plugins (including HERON) can be found [on RAVEN's website](https://github.com/idaholab/raven/wiki/Plugins).
 
-See more on the [HERON wiki](https://github.com/idaholab/HERON/wiki)
+See more on the [HERON wiki](https://github.com/idaholab/HERON/wiki) for installation, examples, and documentation.
 
 ## Publications
 The following are a selection of technical reports, conference proceedings, and journal articles that may be of interest to users and developers of HERON, loosely in order of work performed.
 
 ### Technoeconomic Assessments
 - [A Technical and Economic Assessment of LWR Flexible Operation for Generation and Demand Balancing to Optimize Plant Revenue](https://www.osti.gov/biblio/1844211-technical-economic-assessment-lwr-flexible-operation-generation-demand-balancing-optimize-plant-revenue)
 - [Evaluation of Hybrid FPOG Applications in Regulated and Deregulated Markets Using HERON](https://www.osti.gov/biblio/1755894-evaluation-hybrid-fpog-applications-regulated-deregulated-markets-using-heron)
-- [HERON as a Tool for LWR Market Interaction in a Deregulated Market](https://www.osti.gov/biblio/1581179-heron-tool-lwr-market-interaction-deregulated-market) 
-- [Evaluation of Hydrogen Production Feasibility for a Light Water Reactor in the Midwest](https://www.osti.gov/biblio/1569271-evaluation-hydrogen-production-feasibility-light-water-reactor-midwest) 
-- [Economic Assessment of Nuclear Hybrid Energy Systems: Nuclear-Renewable-Water Integration in Arizona](https://www.osti.gov/biblio/1634115-economic-assessment-nuclear-hybrid-energy-systems-nuclear-renewable-water-integration-arizona) 
-- [Economic analysis of a nuclear hybrid energy system in a stochastic environment including wind turbines in an electricity grid](https://www.osti.gov/biblio/1593858-economic-analysis-nuclear-hybrid-energy-system-stochastic-environment-including-wind-turbines-electricity-grid) 
+- [HERON as a Tool for LWR Market Interaction in a Deregulated Market](https://www.osti.gov/biblio/1581179-heron-tool-lwr-market-interaction-deregulated-market)
+- [Evaluation of Hydrogen Production Feasibility for a Light Water Reactor in the Midwest](https://www.osti.gov/biblio/1569271-evaluation-hydrogen-production-feasibility-light-water-reactor-midwest)
+- [Economic Assessment of Nuclear Hybrid Energy Systems: Nuclear-Renewable-Water Integration in Arizona](https://www.osti.gov/biblio/1634115-economic-assessment-nuclear-hybrid-energy-systems-nuclear-renewable-water-integration-arizona)
+- [Economic analysis of a nuclear hybrid energy system in a stochastic environment including wind turbines in an electricity grid](https://www.osti.gov/biblio/1593858-economic-analysis-nuclear-hybrid-energy-system-stochastic-environment-including-wind-turbines-electricity-grid)
 
 ### Synthetic History Generation
-- [Correlated synthetic time series generation for energy system simulations using Fourier and ARMA signal processing](https://www.osti.gov/biblio/1603186-correlated-synthetic-time-series-generation-energy-system-simulations-using-fourier-arma-signal-processing) 
-- [Synthetic wind speed scenarios generation for probabilistic analysis of hybrid energy systems](https://www.osti.gov/biblio/1361550-synthetic-wind-speed-scenarios-generation-probabilistic-analysis-hybrid-energy-systems) 
+- [Correlated synthetic time series generation for energy system simulations using Fourier and ARMA signal processing](https://www.osti.gov/biblio/1603186-correlated-synthetic-time-series-generation-energy-system-simulations-using-fourier-arma-signal-processing)
+- [Synthetic wind speed scenarios generation for probabilistic analysis of hybrid energy systems](https://www.osti.gov/biblio/1361550-synthetic-wind-speed-scenarios-generation-probabilistic-analysis-hybrid-energy-systems)
 
 ### See More
 - [Integrated Energy Systems](https://ies.inl.gov/SitePages/Home.aspx)
```

### Comparing `heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/PKG-INFO` & `heron-ravenframework-0.3/heron_ravenframework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: heron-ravenframework
-Version: 0.2rc1
+Version: 0.3
 Summary: HERON plugin for RAVEN framework
 Home-page: https://github.com/idaholab/HERON
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 
 ![HERON Logo](./logos/HERON_logo_full.png)
 HERON (Holistic Energy Resource Optimization Network) is a project to construct
 workflows solving complex resource allocation problems to meet target economic
 goals.
 
 It leverages probabalistic analysis tool [raven](https://github.com/idaholab/raven)
 to run constructed workflows. HERON is a plugin for RAVEN.
 
 Instructions for
 installing RAVEN plugins (including HERON) can be found [on RAVEN's website](https://github.com/idaholab/raven/wiki/Plugins).
 
-See more on the [HERON wiki](https://github.com/idaholab/HERON/wiki)
+See more on the [HERON wiki](https://github.com/idaholab/HERON/wiki) for installation, examples, and documentation.
 
 ## Publications
 The following are a selection of technical reports, conference proceedings, and journal articles that may be of interest to users and developers of HERON, loosely in order of work performed.
 
 ### Technoeconomic Assessments
 - [A Technical and Economic Assessment of LWR Flexible Operation for Generation and Demand Balancing to Optimize Plant Revenue](https://www.osti.gov/biblio/1844211-technical-economic-assessment-lwr-flexible-operation-generation-demand-balancing-optimize-plant-revenue)
 - [Evaluation of Hybrid FPOG Applications in Regulated and Deregulated Markets Using HERON](https://www.osti.gov/biblio/1755894-evaluation-hybrid-fpog-applications-regulated-deregulated-markets-using-heron)
-- [HERON as a Tool for LWR Market Interaction in a Deregulated Market](https://www.osti.gov/biblio/1581179-heron-tool-lwr-market-interaction-deregulated-market) 
-- [Evaluation of Hydrogen Production Feasibility for a Light Water Reactor in the Midwest](https://www.osti.gov/biblio/1569271-evaluation-hydrogen-production-feasibility-light-water-reactor-midwest) 
-- [Economic Assessment of Nuclear Hybrid Energy Systems: Nuclear-Renewable-Water Integration in Arizona](https://www.osti.gov/biblio/1634115-economic-assessment-nuclear-hybrid-energy-systems-nuclear-renewable-water-integration-arizona) 
-- [Economic analysis of a nuclear hybrid energy system in a stochastic environment including wind turbines in an electricity grid](https://www.osti.gov/biblio/1593858-economic-analysis-nuclear-hybrid-energy-system-stochastic-environment-including-wind-turbines-electricity-grid) 
+- [HERON as a Tool for LWR Market Interaction in a Deregulated Market](https://www.osti.gov/biblio/1581179-heron-tool-lwr-market-interaction-deregulated-market)
+- [Evaluation of Hydrogen Production Feasibility for a Light Water Reactor in the Midwest](https://www.osti.gov/biblio/1569271-evaluation-hydrogen-production-feasibility-light-water-reactor-midwest)
+- [Economic Assessment of Nuclear Hybrid Energy Systems: Nuclear-Renewable-Water Integration in Arizona](https://www.osti.gov/biblio/1634115-economic-assessment-nuclear-hybrid-energy-systems-nuclear-renewable-water-integration-arizona)
+- [Economic analysis of a nuclear hybrid energy system in a stochastic environment including wind turbines in an electricity grid](https://www.osti.gov/biblio/1593858-economic-analysis-nuclear-hybrid-energy-system-stochastic-environment-including-wind-turbines-electricity-grid)
 
 ### Synthetic History Generation
-- [Correlated synthetic time series generation for energy system simulations using Fourier and ARMA signal processing](https://www.osti.gov/biblio/1603186-correlated-synthetic-time-series-generation-energy-system-simulations-using-fourier-arma-signal-processing) 
-- [Synthetic wind speed scenarios generation for probabilistic analysis of hybrid energy systems](https://www.osti.gov/biblio/1361550-synthetic-wind-speed-scenarios-generation-probabilistic-analysis-hybrid-energy-systems) 
+- [Correlated synthetic time series generation for energy system simulations using Fourier and ARMA signal processing](https://www.osti.gov/biblio/1603186-correlated-synthetic-time-series-generation-energy-system-simulations-using-fourier-arma-signal-processing)
+- [Synthetic wind speed scenarios generation for probabilistic analysis of hybrid energy systems](https://www.osti.gov/biblio/1361550-synthetic-wind-speed-scenarios-generation-probabilistic-analysis-hybrid-energy-systems)
 
 ### See More
 - [Integrated Energy Systems](https://ies.inl.gov/SitePages/Home.aspx)
```

### Comparing `heron-ravenframework-0.2rc1/heron_ravenframework.egg-info/SOURCES.txt` & `heron-ravenframework-0.3/heron_ravenframework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 HERON/src/Components.py
 HERON/src/DispatchBypass.py
 HERON/src/DispatchManager.py
 HERON/src/DispatchPlot.py
 HERON/src/Economics.py
 HERON/src/Herd.py
 HERON/src/Moped.py
+HERON/src/NetworkPlot.py
 HERON/src/Placeholders.py
 HERON/src/SerializationManager.py
 HERON/src/ValuedParamHandler.py
 HERON/src/__init__.py
 HERON/src/_utils.py
 HERON/src/base.py
+HERON/src/input_definition.py
 HERON/src/input_loader.py
 HERON/src/main.py
 HERON/src/Hybrid2Heron/HYBRID_HERON_keywords.csv
 HERON/src/Hybrid2Heron/hybrid2heron_economic.py
 HERON/src/ValuedParams/Activity.py
 HERON/src/ValuedParams/Factory.py
 HERON/src/ValuedParams/Function.py
```

