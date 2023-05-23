# Comparing `tmp/firexapp-4.9.8.tar.gz` & `tmp/firexapp-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexapp-4.9.8.tar", last modified: Mon Nov 29 20:50:16 2021, max compression
+gzip compressed data, was "firexapp-4.9.9.tar", last modified: Mon Nov 29 20:50:19 2021, max compression
```

## Comparing `firexapp-4.9.8.tar` & `firexapp-4.9.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.019177 firexapp-4.9.8/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1592 2021-11-29 20:49:59.000000 firexapp-4.9.8/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2021-11-29 20:49:59.000000 firexapp-4.9.8/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      463 2021-11-29 20:50:16.019177 firexapp-4.9.8/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2021-11-29 20:49:59.000000 firexapp-4.9.8/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-11-29 20:49:59.000000 firexapp-4.9.8/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.020177 firexapp-4.9.8/firexapp/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2021-11-29 20:50:16.020177 firexapp-4.9.8/firexapp/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6113 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/application.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.008177 firexapp-4.9.8/firexapp/broker_manager/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      685 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/broker_manager/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/broker_manager/broker_factory.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13245 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/broker_manager/redis_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12709 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/celery_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6647 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/discovery.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.009177 firexapp-4.9.8/firexapp/engine/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/engine/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/engine/celery.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2044 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/engine/default_celery_config.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5318 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/engine/logging.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.011177 firexapp-4.9.8/firexapp/events/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/events/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3756 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/events/broker_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12149 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/events/event_aggregator.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3475 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/events/model.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/fileregistry.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    14695 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/firex_subprocess.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/info.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10435 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/plugins.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.011177 firexapp-4.9.8/firexapp/reporters/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/reporters/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5034 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/reporters/json_reporter.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.015177 firexapp-4.9.8/firexapp/submit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/arguments.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5301 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/console.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/install_configs.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/report_trigger.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5424 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/reporting.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9212 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/shutdown.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    29791 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/submit.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1490 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/tracking_service.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3250 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/submit/uid.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.017177 firexapp-4.9.8/firexapp/tasks/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/tasks/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/tasks/core_tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/tasks/example.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3180 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/tasks/root_tasks.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.019177 firexapp-4.9.8/firexapp/testing/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/testing/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4323 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/testing/config_base.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13199 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/testing/config_interpreter.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/testing/coverage_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3168 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/testing/pydev_debug_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7228 2021-11-29 20:49:59.000000 firexapp-4.9.8/firexapp/testing/test_infra.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:16.007176 firexapp-4.9.8/firexapp.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      463 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      191 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      187 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-11-29 20:50:15.000000 firexapp-4.9.8/firexapp.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2021-11-29 20:50:16.020177 firexapp-4.9.8/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1690 2021-11-29 20:49:59.000000 firexapp-4.9.8/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-11-29 20:49:59.000000 firexapp-4.9.8/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.169857 firexapp-4.9.9/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1592 2021-11-29 20:50:02.000000 firexapp-4.9.9/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2021-11-29 20:50:02.000000 firexapp-4.9.9/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      463 2021-11-29 20:50:19.169857 firexapp-4.9.9/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2021-11-29 20:50:02.000000 firexapp-4.9.9/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-11-29 20:50:02.000000 firexapp-4.9.9/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.170857 firexapp-4.9.9/firexapp/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2021-11-29 20:50:19.170857 firexapp-4.9.9/firexapp/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6113 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/application.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.158856 firexapp-4.9.9/firexapp/broker_manager/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      685 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/broker_manager/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/broker_manager/broker_factory.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13245 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/broker_manager/redis_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    12709 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/celery_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6647 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/discovery.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.159856 firexapp-4.9.9/firexapp/engine/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/celery.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2044 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/default_celery_config.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5318 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/engine/logging.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.161856 firexapp-4.9.9/firexapp/events/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3756 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/broker_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    12149 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/event_aggregator.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3475 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/events/model.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/fileregistry.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    14695 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/firex_subprocess.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/info.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    10435 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/plugins.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.162856 firexapp-4.9.9/firexapp/reporters/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/reporters/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5173 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/reporters/json_reporter.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.165856 firexapp-4.9.9/firexapp/submit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/arguments.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5301 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/console.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/install_configs.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/report_trigger.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5468 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/reporting.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9212 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/shutdown.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    29935 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/submit.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1490 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/tracking_service.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3250 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/submit/uid.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.167857 firexapp-4.9.9/firexapp/tasks/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/core_tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/example.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3247 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/tasks/root_tasks.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.169857 firexapp-4.9.9/firexapp/testing/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4323 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/config_base.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13199 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/config_interpreter.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/coverage_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3168 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/pydev_debug_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7228 2021-11-29 20:50:02.000000 firexapp-4.9.9/firexapp/testing/test_infra.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-11-29 20:50:19.157856 firexapp-4.9.9/firexapp.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      463 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      191 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      187 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-11-29 20:50:19.000000 firexapp-4.9.9/firexapp.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2021-11-29 20:50:19.170857 firexapp-4.9.9/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1690 2021-11-29 20:50:02.000000 firexapp-4.9.9/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-11-29 20:50:02.000000 firexapp-4.9.9/versioneer.py
```

### Comparing `firexapp-4.9.8/LICENSE` & `firexapp-4.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/fastentrypoints.py` & `firexapp-4.9.9/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/application.py` & `firexapp-4.9.9/firexapp/application.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/broker_manager/__init__.py` & `firexapp-4.9.9/firexapp/broker_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/broker_manager/broker_factory.py` & `firexapp-4.9.9/firexapp/broker_manager/broker_factory.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/broker_manager/redis_manager.py` & `firexapp-4.9.9/firexapp/broker_manager/redis_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/celery_manager.py` & `firexapp-4.9.9/firexapp/celery_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/common.py` & `firexapp-4.9.9/firexapp/common.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/discovery.py` & `firexapp-4.9.9/firexapp/discovery.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/engine/celery.py` & `firexapp-4.9.9/firexapp/engine/celery.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/engine/default_celery_config.py` & `firexapp-4.9.9/firexapp/engine/default_celery_config.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/engine/logging.py` & `firexapp-4.9.9/firexapp/engine/logging.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/events/broker_event_consumer.py` & `firexapp-4.9.9/firexapp/events/broker_event_consumer.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/events/event_aggregator.py` & `firexapp-4.9.9/firexapp/events/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/events/model.py` & `firexapp-4.9.9/firexapp/events/model.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/fileregistry.py` & `firexapp-4.9.9/firexapp/fileregistry.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/firex_subprocess.py` & `firexapp-4.9.9/firexapp/firex_subprocess.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/info.py` & `firexapp-4.9.9/firexapp/info.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/plugins.py` & `firexapp-4.9.9/firexapp/plugins.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/reporters/json_reporter.py` & `firexapp-4.9.9/firexapp/reporters/json_reporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     submission_dir: str
     submission_cmd: List[str]
     # TODO: the following default is temporary to workaround
     # a testing chicken-and-egg problem. It should be removed
     # after 25/11/2021
     viewers: Dict[str, str] = None
     results: Dict = None
