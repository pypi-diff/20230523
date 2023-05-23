# Comparing `tmp/qiboconnection-0.8.0.tar.gz` & `tmp/qiboconnection-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiboconnection-0.8.0.tar", last modified: Tue Apr 25 14:48:45 2023, max compression
+gzip compressed data, was "qiboconnection-0.9.0.tar", last modified: Thu May  4 08:09:29 2023, max compression
```

## Comparing `qiboconnection-0.8.0.tar` & `qiboconnection-0.9.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.106653 qiboconnection-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.118653 qiboconnection-0.8.0/src/qiboconnection/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35447 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15465 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.122653 qiboconnection-0.8.0/src/qiboconnection/constants/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/constants/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.126653 qiboconnection-0.8.0/src/qiboconnection/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/device_characteristics_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/device_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/offline_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/online_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_calibration_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device_characteristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/devices/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/live_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/live_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/runcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/saved_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/saved_experiment_listing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.130653 qiboconnection-0.8.0/src/qiboconnection/typings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/live_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/runcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/typings/saved_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/src/qiboconnection/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.118653 qiboconnection-0.8.0/src/qiboconnection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:48:44.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 14:48:45.000000 qiboconnection-0.8.0/src/qiboconnection.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:48:45.134653 qiboconnection-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28880 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_live_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_live_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_runcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_runcard_typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_saved_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_saved_experiment_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_saved_experiment_typings.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-25 14:48:02.000000 qiboconnection-0.8.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.817157 qiboconnection-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 08:09:29.817157 qiboconnection-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 08:09:29.817157 qiboconnection-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.801157 qiboconnection-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.805157 qiboconnection-0.9.0/src/qiboconnection/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36610 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.809157 qiboconnection-0.9.0/src/qiboconnection/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/constants/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.813157 qiboconnection-0.9.0/src/qiboconnection/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/device_characteristics_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/device_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/offline_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/online_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/quantum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/quantum_device_calibration_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/quantum_device_characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/simulator_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/simulator_device_characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/devices/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/live_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/live_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/runcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/saved_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/saved_experiment_listing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.813157 qiboconnection-0.9.0/src/qiboconnection/typings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/live_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/runcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/typings/saved_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/src/qiboconnection/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.809157 qiboconnection-0.9.0/src/qiboconnection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 08:09:29.000000 qiboconnection-0.9.0/src/qiboconnection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-04 08:09:29.000000 qiboconnection-0.9.0/src/qiboconnection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:09:29.000000 qiboconnection-0.9.0/src/qiboconnection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:09:29.000000 qiboconnection-0.9.0/src/qiboconnection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 08:09:29.000000 qiboconnection-0.9.0/src/qiboconnection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 08:09:29.000000 qiboconnection-0.9.0/src/qiboconnection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:09:29.817157 qiboconnection-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28880 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14769 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_live_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_live_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_runcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_runcard_typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_saved_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_saved_experiment_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_saved_experiment_typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-04 08:08:31.000000 qiboconnection-0.9.0/tests/test_util.py
```

### Comparing `qiboconnection-0.8.0/LICENSE` & `qiboconnection-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/PKG-INFO` & `qiboconnection-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiboconnection
-Version: 0.8.0
+Version: 0.9.0
 Summary: manage the remote connection to send qibo experiment to the quantum devices and simulators
 Home-page: https://github.com/qilimanjaro-tech/qiboconnection
 Author: Qibo team
 Author-email: info@qilimanjaro.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10.0
```

### Comparing `qiboconnection-0.8.0/pyproject.toml` & `qiboconnection-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
-version = "0.8.0"
+version = "0.9.0"
 version_files = [
     "src/qiboconnection/__init__.py",
     "pyproject.toml:version"
 ]
 tag_format = "v$version"
 update_changelog_on_bump = true
```

### Comparing `qiboconnection-0.8.0/setup.py` & `qiboconnection-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/api.py` & `qiboconnection-0.9.0/src/qiboconnection/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,30 +239,58 @@
         linebreak = "\n"
         text = (
             f"Selected devices:{linebreak} -{linebreak.join([f' -{device.name}' for device in self._selected_devices])}"
         )
         logger.info(text)
 
     @typechecked
