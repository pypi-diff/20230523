# Comparing `tmp/suite-py-1.9.8.tar.gz` & `tmp/suite-py-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suite-py-1.9.8.tar", last modified: Thu Aug  6 09:46:24 2020, max compression
+gzip compressed data, was "dist/suite-py-1.9.9.tar", last modified: Tue Aug 11 15:01:48 2020, max compression
```

## Comparing `suite-py-1.9.8.tar` & `suite-py-1.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-06 09:46:24.000000 suite-py-1.9.8/
--rw-r--r--   0 root         (0) root         (0)     9749 2020-08-06 09:45:36.000000 suite-py-1.9.8/LICENSE-APACHE
--rw-r--r--   0 root         (0) root         (0)     1065 2020-08-06 09:45:36.000000 suite-py-1.9.8/LICENSE-MIT
--rw-r--r--   0 root         (0) root         (0)       62 2020-08-06 09:45:36.000000 suite-py-1.9.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1066 2020-08-06 09:46:24.000000 suite-py-1.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2020-08-06 09:45:36.000000 suite-py-1.9.8/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2020-08-06 09:46:24.000000 suite-py-1.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2181 2020-08-06 09:45:36.000000 suite-py-1.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py/
--rw-r--r--   0 root         (0) root         (0)      143 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/__init__.py
--rw-r--r--   0 root         (0) root         (0)       48 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/__version__.py
--rwxr-xr-x   0 root         (0) root         (0)     5081 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3928 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/ask_review.py
--rw-r--r--   0 root         (0) root         (0)     3822 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/check.py
--rw-r--r--   0 root         (0) root         (0)     2211 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/create_branch.py
--rw-r--r--   0 root         (0) root         (0)     4667 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/create_qa.py
--rw-r--r--   0 root         (0) root         (0)      666 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/delete_qa.py
--rw-r--r--   0 root         (0) root         (0)     7560 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/deploy.py
--rw-r--r--   0 root         (0) root         (0)     7004 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/generator.py
--rw-r--r--   0 root         (0) root         (0)     1675 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/ip.py
--rw-r--r--   0 root         (0) root         (0)     6054 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/merge_pr.py
--rw-r--r--   0 root         (0) root         (0)     5254 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/open_pr.py
--rw-r--r--   0 root         (0) root         (0)     1988 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/project_lock.py
--rw-r--r--   0 root         (0) root         (0)     4567 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/rollback.py
--rw-r--r--   0 root         (0) root         (0)     1075 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/commands/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2073 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py/lib/handler/
--rw-r--r--   0 root         (0) root         (0)        0 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6795 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/aws_handler.py
--rw-r--r--   0 root         (0) root         (0)     2090 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/captainhook_handler.py
--rw-r--r--   0 root         (0) root         (0)     5573 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/drone_handler.py
--rw-r--r--   0 root         (0) root         (0)     9076 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/git_handler.py
--rw-r--r--   0 root         (0) root         (0)     2420 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/github_handler.py
--rw-r--r--   0 root         (0) root         (0)     1234 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/prompt_utils.py
--rw-r--r--   0 root         (0) root         (0)     2220 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/handler/youtrack_handler.py
--rw-r--r--   0 root         (0) root         (0)      233 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/logger.py
--rw-r--r--   0 root         (0) root         (0)     1404 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/qainit.py
--rw-r--r--   0 root         (0) root         (0)       60 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/symbol.py
--rw-r--r--   0 root         (0) root         (0)     1475 2020-08-06 09:45:36.000000 suite-py-1.9.8/suite_py/lib/tokens.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1066 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1177 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      218 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2020-08-06 09:46:24.000000 suite-py-1.9.8/suite_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-11 15:01:48.000000 suite-py-1.9.9/
+-rw-r--r--   0 root         (0) root         (0)     9749 2020-08-11 15:01:05.000000 suite-py-1.9.9/LICENSE-APACHE
+-rw-r--r--   0 root         (0) root         (0)     1065 2020-08-11 15:01:05.000000 suite-py-1.9.9/LICENSE-MIT
+-rw-r--r--   0 root         (0) root         (0)       62 2020-08-11 15:01:05.000000 suite-py-1.9.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1066 2020-08-11 15:01:48.000000 suite-py-1.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2020-08-11 15:01:05.000000 suite-py-1.9.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2020-08-11 15:01:48.000000 suite-py-1.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2181 2020-08-11 15:01:05.000000 suite-py-1.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py/
+-rw-r--r--   0 root         (0) root         (0)      143 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       48 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/__version__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5081 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/ask_review.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/check.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/create_branch.py
+-rw-r--r--   0 root         (0) root         (0)     4667 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/create_qa.py
+-rw-r--r--   0 root         (0) root         (0)      666 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/delete_qa.py
+-rw-r--r--   0 root         (0) root         (0)     7560 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     7004 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/ip.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/merge_pr.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/open_pr.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/project_lock.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/rollback.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/commands/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2073 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py/lib/handler/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6795 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/aws_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/captainhook_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5573 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/drone_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/git_handler.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/github_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/prompt_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/handler/youtrack_handler.py
+-rw-r--r--   0 root         (0) root         (0)      233 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/qainit.py
+-rw-r--r--   0 root         (0) root         (0)       60 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/symbol.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2020-08-11 15:01:05.000000 suite-py-1.9.9/suite_py/lib/tokens.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1066 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1177 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      218 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2020-08-11 15:01:48.000000 suite-py-1.9.9/suite_py.egg-info/top_level.txt
```

### Comparing `suite-py-1.9.8/LICENSE-APACHE` & `suite-py-1.9.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/LICENSE-MIT` & `suite-py-1.9.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/PKG-INFO` & `suite-py-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: suite-py
-Version: 1.9.8
+Version: 1.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/primait/suite_py
 Author: Prima Assicurazioni S.p.A
 Author-email: devops@prima.it
 Maintainer: larrywax, EugenioLaghi, michelangelomo
 Maintainer-email: devops@prima.it
 License: MIT/Apache-2.0