+    revoked: bool = False
 
 class FireXJsonReportGenerator(ReportGenerator):
     formatters = ('json',)
 
     reporter_dirname = 'json_reporter'
     initial_report_filename = 'initial_report.json'
     completion_report_filename = 'completion_report.json'
@@ -65,14 +66,15 @@
                       sort_keys=True,
                       indent=4)
 
     def pre_run_report(self, uid, chain, submission_dir, argv, original_cli=None, json_file=None, **kwargs):
         data = self.get_common_run_data(uid=uid, chain=chain, submission_dir=submission_dir, argv=argv,
                                         original_cli=original_cli)
         data['completed'] = False
+        data['revoked'] = False
         report_file = os.path.join(uid.logs_dir, self.reporter_dirname, self.initial_report_filename)
         self.write_report_file(data, report_file)
 
         report_link = os.path.join(uid.logs_dir, self.report_link_filename)
         try:
             create_link(report_file, report_link, delete_link=False)
         except FileExistsError:
@@ -82,19 +84,21 @@
         if json_file:
             try:
                 create_link(report_link, json_file, delete_link=False, relative=True)
             except FileExistsError:
                 logger.debug(f'{json_file} link already exist; '
                              f'post_run must have already created the link to {report_link}')
 
-    def post_run_report(self, uid, chain, root_id, submission_dir, argv, original_cli=None, json_file=None, **kwargs):
+    def post_run_report(self, uid, chain, root_id, submission_dir, argv, original_cli=None, json_file=None,
+                        run_revoked=False, **kwargs):
         data = self.get_common_run_data(uid=uid, chain=chain, submission_dir=submission_dir, argv=argv,
                                         original_cli=original_cli)
         data['completed'] = True
         data['results'] = get_results(root_id)
+        data['revoked'] = run_revoked
         report_file = os.path.join(uid.logs_dir, self.reporter_dirname, self.completion_report_filename)
 
         self.write_report_file(data, report_file)
 
         report_link = os.path.join(uid.logs_dir, self.report_link_filename)
         create_link(report_file, report_link, relative=True)
```

### Comparing `firexapp-4.9.8/firexapp/submit/arguments.py` & `firexapp-4.9.9/firexapp/submit/arguments.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/submit/console.py` & `firexapp-4.9.9/firexapp/submit/console.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/submit/install_configs.py` & `firexapp-4.9.9/firexapp/submit/install_configs.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/submit/report_trigger.py` & `firexapp-4.9.9/firexapp/submit/report_trigger.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/submit/reporting.py` & `firexapp-4.9.9/firexapp/submit/reporting.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     @classmethod
     def pre_run_report(cls, kwargs):
         for report_gen in cls.get_generators():
             report_gen.pre_run_report(**kwargs)
 
     @classmethod
