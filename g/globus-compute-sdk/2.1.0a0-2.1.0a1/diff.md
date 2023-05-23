# Comparing `tmp/globus-compute-sdk-2.1.0a0.tar.gz` & `tmp/globus-compute-sdk-2.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.1.0a0.tar", last modified: Tue May 23 18:43:32 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.1.0a1.tar", last modified: Tue May 23 18:47:03 2023, max compression
```

## Comparing `globus-compute-sdk-2.1.0a0.tar` & `globus-compute-sdk-2.1.0a1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/
--rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/LICENSE
--rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/MANIFEST.in
--rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)      816 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/PyPI.md
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.230188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/
--rw-rw-r--   0 reid      (1000) reid      (1000)      433 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/__init__.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.230188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/errors/
--rw-rw-r--   0 reid      (1000) reid      (1000)      320 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/errors/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1921 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/errors/error_types.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.230188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      986 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/_environments.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      648 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      724 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    11458 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2262 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/batch.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    26362 2023-05-17 18:35:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/client.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2400 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/container_spec.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    46344 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/executor.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/
--rw-rw-r--   0 reid      (1000) reid      (1000)      237 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1787 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      855 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      373 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      954 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7287 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/manager.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      710 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3012 2023-05-04 22:24:51.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2190 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/utils/
--rw-rw-r--   0 reid      (1000) reid      (1000)      212 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/utils/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1207 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/utils/printing.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     8618 2023-05-17 18:37:21.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/web_client.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/
--rw-rw-r--   0 reid      (1000) reid      (1000)      100 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1372 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7513 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/concretes.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3737 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/facade.py
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/utils.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      834 2023-05-23 18:27:36.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk/version.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.230188 globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/
--rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-05-23 18:43:32.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)     1628 2023-05-23 18:43:32.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-23 18:43:32.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      397 2023-05-23 18:43:32.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/requires.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)       19 2023-05-23 18:43:32.000000 globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/top_level.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/setup.cfg
--rw-rw-r--   0 reid      (1000) reid      (1000)     3161 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a0/setup.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:43:32.234188 globus-compute-sdk-2.1.0a0/tests/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/tests/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1962 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a0/tests/conftest.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2276 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a0/tests/utils.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/LICENSE
+-rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/MANIFEST.in
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-05-23 18:47:03.951557 globus-compute-sdk-2.1.0a1/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)      816 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/PyPI.md
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.943557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      433 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/__init__.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.943557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      320 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1921 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/error_types.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      986 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/_environments.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      648 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      724 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11458 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2262 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/batch.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    26362 2023-05-17 18:35:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/client.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2400 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/container_spec.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    46344 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/executor.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      237 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1787 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      855 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      373 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      954 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7287 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      710 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3012 2023-05-04 22:24:51.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2190 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      212 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1207 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/printing.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     8618 2023-05-17 18:37:21.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/web_client.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      100 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1372 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7513 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/concretes.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3737 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/facade.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/utils.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      834 2023-05-23 18:46:25.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/version.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.943557 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1628 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      397 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/requires.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       19 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-05-23 18:47:03.951557 globus-compute-sdk-2.1.0a1/setup.cfg
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3161 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a1/setup.py
+drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/tests/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/tests/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1962 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a1/tests/conftest.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2276 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/tests/utils.py
```

### Comparing `globus-compute-sdk-2.1.0a0/LICENSE` & `globus-compute-sdk-2.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/PKG-INFO` & `globus-compute-sdk-2.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.1.0a0
+Version: 2.1.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.1.0a0/PyPI.md` & `globus-compute-sdk-2.1.0a1/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk/version.py` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.1.0a0"
+__version__ = "2.1.0a1"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.1.0a0
+Version: 2.1.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.1.0a0/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/setup.py` & `globus-compute-sdk-2.1.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/tests/conftest.py` & `globus-compute-sdk-2.1.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a0/tests/utils.py` & `globus-compute-sdk-2.1.0a1/tests/utils.py`

 * *Files identical despite different names*

