# Comparing `tmp/gptgladiator-0.1.1.tar.gz` & `tmp/gptgladiator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptgladiator-0.1.1.tar", last modified: Tue May 23 16:33:34 2023, max compression
+gzip compressed data, was "gptgladiator-0.1.2.tar", last modified: Tue May 23 16:35:57 2023, max compression
```

## Comparing `gptgladiator-0.1.1.tar` & `gptgladiator-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:33:34.155208 gptgladiator-0.1.1/
--rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:33:34.155075 gptgladiator-0.1.1/PKG-INFO
--rw-r--r--   0 willjessup   (501) staff       (20)     2273 2023-05-20 16:31:31.000000 gptgladiator-0.1.1/README.md
-drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:33:34.154382 gptgladiator-0.1.1/gladiator/
--rw-r--r--   0 willjessup   (501) staff       (20)     2345 2023-05-20 16:35:25.000000 gptgladiator-0.1.1/gladiator/ChatBot.py
--rw-r--r--   0 willjessup   (501) staff       (20)      541 2023-05-20 16:32:36.000000 gptgladiator-0.1.1/gladiator/GPTModel.py
--rw-r--r--   0 willjessup   (501) staff       (20)     5545 2023-05-20 16:35:25.000000 gptgladiator-0.1.1/gladiator/Gladiator.py
--rw-r--r--   0 willjessup   (501) staff       (20)       32 2023-05-20 16:36:27.000000 gptgladiator-0.1.1/gladiator/__init__.py
--rw-r--r--   0 willjessup   (501) staff       (20)     2758 2023-05-20 16:31:31.000000 gptgladiator-0.1.1/gladiator/mocks.py
--rw-r--r--   0 willjessup   (501) staff       (20)     1670 2023-05-20 16:31:31.000000 gptgladiator-0.1.1/gladiator/prompts.py
-drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:33:34.154913 gptgladiator-0.1.1/gptgladiator.egg-info/
--rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:33:34.000000 gptgladiator-0.1.1/gptgladiator.egg-info/PKG-INFO
--rw-r--r--   0 willjessup   (501) staff       (20)      325 2023-05-23 16:33:34.000000 gptgladiator-0.1.1/gptgladiator.egg-info/SOURCES.txt
--rw-r--r--   0 willjessup   (501) staff       (20)        1 2023-05-23 16:33:34.000000 gptgladiator-0.1.1/gptgladiator.egg-info/dependency_links.txt
--rw-r--r--   0 willjessup   (501) staff       (20)       49 2023-05-23 16:33:34.000000 gptgladiator-0.1.1/gptgladiator.egg-info/requires.txt
--rw-r--r--   0 willjessup   (501) staff       (20)       23 2023-05-23 16:33:34.000000 gptgladiator-0.1.1/gptgladiator.egg-info/top_level.txt
--rw-r--r--   0 willjessup   (501) staff       (20)       38 2023-05-23 16:33:34.155241 gptgladiator-0.1.1/setup.cfg
--rw-r--r--   0 willjessup   (501) staff       (20)      548 2023-05-23 16:33:23.000000 gptgladiator-0.1.1/setup.py
+drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:35:57.051749 gptgladiator-0.1.2/
+-rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:35:57.051606 gptgladiator-0.1.2/PKG-INFO
+-rw-r--r--   0 willjessup   (501) staff       (20)     2273 2023-05-20 16:31:31.000000 gptgladiator-0.1.2/README.md
+drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:35:57.050823 gptgladiator-0.1.2/gladiator/
+-rw-r--r--   0 willjessup   (501) staff       (20)     2345 2023-05-20 16:35:25.000000 gptgladiator-0.1.2/gladiator/ChatBot.py
+-rw-r--r--   0 willjessup   (501) staff       (20)      541 2023-05-20 16:32:36.000000 gptgladiator-0.1.2/gladiator/GPTModel.py
+-rw-r--r--   0 willjessup   (501) staff       (20)     5545 2023-05-20 16:35:25.000000 gptgladiator-0.1.2/gladiator/Gladiator.py
+-rw-r--r--   0 willjessup   (501) staff       (20)       32 2023-05-20 16:36:27.000000 gptgladiator-0.1.2/gladiator/__init__.py
+-rw-r--r--   0 willjessup   (501) staff       (20)     2758 2023-05-20 16:31:31.000000 gptgladiator-0.1.2/gladiator/mocks.py
+-rw-r--r--   0 willjessup   (501) staff       (20)     1670 2023-05-20 16:31:31.000000 gptgladiator-0.1.2/gladiator/prompts.py
+drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:35:57.051427 gptgladiator-0.1.2/gptgladiator.egg-info/
+-rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:35:57.000000 gptgladiator-0.1.2/gptgladiator.egg-info/PKG-INFO
+-rw-r--r--   0 willjessup   (501) staff       (20)      325 2023-05-23 16:35:57.000000 gptgladiator-0.1.2/gptgladiator.egg-info/SOURCES.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)        1 2023-05-23 16:35:57.000000 gptgladiator-0.1.2/gptgladiator.egg-info/dependency_links.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)       49 2023-05-23 16:35:57.000000 gptgladiator-0.1.2/gptgladiator.egg-info/requires.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)       23 2023-05-23 16:35:57.000000 gptgladiator-0.1.2/gptgladiator.egg-info/top_level.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)       38 2023-05-23 16:35:57.051797 gptgladiator-0.1.2/setup.cfg
+-rw-r--r--   0 willjessup   (501) staff       (20)      548 2023-05-23 16:35:48.000000 gptgladiator-0.1.2/setup.py
```

### Comparing `gptgladiator-0.1.1/README.md` & `gptgladiator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.1/gladiator/ChatBot.py` & `gptgladiator-0.1.2/gladiator/ChatBot.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.1/gladiator/GPTModel.py` & `gptgladiator-0.1.2/gladiator/GPTModel.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.1/gladiator/Gladiator.py` & `gptgladiator-0.1.2/gladiator/Gladiator.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.1/gladiator/mocks.py` & `gptgladiator-0.1.2/gladiator/mocks.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.1/gladiator/prompts.py` & `gptgladiator-0.1.2/gladiator/prompts.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.1/setup.py` & `gptgladiator-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gptgladiator',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'openai==0.27.6',
         'tiktoken==0.3.3',
         'streamlit==1.22.0'
     ],
     py_modules=['gptgladiator'],
```

