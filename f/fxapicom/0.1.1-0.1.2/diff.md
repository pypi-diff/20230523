# Comparing `tmp/fxapicom-0.1.1.tar.gz` & `tmp/fxapicom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fxapicom-0.1.1.tar", last modified: Tue May 23 12:59:47 2023, max compression
+gzip compressed data, was "dist/fxapicom-0.1.2.tar", last modified: Tue May 23 13:02:04 2023, max compression
```

## Comparing `fxapicom-0.1.1.tar` & `fxapicom-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-23 12:59:47.000000 fxapicom-0.1.1/
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     3445 2023-05-23 12:59:47.000000 fxapicom-0.1.1/PKG-INFO
-drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom.egg-info/
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     3445 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom.egg-info/PKG-INFO
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)      217 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom.egg-info/SOURCES.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       17 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom.egg-info/requires.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)        9 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom.egg-info/top_level.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)        1 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom.egg-info/dependency_links.txt
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1672 2023-05-23 12:52:59.000000 fxapicom-0.1.1/README.md
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1503 2023-05-23 12:59:45.000000 fxapicom-0.1.1/setup.py
-drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-23 12:59:47.000000 fxapicom-0.1.1/fxapicom/
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)     2191 2023-05-23 12:53:16.000000 fxapicom-0.1.1/fxapicom/client.py
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       49 2023-05-23 12:58:49.000000 fxapicom-0.1.1/fxapicom/__init__.py
--rw-r--r--   0 andreasaltheimer   (501) staff       (20)       38 2023-05-23 12:59:47.000000 fxapicom-0.1.1/setup.cfg
+drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-23 13:02:04.000000 fxapicom-0.1.2/
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     3454 2023-05-23 13:02:04.000000 fxapicom-0.1.2/PKG-INFO
+drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom.egg-info/
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     3454 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom.egg-info/PKG-INFO
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)      217 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom.egg-info/SOURCES.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       17 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom.egg-info/requires.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)        9 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom.egg-info/top_level.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)        1 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom.egg-info/dependency_links.txt
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1681 2023-05-23 13:01:40.000000 fxapicom-0.1.2/README.md
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     1503 2023-05-23 13:02:00.000000 fxapicom-0.1.2/setup.py
+drwxr-xr-x   0 andreasaltheimer   (501) staff       (20)        0 2023-05-23 13:02:04.000000 fxapicom-0.1.2/fxapicom/
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)     2191 2023-05-23 12:53:16.000000 fxapicom-0.1.2/fxapicom/client.py
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       49 2023-05-23 12:58:49.000000 fxapicom-0.1.2/fxapicom/__init__.py
+-rw-r--r--   0 andreasaltheimer   (501) staff       (20)       38 2023-05-23 13:02:04.000000 fxapicom-0.1.2/setup.cfg
```

### Comparing `fxapicom-0.1.1/PKG-INFO` & `fxapicom-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: fxapicom
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fxapi Python Client
 Home-page: https://github.com/everapihq/fxapi-python
 Author: Everapi
 Author-email: office@everapi.com
 License: MIT
 Description: # fxapi Python Client #
         
         Fxapi Python Client is the official Python Wrapper around the fxapi [API](https://fxapi.com/).
         
         ## Installation
         
         Install from pip:
         ````sh
-        pip install fxapi
+        pip install fxapicom
         ````
         
         Install from code:
         ````sh
         pip install git+https://github.com/everapihq/fxapi-python.git
         ````
         
         ## Usage
         
         All curencyapi API requests are made using the `Client` class. This class must be initialized with your API access key string. [Where is my API access key?](https://app.fxapi.com/dashboard)
         
         In your Python application, import `fxapi` and pass authentication information to initialize it:
         
         ````python
-        import fxapi
-        client = fxapi.Client('API_KEY')
+        import fxapicom
+        client = fxapicom.Client('API_KEY')
         ````
         
         ### Retrieve Status
         
         ```python
         
         print(client.status())
```

### Comparing `fxapicom-0.1.1/fxapicom.egg-info/PKG-INFO` & `fxapicom-0.1.2/fxapicom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: fxapicom
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fxapi Python Client
 Home-page: https://github.com/everapihq/fxapi-python
 Author: Everapi
 Author-email: office@everapi.com
 License: MIT
 Description: # fxapi Python Client #
         
         Fxapi Python Client is the official Python Wrapper around the fxapi [API](https://fxapi.com/).
         
         ## Installation
         
         Install from pip:
         ````sh
-        pip install fxapi
+        pip install fxapicom
         ````
         
         Install from code:
         ````sh
         pip install git+https://github.com/everapihq/fxapi-python.git
         ````
         
         ## Usage
         
         All curencyapi API requests are made using the `Client` class. This class must be initialized with your API access key string. [Where is my API access key?](https://app.fxapi.com/dashboard)
         
         In your Python application, import `fxapi` and pass authentication information to initialize it:
         
         ````python
-        import fxapi
-        client = fxapi.Client('API_KEY')
+        import fxapicom
+        client = fxapicom.Client('API_KEY')
         ````
         
         ### Retrieve Status
         
         ```python
         
         print(client.status())
```

### Comparing `fxapicom-0.1.1/README.md` & `fxapicom-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 Fxapi Python Client is the official Python Wrapper around the fxapi [API](https://fxapi.com/).
 
 ## Installation
 
 Install from pip:
 ````sh
-pip install fxapi
+pip install fxapicom
 ````
 
 Install from code:
 ````sh
 pip install git+https://github.com/everapihq/fxapi-python.git
 ````
 
 ## Usage
 
 All curencyapi API requests are made using the `Client` class. This class must be initialized with your API access key string. [Where is my API access key?](https://app.fxapi.com/dashboard)
 
 In your Python application, import `fxapi` and pass authentication information to initialize it:
 
 ````python
-import fxapi
-client = fxapi.Client('API_KEY')
+import fxapicom
+client = fxapicom.Client('API_KEY')
 ````
 
 ### Retrieve Status
 
 ```python
 
 print(client.status())
```

### Comparing `fxapicom-0.1.1/setup.py` & `fxapicom-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='fxapicom',
-    version='0.1.1',
+    version='0.1.2',
     packages=['fxapicom'],
     url='https://github.com/everapihq/fxapi-python',
     license='MIT',
     author='Everapi',
     author_email='office@everapi.com',
     description='Fxapi Python Client',
     keywords = ['exchange rates api', 'exchange rates', 'rates api', 'fxapi'],
```

### Comparing `fxapicom-0.1.1/fxapicom/client.py` & `fxapicom-0.1.2/fxapicom/client.py`

 * *Files identical despite different names*

