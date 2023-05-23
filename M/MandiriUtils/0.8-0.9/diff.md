# Comparing `tmp/MandiriUtils-0.8.tar.gz` & `tmp/MandiriUtils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MandiriUtils-0.8.tar", last modified: Tue May 23 09:26:29 2023, max compression
+gzip compressed data, was "MandiriUtils-0.9.tar", last modified: Tue May 23 09:37:49 2023, max compression
```

## Comparing `MandiriUtils-0.8.tar` & `MandiriUtils-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:26:29.375113 MandiriUtils-0.8/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.8/LICENSE.txt
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:26:29.371113 MandiriUtils-0.8/MandiriUtils/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     2744 2023-05-23 09:25:08.000000 MandiriUtils-0.8/MandiriUtils/Client.py
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.8/MandiriUtils/__init__.py
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:26:29.375113 MandiriUtils-0.8/MandiriUtils.egg-info/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/requires.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/top_level.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 09:26:29.375113 MandiriUtils-0.8/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.8/README.md
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.8/README.rst
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 09:26:29.375113 MandiriUtils-0.8/setup.cfg
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 09:25:30.000000 MandiriUtils-0.8/setup.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:37:49.223414 MandiriUtils-0.9/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.9/LICENSE.txt
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:37:49.219414 MandiriUtils-0.9/MandiriUtils/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     2745 2023-05-23 09:36:49.000000 MandiriUtils-0.9/MandiriUtils/Client.py
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.9/MandiriUtils/__init__.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:37:49.223414 MandiriUtils-0.9/MandiriUtils.egg-info/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 09:37:49.000000 MandiriUtils-0.9/MandiriUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 09:37:49.000000 MandiriUtils-0.9/MandiriUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 09:37:49.000000 MandiriUtils-0.9/MandiriUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 09:37:49.000000 MandiriUtils-0.9/MandiriUtils.egg-info/requires.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 09:37:49.000000 MandiriUtils-0.9/MandiriUtils.egg-info/top_level.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 09:37:49.223414 MandiriUtils-0.9/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.9/README.md
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.9/README.rst
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 09:37:49.223414 MandiriUtils-0.9/setup.cfg
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 09:37:09.000000 MandiriUtils-0.9/setup.py
```

### Comparing `MandiriUtils-0.8/LICENSE.txt` & `MandiriUtils-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.8/MandiriUtils/Client.py` & `MandiriUtils-0.9/MandiriUtils/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         req_headers = {
             "X-CLIENT-KEY": "{}".format(self.client_id),
             "X-TIMESTAMP": "{}".format(local_time),
             "X-SIGNATURE": "{}".format(signature),
             "Content-Type": "application/x-www-form-urlencoded",
         }
         params = {
-            "grantType":"client_credentials"
+            "grant_type":"client_credentials"
         }
         response = requests.post(
             f"{self.url}/openapi/auth/token", headers=req_headers, data=params
         )
         if response.status_code == 200:
             resp_data = response.json()
             return LoginResult(resp_data['accessToken'], local_time, signature)
```

### Comparing `MandiriUtils-0.8/MandiriUtils.egg-info/PKG-INFO` & `MandiriUtils-0.9/MandiriUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.8
+Version: 0.9
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_08.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_09.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.8/PKG-INFO` & `MandiriUtils-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.8
+Version: 0.9
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_08.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_09.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.8/setup.py` & `MandiriUtils-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'MandiriUtils',         
   packages = ['MandiriUtils'],   
-  version = '0.8',      
+  version = '0.9',      
   license='MIT',        
   description = 'Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API',
   author = 'Hanif Amal Robbani',       
   author_email = 'dev.har07@gmail.com',
   url = 'https://github.com/har07',
-  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_08.tar.gz', 
+  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_09.tar.gz', 
   keywords = ['banking', 'signature', 'token', 'mandiri'], 
   install_requires=[
           'pycryptodome==3.17.0',
           'requests==2.22.0',
           'pyjks==20.0.0',
       ],
   classifiers=[
```

