# Comparing `tmp/pyPhases-1.2.0.tar.gz` & `tmp/pyPhases-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhases-1.2.0.tar", last modified: Mon May 22 06:34:00 2023, max compression
+gzip compressed data, was "pyPhases-1.2.1.tar", last modified: Tue May 23 13:08:48 2023, max compression
```

## Comparing `pyPhases-1.2.0.tar` & `pyPhases-1.2.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.597839 pyPhases-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-22 06:33:46.000000 pyPhases-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-22 06:33:46.000000 pyPhases-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4666 2023-05-22 06:34:00.597839 pyPhases-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4180 2023-05-22 06:33:46.000000 pyPhases-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.589840 pyPhases-1.2.0/pyPhases/
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/Data.py
--rw-rw-rw-   0 root         (0) root         (0)     3319 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/Phase.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/PluginAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    15638 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/Project.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-22 06:33:48.000000 pyPhases-1.2.0/pyPhases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.590839 pyPhases-1.2.0/pyPhases/decorator/
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/decorator/Decorator.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/decorator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.590839 pyPhases-1.2.0/pyPhases/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     2660 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/exporter/DataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/exporter/PickleExporter.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.591839 pyPhases-1.2.0/pyPhases/test/
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/MockLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/Mocks.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/TestCase.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/TestCaseIntegration.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/TestRun.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.593840 pyPhases-1.2.0/pyPhases/util/
--rw-rw-rw-   0 root         (0) root         (0)     2692 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/BatchProgress.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/EventBus.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/EventBusStatic.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/Logger.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/Optionizable.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/pdict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.590839 pyPhases-1.2.0/pyPhases.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4666 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-22 06:33:46.000000 pyPhases-1.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 06:34:00.597839 pyPhases-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-05-22 06:33:48.000000 pyPhases-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.593840 pyPhases-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.594839 pyPhases-1.2.0/tests/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_BaseTest.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_IntegrationTest.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_Mocks.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_TestRun.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test_acceptance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.596840 pyPhases-1.2.0/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_BatchProgress.py
--rw-rw-rw-   0 root         (0) root         (0)     6047 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Data.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_DataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Decorator.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_EventBus.py
--rw-rw-rw-   0 root         (0) root         (0)     3074 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3146 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Loggermock.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Optionizable.py
--rw-rw-rw-   0 root         (0) root         (0)     5056 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Phase.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_PluginAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17896 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Project.py
--rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_csvlogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_exporter_pickleexporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_pdict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.596840 pyPhases-1.2.0/tests/util/
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/util/ExporterTestHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/util/PhaseGenerator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.841060 pyPhases-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-23 13:08:35.000000 pyPhases-1.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-23 13:08:35.000000 pyPhases-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-05-23 13:08:48.841060 pyPhases-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4180 2023-05-23 13:08:35.000000 pyPhases-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.831060 pyPhases-1.2.1/pyPhases/
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/Data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3319 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/Phase.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/PluginAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15638 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-23 13:08:37.000000 pyPhases-1.2.1/pyPhases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.833060 pyPhases-1.2.1/pyPhases/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/decorator/Decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/decorator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.833060 pyPhases-1.2.1/pyPhases/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/exporter/DataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/exporter/PickleExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.834060 pyPhases-1.2.1/pyPhases/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/test/MockLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/test/Mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/test/TestCase.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/test/TestCaseIntegration.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/test/TestRun.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.836060 pyPhases-1.2.1/pyPhases/util/
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/BatchProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/EventBus.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/EventBusStatic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/Optionizable.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyPhases/util/pdict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.832059 pyPhases-1.2.1/pyPhases.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-05-23 13:08:48.000000 pyPhases-1.2.1/pyPhases.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-23 13:08:48.000000 pyPhases-1.2.1/pyPhases.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 13:08:48.000000 pyPhases-1.2.1/pyPhases.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-23 13:08:48.000000 pyPhases-1.2.1/pyPhases.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-23 13:08:48.000000 pyPhases-1.2.1/pyPhases.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-23 13:08:35.000000 pyPhases-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-23 13:08:35.000000 pyPhases-1.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 13:08:48.841060 pyPhases-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-23 13:08:37.000000 pyPhases-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.836060 pyPhases-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.837060 pyPhases-1.2.1/tests/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/test/test_BaseTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/test/test_IntegrationTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/test/test_Mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/test/test_TestRun.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/test_acceptance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.840060 pyPhases-1.2.1/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_BatchProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)     6047 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_DataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_EventBus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_EventBusStatic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3074 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Loggermock.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Optionizable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5056 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Phase.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_PluginAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17896 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_csvlogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_exporter_pickleexporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/unit/test_pdict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 13:08:48.840060 pyPhases-1.2.1/tests/util/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/util/ExporterTestHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/util/PhaseGenerator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 13:08:35.000000 pyPhases-1.2.1/tests/util/__init__.py
```

### Comparing `pyPhases-1.2.0/LICENSE` & `pyPhases-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/PKG-INFO` & `pyPhases-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyPhases
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt/pyPhases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyPhases
```

### Comparing `pyPhases-1.2.0/README.md` & `pyPhases-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/Data.py` & `pyPhases-1.2.1/pyPhases/Data.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/Phase.py` & `pyPhases-1.2.1/pyPhases/Phase.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/Project.py` & `pyPhases-1.2.1/pyPhases/Project.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/decorator/Decorator.py` & `pyPhases-1.2.1/pyPhases/decorator/Decorator.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/exporter/DataExporter.py` & `pyPhases-1.2.1/pyPhases/exporter/DataExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/exporter/PickleExporter.py` & `pyPhases-1.2.1/pyPhases/exporter/PickleExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/test/MockLogger.py` & `pyPhases-1.2.1/pyPhases/test/MockLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/test/TestCase.py` & `pyPhases-1.2.1/pyPhases/test/TestCase.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/test/TestRun.py` & `pyPhases-1.2.1/pyPhases/test/TestRun.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/BatchProgress.py` & `pyPhases-1.2.1/pyPhases/util/BatchProgress.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/CSVLogger.py` & `pyPhases-1.2.1/pyPhases/util/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/EventBus.py` & `pyPhases-1.2.1/pyPhases/util/EventBus.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/EventBusStatic.py` & `pyPhases-1.2.1/pyPhases/util/EventBusStatic.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/Logger.py` & `pyPhases-1.2.1/pyPhases/util/Logger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/Optionizable.py` & `pyPhases-1.2.1/pyPhases/util/Optionizable.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases/util/pdict.py` & `pyPhases-1.2.1/pyPhases/util/pdict.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/pyPhases.egg-info/PKG-INFO` & `pyPhases-1.2.1/pyPhases.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyPhases
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt/pyPhases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyPhases
```

### Comparing `pyPhases-1.2.0/pyPhases.egg-info/SOURCES.txt` & `pyPhases-1.2.1/pyPhases.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 tests/test/test_TestRun.py
 tests/unit/__init__.py
 tests/unit/test_BatchProgress.py
 tests/unit/test_Data.py
 tests/unit/test_DataExporter.py
 tests/unit/test_Decorator.py
 tests/unit/test_EventBus.py