+    def set_device_to_online(self, device_id: int) -> None:
+        """Sets a device into online mode, allowing external traffic and blocking manual manipulation.
+
+        Args:
+            device_id (int): Device identifier
+        """
+        self._devices = self._add_or_update_single_device(device_id=device_id)
+        try:
+            self._devices.set_device_to_online(connection=self._connection, device_id=device_id)
+        except HTTPError as ex:
+            logger.error(json.loads(str(ex))[REST_ERROR.DETAIL])
+            raise ex
+
+    @typechecked
+    def set_device_to_maintenance(self, device_id: int) -> None:
+        """Sets a device in maintenance mode, blocking external traffic and allowing for manual manipulation.
+
+        Args:
+            device_id (int): Device identifier
+        """
+        self._devices = self._add_or_update_single_device(device_id=device_id)
+        try:
+            self._devices.set_device_to_maintenance(connection=self._connection, device_id=device_id)
+        except HTTPError as ex:
+            logger.error(json.loads(str(ex))[REST_ERROR.DETAIL])
+            raise ex
+
+    @typechecked
     def block_device_id(self, device_id: int) -> None:
-        """Blocks a device to avoid others to use it
+        """Blocks a device to avoid others to manually use it.
 
         Args:
             device_id (int): Device identifier
         """
         self._devices = self._add_or_update_single_device(device_id=device_id)
         try:
             self._devices.block_device(connection=self._connection, device_id=device_id)
         except HTTPError as ex:
             logger.error(json.loads(str(ex))[REST_ERROR.DETAIL])
             raise ex
 
     @typechecked
     def release_device(self, device_id: int) -> None:
-        """Releases a device to let others use it
+        """Releases a device to let others manually using it.
 
         Args:
             device_id (int): Device identifier
         """
         self._devices = self._add_or_update_single_device(device_id=device_id)
         try:
             self._devices.release_device(connection=self._connection, device_id=device_id)
```

### Comparing `qiboconnection-0.8.0/src/qiboconnection/api_utils.py` & `qiboconnection-0.9.0/src/qiboconnection/api_utils.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/config.py` & `qiboconnection-0.9.0/src/qiboconnection/config.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/connection.py` & `qiboconnection-0.9.0/src/qiboconnection/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,26 @@
             status (str): device status
 
         Returns:
             Tuple[Any, int]: Http Response
         """
         return self.send_put_auth_remote_api_call(path=f"/devices/{device_id}", data={"status": status})
 
+    def update_device_availability(self, device_id: int, availability: str) -> Tuple[Any, int]:
+        """Makes the request for updating a Device availability with a new value.
+
+        Args:
+            device_id (int): device identifier
+            availability (str): device availability
+
+        Returns:
+            Tuple[Any, int]: Http Response
+        """
+        return self.send_put_auth_remote_api_call(path=f"/devices/{device_id}", data={"availability": availability})
+
     def send_message(self, channel_id: int, message: dict) -> Tuple[Any, int]:
         """Sends a message to a channel registered in the system
 
         Args:
             channel_id (int): channel identifier
             message (dict): message to send
