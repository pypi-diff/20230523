# Comparing `tmp/gensum-0.1.4.tar.gz` & `tmp/gensum-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gensum-0.1.4.tar", last modified: Tue May 23 13:04:48 2023, max compression
+gzip compressed data, was "gensum-0.1.5.tar", last modified: Tue May 23 14:56:29 2023, max compression
```

## Comparing `gensum-0.1.4.tar` & `gensum-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 13:04:48.756878 gensum-0.1.4/
--rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.4/LICENSE
--rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 13:04:48.756701 gensum-0.1.4/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)     4400 2023-05-23 05:21:24.000000 gensum-0.1.4/README.md
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 13:04:48.755508 gensum-0.1.4/gensum/
--rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.4/gensum/__init__.py
--rw-r--r--   0 abriel     (503) staff       (20)    14846 2023-05-23 13:04:07.000000 gensum-0.1.4/gensum/gensum.py
-drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 13:04:48.756463 gensum-0.1.4/gensum.egg-info/
--rw-r--r--   0 abriel     (503) staff       (20)     4700 2023-05-23 13:04:48.000000 gensum-0.1.4/gensum.egg-info/PKG-INFO
--rw-r--r--   0 abriel     (503) staff       (20)      226 2023-05-23 13:04:48.000000 gensum-0.1.4/gensum.egg-info/SOURCES.txt
--rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 13:04:48.000000 gensum-0.1.4/gensum.egg-info/dependency_links.txt
--rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 13:04:48.000000 gensum-0.1.4/gensum.egg-info/requires.txt
--rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 13:04:48.000000 gensum-0.1.4/gensum.egg-info/top_level.txt
--rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 13:04:26.000000 gensum-0.1.4/pyproject.toml
--rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 13:04:48.756927 gensum-0.1.4/setup.cfg
--rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 13:04:34.000000 gensum-0.1.4/setup.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 14:56:29.283572 gensum-0.1.5/
+-rw-r--r--   0 abriel     (503) staff       (20)    11357 2023-05-18 19:51:17.000000 gensum-0.1.5/LICENSE
+-rw-r--r--   0 abriel     (503) staff       (20)     4800 2023-05-23 14:56:29.283405 gensum-0.1.5/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)     4500 2023-05-23 14:56:12.000000 gensum-0.1.5/README.md
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 14:56:29.282220 gensum-0.1.5/gensum/
+-rw-r--r--   0 abriel     (503) staff       (20)       29 2023-05-19 16:34:03.000000 gensum-0.1.5/gensum/__init__.py
+-rw-r--r--   0 abriel     (503) staff       (20)    14846 2023-05-23 13:04:07.000000 gensum-0.1.5/gensum/gensum.py
+drwxr-xr-x   0 abriel     (503) staff       (20)        0 2023-05-23 14:56:29.283117 gensum-0.1.5/gensum.egg-info/
+-rw-r--r--   0 abriel     (503) staff       (20)     4800 2023-05-23 14:56:29.000000 gensum-0.1.5/gensum.egg-info/PKG-INFO
+-rw-r--r--   0 abriel     (503) staff       (20)      226 2023-05-23 14:56:29.000000 gensum-0.1.5/gensum.egg-info/SOURCES.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        1 2023-05-23 14:56:29.000000 gensum-0.1.5/gensum.egg-info/dependency_links.txt
+-rw-r--r--   0 abriel     (503) staff       (20)       20 2023-05-23 14:56:29.000000 gensum-0.1.5/gensum.egg-info/requires.txt
+-rw-r--r--   0 abriel     (503) staff       (20)        7 2023-05-23 14:56:29.000000 gensum-0.1.5/gensum.egg-info/top_level.txt
+-rw-r--r--   0 abriel     (503) staff       (20)      500 2023-05-23 14:56:12.000000 gensum-0.1.5/pyproject.toml
+-rw-r--r--   0 abriel     (503) staff       (20)       38 2023-05-23 14:56:29.283619 gensum-0.1.5/setup.cfg
+-rw-r--r--   0 abriel     (503) staff       (20)      834 2023-05-23 14:56:12.000000 gensum-0.1.5/setup.py
```

### Comparing `gensum-0.1.4/LICENSE` & `gensum-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gensum-0.1.4/PKG-INFO` & `gensum-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 [![PyPI version](https://badge.fury.io/py/gensum.svg)](https://badge.fury.io/py/gensum)
 ![Python 3.10](https://img.shields.io/badge/python-3.6%20%7C%203.7-green.svg)
 
 ## Introduction
 Imbalanced class distribution remains a classic common problem in ML. Undersampling combined with oversampling are two methods of attempting to address this issue. 
 Techniques such as SMOTE and MLSMOTE have been proposed, but the high dimensional nature of numerical vectors created from text makes other data augmentation approaches preferable.
 
-gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation in order to oversample under-represented classes in datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
+gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation by oversampling under-represented classes in text classification datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
 
 It uses [ChatGPT](https://openai.com/blog/chatgpt) by default, but is designed in a modular way to allow you to use any large language models capable of generative summarization. `gensum` is format agnostic, expecting only a DataFrame containing a text and classifier column. 
 
 ## Installation
 ### Via pip
 
 ```bash
@@ -41,15 +41,15 @@
 
 ```bash
 pip install git+https://github.com/aaronbriel/gensum.git
 ```
 
 ## Usage
 
-gensum expects a DataFrame containing a text column which defaults to 'text', and another classifier column which defaults to 'classifier'. All available parameters are detailed in the Parameters section below.
+gensum expects a DataFrame containing a text column which defaults to 'text', and another classifier column which defaults to 'classifier'. All available parameters are detailed in the Parameters section below. Be sure to set the `OPENAI_API_KEY` environmental parameter prior to running the code.
 
 ```bash
 import pandas as pd
 from gensum import Augmentor
 
 csv = 'path_to_csv'
 df = pd.read_csv(csv)
```

### Comparing `gensum-0.1.4/README.md` & `gensum-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![PyPI version](https://badge.fury.io/py/gensum.svg)](https://badge.fury.io/py/gensum)
 ![Python 3.10](https://img.shields.io/badge/python-3.6%20%7C%203.7-green.svg)
 
 ## Introduction
 Imbalanced class distribution remains a classic common problem in ML. Undersampling combined with oversampling are two methods of attempting to address this issue. 
 Techniques such as SMOTE and MLSMOTE have been proposed, but the high dimensional nature of numerical vectors created from text makes other data augmentation approaches preferable.
 
-gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation in order to oversample under-represented classes in datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
+gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation by oversampling under-represented classes in text classification datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
 
 It uses [ChatGPT](https://openai.com/blog/chatgpt) by default, but is designed in a modular way to allow you to use any large language models capable of generative summarization. `gensum` is format agnostic, expecting only a DataFrame containing a text and classifier column. 
 
 ## Installation
 ### Via pip
 
 ```bash
@@ -30,15 +30,15 @@
 
 ```bash
 pip install git+https://github.com/aaronbriel/gensum.git
 ```
 
 ## Usage
 
-gensum expects a DataFrame containing a text column which defaults to 'text', and another classifier column which defaults to 'classifier'. All available parameters are detailed in the Parameters section below.
+gensum expects a DataFrame containing a text column which defaults to 'text', and another classifier column which defaults to 'classifier'. All available parameters are detailed in the Parameters section below. Be sure to set the `OPENAI_API_KEY` environmental parameter prior to running the code.
 
 ```bash
 import pandas as pd
 from gensum import Augmentor
 
 csv = 'path_to_csv'
 df = pd.read_csv(csv)
```

### Comparing `gensum-0.1.4/gensum/gensum.py` & `gensum-0.1.5/gensum/gensum.py`

 * *Files identical despite different names*

### Comparing `gensum-0.1.4/gensum.egg-info/PKG-INFO` & `gensum-0.1.5/gensum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gensum
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generative Summarization for Data Augmentation
 Home-page: https://github.com/aaronbriel/gensum
 Author: Aaron Briel
 Author-email: aaronbriel@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 [![PyPI version](https://badge.fury.io/py/gensum.svg)](https://badge.fury.io/py/gensum)
 ![Python 3.10](https://img.shields.io/badge/python-3.6%20%7C%203.7-green.svg)
 
 ## Introduction
 Imbalanced class distribution remains a classic common problem in ML. Undersampling combined with oversampling are two methods of attempting to address this issue. 
 Techniques such as SMOTE and MLSMOTE have been proposed, but the high dimensional nature of numerical vectors created from text makes other data augmentation approaches preferable.
 
-gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation in order to oversample under-represented classes in datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
+gensum is an NLP library based on [absum](https://github.com/aaronbriel/absum) that uses generative summarization to perform data augmentation by oversampling under-represented classes in text classification datasets. Recent advancements in generative models such as ChatGPT make this approach optimal in achieving realistic *but unique* data for the augmentation process.
 
 It uses [ChatGPT](https://openai.com/blog/chatgpt) by default, but is designed in a modular way to allow you to use any large language models capable of generative summarization. `gensum` is format agnostic, expecting only a DataFrame containing a text and classifier column. 
 
 ## Installation
 ### Via pip
 
 ```bash
@@ -41,15 +41,15 @@
 
 ```bash
 pip install git+https://github.com/aaronbriel/gensum.git
 ```
 
 ## Usage
 
-gensum expects a DataFrame containing a text column which defaults to 'text', and another classifier column which defaults to 'classifier'. All available parameters are detailed in the Parameters section below.
+gensum expects a DataFrame containing a text column which defaults to 'text', and another classifier column which defaults to 'classifier'. All available parameters are detailed in the Parameters section below. Be sure to set the `OPENAI_API_KEY` environmental parameter prior to running the code.
 
 ```bash
 import pandas as pd
 from gensum import Augmentor
 
 csv = 'path_to_csv'
 df = pd.read_csv(csv)
```

### Comparing `gensum-0.1.4/setup.py` & `gensum-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 PACKAGE_NAME = 'gensum'
 AUTHOR = 'Aaron Briel'
 AUTHOR_EMAIL = 'aaronbriel@gmail.com'
 URL = 'https://github.com/aaronbriel/gensum'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'Generative Summarization for Data Augmentation'
```

