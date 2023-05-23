# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230523150920.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230523171328.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230523150920.tar", last modified: Tue May 23 15:10:00 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230523171328.tar", last modified: Tue May 23 17:14:09 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:10:00.547670 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-23 15:09:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 15:10:00.547670 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-23 15:09:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:10:00.547670 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 15:09:57.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:10:00.543670 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:10:00.547670 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:09:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12138 2023-05-23 15:09:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-05-23 15:09:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:10:00.547670 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 15:10:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-23 15:10:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:10:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 15:10:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 15:10:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.609365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 17:14:09.609365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 17:14:09.609365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 17:14:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.605365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.605365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12138 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.605365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230523150920
+Version: 1.0.0.dev20230523171328
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230523150920",
+  version="1.0.0.dev20230523171328",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523150920/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230523150920
+Version: 1.0.0.dev20230523171328
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