```

### Comparing `suite-py-1.9.8/README.rst` & `suite-py-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/setup.py` & `suite-py-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/cli.py` & `suite-py-1.9.9/suite_py/cli.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/ask_review.py` & `suite-py-1.9.9/suite_py/commands/ask_review.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/check.py` & `suite-py-1.9.9/suite_py/commands/check.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/create_branch.py` & `suite-py-1.9.9/suite_py/commands/create_branch.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/create_qa.py` & `suite-py-1.9.9/suite_py/commands/create_qa.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/delete_qa.py` & `suite-py-1.9.9/suite_py/commands/delete_qa.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/deploy.py` & `suite-py-1.9.9/suite_py/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/generator.py` & `suite-py-1.9.9/suite_py/commands/generator.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/ip.py` & `suite-py-1.9.9/suite_py/commands/ip.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/merge_pr.py` & `suite-py-1.9.9/suite_py/commands/merge_pr.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/open_pr.py` & `suite-py-1.9.9/suite_py/commands/open_pr.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/project_lock.py` & `suite-py-1.9.9/suite_py/commands/project_lock.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/rollback.py` & `suite-py-1.9.9/suite_py/commands/rollback.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/commands/status.py` & `suite-py-1.9.9/suite_py/commands/status.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/config.py` & `suite-py-1.9.9/suite_py/lib/config.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/aws_handler.py` & `suite-py-1.9.9/suite_py/lib/handler/aws_handler.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/captainhook_handler.py` & `suite-py-1.9.9/suite_py/lib/handler/captainhook_handler.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/drone_handler.py` & `suite-py-1.9.9/suite_py/lib/handler/drone_handler.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/git_handler.py` & `suite-py-1.9.9/suite_py/lib/handler/git_handler.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/github_handler.py` & `suite-py-1.9.9/suite_py/lib/handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/prompt_utils.py` & `suite-py-1.9.9/suite_py/lib/handler/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/handler/youtrack_handler.py` & `suite-py-1.9.9/suite_py/lib/handler/youtrack_handler.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/qainit.py` & `suite-py-1.9.9/suite_py/lib/qainit.py`

 * *Files identical despite different names*

### Comparing `suite-py-1.9.8/suite_py/lib/tokens.py` & `suite-py-1.9.9/suite_py/lib/tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 TOKENS = ["github", "youtrack", "drone"]
 
 
 class Tokens:
     def __init__(self, file_name=os.path.join(os.environ["HOME"], ".suite_py/tokens")):
         self._file_name = file_name
+        self._tokens = {}
         try:
             self.load()
         except Exception:
             pass
 
         self._changed = False
         self.check()
```

### Comparing `suite-py-1.9.8/suite_py.egg-info/PKG-INFO` & `suite-py-1.9.9/suite_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: suite-py
-Version: 1.9.8
+Version: 1.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/primait/suite_py
 Author: Prima Assicurazioni S.p.A
 Author-email: devops@prima.it
 Maintainer: larrywax, EugenioLaghi, michelangelomo
 Maintainer-email: devops@prima.it
 License: MIT/Apache-2.0
```

### Comparing `suite-py-1.9.8/suite_py.egg-info/SOURCES.txt` & `suite-py-1.9.9/suite_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

