# Comparing `tmp/mypy-boto3-sagemaker-1.26.88.tar.gz` & `tmp/mypy-boto3-sagemaker-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-1.26.88.tar", last modified: Thu Mar  9 20:38:41 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-1.26.98.tar", last modified: Thu Mar 23 19:33:06 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-1.26.88.tar` & `mypy-boto3-sagemaker-1.26.98.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.698347 mypy-boto3-sagemaker-1.26.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    79304 2023-03-09 20:38:41.698347 mypy-boto3-sagemaker-1.26.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    77809 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.690347 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   259066 2023-03-09 20:38:04.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   258678 2023-03-09 20:38:03.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55040 2023-03-09 20:38:07.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55038 2023-03-09 20:38:07.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    97334 2023-03-09 20:38:05.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    97263 2023-03-09 20:38:04.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   481738 2023-03-09 20:38:21.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   481121 2023-03-09 20:38:14.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-03-09 20:38:05.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-03-09 20:38:05.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.698347 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    79304 2023-03-09 20:38:41.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-09 20:38:41.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-09 20:38:41.000000 mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:41.698347 mypy-boto3-sagemaker-1.26.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-09 20:38:00.000000 mypy-boto3-sagemaker-1.26.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.871667 mypy-boto3-sagemaker-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:30.000000 mypy-boto3-sagemaker-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    79614 2023-03-23 19:33:06.871667 mypy-boto3-sagemaker-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    78119 2023-03-23 19:32:30.000000 mypy-boto3-sagemaker-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.871667 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-03-23 19:32:30.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-03-23 19:32:30.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-23 19:32:31.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   260887 2023-03-23 19:32:33.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   260497 2023-03-23 19:32:32.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55241 2023-03-23 19:32:36.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55239 2023-03-23 19:32:35.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    97334 2023-03-23 19:32:34.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97263 2023-03-23 19:32:34.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:31.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   485583 2023-03-23 19:32:48.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   484964 2023-03-23 19:32:42.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:30.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-03-23 19:32:34.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-03-23 19:32:34.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.871667 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    79614 2023-03-23 19:33:06.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-23 19:33:06.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:06.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 19:33:06.000000 mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:06.871667 mypy-boto3-sagemaker-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-23 19:32:30.000000 mypy-boto3-sagemaker-1.26.98/setup.py
```

### Comparing `mypy-boto3-sagemaker-1.26.88/LICENSE` & `mypy-boto3-sagemaker-1.26.98/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-sagemaker-1.26.88/PKG-INFO` & `mypy-boto3-sagemaker-1.26.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sagemaker
-Version: 1.26.88
-Summary: Type annotations for boto3.SageMaker 1.26.88 service generated with mypy-boto3-builder 7.12.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-sagemaker"></a>
 
 # mypy-boto3-sagemaker
 
 [![PyPI - mypy-boto3-sagemaker](https://img.shields.io/pypi/v/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -596,14 +564,15 @@
     AutoMLChannelTypeType,
     AutoMLJobObjectiveTypeType,
     AutoMLJobSecondaryStatusType,
     AutoMLJobStatusType,
     AutoMLMetricEnumType,
     AutoMLMetricExtendedEnumType,
     AutoMLModeType,
+    AutoMLProcessingUnitType,
     AutoMLS3DataTypeType,
     AutoMLSortByType,
     AutoMLSortOrderType,
     AwsManagedHumanLoopRequestSourceType,
     BatchStrategyType,
     BooleanOperatorType,
     CandidateSortByType,
@@ -1086,14 +1055,15 @@
     DescribeActionRequestRequestTypeDef,
     DescribeAlgorithmInputRequestTypeDef,
     DescribeAppImageConfigRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeArtifactRequestRequestTypeDef,
     DescribeAutoMLJobRequestRequestTypeDef,
     ModelDeployResultTypeDef,
+    DescribeAutoMLJobV2RequestRequestTypeDef,
     DescribeCodeRepositoryInputRequestTypeDef,
     DescribeCompilationJobRequestRequestTypeDef,
     ModelArtifactsTypeDef,
     ModelDigestsTypeDef,
     DescribeContextRequestRequestTypeDef,
     DescribeDataQualityJobDefinitionRequestRequestTypeDef,
     DescribeDeviceFleetRequestRequestTypeDef,
@@ -1409,14 +1379,15 @@
     AssociateTrialComponentResponseTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
+    CreateAutoMLJobV2ResponseTypeDef,
     CreateCodeRepositoryOutputTypeDef,
     CreateCompilationJobResponseTypeDef,
     CreateContextResponseTypeDef,
     CreateDataQualityJobDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEdgeDeploymentPlanResponseTypeDef,
     CreateEndpointConfigOutputTypeDef,
@@ -1525,14 +1496,16 @@
     AlgorithmStatusDetailsTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAppsResponseTypeDef,
     ArtifactSourceTypeDef,
     AsyncInferenceOutputConfigTypeDef,
     AutoMLCandidateGenerationConfigTypeDef,
     AutoMLDataSourceTypeDef,
+    ImageClassificationJobConfigTypeDef,
+    TextClassificationJobConfigTypeDef,
     ResolvedAttributesTypeDef,
     AutoMLJobSummaryTypeDef,
     AutoMLSecurityConfigTypeDef,
     LabelingJobResourceConfigTypeDef,
     MonitoringNetworkConfigTypeDef,
     NetworkConfigTypeDef,
     BiasTypeDef,
@@ -1803,14 +1776,16 @@
     WorkforceTypeDef,
     ListActionsResponseTypeDef,
     ArtifactSummaryTypeDef,
     CreateArtifactRequestRequestTypeDef,
     DeleteArtifactRequestRequestTypeDef,
     AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
+    AutoMLJobChannelTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
     ListAutoMLJobsResponseTypeDef,
     AutoMLJobConfigTypeDef,
     LabelingJobAlgorithmsConfigTypeDef,
     ModelMetricsTypeDef,
     PipelineExecutionStepMetadataTypeDef,
     AutoMLCandidateTypeDef,
     BlueGreenUpdatePolicyTypeDef,
@@ -1897,17 +1872,19 @@
     HumanTaskConfigTypeDef,
     AlgorithmSpecificationTypeDef,
     TransformInputTypeDef,
     DescribeWorkforceResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     ListArtifactsResponseTypeDef,
+    CreateAutoMLJobV2RequestRequestTypeDef,
     CreateAutoMLJobRequestRequestTypeDef,
     PipelineExecutionStepTypeDef,
     DescribeAutoMLJobResponseTypeDef,
+    DescribeAutoMLJobV2ResponseTypeDef,
     ListCandidatesForAutoMLJobResponseTypeDef,
     DeploymentConfigTypeDef,
     RecommendationJobInputConfigTypeDef,
     ExplainerConfigTypeDef,
     CreateSpaceRequestRequestTypeDef,
     DescribeSpaceResponseTypeDef,
     UpdateSpaceRequestRequestTypeDef,
@@ -2012,42 +1989,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sagemaker-1.26.88/README.md` & `mypy-boto3-sagemaker-1.26.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sagemaker
+Version: 1.26.98
+Summary: Type annotations for boto3.SageMaker 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sagemaker type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-sagemaker"></a>
 
 # mypy-boto3-sagemaker
 
 [![PyPI - mypy-boto3-sagemaker](https://img.shields.io/pypi/v/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -564,14 +596,15 @@
     AutoMLChannelTypeType,
     AutoMLJobObjectiveTypeType,
     AutoMLJobSecondaryStatusType,
     AutoMLJobStatusType,
     AutoMLMetricEnumType,
     AutoMLMetricExtendedEnumType,
     AutoMLModeType,
+    AutoMLProcessingUnitType,
     AutoMLS3DataTypeType,
     AutoMLSortByType,
     AutoMLSortOrderType,
     AwsManagedHumanLoopRequestSourceType,
     BatchStrategyType,
     BooleanOperatorType,
     CandidateSortByType,
@@ -1054,14 +1087,15 @@
     DescribeActionRequestRequestTypeDef,
     DescribeAlgorithmInputRequestTypeDef,
     DescribeAppImageConfigRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeArtifactRequestRequestTypeDef,
     DescribeAutoMLJobRequestRequestTypeDef,
     ModelDeployResultTypeDef,
+    DescribeAutoMLJobV2RequestRequestTypeDef,
     DescribeCodeRepositoryInputRequestTypeDef,
     DescribeCompilationJobRequestRequestTypeDef,
     ModelArtifactsTypeDef,
     ModelDigestsTypeDef,
     DescribeContextRequestRequestTypeDef,
     DescribeDataQualityJobDefinitionRequestRequestTypeDef,
     DescribeDeviceFleetRequestRequestTypeDef,
@@ -1377,14 +1411,15 @@
     AssociateTrialComponentResponseTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
+    CreateAutoMLJobV2ResponseTypeDef,
     CreateCodeRepositoryOutputTypeDef,
     CreateCompilationJobResponseTypeDef,
     CreateContextResponseTypeDef,
     CreateDataQualityJobDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEdgeDeploymentPlanResponseTypeDef,
     CreateEndpointConfigOutputTypeDef,
@@ -1493,14 +1528,16 @@
     AlgorithmStatusDetailsTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAppsResponseTypeDef,
     ArtifactSourceTypeDef,
     AsyncInferenceOutputConfigTypeDef,
     AutoMLCandidateGenerationConfigTypeDef,
     AutoMLDataSourceTypeDef,
+    ImageClassificationJobConfigTypeDef,
+    TextClassificationJobConfigTypeDef,
     ResolvedAttributesTypeDef,
     AutoMLJobSummaryTypeDef,
     AutoMLSecurityConfigTypeDef,
     LabelingJobResourceConfigTypeDef,
     MonitoringNetworkConfigTypeDef,
     NetworkConfigTypeDef,
     BiasTypeDef,
@@ -1771,14 +1808,16 @@
     WorkforceTypeDef,
     ListActionsResponseTypeDef,
     ArtifactSummaryTypeDef,
     CreateArtifactRequestRequestTypeDef,
     DeleteArtifactRequestRequestTypeDef,
     AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
+    AutoMLJobChannelTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
     ListAutoMLJobsResponseTypeDef,
     AutoMLJobConfigTypeDef,
     LabelingJobAlgorithmsConfigTypeDef,
     ModelMetricsTypeDef,
     PipelineExecutionStepMetadataTypeDef,
     AutoMLCandidateTypeDef,
     BlueGreenUpdatePolicyTypeDef,
@@ -1865,17 +1904,19 @@
     HumanTaskConfigTypeDef,
     AlgorithmSpecificationTypeDef,
     TransformInputTypeDef,
     DescribeWorkforceResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     ListArtifactsResponseTypeDef,
+    CreateAutoMLJobV2RequestRequestTypeDef,
     CreateAutoMLJobRequestRequestTypeDef,
     PipelineExecutionStepTypeDef,
     DescribeAutoMLJobResponseTypeDef,
+    DescribeAutoMLJobV2ResponseTypeDef,
     ListCandidatesForAutoMLJobResponseTypeDef,
     DeploymentConfigTypeDef,
     RecommendationJobInputConfigTypeDef,
     ExplainerConfigTypeDef,
     CreateSpaceRequestRequestTypeDef,
     DescribeSpaceResponseTypeDef,
     UpdateSpaceRequestRequestTypeDef,
@@ -1980,42 +2021,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/__init__.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/__init__.pyi` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/__main__.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMaker 1.26.88\nVersion:         1.26.88\nBuilder version:"
-        " 7.12.5\nDocs:           "
+        "Type annotations for boto3.SageMaker 1.26.98\nVersion:         1.26.98\nBuilder version:"
+        " 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.88")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/client.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,30 +205,35 @@
     AlgorithmSpecificationTypeDef,
     AlgorithmValidationSpecificationTypeDef,
     AppSpecificationTypeDef,
     ArtifactSourceTypeDef,
     AssociateTrialComponentResponseTypeDef,
     AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
+    AutoMLDataSplitConfigTypeDef,
+    AutoMLJobChannelTypeDef,
     AutoMLJobConfigTypeDef,
     AutoMLJobObjectiveTypeDef,
     AutoMLOutputDataConfigTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
+    AutoMLSecurityConfigTypeDef,
     BatchDataCaptureConfigTypeDef,
     BatchDescribeModelPackageOutputTypeDef,
     ChannelTypeDef,
     CheckpointConfigTypeDef,
     CognitoConfigTypeDef,
     ContainerDefinitionTypeDef,
     ContextSourceTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
+    CreateAutoMLJobV2ResponseTypeDef,
     CreateCodeRepositoryOutputTypeDef,
     CreateCompilationJobResponseTypeDef,
     CreateContextResponseTypeDef,
     CreateDataQualityJobDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEdgeDeploymentPlanResponseTypeDef,
     CreateEndpointConfigOutputTypeDef,
@@ -291,14 +296,15 @@
     DeploymentStageTypeDef,
     DescribeActionResponseTypeDef,
     DescribeAlgorithmOutputTypeDef,
     DescribeAppImageConfigResponseTypeDef,
     DescribeAppResponseTypeDef,
     DescribeArtifactResponseTypeDef,
     DescribeAutoMLJobResponseTypeDef,
+    DescribeAutoMLJobV2ResponseTypeDef,
     DescribeCodeRepositoryOutputTypeDef,
     DescribeCompilationJobResponseTypeDef,
     DescribeContextResponseTypeDef,
     DescribeDataQualityJobDefinitionResponseTypeDef,
     DescribeDeviceFleetResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     DescribeDomainResponseTypeDef,
@@ -794,14 +800,36 @@
         """
         Creates an Autopilot job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_auto_ml_job)
         """
 
+    def create_auto_ml_job_v2(
+        self,
+        *,
+        AutoMLJobName: str,
+        AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],
+        OutputDataConfig: AutoMLOutputDataConfigTypeDef,
+        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
+        RoleArn: str,
+        Tags: Sequence[TagTypeDef] = ...,
+        SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
+        AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
+        ModelDeployConfig: ModelDeployConfigTypeDef = ...,
+        DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...
+    ) -> CreateAutoMLJobV2ResponseTypeDef:
+        """
+        Creates an Amazon SageMaker AutoML job that uses non-tabular data such as images
+        or text for Computer Vision or Natural Language Processing problems.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_auto_ml_job_v2)
+        """
+
     def create_code_repository(
         self,
         *,
         CodeRepositoryName: str,
         GitConfig: GitConfigTypeDef,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateCodeRepositoryOutputTypeDef:
@@ -1608,15 +1636,15 @@
         Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,
         InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateTrialComponentResponseTypeDef:
         """
-        Creates a *trial component* , which is a stage of a machine learning *trial*.
+        Creates a *trial component*, which is a stage of a machine learning *trial*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_trial_component)
         """
 
     def create_user_profile(
         self,
@@ -2149,14 +2177,22 @@
         """
         Returns information about an Amazon SageMaker AutoML job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_auto_ml_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_auto_ml_job)
         """
 
+    def describe_auto_ml_job_v2(self, *, AutoMLJobName: str) -> DescribeAutoMLJobV2ResponseTypeDef:
+        """
+        Returns information about an Amazon SageMaker AutoML V2 job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_auto_ml_job_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_auto_ml_job_v2)
+        """
+
     def describe_code_repository(
         self, *, CodeRepositoryName: str
     ) -> DescribeCodeRepositoryOutputTypeDef:
         """
         Gets details about the specified Git repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_code_repository)
@@ -2620,15 +2656,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_user_profile)
         """
 
     def describe_workforce(self, *, WorkforceName: str) -> DescribeWorkforceResponseTypeDef:
         """
         Lists private workforce information, including workforce name, Amazon Resource
         Name (ARN), and, if applicable, allowed IP address ranges (
-        [CIDRs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)_ ).
+        [CIDRs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)_).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_workforce)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_workforce)
         """
 
     def describe_workteam(self, *, WorkteamName: str) -> DescribeWorkteamResponseTypeDef:
         """
@@ -3155,15 +3191,15 @@
         CreationTimeBefore: Union[datetime, str] = ...,
         SortOrder: FeatureGroupSortOrderType = ...,
         SortBy: FeatureGroupSortByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFeatureGroupsResponseTypeDef:
         """
-        List `FeatureGroup` s based on given filter and order.
+        List `FeatureGroup`s based on given filter and order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_feature_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#list_feature_groups)
         """
 
     def list_flow_definitions(
         self,
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/client.pyi` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -205,30 +205,35 @@
     AlgorithmSpecificationTypeDef,
     AlgorithmValidationSpecificationTypeDef,
     AppSpecificationTypeDef,
     ArtifactSourceTypeDef,
     AssociateTrialComponentResponseTypeDef,
     AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
+    AutoMLDataSplitConfigTypeDef,
+    AutoMLJobChannelTypeDef,
     AutoMLJobConfigTypeDef,
     AutoMLJobObjectiveTypeDef,
     AutoMLOutputDataConfigTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
+    AutoMLSecurityConfigTypeDef,
     BatchDataCaptureConfigTypeDef,
     BatchDescribeModelPackageOutputTypeDef,
     ChannelTypeDef,
     CheckpointConfigTypeDef,
     CognitoConfigTypeDef,
     ContainerDefinitionTypeDef,
     ContextSourceTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
+    CreateAutoMLJobV2ResponseTypeDef,
     CreateCodeRepositoryOutputTypeDef,
     CreateCompilationJobResponseTypeDef,
     CreateContextResponseTypeDef,
     CreateDataQualityJobDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEdgeDeploymentPlanResponseTypeDef,
     CreateEndpointConfigOutputTypeDef,
@@ -291,14 +296,15 @@
     DeploymentStageTypeDef,
     DescribeActionResponseTypeDef,
     DescribeAlgorithmOutputTypeDef,
     DescribeAppImageConfigResponseTypeDef,
     DescribeAppResponseTypeDef,
     DescribeArtifactResponseTypeDef,
     DescribeAutoMLJobResponseTypeDef,
+    DescribeAutoMLJobV2ResponseTypeDef,
     DescribeCodeRepositoryOutputTypeDef,
     DescribeCompilationJobResponseTypeDef,
     DescribeContextResponseTypeDef,
     DescribeDataQualityJobDefinitionResponseTypeDef,
     DescribeDeviceFleetResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     DescribeDomainResponseTypeDef,
@@ -777,14 +783,35 @@
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_auto_ml_job)
         """
+    def create_auto_ml_job_v2(
+        self,
+        *,
+        AutoMLJobName: str,
+        AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],
+        OutputDataConfig: AutoMLOutputDataConfigTypeDef,
+        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
+        RoleArn: str,
+        Tags: Sequence[TagTypeDef] = ...,
+        SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
+        AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
+        ModelDeployConfig: ModelDeployConfigTypeDef = ...,
+        DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...
+    ) -> CreateAutoMLJobV2ResponseTypeDef:
+        """
+        Creates an Amazon SageMaker AutoML job that uses non-tabular data such as images
+        or text for Computer Vision or Natural Language Processing problems.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_auto_ml_job_v2)
+        """
     def create_code_repository(
         self,
         *,
         CodeRepositoryName: str,
         GitConfig: GitConfigTypeDef,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateCodeRepositoryOutputTypeDef:
@@ -1548,15 +1575,15 @@
         Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,
         InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateTrialComponentResponseTypeDef:
         """
-        Creates a *trial component* , which is a stage of a machine learning *trial*.
+        Creates a *trial component*, which is a stage of a machine learning *trial*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#create_trial_component)
         """
     def create_user_profile(
         self,
         *,
@@ -2033,14 +2060,21 @@
     def describe_auto_ml_job(self, *, AutoMLJobName: str) -> DescribeAutoMLJobResponseTypeDef:
         """
         Returns information about an Amazon SageMaker AutoML job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_auto_ml_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_auto_ml_job)
         """
+    def describe_auto_ml_job_v2(self, *, AutoMLJobName: str) -> DescribeAutoMLJobV2ResponseTypeDef:
+        """
+        Returns information about an Amazon SageMaker AutoML V2 job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_auto_ml_job_v2)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_auto_ml_job_v2)
+        """
     def describe_code_repository(
         self, *, CodeRepositoryName: str
     ) -> DescribeCodeRepositoryOutputTypeDef:
         """
         Gets details about the specified Git repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_code_repository)
