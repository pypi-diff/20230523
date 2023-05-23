# Comparing `tmp/dcicutils-7.4.3.5b19.tar.gz` & `tmp/dcicutils-7.4.4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.3.5b19.tar", max compression
+gzip compressed data, was "dcicutils-7.4.4.1b2.tar", max compression
```

## Comparing `dcicutils-7.4.3.5b19.tar` & `dcicutils-7.4.4.1b2.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0     1098 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/README.rst
--rw-r--r--   0        0        0        0 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-22 08:05:57.994824 dcicutils-7.4.3.5b19/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    28556 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3968 2023-05-22 08:05:57.998824 dcicutils-7.4.3.5b19/pyproject.toml
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.3.5b19/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.3.5b19/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/README.rst
+-rw-r--r--   0        0        0        0 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154684 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11525 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3948 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.4.4.1b2/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.4.4.1b2/PKG-INFO
```

### Comparing `dcicutils-7.4.3.5b19/LICENSE.txt` & `dcicutils-7.4.4.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/README.rst` & `dcicutils-7.4.4.1b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/base.py` & `dcicutils-7.4.4.1b2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/codebuild_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/command_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/common.py` & `dcicutils-7.4.4.1b2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/creds_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/data_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/deployment_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/diff_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/docker_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/ecr_scripts.py` & `dcicutils-7.4.4.1b2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/ecr_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/ecs_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/env_base.py` & `dcicutils-7.4.4.1b2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/env_manager.py` & `dcicutils-7.4.4.1b2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/env_scripts.py` & `dcicutils-7.4.4.1b2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/env_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.4.1b2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/es_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/exceptions.py` & `dcicutils-7.4.4.1b2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/ff_mocks.py` & `dcicutils-7.4.4.1b2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/ff_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.4.1b2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/glacier_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/jh_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.4.1b2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/kibana/readme.md` & `dcicutils-7.4.4.1b2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/lang_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/log_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/misc_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/opensearch_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/qa_checkers.py` & `dcicutils-7.4.4.1b2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/qa_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/qa_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,24 +414,20 @@
             PRINT(f"Writing {content!r} to {self.file}.")
         file_system.files[self.file] = content if isinstance(content, bytes) else content.encode(self.encoding)
 
 
 class MockFileSystem:
     """Extremely low-tech mock file system."""
 
-    MOCK_USER_HOME = "/home/mock"
-    MOCK_ROOT_HOME = "/root"
-
     def __init__(self, files=None, default_encoding='utf-8', auto_mirror_files_for_read=False, do_not_auto_mirror=()):
         self.default_encoding = default_encoding
         # Setting this dynamically will make things inconsistent
         self._auto_mirror_files_for_read = auto_mirror_files_for_read
         self._do_not_auto_mirror = set(do_not_auto_mirror or [])
         self.files = {filename: content.encode(default_encoding) for filename, content in (files or {}).items()}
-        self.working_dir = self.MOCK_USER_HOME
         for filename in self.files:
             self._do_not_mirror(filename)
 
     IO_OPEN = staticmethod(io.open)
     OS_PATH_EXISTS = staticmethod(os.path.exists)
     OS_REMOVE = staticmethod(os.remove)
 
@@ -458,43 +454,14 @@
         return self.files.get(file) is not None  # don't want an empty file to pass for missing
 
     def remove(self, file):
         self._maybe_auto_mirror_file(file)
         if self.files.pop(file, None) is None:
             raise FileNotFoundError("No such file or directory: %s" % file)
 
