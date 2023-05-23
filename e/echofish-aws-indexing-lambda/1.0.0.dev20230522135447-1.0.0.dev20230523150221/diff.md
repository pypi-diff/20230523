# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230522135447.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230523150221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230522135447.tar", last modified: Mon May 22 13:55:30 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230523150221.tar", last modified: Tue May 23 15:03:03 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:55:30.562215 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-22 13:54:41.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-22 13:55:30.562215 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-22 13:54:41.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 13:55:30.562215 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-22 13:55:27.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:55:30.558215 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:55:30.558215 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 13:54:41.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12138 2023-05-22 13:54:41.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-05-22 13:54:41.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:55:30.562215 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-22 13:55:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-22 13:55:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 13:55:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-22 13:55:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 13:55:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:03:03.851119 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-23 15:02:14.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 15:03:03.851119 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-23 15:02:14.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:03:03.851119 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 15:03:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:03:03.847119 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:03:03.847119 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:02:14.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12138 2023-05-23 15:02:14.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-23 15:02:14.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:03:03.851119 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 15:03:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-23 15:03:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:03:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 15:03:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 15:03:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230522135447
+Version: 1.0.0.dev20230523150221
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230522135447",
+  version="1.0.0.dev20230523150221",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230522135447/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230523150221/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230522135447
+Version: 1.0.0.dev20230523150221
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