@@ -2455,15 +2489,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_user_profile)
         """
     def describe_workforce(self, *, WorkforceName: str) -> DescribeWorkforceResponseTypeDef:
         """
         Lists private workforce information, including workforce name, Amazon Resource
         Name (ARN), and, if applicable, allowed IP address ranges (
-        [CIDRs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)_ ).
+        [CIDRs](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)_).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_workforce)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#describe_workforce)
         """
     def describe_workteam(self, *, WorkteamName: str) -> DescribeWorkteamResponseTypeDef:
         """
         Gets information about a specific work team.
@@ -2957,15 +2991,15 @@
         CreationTimeBefore: Union[datetime, str] = ...,
         SortOrder: FeatureGroupSortOrderType = ...,
         SortBy: FeatureGroupSortByType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFeatureGroupsResponseTypeDef:
         """
-        List `FeatureGroup` s based on given filter and order.
+        List `FeatureGroup`s based on given filter and order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_feature_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/client/#list_feature_groups)
         """
     def list_flow_definitions(
         self,
         *,
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/literals.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "AutoMLChannelTypeType",
     "AutoMLJobObjectiveTypeType",
     "AutoMLJobSecondaryStatusType",
     "AutoMLJobStatusType",
     "AutoMLMetricEnumType",
     "AutoMLMetricExtendedEnumType",
     "AutoMLModeType",
+    "AutoMLProcessingUnitType",
     "AutoMLS3DataTypeType",
     "AutoMLSortByType",
     "AutoMLSortOrderType",
     "AwsManagedHumanLoopRequestSourceType",
     "BatchStrategyType",
     "BooleanOperatorType",
     "CandidateSortByType",
@@ -363,14 +364,15 @@
     "ml.g5.16xlarge",
     "ml.g5.24xlarge",
     "ml.g5.2xlarge",
     "ml.g5.48xlarge",
     "ml.g5.4xlarge",
     "ml.g5.8xlarge",
     "ml.g5.xlarge",
+    "ml.geospatial.interactive",
     "ml.m5.12xlarge",
     "ml.m5.16xlarge",
     "ml.m5.24xlarge",
     "ml.m5.2xlarge",
     "ml.m5.4xlarge",
     "ml.m5.8xlarge",
     "ml.m5.large",
@@ -443,14 +445,15 @@
     "MaxCandidatesReached",
     "ModelDeploymentError",
     "ModelInsightsError",
     "ModelTuning",
     "Starting",
     "Stopped",
     "Stopping",
+    "TrainingModels",
 ]
 AutoMLJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 AutoMLMetricEnumType = Literal[
     "AUC",
     "Accuracy",
     "BalancedAccuracy",
     "F1",
@@ -478,15 +481,16 @@
     "PrecisionMacro",
     "R2",
     "RMSE",
     "Recall",
     "RecallMacro",
 ]
 AutoMLModeType = Literal["AUTO", "ENSEMBLING", "HYPERPARAMETER_TUNING"]