-    def expanduser(self, file):
-        if file.startswith("~/"):
-            return os.path.join(self.MOCK_USER_HOME, file[2:])
-        elif file.startswith("~root/"):
-            return os.path.join(self.MOCK_ROOT_HOME, file[6:])
-        elif file == "~":
-            return self.MOCK_USER_HOME
-        elif file == "~root":
-            return self.MOCK_ROOT_HOME
-        else:
-            return file
-
-    def chdir(self, dirname):
-        assert isinstance(dirname, str), f"The argument to chdir must be a string: {dirname}"
-        self.working_dir = os.path.join(self.working_dir, dirname)
-
-    def getcwd(self):
-        return self.working_dir
-
-    def abspath(self, file):
-        if file.startswith("/"):
-            return file
-        elif file == ".":
-            return self.working_dir
-        elif file.startswith("./"):
-            return os.path.join(self.working_dir, file[2:])
-        else:
-            return os.path.join(self.working_dir, file)
-
     def open(self, file, mode='r', encoding=None):
         if FILE_SYSTEM_VERBOSE:  # pragma: no cover - Debugging option. Doesn't need testing.
             PRINT("Opening %r in mode %r." % (file, mode))
         if mode in ('w', 'wt', 'w+', 'w+t', 'wt+'):
             return self._open_for_write(file_system=self, file=file, binary=False, encoding=encoding)
         elif mode in ('wb', 'w+b', 'wb+'):
             return self._open_for_write(file_system=self, file=file, binary=True, encoding=encoding)
@@ -522,24 +489,14 @@
     @contextlib.contextmanager
     def mock_exists_open_remove(self):
         with mock.patch("os.path.exists", self.exists):
             with mock.patch("io.open", self.open):
                 with mock.patch("os.remove", self.remove):
                     yield self
 
-    @contextlib.contextmanager
-    def mock_exists_open_remove_abspath_getcwd_chdir(self):
-        with mock.patch("os.path.exists", self.exists):
-            with mock.patch("io.open", self.open):
-                with mock.patch("os.remove", self.remove):
-                    with mock.patch("os.path.abspath", self.abspath):
-                        with mock.patch("os.getcwd", self.getcwd):
-                            with mock.patch("os.chdir", self.chdir):
-                                yield self
-
 
 class MockAWSFileSystem(MockFileSystem):
 
     def __init__(self, boto3=None, s3=None, versioning_buckets: Union[Literal[True], list, set, tuple] = True,
                  **kwargs):
         self.boto3 = boto3 or MockBoto3()
         self.s3: MockBotoS3Client = s3 or self.boto3.client('s3')
```

### Comparing `dcicutils-7.4.3.5b19/dcicutils/redis_tools.py` & `dcicutils-7.4.4.1b2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/redis_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/s3_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.4.1b2/dcicutils/scripts/publish_to_pypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,23 +199,29 @@
         return False
     return True
 
 
 def get_untracked_files() -> list:
     """
     Returns a list of untracked files for the current git repo; empty list of no untracked changes.
+    We ignore __pycache__ directories which are excluded by poetry publish.
+    We ignore the .gitignore file for this.
     """
     package_directories = get_package_directories()
     untracked_files = []
     for package_directory in package_directories:
-        git_status_results, _ = execute_command(["git", "status", "-s", package_directory])
+        # The --ignored option ignores the .gitignore file.
+        git_status_results, _ = execute_command(["git", "status", "-s", "--ignored", package_directory])
         for git_status_result in git_status_results:
-            if git_status_result and git_status_result.startswith("??"):
+            if git_status_result and (git_status_result.startswith("??") or git_status_result.startswith("!!")):
                 untracked_file = git_status_result[2:].strip()
                 if untracked_file:
+                    # Ignore any __pycache__ directories as the are ignored by poetry publish.
+                    if os.path.isdir(untracked_file) and os.path.basename(untracked_file.rstrip("/")) == "__pycache__":
+                        continue
                     untracked_files.append(untracked_file)
     return untracked_files
 
 
 def get_package_version() -> str:
     """
     Returns the tag name of the most recently created tag in the current git repo.
```

### Comparing `dcicutils-7.4.3.5b19/dcicutils/secrets_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/snapshot_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/task_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/dcicutils/trace_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b19/pyproject.toml` & `dcicutils-7.4.4.1b2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.3.5b19"  # to become 7.5.0
+version = "7.4.4.1b2"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.3.5b19/setup.py` & `dcicutils-7.4.4.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.3.5b19',
+    'version': '7.4.4.1b2',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.3.5b19/PKG-INFO` & `dcicutils-7.4.4.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.3.5b19
+Version: 7.4.4.1b2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

