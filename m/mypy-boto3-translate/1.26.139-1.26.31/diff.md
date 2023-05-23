# Comparing `tmp/mypy-boto3-translate-1.26.139.tar.gz` & `tmp/mypy-boto3-translate-1.26.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-translate-1.26.139.tar", last modified: Tue May 23 21:04:52 2023, max compression
+gzip compressed data, was "mypy-boto3-translate-1.26.31.tar", last modified: Thu Dec 15 20:33:07 2022, max compression
```

## Comparing `mypy-boto3-translate-1.26.139.tar` & `mypy-boto3-translate-1.26.31.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:52.366521 mypy-boto3-translate-1.26.139/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-23 21:04:52.366521 mypy-boto3-translate-1.26.139/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:52.366521 mypy-boto3-translate-1.26.139/mypy_boto3_translate/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20101 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:04:52.366521 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-23 21:04:52.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-23 21:04:52.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:04:52.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:04:52.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 21:04:52.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 21:04:52.000000 mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:04:52.366521 mypy-boto3-translate-1.26.139/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 21:04:41.000000 mypy-boto3-translate-1.26.139/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13398 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/mypy_boto3_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15931 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2022-12-15 20:32:56.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2022-12-15 20:32:56.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18664 2022-12-15 20:32:57.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2022-12-15 20:32:56.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-15 20:33:07.000000 mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 20:33:07.332147 mypy-boto3-translate-1.26.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2022-12-15 20:32:55.000000 mypy-boto3-translate-1.26.31/setup.py
```

### Comparing `mypy-boto3-translate-1.26.139/LICENSE` & `mypy-boto3-translate-1.26.31/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-translate-1.26.139/PKG-INFO` & `mypy-boto3-translate-1.26.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.26.139
-Summary: Type annotations for boto3.Translate 1.26.139 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.31
+Summary: Type annotations for boto3.Translate 1.26.31 service generated with mypy-boto3-builder 7.12.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.26.139](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,15 +338,14 @@
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
-    DocumentTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
@@ -355,15 +354,14 @@
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
     TranslationSettingsTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
-    TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
@@ -375,17 +373,15 @@
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     UpdateParallelDataResponseTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
     ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
-    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
@@ -402,42 +398,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-translate-1.26.139/README.md` & `mypy-boto3-translate-1.26.31/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.26.139](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,15 +306,14 @@
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
-    DocumentTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
@@ -323,15 +322,14 @@
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
     TranslationSettingsTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
-    TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
@@ -343,17 +341,15 @@
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     UpdateParallelDataResponseTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
     ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
-    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
@@ -370,42 +366,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/__init__.py` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/__init__.pyi` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/__main__.py` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Translate 1.26.139\nVersion:         1.26.139\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Translate 1.26.31\nVersion:         1.26.31\nBuilder version:"
+        " 7.12.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.139")
+    print("1.26.31")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/client.py` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 from .literals import DisplayLanguageCodeType, TerminologyDataFormatType
 from .paginator import ListTerminologiesPaginator
 from .type_defs import (
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataResponseTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
-    DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionKeyTypeDef,
     GetParallelDataResponseTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     InputDataConfigTypeDef,
     ListLanguagesResponseTypeDef,
@@ -39,15 +38,14 @@
     OutputDataConfigTypeDef,
     ParallelDataConfigTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     TagTypeDef,
     TerminologyDataTypeDef,
     TextTranslationJobFilterTypeDef,
-    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     TranslationSettingsTypeDef,
     UpdateParallelDataResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -304,30 +302,14 @@
         """
         Associates a specific tag with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#tag_resource)
         """
 
-    def translate_document(
-        self,
-        *,
-        Document: DocumentTypeDef,
-        SourceLanguageCode: str,
-        TargetLanguageCode: str,
-        TerminologyNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
-    ) -> TranslateDocumentResponseTypeDef:
-        """
-        Translates the input document from the source language to the target language.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_document)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#translate_document)
-        """
-
     def translate_text(
         self,
         *,
         Text: str,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/client.pyi` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 from .literals import DisplayLanguageCodeType, TerminologyDataFormatType
 from .paginator import ListTerminologiesPaginator
 from .type_defs import (
     CreateParallelDataResponseTypeDef,
     DeleteParallelDataResponseTypeDef,
     DescribeTextTranslationJobResponseTypeDef,
-    DocumentTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionKeyTypeDef,
     GetParallelDataResponseTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     InputDataConfigTypeDef,
     ListLanguagesResponseTypeDef,
@@ -39,15 +38,14 @@
     OutputDataConfigTypeDef,
     ParallelDataConfigTypeDef,
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     TagTypeDef,
     TerminologyDataTypeDef,
     TextTranslationJobFilterTypeDef,
-    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     TranslationSettingsTypeDef,
     UpdateParallelDataResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -281,29 +279,14 @@
     def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Associates a specific tag with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#tag_resource)
         """
-    def translate_document(
-        self,
-        *,
-        Document: DocumentTypeDef,
-        SourceLanguageCode: str,
-        TargetLanguageCode: str,
-        TerminologyNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
-    ) -> TranslateDocumentResponseTypeDef:
-        """
-        Translates the input document from the source language to the target language.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_document)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/client/#translate_document)
-        """
     def translate_text(
         self,
         *,
         Text: str,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/literals.py` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DirectionalityType",
     "DisplayLanguageCodeType",
     "EncryptionKeyTypeType",
     "FormalityType",
     "JobStatusType",
     "ListTerminologiesPaginatorName",
@@ -34,15 +33,14 @@
     "TranslateServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DirectionalityType = Literal["MULTI", "UNI"]
 DisplayLanguageCodeType = Literal["de", "en", "es", "fr", "it", "ja", "ko", "pt", "zh", "zh-TW"]
 EncryptionKeyTypeType = Literal["KMS"]
 FormalityType = Literal["FORMAL", "INFORMAL"]
 JobStatusType = Literal[
     "COMPLETED",
     "COMPLETED_WITH_ERROR",
@@ -98,26 +96,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -203,15 +199,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -222,38 +217,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -266,15 +257,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -293,15 +283,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -383,20 +372,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/literals.pyi` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DirectionalityType",
     "DisplayLanguageCodeType",
     "EncryptionKeyTypeType",
     "FormalityType",
     "JobStatusType",
     "ListTerminologiesPaginatorName",
@@ -33,14 +34,15 @@
     "TranslateServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DirectionalityType = Literal["MULTI", "UNI"]
 DisplayLanguageCodeType = Literal["de", "en", "es", "fr", "it", "ja", "ko", "pt", "zh", "zh-TW"]
 EncryptionKeyTypeType = Literal["KMS"]
 FormalityType = Literal["FORMAL", "INFORMAL"]
 JobStatusType = Literal[
     "COMPLETED",
     "COMPLETED_WITH_ERROR",
@@ -96,26 +98,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -201,15 +201,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -220,38 +219,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -264,15 +259,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -291,15 +285,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -381,20 +374,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/paginator.py` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/paginator.pyi` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/type_defs.py` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
-    "DocumentTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
@@ -59,15 +57,14 @@
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
     "TranslationSettingsTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
-    "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
     "TerminologyPropertiesTypeDef",
     "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
@@ -79,17 +76,15 @@
     "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobResponseTypeDef",
     "UpdateParallelDataResponseTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
     "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
-    "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
-    "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
     "ImportTerminologyResponseTypeDef",
     "ListTerminologiesResponseTypeDef",
     "GetParallelDataResponseTypeDef",
@@ -159,22 +154,14 @@
 DescribeTextTranslationJobRequestRequestTypeDef = TypedDict(
     "DescribeTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DocumentTypeDef = TypedDict(
-    "DocumentTypeDef",
-    {
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -196,21 +183,19 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
-
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -226,19 +211,17 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
-
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
-
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -329,21 +312,14 @@
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-TranslatedDocumentTypeDef = TypedDict(
-    "TranslatedDocumentTypeDef",
-    {
-        "Content": bytes,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -367,19 +343,17 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-
 TerminologyPropertiesTypeDef = TypedDict(
     "TerminologyPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
         "SourceLanguageCode": str,
@@ -433,22 +407,20 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -459,22 +431,20 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -555,21 +525,19 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
-
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -590,38 +558,14 @@
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredTranslateDocumentRequestRequestTypeDef",
-    {
-        "Document": DocumentTypeDef,
-        "SourceLanguageCode": str,
-        "TargetLanguageCode": str,
-    },
-)
-_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalTranslateDocumentRequestRequestTypeDef",
-    {
-        "TerminologyNames": Sequence[str],
-        "Settings": TranslationSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class TranslateDocumentRequestRequestTypeDef(
-    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -631,33 +575,19 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
-
-TranslateDocumentResponseTypeDef = TypedDict(
-    "TranslateDocumentResponseTypeDef",
-    {
-        "TranslatedDocument": TranslatedDocumentTypeDef,
-        "SourceLanguageCode": str,
-        "TargetLanguageCode": str,
-        "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
         "AppliedTerminologies": List[AppliedTerminologyTypeDef],
@@ -684,22 +614,20 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
-
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate/type_defs.pyi` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TermTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteParallelDataRequestRequestTypeDef",
     "DeleteTerminologyRequestRequestTypeDef",
     "DescribeTextTranslationJobRequestRequestTypeDef",
-    "DocumentTypeDef",
     "GetParallelDataRequestRequestTypeDef",
     "ParallelDataDataLocationTypeDef",
     "GetTerminologyRequestRequestTypeDef",
     "TerminologyDataLocationTypeDef",
     "TerminologyDataTypeDef",
     "InputDataConfigTypeDef",
     "JobDetailsTypeDef",
@@ -58,15 +58,14 @@
     "ListParallelDataRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTerminologiesRequestRequestTypeDef",
     "TextTranslationJobFilterTypeDef",
     "TranslationSettingsTypeDef",
     "StopTextTranslationJobRequestRequestTypeDef",
-    "TranslatedDocumentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppliedTerminologyTypeDef",
     "OutputDataConfigTypeDef",
     "TerminologyPropertiesTypeDef",
     "ParallelDataPropertiesTypeDef",
     "UpdateParallelDataRequestRequestTypeDef",
     "CreateParallelDataRequestRequestTypeDef",
@@ -78,17 +77,15 @@
     "StartTextTranslationJobResponseTypeDef",
     "StopTextTranslationJobResponseTypeDef",
     "UpdateParallelDataResponseTypeDef",
     "ImportTerminologyRequestRequestTypeDef",
     "ListLanguagesResponseTypeDef",
     "ListTerminologiesRequestListTerminologiesPaginateTypeDef",
     "ListTextTranslationJobsRequestRequestTypeDef",
-    "TranslateDocumentRequestRequestTypeDef",
     "TranslateTextRequestRequestTypeDef",
-    "TranslateDocumentResponseTypeDef",
     "TranslateTextResponseTypeDef",
     "StartTextTranslationJobRequestRequestTypeDef",
     "TextTranslationJobPropertiesTypeDef",
     "GetTerminologyResponseTypeDef",
     "ImportTerminologyResponseTypeDef",
     "ListTerminologiesResponseTypeDef",
     "GetParallelDataResponseTypeDef",
@@ -158,22 +155,14 @@
 DescribeTextTranslationJobRequestRequestTypeDef = TypedDict(
     "DescribeTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DocumentTypeDef = TypedDict(
-    "DocumentTypeDef",
-    {
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-
 GetParallelDataRequestRequestTypeDef = TypedDict(
     "GetParallelDataRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -195,19 +184,21 @@
     "_OptionalGetTerminologyRequestRequestTypeDef",
     {
         "TerminologyDataFormat": TerminologyDataFormatType,
     },
     total=False,
 )
 
+
 class GetTerminologyRequestRequestTypeDef(
     _RequiredGetTerminologyRequestRequestTypeDef, _OptionalGetTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 TerminologyDataLocationTypeDef = TypedDict(
     "TerminologyDataLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
     },
 )
@@ -223,17 +214,19 @@
     "_OptionalTerminologyDataTypeDef",
     {
         "Directionality": DirectionalityType,
     },
     total=False,
 )
 
+
 class TerminologyDataTypeDef(_RequiredTerminologyDataTypeDef, _OptionalTerminologyDataTypeDef):
     pass
 
+
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
         "ContentType": str,
     },
 )
@@ -324,21 +317,14 @@
 StopTextTranslationJobRequestRequestTypeDef = TypedDict(
     "StopTextTranslationJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-TranslatedDocumentTypeDef = TypedDict(
-    "TranslatedDocumentTypeDef",
-    {
-        "Content": bytes,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -362,17 +348,19 @@
     "_OptionalOutputDataConfigTypeDef",
     {
         "EncryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
+
 TerminologyPropertiesTypeDef = TypedDict(
     "TerminologyPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
         "SourceLanguageCode": str,
@@ -426,20 +414,22 @@
     "_OptionalUpdateParallelDataRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateParallelDataRequestRequestTypeDef(
     _RequiredUpdateParallelDataRequestRequestTypeDef,
     _OptionalUpdateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateParallelDataRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParallelDataRequestRequestTypeDef",
     {
         "Name": str,
         "ParallelDataConfig": ParallelDataConfigTypeDef,
         "ClientToken": str,
     },
@@ -450,20 +440,22 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateParallelDataRequestRequestTypeDef(
     _RequiredCreateParallelDataRequestRequestTypeDef,
     _OptionalCreateParallelDataRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -544,19 +536,21 @@
         "Description": str,
         "EncryptionKey": EncryptionKeyTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportTerminologyRequestRequestTypeDef(
     _RequiredImportTerminologyRequestRequestTypeDef, _OptionalImportTerminologyRequestRequestTypeDef
 ):
     pass
 
+
 ListLanguagesResponseTypeDef = TypedDict(
     "ListLanguagesResponseTypeDef",
     {
         "Languages": List[LanguageTypeDef],
         "DisplayLanguageCode": DisplayLanguageCodeType,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -577,36 +571,14 @@
         "Filter": TextTranslationJobFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_RequiredTranslateDocumentRequestRequestTypeDef",
-    {
-        "Document": DocumentTypeDef,
-        "SourceLanguageCode": str,
-        "TargetLanguageCode": str,
-    },
-)
-_OptionalTranslateDocumentRequestRequestTypeDef = TypedDict(
-    "_OptionalTranslateDocumentRequestRequestTypeDef",
-    {
-        "TerminologyNames": Sequence[str],
-        "Settings": TranslationSettingsTypeDef,
-    },
-    total=False,
-)
-
-class TranslateDocumentRequestRequestTypeDef(
-    _RequiredTranslateDocumentRequestRequestTypeDef, _OptionalTranslateDocumentRequestRequestTypeDef
-):
-    pass
-
 _RequiredTranslateTextRequestRequestTypeDef = TypedDict(
     "_RequiredTranslateTextRequestRequestTypeDef",
     {
         "Text": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
     },
@@ -616,30 +588,20 @@
     {
         "TerminologyNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class TranslateTextRequestRequestTypeDef(
     _RequiredTranslateTextRequestRequestTypeDef, _OptionalTranslateTextRequestRequestTypeDef
 ):
     pass
 
-TranslateDocumentResponseTypeDef = TypedDict(
-    "TranslateDocumentResponseTypeDef",
-    {
-        "TranslatedDocument": TranslatedDocumentTypeDef,
-        "SourceLanguageCode": str,
-        "TargetLanguageCode": str,
-        "AppliedTerminologies": List[AppliedTerminologyTypeDef],
-        "AppliedSettings": TranslationSettingsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 TranslateTextResponseTypeDef = TypedDict(
     "TranslateTextResponseTypeDef",
     {
         "TranslatedText": str,
         "SourceLanguageCode": str,
         "TargetLanguageCode": str,
@@ -667,20 +629,22 @@
         "TerminologyNames": Sequence[str],
         "ParallelDataNames": Sequence[str],
         "Settings": TranslationSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StartTextTranslationJobRequestRequestTypeDef(
     _RequiredStartTextTranslationJobRequestRequestTypeDef,
     _OptionalStartTextTranslationJobRequestRequestTypeDef,
 ):
     pass
 
+
 TextTranslationJobPropertiesTypeDef = TypedDict(
     "TextTranslationJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "JobDetails": JobDetailsTypeDef,
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/PKG-INFO` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-translate
-Version: 1.26.139
-Summary: Type annotations for boto3.Translate 1.26.139 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.31
+Summary: Type annotations for boto3.Translate 1.26.31 service generated with mypy-boto3-builder 7.12.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-translate"></a>
 
 # mypy-boto3-translate
 
 [![PyPI - mypy-boto3-translate](https://img.shields.io/pypi/v/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-translate.svg?color=blue)](https://pypi.org/project/mypy-boto3-translate)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-translate?color=blue)](https://pypistats.org/packages/mypy-boto3-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Translate 1.26.139](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[boto3.Translate 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-translate docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,15 +338,14 @@
     EncryptionKeyTypeDef,
     ParallelDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteParallelDataRequestRequestTypeDef,
     DeleteTerminologyRequestRequestTypeDef,
     DescribeTextTranslationJobRequestRequestTypeDef,
-    DocumentTypeDef,
     GetParallelDataRequestRequestTypeDef,
     ParallelDataDataLocationTypeDef,
     GetTerminologyRequestRequestTypeDef,
     TerminologyDataLocationTypeDef,
     TerminologyDataTypeDef,
     InputDataConfigTypeDef,
     JobDetailsTypeDef,
@@ -355,15 +354,14 @@
     ListParallelDataRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTerminologiesRequestRequestTypeDef,
     TextTranslationJobFilterTypeDef,
     TranslationSettingsTypeDef,
     StopTextTranslationJobRequestRequestTypeDef,
-    TranslatedDocumentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppliedTerminologyTypeDef,
     OutputDataConfigTypeDef,
     TerminologyPropertiesTypeDef,
     ParallelDataPropertiesTypeDef,
     UpdateParallelDataRequestRequestTypeDef,
     CreateParallelDataRequestRequestTypeDef,
@@ -375,17 +373,15 @@
     StartTextTranslationJobResponseTypeDef,
     StopTextTranslationJobResponseTypeDef,
     UpdateParallelDataResponseTypeDef,
     ImportTerminologyRequestRequestTypeDef,
     ListLanguagesResponseTypeDef,
     ListTerminologiesRequestListTerminologiesPaginateTypeDef,
     ListTextTranslationJobsRequestRequestTypeDef,
-    TranslateDocumentRequestRequestTypeDef,
     TranslateTextRequestRequestTypeDef,
-    TranslateDocumentResponseTypeDef,
     TranslateTextResponseTypeDef,
     StartTextTranslationJobRequestRequestTypeDef,
     TextTranslationJobPropertiesTypeDef,
     GetTerminologyResponseTypeDef,
     ImportTerminologyResponseTypeDef,
     ListTerminologiesResponseTypeDef,
     GetParallelDataResponseTypeDef,
@@ -402,42 +398,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-translate-1.26.139/mypy_boto3_translate.egg-info/SOURCES.txt` & `mypy-boto3-translate-1.26.31/mypy_boto3_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-translate-1.26.139/setup.py` & `mypy-boto3-translate-1.26.31/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-translate.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-translate",
-    version="1.26.139",
+    version="1.26.31",
     packages=["mypy_boto3_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Translate 1.26.139 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Translate 1.26.31 service generated with mypy-boto3-builder"
+        " 7.12.0"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_translate/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

