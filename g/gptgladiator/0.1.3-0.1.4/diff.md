# Comparing `tmp/gptgladiator-0.1.3.tar.gz` & `tmp/gptgladiator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptgladiator-0.1.3.tar", last modified: Tue May 23 16:40:50 2023, max compression
+gzip compressed data, was "gptgladiator-0.1.4.tar", last modified: Tue May 23 16:50:02 2023, max compression
```

## Comparing `gptgladiator-0.1.3.tar` & `gptgladiator-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:40:50.539707 gptgladiator-0.1.3/
--rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:40:50.539553 gptgladiator-0.1.3/PKG-INFO
--rw-r--r--   0 willjessup   (501) staff       (20)     2273 2023-05-20 16:31:31.000000 gptgladiator-0.1.3/README.md
-drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:40:50.538680 gptgladiator-0.1.3/gptgladiator/
--rw-r--r--   0 willjessup   (501) staff       (20)     2348 2023-05-23 16:40:10.000000 gptgladiator-0.1.3/gptgladiator/ChatBot.py
--rw-r--r--   0 willjessup   (501) staff       (20)      541 2023-05-20 16:32:36.000000 gptgladiator-0.1.3/gptgladiator/GPTModel.py
--rw-r--r--   0 willjessup   (501) staff       (20)     5557 2023-05-23 16:40:05.000000 gptgladiator-0.1.3/gptgladiator/Gladiator.py
--rw-r--r--   0 willjessup   (501) staff       (20)       32 2023-05-20 16:36:27.000000 gptgladiator-0.1.3/gptgladiator/__init__.py
--rw-r--r--   0 willjessup   (501) staff       (20)     2758 2023-05-20 16:31:31.000000 gptgladiator-0.1.3/gptgladiator/mocks.py
--rw-r--r--   0 willjessup   (501) staff       (20)     1670 2023-05-20 16:31:31.000000 gptgladiator-0.1.3/gptgladiator/prompts.py
-drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:40:50.539273 gptgladiator-0.1.3/gptgladiator.egg-info/
--rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:40:50.000000 gptgladiator-0.1.3/gptgladiator.egg-info/PKG-INFO
--rw-r--r--   0 willjessup   (501) staff       (20)      343 2023-05-23 16:40:50.000000 gptgladiator-0.1.3/gptgladiator.egg-info/SOURCES.txt
--rw-r--r--   0 willjessup   (501) staff       (20)        1 2023-05-23 16:40:50.000000 gptgladiator-0.1.3/gptgladiator.egg-info/dependency_links.txt
--rw-r--r--   0 willjessup   (501) staff       (20)       49 2023-05-23 16:40:50.000000 gptgladiator-0.1.3/gptgladiator.egg-info/requires.txt
--rw-r--r--   0 willjessup   (501) staff       (20)       13 2023-05-23 16:40:50.000000 gptgladiator-0.1.3/gptgladiator.egg-info/top_level.txt
--rw-r--r--   0 willjessup   (501) staff       (20)       38 2023-05-23 16:40:50.539747 gptgladiator-0.1.3/setup.cfg
--rw-r--r--   0 willjessup   (501) staff       (20)      548 2023-05-23 16:40:41.000000 gptgladiator-0.1.3/setup.py
+drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:50:02.324606 gptgladiator-0.1.4/
+-rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:50:02.324477 gptgladiator-0.1.4/PKG-INFO
+-rw-r--r--   0 willjessup   (501) staff       (20)     2273 2023-05-20 16:31:31.000000 gptgladiator-0.1.4/README.md
+drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:50:02.323778 gptgladiator-0.1.4/gptgladiator/
+-rw-r--r--   0 willjessup   (501) staff       (20)     2348 2023-05-23 16:40:10.000000 gptgladiator-0.1.4/gptgladiator/ChatBot.py
+-rw-r--r--   0 willjessup   (501) staff       (20)      541 2023-05-20 16:32:36.000000 gptgladiator-0.1.4/gptgladiator/GPTModel.py
+-rw-r--r--   0 willjessup   (501) staff       (20)     5557 2023-05-23 16:40:05.000000 gptgladiator-0.1.4/gptgladiator/Gladiator.py
+-rw-r--r--   0 willjessup   (501) staff       (20)       32 2023-05-20 16:36:27.000000 gptgladiator-0.1.4/gptgladiator/__init__.py
+-rw-r--r--   0 willjessup   (501) staff       (20)     2758 2023-05-20 16:31:31.000000 gptgladiator-0.1.4/gptgladiator/mocks.py
+-rw-r--r--   0 willjessup   (501) staff       (20)     1670 2023-05-20 16:31:31.000000 gptgladiator-0.1.4/gptgladiator/prompts.py
+drwxr-xr-x   0 willjessup   (501) staff       (20)        0 2023-05-23 16:50:02.324303 gptgladiator-0.1.4/gptgladiator.egg-info/
+-rw-r--r--   0 willjessup   (501) staff       (20)      308 2023-05-23 16:50:02.000000 gptgladiator-0.1.4/gptgladiator.egg-info/PKG-INFO
+-rw-r--r--   0 willjessup   (501) staff       (20)      343 2023-05-23 16:50:02.000000 gptgladiator-0.1.4/gptgladiator.egg-info/SOURCES.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)        1 2023-05-23 16:50:02.000000 gptgladiator-0.1.4/gptgladiator.egg-info/dependency_links.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)       49 2023-05-23 16:50:02.000000 gptgladiator-0.1.4/gptgladiator.egg-info/requires.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)       13 2023-05-23 16:50:02.000000 gptgladiator-0.1.4/gptgladiator.egg-info/top_level.txt
+-rw-r--r--   0 willjessup   (501) staff       (20)       38 2023-05-23 16:50:02.324637 gptgladiator-0.1.4/setup.cfg
+-rw-r--r--   0 willjessup   (501) staff       (20)      548 2023-05-23 16:43:51.000000 gptgladiator-0.1.4/setup.py
```

### Comparing `gptgladiator-0.1.3/README.md` & `gptgladiator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.3/gptgladiator/ChatBot.py` & `gptgladiator-0.1.4/gptgladiator/ChatBot.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.3/gptgladiator/GPTModel.py` & `gptgladiator-0.1.4/gptgladiator/GPTModel.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.3/gptgladiator/Gladiator.py` & `gptgladiator-0.1.4/gptgladiator/Gladiator.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.3/gptgladiator/mocks.py` & `gptgladiator-0.1.4/gptgladiator/mocks.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.3/gptgladiator/prompts.py` & `gptgladiator-0.1.4/gptgladiator/prompts.py`

 * *Files identical despite different names*

### Comparing `gptgladiator-0.1.3/setup.py` & `gptgladiator-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gptgladiator',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'openai==0.27.6',
         'tiktoken==0.3.3',
         'streamlit==1.22.0'
     ],
     py_modules=['gptgladiator'],
```