-AutoMLS3DataTypeType = Literal["ManifestFile", "S3Prefix"]
+AutoMLProcessingUnitType = Literal["CPU", "GPU"]
+AutoMLS3DataTypeType = Literal["AugmentedManifestFile", "ManifestFile", "S3Prefix"]
 AutoMLSortByType = Literal["CreationTime", "Name", "Status"]
 AutoMLSortOrderType = Literal["Ascending", "Descending"]
 AwsManagedHumanLoopRequestSourceType = Literal[
     "AWS/Rekognition/DetectModerationLabels/Image/V3", "AWS/Textract/AnalyzeDocument/Forms/V1"
 ]
 BatchStrategyType = Literal["MultiRecord", "SingleRecord"]
 BooleanOperatorType = Literal["And", "Or"]
@@ -1521,14 +1525,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -1806,14 +1811,15 @@
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/literals.pyi` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "AutoMLChannelTypeType",
     "AutoMLJobObjectiveTypeType",
     "AutoMLJobSecondaryStatusType",
     "AutoMLJobStatusType",
     "AutoMLMetricEnumType",
     "AutoMLMetricExtendedEnumType",
     "AutoMLModeType",
+    "AutoMLProcessingUnitType",
     "AutoMLS3DataTypeType",
     "AutoMLSortByType",
     "AutoMLSortOrderType",
     "AwsManagedHumanLoopRequestSourceType",
     "BatchStrategyType",
     "BooleanOperatorType",
     "CandidateSortByType",
@@ -361,14 +362,15 @@
     "ml.g5.16xlarge",
     "ml.g5.24xlarge",
     "ml.g5.2xlarge",
     "ml.g5.48xlarge",
     "ml.g5.4xlarge",
     "ml.g5.8xlarge",
     "ml.g5.xlarge",
+    "ml.geospatial.interactive",
     "ml.m5.12xlarge",
     "ml.m5.16xlarge",
     "ml.m5.24xlarge",
     "ml.m5.2xlarge",
     "ml.m5.4xlarge",
     "ml.m5.8xlarge",
     "ml.m5.large",
@@ -441,14 +443,15 @@
     "MaxCandidatesReached",
     "ModelDeploymentError",
     "ModelInsightsError",
     "ModelTuning",
     "Starting",
     "Stopped",
     "Stopping",
+    "TrainingModels",
 ]
 AutoMLJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 AutoMLMetricEnumType = Literal[
     "AUC",
     "Accuracy",
     "BalancedAccuracy",
     "F1",
@@ -476,15 +479,16 @@
     "PrecisionMacro",
     "R2",
     "RMSE",
     "Recall",
     "RecallMacro",
 ]
 AutoMLModeType = Literal["AUTO", "ENSEMBLING", "HYPERPARAMETER_TUNING"]
-AutoMLS3DataTypeType = Literal["ManifestFile", "S3Prefix"]
+AutoMLProcessingUnitType = Literal["CPU", "GPU"]
+AutoMLS3DataTypeType = Literal["AugmentedManifestFile", "ManifestFile", "S3Prefix"]
 AutoMLSortByType = Literal["CreationTime", "Name", "Status"]
 AutoMLSortOrderType = Literal["Ascending", "Descending"]
 AwsManagedHumanLoopRequestSourceType = Literal[
     "AWS/Rekognition/DetectModerationLabels/Image/V3", "AWS/Textract/AnalyzeDocument/Forms/V1"
 ]
 BatchStrategyType = Literal["MultiRecord", "SingleRecord"]
 BooleanOperatorType = Literal["And", "Or"]
@@ -1519,14 +1523,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -1804,14 +1809,15 @@
     "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/paginator.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/paginator.pyi` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/type_defs.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     AutoMLChannelTypeType,
     AutoMLJobObjectiveTypeType,
     AutoMLJobSecondaryStatusType,
     AutoMLJobStatusType,
     AutoMLMetricEnumType,
     AutoMLMetricExtendedEnumType,
     AutoMLModeType,
