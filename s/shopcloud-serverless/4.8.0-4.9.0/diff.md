# Comparing `tmp/shopcloud-serverless-4.8.0.tar.gz` & `tmp/shopcloud-serverless-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud-serverless-4.8.0.tar", last modified: Sun Apr  2 06:48:56 2023, max compression
+gzip compressed data, was "shopcloud-serverless-4.9.0.tar", last modified: Sun May 21 13:57:08 2023, max compression
```

## Comparing `shopcloud-serverless-4.8.0.tar` & `shopcloud-serverless-4.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 06:48:56.750018 shopcloud-serverless-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-02 06:48:56.750018 shopcloud-serverless-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 06:48:56.746019 shopcloud-serverless-4.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/scripts/serverless
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 06:48:56.750018 shopcloud-serverless-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-02 06:48:54.000000 shopcloud-serverless-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 06:48:56.750018 shopcloud-serverless-4.8.0/shopcloud_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/file_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-02 06:48:42.000000 shopcloud-serverless-4.8.0/shopcloud_serverless/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 06:48:56.750018 shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-02 06:48:56.000000 shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-02 06:48:56.000000 shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 06:48:56.000000 shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-02 06:48:56.000000 shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-02 06:48:56.000000 shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:57:08.225619 shopcloud-serverless-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-21 13:57:08.225619 shopcloud-serverless-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:57:08.221619 shopcloud-serverless-4.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/scripts/serverless
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:57:08.225619 shopcloud-serverless-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-21 13:57:05.000000 shopcloud-serverless-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:57:08.221619 shopcloud-serverless-4.9.0/shopcloud_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/file_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-21 13:56:52.000000 shopcloud-serverless-4.9.0/shopcloud_serverless/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:57:08.225619 shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-21 13:57:08.000000 shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-21 13:57:08.000000 shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:57:08.000000 shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-21 13:57:08.000000 shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 13:57:08.000000 shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/top_level.txt
```

### Comparing `shopcloud-serverless-4.8.0/LICENSE` & `shopcloud-serverless-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/PKG-INFO` & `shopcloud-serverless-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-serverless
-Version: 4.8.0
+Version: 4.9.0
 Summary: CLI tool for creating a serverles api with API Gateway and Cloud Functions
 Home-page: https://github.com/Talk-Point/shopcloud-serverless-cli
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud-serverless-4.8.0/README.md` & `shopcloud-serverless-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/setup.py` & `shopcloud-serverless-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = {
     "name": 'shopcloud-serverless',
-    "version": '4.8.0',
+    "version": '4.9.0',
     "description": 'CLI tool for creating a serverles api with API Gateway and Cloud Functions',
     "long_description_content_type": "text/markdown",
     "long_description": README,
     "license": 'MIT',
     "packages": find_packages(),
     "author": 'Konstantin Stoldt',
     "author_email": 'konstantin.stoldt@talk-point.de',
```

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/__main__.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/__main__.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/cli.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/cli.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/configs.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/configs.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/endpoints.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         is_simulate = kwargs.get('is_simulate', False)
         env = {
             **self._env_secrets(config, is_simulate=is_simulate),
             **{
                 'ENV': 'production',
             }
         }
-        env = yaml.dump(env, default_flow_style=False)
+        env = yaml.dump(env, explicit_start=True, sort_keys=False, indent=2, width=1000)
         env = env.replace("'{{", "{{").replace("}}'", '}}')
         return env
 
 
 def endpoint_load(config: Config) -> dict:
     with open(f"{config.base_dir}/api.yaml") as f:
         data = yaml.safe_load(f)
```

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/file_contents.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/file_contents.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/gateways.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/gateways.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/helpers.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/helpers.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/jobs.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/jobs.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless/steps.py` & `shopcloud-serverless-4.9.0/shopcloud_serverless/steps.py`

 * *Files identical despite different names*

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/PKG-INFO` & `shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-serverless
-Version: 4.8.0
+Version: 4.9.0
 Summary: CLI tool for creating a serverles api with API Gateway and Cloud Functions
 Home-page: https://github.com/Talk-Point/shopcloud-serverless-cli
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud-serverless-4.8.0/shopcloud_serverless.egg-info/SOURCES.txt` & `shopcloud-serverless-4.9.0/shopcloud_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

