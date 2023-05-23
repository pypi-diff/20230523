# Comparing `tmp/torchlearn-0.1.0.tar.gz` & `tmp/torchlearn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlearn-0.1.0.tar", last modified: Sun Aug 28 11:11:40 2022, max compression
+gzip compressed data, was "torchlearn-0.2.0.tar", last modified: Tue May 23 18:28:34 2023, max compression
```

## Comparing `torchlearn-0.1.0.tar` & `torchlearn-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,54 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2022-08-28 11:11:40.899293 torchlearn-0.1.0/
--rw-r--r--   0 vincent    (501) staff       (20)    11357 2022-08-28 10:45:59.000000 torchlearn-0.1.0/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)       69 2022-08-28 10:58:26.000000 torchlearn-0.1.0/MANIFEST.in
--rw-r--r--   0 vincent    (501) staff       (20)      482 2022-08-28 11:11:40.899670 torchlearn-0.1.0/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       12 2022-08-28 10:45:59.000000 torchlearn-0.1.0/README.md
--rw-r--r--   0 vincent    (501) staff       (20)        5 2022-08-28 10:49:43.000000 torchlearn-0.1.0/VERSION
--rw-r--r--   0 vincent    (501) staff       (20)    22696 2022-08-28 10:49:19.000000 torchlearn-0.1.0/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)      158 2022-08-28 11:07:42.000000 torchlearn-0.1.0/requirements-dev.txt
--rw-r--r--   0 vincent    (501) staff       (20)        5 2022-08-28 10:54:50.000000 torchlearn-0.1.0/requirements.txt
--rw-r--r--   0 vincent    (501) staff       (20)      686 2022-08-28 11:11:40.902531 torchlearn-0.1.0/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)      122 2022-08-28 10:57:14.000000 torchlearn-0.1.0/setup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2022-08-28 11:11:40.895028 torchlearn-0.1.0/torchlearn/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2022-08-28 10:48:24.000000 torchlearn-0.1.0/torchlearn/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2022-08-28 11:11:40.898645 torchlearn-0.1.0/torchlearn.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      482 2022-08-28 11:11:40.000000 torchlearn-0.1.0/torchlearn.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      334 2022-08-28 11:11:40.000000 torchlearn-0.1.0/torchlearn.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2022-08-28 11:11:40.000000 torchlearn-0.1.0/torchlearn.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2022-08-28 10:53:53.000000 torchlearn-0.1.0/torchlearn.egg-info/not-zip-safe
--rw-r--r--   0 vincent    (501) staff       (20)      172 2022-08-28 11:11:40.000000 torchlearn-0.1.0/torchlearn.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       11 2022-08-28 11:11:40.000000 torchlearn-0.1.0/torchlearn.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11344 2023-05-23 18:24:04.000000 torchlearn-0.2.0/LICENSE
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       69 2023-05-23 18:21:28.000000 torchlearn-0.2.0/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1848 2023-05-23 18:28:34.649558 torchlearn-0.2.0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1390 2023-05-23 18:21:28.000000 torchlearn-0.2.0/README.md
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        5 2023-05-23 18:21:28.000000 torchlearn-0.2.0/VERSION
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    22727 2023-05-23 18:21:28.000000 torchlearn-0.2.0/pyproject.toml
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      158 2023-05-23 18:21:28.000000 torchlearn-0.2.0/requirements-dev.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       34 2023-05-23 18:21:35.000000 torchlearn-0.2.0/requirements.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      684 2023-05-23 18:28:34.649558 torchlearn-0.2.0/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      123 2023-05-23 18:21:28.000000 torchlearn-0.2.0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/metric/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1089 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/average_metric.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15375 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/classification.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      563 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/loss.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      384 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/metric.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      886 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/metric_dict.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2638 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/metric_value.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2039 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/metric/state.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/model/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1182 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/mlp.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      826 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/model/perceptron.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/objective/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/objective/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1507 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/objective/objective.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3592 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/objective/pareto.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/processing/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/processing/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5011 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/processing/graph.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/training/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      366 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/callback.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1756 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/early_stopping.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1875 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/pareto.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1786 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/results.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      225 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/schedulers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6408 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/training/trainer.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn/utils/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      738 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/arguments.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2604 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/graph.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      239 2023-05-23 18:21:28.000000 torchlearn-0.2.0/torchlearn/utils/numbers.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-23 18:28:34.649558 torchlearn-0.2.0/torchlearn.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1848 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1203 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-16 14:51:48.000000 torchlearn-0.2.0/torchlearn.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      201 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       11 2023-05-23 18:28:34.000000 torchlearn-0.2.0/torchlearn.egg-info/top_level.txt
```

### Comparing `torchlearn-0.1.0/LICENSE` & `torchlearn-0.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Vincent Coriou
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `torchlearn-0.1.0/pyproject.toml` & `torchlearn-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=62",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [tool.black]
-line-length = 79
+line-length = 120
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
   | \.mypy_cache
   | \.tox
@@ -20,16 +20,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.isort]
-profile = "black"
-line_length = 79
+line_length = 120
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q --cov-report term-missing --cov-report xml:.tests/coverage.xml --junitxml=.tests/test.xml"
 testpaths = ["tests"]
 
 [tool.coverage.run]
@@ -75,15 +74,15 @@
 fail-under = 10
 
 # Interpret the stdin as a python script, whose filename needs to be passed as
 # the module_or_package argument.
 # from-stdin =
 
 # Files or directories to be skipped. They should be base names, not paths.
-ignore = ["third_party"]
+ignore = ["tests"]
 
 # Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against paths and can be in Posix or Windows format.
 # ignore-paths =
 
 # Files or directories matching the regex patterns are skipped. The regex matches
 # against base names, not paths. The default value ignores Emacs file locks
@@ -303,15 +302,15 @@
 max-statements = 50
 
 # Minimum number of public methods for a class (see R0903).
 min-public-methods = 2
 
 [tool.pylint.exceptions]
 # Exceptions that will emit a warning when caught.
-overgeneral-exceptions = ["StandardError", "Exception", "BaseException"]
+overgeneral-exceptions = ["builtins.StandardError", "builtins.Exception", "builtins.BaseException"]
 
 [tool.pylint.format]
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 # expected-line-ending-format =
 
 # Regexp for a line that is allowed to be longer than the limit.
 ignore-long-lines = "(?x)(^\\s*(\\#\\ )?<?https?://\\S+>?$|^\\s*(from\\s+\\S+\\s+)?import\\s+.+$)"
@@ -320,15 +319,15 @@
 indent-after-paren = 4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
 indent-string = "    "
 
 # Maximum number of characters on a single line.
-max-line-length = 80
+max-line-length = 120
 
 # Maximum number of lines in a module.
 max-module-lines = 99999
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 # single-line-class-stmt =
@@ -569,8 +568,9 @@
 [tool.mypy]
 disallow_untyped_defs = true
 disallow_any_unimported = true
 no_implicit_optional = true
 check_untyped_defs = true
 warn_return_any = true
 warn_unused_ignores = true
-show_error_codes = true
+show_error_codes = true
+exclude = "test_.*\\.py"
```

### Comparing `torchlearn-0.1.0/setup.cfg` & `torchlearn-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = torchlearn
 version = file:VERSION
 author = Vincent Coriou
 author_email = vincent.coriou@gmail.com
 url = https://github.com/VincentCoriou
-description = ""
+description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "Apache License 2.0"
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
```

