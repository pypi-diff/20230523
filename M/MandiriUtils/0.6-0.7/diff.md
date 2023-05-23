# Comparing `tmp/MandiriUtils-0.6.tar.gz` & `tmp/MandiriUtils-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MandiriUtils-0.6.tar", last modified: Tue May 23 07:37:42 2023, max compression
+gzip compressed data, was "MandiriUtils-0.7.tar", last modified: Tue May 23 08:02:04 2023, max compression
```

## Comparing `MandiriUtils-0.6.tar` & `MandiriUtils-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 07:37:42.393032 MandiriUtils-0.6/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.6/LICENSE.txt
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 07:37:42.393032 MandiriUtils-0.6/MandiriUtils/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     2755 2023-05-23 07:36:03.000000 MandiriUtils-0.6/MandiriUtils/Client.py
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.6/MandiriUtils/__init__.py
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 07:37:42.393032 MandiriUtils-0.6/MandiriUtils.egg-info/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/requires.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/top_level.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 07:37:42.393032 MandiriUtils-0.6/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.6/README.md
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.6/README.rst
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 07:37:42.393032 MandiriUtils-0.6/setup.cfg
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 07:36:12.000000 MandiriUtils-0.6/setup.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 08:02:04.539270 MandiriUtils-0.7/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.7/LICENSE.txt
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 08:02:04.539270 MandiriUtils-0.7/MandiriUtils/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     2739 2023-05-23 07:58:28.000000 MandiriUtils-0.7/MandiriUtils/Client.py
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.7/MandiriUtils/__init__.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 08:02:04.539270 MandiriUtils-0.7/MandiriUtils.egg-info/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/requires.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/top_level.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 08:02:04.539270 MandiriUtils-0.7/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.7/README.md
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.7/README.rst
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 08:02:04.539270 MandiriUtils-0.7/setup.cfg
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 07:58:41.000000 MandiriUtils-0.7/setup.py
```

### Comparing `MandiriUtils-0.6/LICENSE.txt` & `MandiriUtils-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.6/MandiriUtils/Client.py` & `MandiriUtils-0.7/MandiriUtils/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,14 @@
             "X-SIGNATURE": "{}".format(signature),
             "Content-Type": "application/x-www-form-urlencoded",
         }
         params = {
             "grantType":"client_credentials"
         }
         response = requests.post(
-            f"{self.url}/openapi/auth/v2.0/access-token/b2b", headers=req_headers, data=params
+            f"{self.url}/openapi/auth/token", headers=req_headers, data=params
         )
         if response.status_code == 200:
             resp_data = response.json()
             return LoginResult(resp_data['accessToken'], local_time, signature)
         else:
             return LoginResult("", local_time, signature, False, response.text)
```

### Comparing `MandiriUtils-0.6/MandiriUtils.egg-info/PKG-INFO` & `MandiriUtils-0.7/MandiriUtils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.6
+Version: 0.7
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_06.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_07.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.6/PKG-INFO` & `MandiriUtils-0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.6
+Version: 0.7
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_06.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_07.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.6/setup.py` & `MandiriUtils-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'MandiriUtils',         
   packages = ['MandiriUtils'],   
-  version = '0.6',      
+  version = '0.7',      
   license='MIT',        
   description = 'Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API',
   author = 'Hanif Amal Robbani',       
   author_email = 'dev.har07@gmail.com',
   url = 'https://github.com/har07',
-  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_06.tar.gz', 
+  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_07.tar.gz', 
   keywords = ['banking', 'signature', 'token', 'mandiri'], 
   install_requires=[
           'pycryptodome==3.17.0',
           'requests==2.22.0',
           'pyjks==20.0.0',
       ],
   classifiers=[
```

