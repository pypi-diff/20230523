# Comparing `tmp/gensum-0.1.0.tar.gz` & `tmp/gensum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensum-0.1.0.tar", last modified: Tue May 23 05:16:51 2023, max compression
+gzip compressed data, was "gensum-0.1.1.tar", last modified: Tue May 23 05:22:08 2023, max compression
```

## Comparing `gensum-0.1.0.tar` & `gensum-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:16:51.989255 gensum-0.1.0/
--rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.0/LICENSE
--rw-r--r--   0 abriel     (503) staff       (20)     5491 2023-05-23 05:16:51.989083 gensum-0.1.0/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)     5191 2023-05-23 05:00:18.000000 gensum-0.1.0/README.md
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:16:51.987539 gensum-0.1.0/gensum/
--rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.0/gensum/__init__.py
--rw-r--r--   0 abriel     (503) staff       (20)     3561 2023-05-19 16:41:16.000000 gensum-0.1.0/gensum/generator.py
--rw-r--r--   0 abriel     (503) staff       (20)    12726 2023-05-22 22:10:22.000000 gensum-0.1.0/gensum/gensum.py
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:16:51.988844 gensum-0.1.0/gensum.egg-info/
--rw-r--r--   0 abriel     (503) staff       (20)     5491 2023-05-23 05:16:51.000000 gensum-0.1.0/gensum.egg-info/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)      246 2023-05-23 05:16:51.000000 gensum-0.1.0/gensum.egg-info/SOURCES.txt
--rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 05:16:51.000000 gensum-0.1.0/gensum.egg-info/dependency_links.txt
--rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 05:16:51.000000 gensum-0.1.0/gensum.egg-info/requires.txt
--rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 05:16:51.000000 gensum-0.1.0/gensum.egg-info/top_level.txt
--rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-18 20:55:17.000000 gensum-0.1.0/pyproject.toml
--rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 05:16:51.989304 gensum-0.1.0/setup.cfg
--rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 05:06:35.000000 gensum-0.1.0/setup.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:22:08.094605 gensum-0.1.1/
+-rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.1/LICENSE
+-rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:22:08.094260 gensum-0.1.1/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)     4400 2023-05-23 05:21:24.000000 gensum-0.1.1/README.md
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:22:08.093012 gensum-0.1.1/gensum/
+-rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.1/gensum/__init__.py
+-rw-r--r--   0 abriel     (503) staff       (20)     3561 2023-05-19 16:41:16.000000 gensum-0.1.1/gensum/generator.py
+-rw-r--r--   0 abriel     (503) staff       (20)    12726 2023-05-22 22:10:22.000000 gensum-0.1.1/gensum/gensum.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 05:22:08.094042 gensum-0.1.1/gensum.egg-info/
+-rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)      246 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/SOURCES.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/dependency_links.txt
+-rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/requires.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 05:22:08.000000 gensum-0.1.1/gensum.egg-info/top_level.txt
+-rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 05:21:45.000000 gensum-0.1.1/pyproject.toml
+-rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 05:22:08.094656 gensum-0.1.1/setup.cfg
+-rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 05:21:52.000000 gensum-0.1.1/setup.py
```

### Comparing `gensum-0.1.0/LICENSE` & `gensum-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gensum-0.1.0/PKG-INFO` & `gensum-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,31 +12,21 @@
 # gensum - Generative Summarization for Data Augmentation
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI version](https://badge.fury.io/py/gensum.svg)](https://badge.fury.io/py/gensum)
 ![Python 3.10](https://img.shields.io/badge/python-3.6%20%7C%203.7-green.svg)
 
 ## Introduction
-Imbalanced class distribution is a common problem in ML. Undersampling combined with oversampling are two methods of addressing this issue. 
-A technique such as SMOTE can be effective for oversampling, although the problem becomes a bit more difficult with multilabel datasets. 
-[MLSMOTE](https://www.sciencedirect.com/science/article/abs/pii/S0950705115002737) has been proposed, but the high dimensional nature of numerical vectors created from text can sometimes make other forms of data augmentation more appealing.
+Imbalanced class distribution remains a classic common problem in ML. Undersampling combined with oversampling are two methods of attempting to address this issue. 
+Techniques such as SMOTE and MLSMOTE have been proposed, but the high dimensional nature of numerical vectors created from text makes other data augmentation approaches preferable.
 
 gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation in order to oversample under-represented classes in datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
 
 It uses [ChatGPT](https://openai.com/blog/chatgpt) by default, but is designed in a modular way to allow you to use any large language models capable of generative summarization. `gensum` is format agnostic, expecting only a DataFrame containing a text and classifier column. 
 
-## Algorithm
-1. Append counts or the number of rows to add for each classifier value are first calculated with a ceiling threshold. Namely, if a given classifier value has 1000 rows and the ceiling is 100, its append count will be 0.
-
-2. For each classifier value it then completes a loop from an append index range to the append count specified for that given value.
-
-3. Generative summarization is completed for a specified size subset of all rows that uniquely have the given classifier value. 
-
-4. Each summarization is parsed into sentences and appended to a new dataframe with the respective classifier value.
-
 ## Installation
 ### Via pip
 
 ```bash
 pip install gensum
 ```
```

### Comparing `gensum-0.1.0/README.md` & `gensum-0.1.1/gensum.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+Metadata-Version: 2.1
+Name: gensum
+Version: 0.1.1
+Summary: Generative Summarization for Data Augmentation
+Home-page: https://github.com/aaronbriel/gensum
+Author: Aaron Briel
+Author-email: aaronbriel@gmail.com
+License: Apache License 2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gensum - Generative Summarization for Data Augmentation
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI version](https://badge.fury.io/py/gensum.svg)](https://badge.fury.io/py/gensum)
 ![Python 3.10](https://img.shields.io/badge/python-3.6%20%7C%203.7-green.svg)
 
 ## Introduction
-Imbalanced class distribution is a common problem in ML. Undersampling combined with oversampling are two methods of addressing this issue. 
-A technique such as SMOTE can be effective for oversampling, although the problem becomes a bit more difficult with multilabel datasets. 
-[MLSMOTE](https://www.sciencedirect.com/science/article/abs/pii/S0950705115002737) has been proposed, but the high dimensional nature of numerical vectors created from text can sometimes make other forms of data augmentation more appealing.
+Imbalanced class distribution remains a classic common problem in ML. Undersampling combined with oversampling are two methods of attempting to address this issue. 
+Techniques such as SMOTE and MLSMOTE have been proposed, but the high dimensional nature of numerical vectors created from text makes other data augmentation approaches preferable.
 
 gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation in order to oversample under-represented classes in datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
 
 It uses [ChatGPT](https://openai.com/blog/chatgpt) by default, but is designed in a modular way to allow you to use any large language models capable of generative summarization. `gensum` is format agnostic, expecting only a DataFrame containing a text and classifier column. 
 
-## Algorithm
-1. Append counts or the number of rows to add for each classifier value are first calculated with a ceiling threshold. Namely, if a given classifier value has 1000 rows and the ceiling is 100, its append count will be 0.
-
-2. For each classifier value it then completes a loop from an append index range to the append count specified for that given value.
-
-3. Generative summarization is completed for a specified size subset of all rows that uniquely have the given classifier value. 
-
-4. Each summarization is parsed into sentences and appended to a new dataframe with the respective classifier value.
-
 ## Installation
 ### Via pip
 
 ```bash
 pip install gensum
 ```
```

### Comparing `gensum-0.1.0/gensum/generator.py` & `gensum-0.1.1/gensum/generator.py`

 * *Files identical despite different names*

### Comparing `gensum-0.1.0/gensum/gensum.py` & `gensum-0.1.1/gensum/gensum.py`

 * *Files identical despite different names*

### Comparing `gensum-0.1.0/gensum.egg-info/PKG-INFO` & `gensum-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,21 @@
-Metadata-Version: 2.1
-Name: gensum
-Version: 0.1.0
-Summary: Generative Summarization for Data Augmentation
-Home-page: https://github.com/aaronbriel/gensum
-Author: Aaron Briel
-Author-email: aaronbriel@gmail.com
-License: Apache License 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gensum - Generative Summarization for Data Augmentation
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI version](https://badge.fury.io/py/gensum.svg)](https://badge.fury.io/py/gensum)
 ![Python 3.10](https://img.shields.io/badge/python-3.6%20%7C%203.7-green.svg)
 
 ## Introduction
-Imbalanced class distribution is a common problem in ML. Undersampling combined with oversampling are two methods of addressing this issue. 
-A technique such as SMOTE can be effective for oversampling, although the problem becomes a bit more difficult with multilabel datasets. 
-[MLSMOTE](https://www.sciencedirect.com/science/article/abs/pii/S0950705115002737) has been proposed, but the high dimensional nature of numerical vectors created from text can sometimes make other forms of data augmentation more appealing.
+Imbalanced class distribution remains a classic common problem in ML. Undersampling combined with oversampling are two methods of attempting to address this issue. 
+Techniques such as SMOTE and MLSMOTE have been proposed, but the high dimensional nature of numerical vectors created from text makes other data augmentation approaches preferable.
 
 gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation in order to oversample under-represented classes in datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
 
 It uses [ChatGPT](https://openai.com/blog/chatgpt) by default, but is designed in a modular way to allow you to use any large language models capable of generative summarization. `gensum` is format agnostic, expecting only a DataFrame containing a text and classifier column. 
 
-## Algorithm
-1. Append counts or the number of rows to add for each classifier value are first calculated with a ceiling threshold. Namely, if a given classifier value has 1000 rows and the ceiling is 100, its append count will be 0.
-
-2. For each classifier value it then completes a loop from an append index range to the append count specified for that given value.
-
-3. Generative summarization is completed for a specified size subset of all rows that uniquely have the given classifier value. 
-
-4. Each summarization is parsed into sentences and appended to a new dataframe with the respective classifier value.
-
 ## Installation
 ### Via pip
 
 ```bash
 pip install gensum
 ```
```

### Comparing `gensum-0.1.0/setup.py` & `gensum-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 PACKAGE_NAME = 'gensum'
 AUTHOR = 'Aaron Briel'
 AUTHOR_EMAIL = 'aaronbriel@gmail.com'
 URL = 'https://github.com/aaronbriel/gensum'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'Generative Summarization for Data Augmentation'
```