```

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/device_details.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/device_details.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/devices.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/devices.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def select_device(
         self,
         device_id: int,
     ) -> Device:
         """Finds the specific device and returns it
 
         Args:
-            id (int): Device identifier
+            device_id (int): Device identifier
 
         Returns:
             Union[QuantumDevice, SimulatorDevice]: Device selected
         """
         return self._find_device(device_id)
 
     def _find_device(self, device_id: int) -> Device:
@@ -141,18 +141,41 @@
 
         Args:
             connection (Connection): Qibo remote connection
             device_id (int): Device identifier
         """
         device_found = self._find_device(device_id)
         block_device(connection=connection, device=device_found)
+        logger.info("Device %s blocked for execution. AVAILABILITY: blocked", device_found.name)
 
     def release_device(self, connection: Connection, device_id: int) -> None:
         """Releases a device to let others use it
 
         Args:
             connection (Connection): Qibo remote connection
             device_id (int): Device identifier
         """
         device_found = self._find_device(device_id)
         device_found.release_device(connection=connection)
-        logger.info("Device %s released.", device_found.name)
+        logger.info("Device %s released. AVAILABILITY: AVAILABLE", device_found.name)
+
+    def set_device_to_online(self, connection: Connection, device_id: int) -> None:
+        """Releases a device to let others use it
+
+        Args:
+            connection (Connection): Qibo remote connection
+            device_id (int): Device identifier
+        """
+        device_found = self._find_device(device_id)
+        device_found.set_to_online(connection=connection)
+        logger.info("Device %s set online. STATUS: ONLINE", device_found.name)
+
+    def set_device_to_maintenance(self, connection: Connection, device_id: int) -> None:
+        """Releases a device to let others use it
+
+        Args:
+            connection (Connection): Qibo remote connection
+            device_id (int): Device identifier
+        """
+        device_found = self._find_device(device_id)
+        device_found.set_to_maintenance(connection=connection)
+        logger.info("Device %s set to maintenance. STATUS: MAINTENANCE", device_found.name)
```

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/offline_device.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/offline_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/online_device.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/online_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/quantum_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_calibration_details.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/quantum_device_calibration_details.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/quantum_device_characteristics.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/quantum_device_characteristics.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/simulator_device.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/simulator_device_characteristics.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/simulator_device_characteristics.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/devices/util.py` & `qiboconnection-0.9.0/src/qiboconnection/devices/util.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/errors.py` & `qiboconnection-0.9.0/src/qiboconnection/errors.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/job.py` & `qiboconnection-0.9.0/src/qiboconnection/job.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/job_result.py` & `qiboconnection-0.9.0/src/qiboconnection/job_result.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/live_plot.py` & `qiboconnection-0.9.0/src/qiboconnection/live_plot.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/live_plots.py` & `qiboconnection-0.9.0/src/qiboconnection/live_plots.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/runcard.py` & `qiboconnection-0.9.0/src/qiboconnection/runcard.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/saved_experiment.py` & `qiboconnection-0.9.0/src/qiboconnection/saved_experiment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/saved_experiment_listing.py` & `qiboconnection-0.9.0/src/qiboconnection/saved_experiment_listing.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/algorithm.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/algorithm.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/auth_config.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/auth_config.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/connection.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/connection.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/device.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 """ Device Typing """
 import enum
 from dataclasses import InitVar, dataclass
 from typing import Literal, Optional
 
 
-class DeviceStatus(enum.Enum):
-    """Device Status
+class DeviceStatus(str, enum.Enum):
+    """Device status"""
 
-    Args:
-        enum (str): Device Status options available:
-            * available
-            * busy
-            * offline
-    """
+    ONLINE = "online"
+    MAINTENANCE = "maintenance"
+    OFFLINE = "offline"
+
+
+class DeviceAvailability(str, enum.Enum):
+    """Device availability"""
 
     AVAILABLE = "available"
-    BUSY = "busy"
-    OFFLINE = "offline"
+    BLOCKED = "blocked"
 
 
-class DeviceType(enum.Enum):
+class DeviceType(str, enum.Enum):
     """Device Type
 
     Args:
         enum (str): Device type options available:
         * quantum
         * simulator
     """
 
     QUANTUM = "quantum"
     SIMULATOR = "simulator"
 
 
-@dataclass
+@dataclass(kw_only=True)
 class QuantumDeviceCharacteristicsInput:
     """Quantum Device Characteristics Input
 
     Attributes:
         type (str): device type, "quantum"
         description (str): device description
 
     """
 
     type: Literal[DeviceType.QUANTUM, "quantum"]
     description: str | None = None
 
 