-    def post_run_report(cls, results, kwargs):
+    def post_run_report(cls, results, kwargs, run_revoked=False):
         if kwargs is None:
             kwargs = {}
 
         if results:
             from celery import current_app
             logger.debug("Processing results data for reports")
             for task_result in recurse_results_tree(results):
@@ -99,15 +99,15 @@
                     logger.error(f"Failed to add report entry for task result {task_result}", exc_info=True)
 
             logger.debug("Completed processing results data for reports")
 
         for report_gen in cls.get_generators():
             try:
                 logger.debug(f'Running post_run_report for {report_gen}')
-                report_gen.post_run_report(root_id=results, **kwargs)
+                report_gen.post_run_report(root_id=results, run_revoked=run_revoked, **kwargs)
                 logger.debug(f'Completed post_run_report for {report_gen}')
             except Exception:
                 # Failure in one report generator should not impact another
                 logger.error(f'Error in the post_run_report for {report_gen}', exc_info=True)
```

### Comparing `firexapp-4.9.8/firexapp/submit/shutdown.py` & `firexapp-4.9.9/firexapp/submit/shutdown.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/submit/submit.py` & `firexapp-4.9.9/firexapp/submit/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,21 +521,23 @@
             mssg += '\n' + str(reason)
         logger.error(mssg)
         if self.broker:
             self.self_destruct(chain_details=chain_details, reason=reason)
         if self.uid:
             self.copy_submission_log()
 
-    def self_destruct(self, chain_details=None, reason=None):
+    def self_destruct(self, chain_details=None, reason=None, run_revoked=False):
         if chain_details:
             chain_result, chain_args = chain_details
             try:
                 logger.debug("Generating reports")
                 from firexapp.submit.reporting import ReportersRegistry
-                ReportersRegistry.post_run_report(results=chain_result, kwargs=chain_args)
+                ReportersRegistry.post_run_report(results=chain_result,
+                                                  kwargs=chain_args,
+                                                  run_revoked=run_revoked)
                 logger.debug('Reports successfully generated')
             except Exception:
                 # Under no circumstances should report generation prevent celery and broker cleanup
                 logger.error('Error in generating reports', exc_info=True)
             finally:
                 # AsyncResult objects access self.backend when garbage collected. Since we're about to initiate a
                 # process to stop the backend, prevent all AsyncResult objects from accessing self.backend.
```

### Comparing `firexapp-4.9.8/firexapp/submit/tracking_service.py` & `firexapp-4.9.9/firexapp/submit/tracking_service.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/submit/uid.py` & `firexapp-4.9.9/firexapp/submit/uid.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/tasks/core_tasks.py` & `firexapp-4.9.9/firexapp/tasks/core_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/tasks/example.py` & `firexapp-4.9.9/firexapp/tasks/example.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/tasks/root_tasks.py` & `firexapp-4.9.9/firexapp/tasks/root_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,22 +51,24 @@
         logger.warning("Cannot find submit_app. Root task post-run handling aborted.")
         return
 
     result = task.AsyncResult(task_id)
     sync = kwargs.get("sync", False)
 
     result_state = result.state
-    if sync and result_state != REVOKED and result_state != RETRY:  # Revoked can be in retry state with celery 5.1.0
+    is_revoked = result_state in [REVOKED, RETRY] # Revoked can be in retry state with celery 5.1.0
+    if sync and not is_revoked:
         logger.debug("Sync run has not been revoked. Cleanup skipped.")
         # Only if --sync run was revoked do we want to do the shutdown here; else it's done in firex.py
         return
 
     # Let this signal cause self-destruct
     submit_app.self_destruct(chain_details=(result, kwargs),
-                             reason=f'Root task completion ({result.state}) detected via postrun signal.')
+                             reason=f'Root task completion ({result.state}) detected via postrun signal.',
+                             run_revoked=is_revoked)
 
     logger.info("Root task post run signal completed")
 
 
 class BrokerShutdown(bootsteps.StartStopStep):
     """ This celery shutdown step will cleanup redis """
     label = "Broker"
```

### Comparing `firexapp-4.9.8/firexapp/testing/config_base.py` & `firexapp-4.9.9/firexapp/testing/config_base.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/testing/config_interpreter.py` & `firexapp-4.9.9/firexapp/testing/config_interpreter.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/testing/coverage_plugin.py` & `firexapp-4.9.9/firexapp/testing/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/testing/pydev_debug_plugin.py` & `firexapp-4.9.9/firexapp/testing/pydev_debug_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp/testing/test_infra.py` & `firexapp-4.9.9/firexapp/testing/test_infra.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/firexapp.egg-info/SOURCES.txt` & `firexapp-4.9.9/firexapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/setup.py` & `firexapp-4.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `firexapp-4.9.8/versioneer.py` & `firexapp-4.9.9/versioneer.py`

 * *Files identical despite different names*