+    AutoMLProcessingUnitType,
     AutoMLS3DataTypeType,
     AutoMLSortByType,
     AutoMLSortOrderType,
     AwsManagedHumanLoopRequestSourceType,
     BatchStrategyType,
     BooleanOperatorType,
     CandidateSortByType,
@@ -425,14 +426,15 @@
     "DescribeActionRequestRequestTypeDef",
     "DescribeAlgorithmInputRequestTypeDef",
     "DescribeAppImageConfigRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeArtifactRequestRequestTypeDef",
     "DescribeAutoMLJobRequestRequestTypeDef",
     "ModelDeployResultTypeDef",
+    "DescribeAutoMLJobV2RequestRequestTypeDef",
     "DescribeCodeRepositoryInputRequestTypeDef",
     "DescribeCompilationJobRequestRequestTypeDef",
     "ModelArtifactsTypeDef",
     "ModelDigestsTypeDef",
     "DescribeContextRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDeviceFleetRequestRequestTypeDef",
@@ -748,14 +750,15 @@
     "AssociateTrialComponentResponseTypeDef",
     "CreateActionResponseTypeDef",
     "CreateAlgorithmOutputTypeDef",
     "CreateAppImageConfigResponseTypeDef",
     "CreateAppResponseTypeDef",
     "CreateArtifactResponseTypeDef",
     "CreateAutoMLJobResponseTypeDef",
