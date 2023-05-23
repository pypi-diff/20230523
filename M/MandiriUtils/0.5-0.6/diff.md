# Comparing `tmp/MandiriUtils-0.5.tar.gz` & `tmp/MandiriUtils-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MandiriUtils-0.5.tar", last modified: Tue May 23 06:07:36 2023, max compression
+gzip compressed data, was "MandiriUtils-0.6.tar", last modified: Tue May 23 07:37:42 2023, max compression
```

## Comparing `MandiriUtils-0.5.tar` & `MandiriUtils-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 06:07:36.958264 MandiriUtils-0.5/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.5/LICENSE.txt
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 06:07:36.958264 MandiriUtils-0.5/MandiriUtils/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     2690 2023-05-23 06:04:50.000000 MandiriUtils-0.5/MandiriUtils/Client.py
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.5/MandiriUtils/__init__.py
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 06:07:36.958264 MandiriUtils-0.5/MandiriUtils.egg-info/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 06:07:36.000000 MandiriUtils-0.5/MandiriUtils.egg-info/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 06:07:36.000000 MandiriUtils-0.5/MandiriUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 06:07:36.000000 MandiriUtils-0.5/MandiriUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 06:07:36.000000 MandiriUtils-0.5/MandiriUtils.egg-info/requires.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 06:07:36.000000 MandiriUtils-0.5/MandiriUtils.egg-info/top_level.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 06:07:36.958264 MandiriUtils-0.5/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.5/README.md
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.5/README.rst
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 06:07:36.958264 MandiriUtils-0.5/setup.cfg
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 06:06:14.000000 MandiriUtils-0.5/setup.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 07:37:42.393032 MandiriUtils-0.6/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.6/LICENSE.txt
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 07:37:42.393032 MandiriUtils-0.6/MandiriUtils/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     2755 2023-05-23 07:36:03.000000 MandiriUtils-0.6/MandiriUtils/Client.py
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.6/MandiriUtils/__init__.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 07:37:42.393032 MandiriUtils-0.6/MandiriUtils.egg-info/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/requires.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 07:37:42.000000 MandiriUtils-0.6/MandiriUtils.egg-info/top_level.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 07:37:42.393032 MandiriUtils-0.6/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.6/README.md
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.6/README.rst
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 07:37:42.393032 MandiriUtils-0.6/setup.cfg
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 07:36:12.000000 MandiriUtils-0.6/setup.py
```

### Comparing `MandiriUtils-0.5/LICENSE.txt` & `MandiriUtils-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.5/MandiriUtils/Client.py` & `MandiriUtils-0.6/MandiriUtils/Client.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,25 @@
         self.access_token = access_token
         self.timestamp = timestamp
         self.signature = signature
         self.success = success
         self.message = message
 
 class Client(object):
-    def __init__(self, url, pk_pass, client_id, client_secret, pk_path='', pk='') -> None:
+    def __init__(self, url, pk_pass, client_id, client_secret, pk_path='', pk='', tz_offset='+07:00') -> None:
         if pk_path == '' and pk == '':
             raise Exception("pk_path or pk is required")
         
         self.url = url
         self.pk_path = pk_path
         self.pk = pk
         self.pk_pass = pk_pass
         self.client_id = client_id
         self.client_secret = client_secret
+        self.tz_offset = tz_offset
 
     def load_privatekey(self):
         if self.pk != '':
             return RSA.importKey(self.pk, self.pk_pass)
         return RSA.importKey(open(self.pk_path).read(), self.pk_pass)
 
 
@@ -49,15 +50,15 @@
         return signature
 
     def minified_data(self, data):
         string = json.dumps(data, separators=(',', ':'))
         return string
 
     def get_token(self):
-        local_time = datetime.now().strftime('%Y-%m-%dT%H:%M:%S+07:00') 
+        local_time = datetime.now().strftime('%Y-%m-%dT%H:%M:%S') + self.tz_offset
         data = "{}|{}".format(self.client_id, local_time)
 
         private_key = self.load_privatekey()
         signature = self.generate_signature(data, private_key)
 
         req_headers = {
             "X-CLIENT-KEY": "{}".format(self.client_id),
```

### Comparing `MandiriUtils-0.5/MandiriUtils.egg-info/PKG-INFO` & `MandiriUtils-0.6/MandiriUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.5
+Version: 0.6
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_05.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_06.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.5/PKG-INFO` & `MandiriUtils-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.5
+Version: 0.6
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_05.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_06.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.5/setup.py` & `MandiriUtils-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'MandiriUtils',         
   packages = ['MandiriUtils'],   
-  version = '0.5',      
+  version = '0.6',      
   license='MIT',        
   description = 'Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API',
   author = 'Hanif Amal Robbani',       
   author_email = 'dev.har07@gmail.com',
   url = 'https://github.com/har07',
-  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_05.tar.gz', 
+  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_06.tar.gz', 
   keywords = ['banking', 'signature', 'token', 'mandiri'], 
   install_requires=[
           'pycryptodome==3.17.0',
           'requests==2.22.0',
           'pyjks==20.0.0',
       ],
   classifiers=[
```