-@dataclass
+@dataclass(kw_only=True)
 class SimulatorDeviceCharacteristicsInput:
     """Simulator Device Characteristics Input
 
     Attributes:
         type (str): device type, "simulator"
         cpu (str): device cpu
         gpu (str): device gpu
@@ -64,73 +64,73 @@
     cpu: str | None = None
     gpu: str | None = None
     os: str | None = None  # pylint: disable=invalid-name
     kernel: str | None = None
     ram: str | None = None
 
 
-@dataclass
+@dataclass(kw_only=True)
 class DeviceInput:
     """Device Input
 
     Attributes:
         device_id (int): device identifier
         device_name (str): device name
         status (str | DeviceStatus): device status
     """
 
     device_id: int
     device_name: str
     status: str | DeviceStatus
+    availability: str | DeviceAvailability
     channel_id: int | None
+    number_pending_jobs: Optional[int] = 0
 
 
-@dataclass
+@dataclass(kw_only=True)
 class CalibrationDetailsInput:
     """Calibration Details Input
 
     Attributes:
         elapsed_time (int | None): elapsed time
         t1 (int | None): last calibrated t1 time
         frequency (int | None): last calibrated frequency
     """
 
     elapsed_time: int | None = None
     t1: int | None = None  # pylint: disable=invalid-name
     frequency: int | None = None
 
 
-@dataclass
+@dataclass(kw_only=True)
 class OfflineDeviceInput(DeviceInput):
     """Offline Device Input"""
 
 
-@dataclass
+@dataclass(kw_only=True)
 class OnlineDeviceInput(DeviceInput):
     """Online Device Input"""
 
-    number_pending_jobs: Optional[int] = 0
-
 
-@dataclass
+@dataclass(kw_only=True)
 class SimulatorDeviceInput(OnlineDeviceInput):
     """Simulator Device Input"""
 
     characteristics: InitVar[dict | None] = None
 
     def __post_init__(self, characteristics):
         self._characteristics = SimulatorDeviceCharacteristicsInput(**characteristics)
 
     @property
     def s_characteristics(self):
         """Characteristics getter"""
         return self._characteristics
 
 
-@dataclass
+@dataclass(kw_only=True)
 class QuantumDeviceInput(OnlineDeviceInput):
     """Quantum Device Input"""
 
     last_calibration_time: str | None = ""
     characteristics: InitVar[dict | None] = None
     calibration_details: InitVar[dict | None] = None
```

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/job.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/job.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/live_plot.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/live_plot.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/typings/saved_experiment.py` & `qiboconnection-0.9.0/src/qiboconnection/typings/saved_experiment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection/util.py` & `qiboconnection-0.9.0/src/qiboconnection/util.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/src/qiboconnection.egg-info/PKG-INFO` & `qiboconnection-0.9.0/src/qiboconnection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiboconnection
-Version: 0.8.0
+Version: 0.9.0
 Summary: manage the remote connection to send qibo experiment to the quantum devices and simulators
 Home-page: https://github.com/qilimanjaro-tech/qiboconnection
 Author: Qibo team
 Author-email: info@qilimanjaro.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10.0
```

### Comparing `qiboconnection-0.8.0/src/qiboconnection.egg-info/SOURCES.txt` & `qiboconnection-0.9.0/src/qiboconnection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_algorithm.py` & `qiboconnection-0.9.0/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_api.py` & `qiboconnection-0.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_connection.py` & `qiboconnection-0.9.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_device.py` & `qiboconnection-0.9.0/tests/test_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,39 +51,42 @@
     """Tests Device().__str__() method"""
     device = Device(device_input=device_input)
 
     assert (
         device.__str__() == f"<Device: device_id={device._device_id},"
         f" device_name='{device._device_name}',"
         f" status='{device._status.value}',"
+        f" availability='{device._availability.value}',"
         f" channel_id=None"
         f">"
     )
 
 
 @pytest.mark.parametrize("device_input", device_inputs)
 def test_device_dict_representation(device_input: DeviceInput):
     """Tests Device().__dict__ property"""
     device = Device(device_input=device_input)
     expected_dict = {
         "device_id": device._device_id,
         "device_name": device._device_name,
         "status": device._status.value,
+        "availability": device._availability.value,
     }
     assert device.__dict__ == expected_dict
 
 
 @pytest.mark.parametrize("device_input", device_inputs)
 def test_device_json_representation(device_input: DeviceInput):
     """Tests Device().toJSON() method"""
     device = Device(device_input=device_input)
     expected_dict = {
         "device_id": device._device_id,
         "device_name": device._device_name,
         "status": device._status.value,
+        "availability": device._availability.value,
     }
     assert json.loads(device.toJSON()) == expected_dict
 
 
 @pytest.mark.parametrize("simulator_device_input", simulator_device_inputs)
 def test_simulator_device_constructor(simulator_device_input: SimulatorDeviceInput):
     """Tests SimulatorDevice class constructor"""
@@ -96,28 +99,30 @@
 def test_simulator_device_dict_representation(simulator_device_input: SimulatorDeviceInput):
     """Tests SimulatorDevice().__str__() method"""
     device = SimulatorDevice(device_input=simulator_device_input)
     expected_dict = {
         "device_id": device._device_id,
         "device_name": device._device_name,
         "status": device._status.value,
+        "availability": device._availability.value,
     }
     if device._characteristics:
         expected_dict |= {"characteristics": device._characteristics.__dict__}
     assert device.__dict__ == expected_dict
 
 
 @pytest.mark.parametrize("simulator_device_input", simulator_device_inputs)
 def test_simulator_device_json_representation(simulator_device_input: SimulatorDeviceInput):
     """Tests SimulatorDevice().toJSON() method"""
     device = SimulatorDevice(device_input=simulator_device_input)
     expected_dict = {
         "device_id": device._device_id,
         "device_name": device._device_name,
         "status": device._status.value,
+        "availability": device._availability.value,
     }
     if device._characteristics:
         expected_dict |= {"characteristics": device._characteristics.__dict__}
     assert json.loads(device.toJSON()) == expected_dict
 
 
 @pytest.mark.parametrize("simulator_device_characteristics_input", simulator_device_characteristics_inputs)
@@ -158,14 +163,15 @@
 def test_quantum_device_dict_representation(quantum_device_input: QuantumDeviceInput):
     """Tests QuantumDevice().__dict__ property"""
     device = QuantumDevice(device_input=quantum_device_input)
     expected_dict = {
         "device_id": device._device_id,
         "device_name": device._device_name,
         "status": device._status.value,
+        "availability": device._availability.value,
     }
     if device._last_calibration_time is not None:
         expected_dict |= {"last_calibration_time": device._last_calibration_time.__str__()}
     if device._characteristics is not None:
         expected_dict |= {"characteristics": device._characteristics.__dict__}
     if device._calibration_details is not None:
         expected_dict |= {"calibration_details": device._calibration_details.__dict__}
@@ -176,14 +182,15 @@
 def test_quantum_device_json_representation(quantum_device_input: QuantumDeviceInput):
     """Tests QuantumDevice().toJSON() representation"""
     device = QuantumDevice(device_input=quantum_device_input)
     expected_dict = {
         "device_id": device._device_id,
         "device_name": device._device_name,
         "status": device._status.value,
+        "availability": device._availability.value,
     }
     if device._last_calibration_time is not None:
         expected_dict |= {"last_calibration_time": device._last_calibration_time.__str__()}
     if device._characteristics is not None:
         expected_dict |= {"characteristics": device._characteristics.__dict__}
     if device._calibration_details is not None:
         expected_dict |= {"calibration_details": device._calibration_details.__dict__}
```

### Comparing `qiboconnection-0.8.0/tests/test_devices.py` & `qiboconnection-0.9.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_environment.py` & `qiboconnection-0.9.0/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_errors.py` & `qiboconnection-0.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_job.py` & `qiboconnection-0.9.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_job_result.py` & `qiboconnection-0.9.0/tests/test_job_result.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_live_plot.py` & `qiboconnection-0.9.0/tests/test_live_plot.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_live_plots.py` & `qiboconnection-0.9.0/tests/test_live_plots.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_runcard.py` & `qiboconnection-0.9.0/tests/test_runcard.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_runcard_typings.py` & `qiboconnection-0.9.0/tests/test_runcard_typings.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_saved_experiment.py` & `qiboconnection-0.9.0/tests/test_saved_experiment.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_saved_experiment_listing.py` & `qiboconnection-0.9.0/tests/test_saved_experiment_listing.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_saved_experiment_typings.py` & `qiboconnection-0.9.0/tests/test_saved_experiment_typings.py`

 * *Files identical despite different names*

### Comparing `qiboconnection-0.8.0/tests/test_util.py` & `qiboconnection-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

