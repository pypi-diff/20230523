# Comparing `tmp/MandiriUtils-0.7.tar.gz` & `tmp/MandiriUtils-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MandiriUtils-0.7.tar", last modified: Tue May 23 08:02:04 2023, max compression
+gzip compressed data, was "MandiriUtils-0.8.tar", last modified: Tue May 23 09:26:29 2023, max compression
```

## Comparing `MandiriUtils-0.7.tar` & `MandiriUtils-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 08:02:04.539270 MandiriUtils-0.7/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.7/LICENSE.txt
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 08:02:04.539270 MandiriUtils-0.7/MandiriUtils/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     2739 2023-05-23 07:58:28.000000 MandiriUtils-0.7/MandiriUtils/Client.py
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.7/MandiriUtils/__init__.py
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 08:02:04.539270 MandiriUtils-0.7/MandiriUtils.egg-info/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/requires.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 08:02:04.000000 MandiriUtils-0.7/MandiriUtils.egg-info/top_level.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 08:02:04.539270 MandiriUtils-0.7/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.7/README.md
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.7/README.rst
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 08:02:04.539270 MandiriUtils-0.7/setup.cfg
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 07:58:41.000000 MandiriUtils-0.7/setup.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:26:29.375113 MandiriUtils-0.8/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.8/LICENSE.txt
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:26:29.371113 MandiriUtils-0.8/MandiriUtils/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     2744 2023-05-23 09:25:08.000000 MandiriUtils-0.8/MandiriUtils/Client.py
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.8/MandiriUtils/__init__.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 09:26:29.375113 MandiriUtils-0.8/MandiriUtils.egg-info/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/requires.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 09:26:29.000000 MandiriUtils-0.8/MandiriUtils.egg-info/top_level.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 09:26:29.375113 MandiriUtils-0.8/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.8/README.md
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.8/README.rst
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 09:26:29.375113 MandiriUtils-0.8/setup.cfg
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 09:25:30.000000 MandiriUtils-0.8/setup.py
```

### Comparing `MandiriUtils-0.7/LICENSE.txt` & `MandiriUtils-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.7/MandiriUtils/Client.py` & `MandiriUtils-0.8/MandiriUtils/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return signature
 
     def minified_data(self, data):
         string = json.dumps(data, separators=(',', ':'))
         return string
 
     def get_token(self):
-        local_time = datetime.now().strftime('%Y-%m-%dT%H:%M:%S') + self.tz_offset
+        local_time = datetime.now().strftime('%Y-%m-%dT%H:%M:%S.000T') + self.tz_offset
         data = "{}|{}".format(self.client_id, local_time)
 
         private_key = self.load_privatekey()
         signature = self.generate_signature(data, private_key)
 
         req_headers = {
             "X-CLIENT-KEY": "{}".format(self.client_id),
```

### Comparing `MandiriUtils-0.7/MandiriUtils.egg-info/PKG-INFO` & `MandiriUtils-0.8/MandiriUtils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.7
+Version: 0.8
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_07.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_08.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.7/PKG-INFO` & `MandiriUtils-0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.7
+Version: 0.8
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_07.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_08.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.7/setup.py` & `MandiriUtils-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'MandiriUtils',         
   packages = ['MandiriUtils'],   
-  version = '0.7',      
+  version = '0.8',      
   license='MIT',        
   description = 'Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API',
   author = 'Hanif Amal Robbani',       
   author_email = 'dev.har07@gmail.com',
   url = 'https://github.com/har07',
-  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_07.tar.gz', 
+  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_08.tar.gz', 
   keywords = ['banking', 'signature', 'token', 'mandiri'], 
   install_requires=[
           'pycryptodome==3.17.0',
           'requests==2.22.0',
           'pyjks==20.0.0',
       ],
   classifiers=[
```