+tests/unit/test_EventBusStatic.py
 tests/unit/test_Logger.py
 tests/unit/test_Loggermock.py
 tests/unit/test_Optionizable.py
 tests/unit/test_Phase.py
 tests/unit/test_PluginAdapter.py
 tests/unit/test_Project.py
 tests/unit/test_csvlogger.py
```

### Comparing `pyPhases-1.2.0/setup.py` & `pyPhases-1.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhases",
-    version="v1.2.0"[1:],
+    version="v1.2.1"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt/pyPhases",
     packages=setuptools.find_packages(exclude="tests"),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["tqdm", "PyYAML"],
     python_requires=">=3.5",
 )
```

### Comparing `pyPhases-1.2.0/tests/test/test_BaseTest.py` & `pyPhases-1.2.1/tests/test/test_BaseTest.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/test/test_IntegrationTest.py` & `pyPhases-1.2.1/tests/test/test_IntegrationTest.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/test/test_Mocks.py` & `pyPhases-1.2.1/tests/test/test_Mocks.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/test/test_TestRun.py` & `pyPhases-1.2.1/tests/test/test_TestRun.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_BatchProgress.py` & `pyPhases-1.2.1/tests/unit/test_BatchProgress.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_Data.py` & `pyPhases-1.2.1/tests/unit/test_Data.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_DataExporter.py` & `pyPhases-1.2.1/tests/unit/test_DataExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_EventBus.py` & `pyPhases-1.2.1/tests/unit/test_EventBus.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_Logger.py` & `pyPhases-1.2.1/tests/unit/test_Logger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_Loggermock.py` & `pyPhases-1.2.1/tests/unit/test_Loggermock.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_Optionizable.py` & `pyPhases-1.2.1/tests/unit/test_Optionizable.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_Phase.py` & `pyPhases-1.2.1/tests/unit/test_Phase.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_PluginAdapter.py` & `pyPhases-1.2.1/tests/unit/test_PluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_Project.py` & `pyPhases-1.2.1/tests/unit/test_Project.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_csvlogger.py` & `pyPhases-1.2.1/tests/unit/test_csvlogger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_exporter_pickleexporter.py` & `pyPhases-1.2.1/tests/unit/test_exporter_pickleexporter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/unit/test_pdict.py` & `pyPhases-1.2.1/tests/unit/test_pdict.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/util/ExporterTestHelper.py` & `pyPhases-1.2.1/tests/util/ExporterTestHelper.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.2.0/tests/util/PhaseGenerator.py` & `pyPhases-1.2.1/tests/util/PhaseGenerator.py`

 * *Files identical despite different names*