+    "CreateAutoMLJobV2ResponseTypeDef",
     "CreateCodeRepositoryOutputTypeDef",
     "CreateCompilationJobResponseTypeDef",
     "CreateContextResponseTypeDef",
     "CreateDataQualityJobDefinitionResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateEdgeDeploymentPlanResponseTypeDef",
     "CreateEndpointConfigOutputTypeDef",
@@ -864,14 +867,16 @@
     "AlgorithmStatusDetailsTypeDef",
     "ListAlgorithmsOutputTypeDef",
     "ListAppsResponseTypeDef",
     "ArtifactSourceTypeDef",
     "AsyncInferenceOutputConfigTypeDef",
     "AutoMLCandidateGenerationConfigTypeDef",
     "AutoMLDataSourceTypeDef",
+    "ImageClassificationJobConfigTypeDef",
+    "TextClassificationJobConfigTypeDef",
     "ResolvedAttributesTypeDef",
     "AutoMLJobSummaryTypeDef",
     "AutoMLSecurityConfigTypeDef",
     "LabelingJobResourceConfigTypeDef",
     "MonitoringNetworkConfigTypeDef",
     "NetworkConfigTypeDef",
     "BiasTypeDef",
@@ -1142,14 +1147,16 @@
     "WorkforceTypeDef",
     "ListActionsResponseTypeDef",
     "ArtifactSummaryTypeDef",
     "CreateArtifactRequestRequestTypeDef",
     "DeleteArtifactRequestRequestTypeDef",
     "AsyncInferenceConfigTypeDef",
     "AutoMLChannelTypeDef",
+    "AutoMLJobChannelTypeDef",
+    "AutoMLProblemTypeConfigTypeDef",
     "ListAutoMLJobsResponseTypeDef",
     "AutoMLJobConfigTypeDef",
     "LabelingJobAlgorithmsConfigTypeDef",
     "ModelMetricsTypeDef",
     "PipelineExecutionStepMetadataTypeDef",
     "AutoMLCandidateTypeDef",
     "BlueGreenUpdatePolicyTypeDef",
@@ -1236,17 +1243,19 @@
     "HumanTaskConfigTypeDef",
     "AlgorithmSpecificationTypeDef",
     "TransformInputTypeDef",
     "DescribeWorkforceResponseTypeDef",
     "ListWorkforcesResponseTypeDef",
     "UpdateWorkforceResponseTypeDef",
     "ListArtifactsResponseTypeDef",
+    "CreateAutoMLJobV2RequestRequestTypeDef",
     "CreateAutoMLJobRequestRequestTypeDef",
     "PipelineExecutionStepTypeDef",
     "DescribeAutoMLJobResponseTypeDef",
+    "DescribeAutoMLJobV2ResponseTypeDef",
     "ListCandidatesForAutoMLJobResponseTypeDef",
     "DeploymentConfigTypeDef",
     "RecommendationJobInputConfigTypeDef",
     "ExplainerConfigTypeDef",
     "CreateSpaceRequestRequestTypeDef",
     "DescribeSpaceResponseTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
@@ -3497,14 +3506,21 @@
     "ModelDeployResultTypeDef",
     {
         "EndpointName": str,
     },
     total=False,
 )
 
+DescribeAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "DescribeAutoMLJobV2RequestRequestTypeDef",
+    {
+        "AutoMLJobName": str,
+    },
+)
+
 DescribeCodeRepositoryInputRequestTypeDef = TypedDict(
     "DescribeCodeRepositoryInputRequestTypeDef",
     {
         "CodeRepositoryName": str,
     },
 )
 
@@ -7921,14 +7937,22 @@
     "CreateAutoMLJobResponseTypeDef",
     {
         "AutoMLJobArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAutoMLJobV2ResponseTypeDef = TypedDict(
+    "CreateAutoMLJobV2ResponseTypeDef",
+    {
+        "AutoMLJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCodeRepositoryOutputTypeDef = TypedDict(
     "CreateCodeRepositoryOutputTypeDef",
     {
         "CodeRepositoryArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9014,14 +9038,32 @@
 AutoMLDataSourceTypeDef = TypedDict(
     "AutoMLDataSourceTypeDef",
     {
         "S3DataSource": AutoMLS3DataSourceTypeDef,
     },
 )
 
+ImageClassificationJobConfigTypeDef = TypedDict(
+    "ImageClassificationJobConfigTypeDef",
+    {
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+    },
+    total=False,
+)
+
+TextClassificationJobConfigTypeDef = TypedDict(
+    "TextClassificationJobConfigTypeDef",
+    {
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+        "ContentColumn": str,
+        "TargetLabelColumn": str,
+    },
+    total=False,
+)
+
 ResolvedAttributesTypeDef = TypedDict(
     "ResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
@@ -13394,14 +13436,34 @@
 )
 
 
 class AutoMLChannelTypeDef(_RequiredAutoMLChannelTypeDef, _OptionalAutoMLChannelTypeDef):
     pass
 
 
+AutoMLJobChannelTypeDef = TypedDict(
+    "AutoMLJobChannelTypeDef",
+    {
+        "ChannelType": AutoMLChannelTypeType,
+        "ContentType": str,
+        "CompressionType": CompressionTypeType,
+        "DataSource": AutoMLDataSourceTypeDef,
+    },
+    total=False,
+)
+
+AutoMLProblemTypeConfigTypeDef = TypedDict(
+    "AutoMLProblemTypeConfigTypeDef",
+    {
+        "ImageClassificationJobConfig": ImageClassificationJobConfigTypeDef,
+        "TextClassificationJobConfig": TextClassificationJobConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAutoMLJobsResponseTypeDef = TypedDict(
     "ListAutoMLJobsResponseTypeDef",
     {
         "AutoMLJobSummaries": List[AutoMLJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -13488,14 +13550,17 @@
     "_OptionalAutoMLCandidateTypeDef",
     {
         "FinalAutoMLJobObjectiveMetric": FinalAutoMLJobObjectiveMetricTypeDef,
         "InferenceContainers": List[AutoMLContainerDefinitionTypeDef],
         "EndTime": datetime,
         "FailureReason": str,
         "CandidateProperties": CandidatePropertiesTypeDef,
+        "InferenceContainerDefinitions": Dict[
+            AutoMLProcessingUnitType, List[AutoMLContainerDefinitionTypeDef]
+        ],
     },
     total=False,
 )
 
 
 class AutoMLCandidateTypeDef(_RequiredAutoMLCandidateTypeDef, _OptionalAutoMLCandidateTypeDef):
     pass
@@ -15040,14 +15105,43 @@
     {
         "ArtifactSummaries": List[ArtifactSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutoMLJobV2RequestRequestTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutoMLJobV2RequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
+        "ModelDeployConfig": ModelDeployConfigTypeDef,
+        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAutoMLJobV2RequestRequestTypeDef(
+    _RequiredCreateAutoMLJobV2RequestRequestTypeDef, _OptionalCreateAutoMLJobV2RequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAutoMLJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobRequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "InputDataConfig": Sequence[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
@@ -15114,14 +15208,40 @@
         "ResolvedAttributes": ResolvedAttributesTypeDef,
         "ModelDeployConfig": ModelDeployConfigTypeDef,
         "ModelDeployResult": ModelDeployResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
+    "DescribeAutoMLJobV2ResponseTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobArn": str,
+        "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "RoleArn": str,
+        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
+        "BestCandidate": AutoMLCandidateTypeDef,
+        "AutoMLJobStatus": AutoMLJobStatusType,
+        "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
+        "ModelDeployConfig": ModelDeployConfigTypeDef,
+        "ModelDeployResult": ModelDeployResultTypeDef,
+        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
+        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCandidatesForAutoMLJobResponseTypeDef = TypedDict(
     "ListCandidatesForAutoMLJobResponseTypeDef",
     {
         "Candidates": List[AutoMLCandidateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/type_defs.pyi` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     AutoMLChannelTypeType,
     AutoMLJobObjectiveTypeType,
     AutoMLJobSecondaryStatusType,
     AutoMLJobStatusType,
     AutoMLMetricEnumType,
     AutoMLMetricExtendedEnumType,
     AutoMLModeType,
+    AutoMLProcessingUnitType,
     AutoMLS3DataTypeType,
     AutoMLSortByType,
     AutoMLSortOrderType,
     AwsManagedHumanLoopRequestSourceType,
     BatchStrategyType,
     BooleanOperatorType,
     CandidateSortByType,
@@ -424,14 +425,15 @@
     "DescribeActionRequestRequestTypeDef",
     "DescribeAlgorithmInputRequestTypeDef",
     "DescribeAppImageConfigRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeArtifactRequestRequestTypeDef",
     "DescribeAutoMLJobRequestRequestTypeDef",
     "ModelDeployResultTypeDef",
+    "DescribeAutoMLJobV2RequestRequestTypeDef",
     "DescribeCodeRepositoryInputRequestTypeDef",
     "DescribeCompilationJobRequestRequestTypeDef",
     "ModelArtifactsTypeDef",
     "ModelDigestsTypeDef",
     "DescribeContextRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDeviceFleetRequestRequestTypeDef",
@@ -747,14 +749,15 @@
     "AssociateTrialComponentResponseTypeDef",
     "CreateActionResponseTypeDef",
     "CreateAlgorithmOutputTypeDef",
     "CreateAppImageConfigResponseTypeDef",
     "CreateAppResponseTypeDef",
     "CreateArtifactResponseTypeDef",
     "CreateAutoMLJobResponseTypeDef",
+    "CreateAutoMLJobV2ResponseTypeDef",
     "CreateCodeRepositoryOutputTypeDef",
     "CreateCompilationJobResponseTypeDef",
     "CreateContextResponseTypeDef",
     "CreateDataQualityJobDefinitionResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateEdgeDeploymentPlanResponseTypeDef",
     "CreateEndpointConfigOutputTypeDef",
@@ -863,14 +866,16 @@
     "AlgorithmStatusDetailsTypeDef",
     "ListAlgorithmsOutputTypeDef",
     "ListAppsResponseTypeDef",
     "ArtifactSourceTypeDef",
     "AsyncInferenceOutputConfigTypeDef",
     "AutoMLCandidateGenerationConfigTypeDef",
     "AutoMLDataSourceTypeDef",
+    "ImageClassificationJobConfigTypeDef",
+    "TextClassificationJobConfigTypeDef",
     "ResolvedAttributesTypeDef",
     "AutoMLJobSummaryTypeDef",
     "AutoMLSecurityConfigTypeDef",
     "LabelingJobResourceConfigTypeDef",
     "MonitoringNetworkConfigTypeDef",
     "NetworkConfigTypeDef",
     "BiasTypeDef",
@@ -1141,14 +1146,16 @@
     "WorkforceTypeDef",
     "ListActionsResponseTypeDef",
     "ArtifactSummaryTypeDef",
     "CreateArtifactRequestRequestTypeDef",
     "DeleteArtifactRequestRequestTypeDef",
     "AsyncInferenceConfigTypeDef",
     "AutoMLChannelTypeDef",
+    "AutoMLJobChannelTypeDef",
+    "AutoMLProblemTypeConfigTypeDef",
     "ListAutoMLJobsResponseTypeDef",
     "AutoMLJobConfigTypeDef",
     "LabelingJobAlgorithmsConfigTypeDef",
     "ModelMetricsTypeDef",
     "PipelineExecutionStepMetadataTypeDef",
     "AutoMLCandidateTypeDef",
     "BlueGreenUpdatePolicyTypeDef",
@@ -1235,17 +1242,19 @@
     "HumanTaskConfigTypeDef",
     "AlgorithmSpecificationTypeDef",
     "TransformInputTypeDef",
     "DescribeWorkforceResponseTypeDef",
     "ListWorkforcesResponseTypeDef",
     "UpdateWorkforceResponseTypeDef",
     "ListArtifactsResponseTypeDef",
+    "CreateAutoMLJobV2RequestRequestTypeDef",
     "CreateAutoMLJobRequestRequestTypeDef",
     "PipelineExecutionStepTypeDef",
     "DescribeAutoMLJobResponseTypeDef",
+    "DescribeAutoMLJobV2ResponseTypeDef",
     "ListCandidatesForAutoMLJobResponseTypeDef",
     "DeploymentConfigTypeDef",
     "RecommendationJobInputConfigTypeDef",
     "ExplainerConfigTypeDef",
     "CreateSpaceRequestRequestTypeDef",
     "DescribeSpaceResponseTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
@@ -3404,14 +3413,21 @@
     "ModelDeployResultTypeDef",
     {
         "EndpointName": str,
     },
     total=False,
 )
 
+DescribeAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "DescribeAutoMLJobV2RequestRequestTypeDef",
+    {
+        "AutoMLJobName": str,
+    },
+)
+
 DescribeCodeRepositoryInputRequestTypeDef = TypedDict(
     "DescribeCodeRepositoryInputRequestTypeDef",
     {
         "CodeRepositoryName": str,
     },
 )
 
@@ -7656,14 +7672,22 @@
     "CreateAutoMLJobResponseTypeDef",
     {
         "AutoMLJobArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateAutoMLJobV2ResponseTypeDef = TypedDict(
+    "CreateAutoMLJobV2ResponseTypeDef",
+    {
+        "AutoMLJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCodeRepositoryOutputTypeDef = TypedDict(
     "CreateCodeRepositoryOutputTypeDef",
     {
         "CodeRepositoryArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8733,14 +8757,32 @@
 AutoMLDataSourceTypeDef = TypedDict(
     "AutoMLDataSourceTypeDef",
     {
         "S3DataSource": AutoMLS3DataSourceTypeDef,
     },
 )
 
+ImageClassificationJobConfigTypeDef = TypedDict(
+    "ImageClassificationJobConfigTypeDef",
+    {
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+    },
+    total=False,
+)
+
+TextClassificationJobConfigTypeDef = TypedDict(
+    "TextClassificationJobConfigTypeDef",
+    {
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+        "ContentColumn": str,
+        "TargetLabelColumn": str,
+    },
+    total=False,
+)
+
 ResolvedAttributesTypeDef = TypedDict(
     "ResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
@@ -12925,14 +12967,34 @@
     },
     total=False,
 )
 
 class AutoMLChannelTypeDef(_RequiredAutoMLChannelTypeDef, _OptionalAutoMLChannelTypeDef):
     pass
 
+AutoMLJobChannelTypeDef = TypedDict(
+    "AutoMLJobChannelTypeDef",
+    {
+        "ChannelType": AutoMLChannelTypeType,
+        "ContentType": str,
+        "CompressionType": CompressionTypeType,
+        "DataSource": AutoMLDataSourceTypeDef,
+    },
+    total=False,
+)
+
+AutoMLProblemTypeConfigTypeDef = TypedDict(
+    "AutoMLProblemTypeConfigTypeDef",
+    {
+        "ImageClassificationJobConfig": ImageClassificationJobConfigTypeDef,
+        "TextClassificationJobConfig": TextClassificationJobConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAutoMLJobsResponseTypeDef = TypedDict(
     "ListAutoMLJobsResponseTypeDef",
     {
         "AutoMLJobSummaries": List[AutoMLJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -13017,14 +13079,17 @@
     "_OptionalAutoMLCandidateTypeDef",
     {
         "FinalAutoMLJobObjectiveMetric": FinalAutoMLJobObjectiveMetricTypeDef,
         "InferenceContainers": List[AutoMLContainerDefinitionTypeDef],
         "EndTime": datetime,
         "FailureReason": str,
         "CandidateProperties": CandidatePropertiesTypeDef,
+        "InferenceContainerDefinitions": Dict[
+            AutoMLProcessingUnitType, List[AutoMLContainerDefinitionTypeDef]
+        ],
     },
     total=False,
 )
 
 class AutoMLCandidateTypeDef(_RequiredAutoMLCandidateTypeDef, _OptionalAutoMLCandidateTypeDef):
     pass
 
@@ -14505,14 +14570,41 @@
     {
         "ArtifactSummaries": List[ArtifactSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAutoMLJobV2RequestRequestTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAutoMLJobV2RequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
+        "ModelDeployConfig": ModelDeployConfigTypeDef,
+        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateAutoMLJobV2RequestRequestTypeDef(
+    _RequiredCreateAutoMLJobV2RequestRequestTypeDef, _OptionalCreateAutoMLJobV2RequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateAutoMLJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobRequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "InputDataConfig": Sequence[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
@@ -14577,14 +14669,40 @@
         "ResolvedAttributes": ResolvedAttributesTypeDef,
         "ModelDeployConfig": ModelDeployConfigTypeDef,
         "ModelDeployResult": ModelDeployResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
+    "DescribeAutoMLJobV2ResponseTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobArn": str,
+        "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "RoleArn": str,
+        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
+        "BestCandidate": AutoMLCandidateTypeDef,
+        "AutoMLJobStatus": AutoMLJobStatusType,
+        "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
+        "ModelDeployConfig": ModelDeployConfigTypeDef,
+        "ModelDeployResult": ModelDeployResultTypeDef,
+        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
+        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCandidatesForAutoMLJobResponseTypeDef = TypedDict(
     "ListCandidatesForAutoMLJobResponseTypeDef",
     {
         "Candidates": List[AutoMLCandidateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/waiter.py` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker/waiter.pyi` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.26.88
-Summary: Type annotations for boto3.SageMaker 1.26.88 service generated with mypy-boto3-builder 7.12.5
+Version: 1.26.98
+Summary: Type annotations for boto3.SageMaker 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-sagemaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -596,14 +596,15 @@
     AutoMLChannelTypeType,
     AutoMLJobObjectiveTypeType,
     AutoMLJobSecondaryStatusType,
     AutoMLJobStatusType,
     AutoMLMetricEnumType,
     AutoMLMetricExtendedEnumType,
     AutoMLModeType,
+    AutoMLProcessingUnitType,
     AutoMLS3DataTypeType,
     AutoMLSortByType,
     AutoMLSortOrderType,
     AwsManagedHumanLoopRequestSourceType,
     BatchStrategyType,
     BooleanOperatorType,
     CandidateSortByType,
@@ -1086,14 +1087,15 @@
     DescribeActionRequestRequestTypeDef,
     DescribeAlgorithmInputRequestTypeDef,
     DescribeAppImageConfigRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeArtifactRequestRequestTypeDef,
     DescribeAutoMLJobRequestRequestTypeDef,
     ModelDeployResultTypeDef,
+    DescribeAutoMLJobV2RequestRequestTypeDef,
     DescribeCodeRepositoryInputRequestTypeDef,
     DescribeCompilationJobRequestRequestTypeDef,
     ModelArtifactsTypeDef,
     ModelDigestsTypeDef,
     DescribeContextRequestRequestTypeDef,
     DescribeDataQualityJobDefinitionRequestRequestTypeDef,
     DescribeDeviceFleetRequestRequestTypeDef,
@@ -1409,14 +1411,15 @@
     AssociateTrialComponentResponseTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
+    CreateAutoMLJobV2ResponseTypeDef,
     CreateCodeRepositoryOutputTypeDef,
     CreateCompilationJobResponseTypeDef,
     CreateContextResponseTypeDef,
     CreateDataQualityJobDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEdgeDeploymentPlanResponseTypeDef,
     CreateEndpointConfigOutputTypeDef,
@@ -1525,14 +1528,16 @@
     AlgorithmStatusDetailsTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAppsResponseTypeDef,
     ArtifactSourceTypeDef,
     AsyncInferenceOutputConfigTypeDef,
     AutoMLCandidateGenerationConfigTypeDef,
     AutoMLDataSourceTypeDef,
+    ImageClassificationJobConfigTypeDef,
+    TextClassificationJobConfigTypeDef,
     ResolvedAttributesTypeDef,
     AutoMLJobSummaryTypeDef,
     AutoMLSecurityConfigTypeDef,
     LabelingJobResourceConfigTypeDef,
     MonitoringNetworkConfigTypeDef,
     NetworkConfigTypeDef,
     BiasTypeDef,
@@ -1803,14 +1808,16 @@
     WorkforceTypeDef,
     ListActionsResponseTypeDef,
     ArtifactSummaryTypeDef,
     CreateArtifactRequestRequestTypeDef,
     DeleteArtifactRequestRequestTypeDef,
     AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
+    AutoMLJobChannelTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
     ListAutoMLJobsResponseTypeDef,
     AutoMLJobConfigTypeDef,
     LabelingJobAlgorithmsConfigTypeDef,
     ModelMetricsTypeDef,
     PipelineExecutionStepMetadataTypeDef,
     AutoMLCandidateTypeDef,
     BlueGreenUpdatePolicyTypeDef,
@@ -1897,17 +1904,19 @@
     HumanTaskConfigTypeDef,
     AlgorithmSpecificationTypeDef,
     TransformInputTypeDef,
     DescribeWorkforceResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     ListArtifactsResponseTypeDef,
+    CreateAutoMLJobV2RequestRequestTypeDef,
     CreateAutoMLJobRequestRequestTypeDef,
     PipelineExecutionStepTypeDef,
     DescribeAutoMLJobResponseTypeDef,
+    DescribeAutoMLJobV2ResponseTypeDef,
     ListCandidatesForAutoMLJobResponseTypeDef,
     DeploymentConfigTypeDef,
     RecommendationJobInputConfigTypeDef,
     ExplainerConfigTypeDef,
     CreateSpaceRequestRequestTypeDef,
     DescribeSpaceResponseTypeDef,
     UpdateSpaceRequestRequestTypeDef,
@@ -2012,42 +2021,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-sagemaker-1.26.88/mypy_boto3_sagemaker.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-1.26.98/mypy_boto3_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.26.88/setup.py` & `mypy-boto3-sagemaker-1.26.98/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-sagemaker.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker",
-    version="1.26.88",
+    version="1.26.98",
     packages=["mypy_boto3_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMaker 1.26.88 service generated with mypy-boto3-builder"
-        " 7.12.5"
+        "Type annotations for boto3.SageMaker 1.26.98 service generated with mypy-boto3-builder"
+        " 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

