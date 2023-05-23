# Comparing `tmp/MandiriUtils-0.2.tar.gz` & `tmp/MandiriUtils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MandiriUtils-0.2.tar", last modified: Tue May 23 03:12:09 2023, max compression
+gzip compressed data, was "MandiriUtils-0.4.tar", last modified: Tue May 23 05:42:19 2023, max compression
```

## Comparing `MandiriUtils-0.2.tar` & `MandiriUtils-0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:12:09.379016 MandiriUtils-0.2/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.2/LICENSE.txt
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:12:09.375016 MandiriUtils-0.2/MandiriUtils/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     2457 2023-05-23 02:47:09.000000 MandiriUtils-0.2/MandiriUtils/Client.py
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.2/MandiriUtils/__init__.py
-drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 03:12:09.379016 MandiriUtils-0.2/MandiriUtils.egg-info/
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      267 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/requires.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 03:12:09.000000 MandiriUtils-0.2/MandiriUtils.egg-info/top_level.txt
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 03:12:09.379016 MandiriUtils-0.2/PKG-INFO
--rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.2/README.md
--rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 03:12:09.379016 MandiriUtils-0.2/setup.cfg
--rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 03:12:06.000000 MandiriUtils-0.2/setup.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 05:42:19.265515 MandiriUtils-0.4/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1061 2023-05-23 02:56:32.000000 MandiriUtils-0.4/LICENSE.txt
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 05:42:19.265515 MandiriUtils-0.4/MandiriUtils/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     2675 2023-05-23 05:39:05.000000 MandiriUtils-0.4/MandiriUtils/Client.py
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       51 2023-05-23 03:10:49.000000 MandiriUtils-0.4/MandiriUtils/__init__.py
+drwxrwxr-x   0 hanif     (1000) hanif     (1000)        0 2023-05-23 05:42:19.265515 MandiriUtils-0.4/MandiriUtils.egg-info/
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 05:42:19.000000 MandiriUtils-0.4/MandiriUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      278 2023-05-23 05:42:19.000000 MandiriUtils-0.4/MandiriUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)        1 2023-05-23 05:42:19.000000 MandiriUtils-0.4/MandiriUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       52 2023-05-23 05:42:19.000000 MandiriUtils-0.4/MandiriUtils.egg-info/requires.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       13 2023-05-23 05:42:19.000000 MandiriUtils-0.4/MandiriUtils.egg-info/top_level.txt
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      731 2023-05-23 05:42:19.265515 MandiriUtils-0.4/PKG-INFO
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 02:40:14.000000 MandiriUtils-0.4/README.md
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)      112 2023-05-23 05:41:02.000000 MandiriUtils-0.4/README.rst
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)       79 2023-05-23 05:42:19.265515 MandiriUtils-0.4/setup.cfg
+-rw-rw-r--   0 hanif     (1000) hanif     (1000)     1146 2023-05-23 05:39:36.000000 MandiriUtils-0.4/setup.py
```

### Comparing `MandiriUtils-0.2/LICENSE.txt` & `MandiriUtils-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MandiriUtils-0.2/MandiriUtils/Client.py` & `MandiriUtils-0.4/MandiriUtils/Client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,28 @@
         self.access_token = access_token
         self.timestamp = timestamp
         self.signature = signature
         self.success = success
         self.message = message
 
 class Client(object):
-    def __init__(self, url, pk_path, pk_pass, client_id, client_secret) -> None:
+    def __init__(self, url, pk_pass, client_id, client_secret, pk_path='', pk='') -> None:
+        if pk_path == '' and pk == '':
+            raise Exception("pk_path or pk is required")
+        
         self.url = url
         self.pk_path = pk_path
+        self.pk = pk
         self.pk_pass = pk_pass
         self.client_id = client_id
         self.client_secret = client_secret
 
     def load_privatekey(self):
+        if self.pk != '':
+            return RSA.importKey(self.pk, self.pk_pass)
         return RSA.importKey(open(self.pk_path).read(), self.pk_pass)
 
 
     def generate_signature(self, data, private_key):
         digest = SHA256.new()
         digest.update(str.encode(data))
         signer = PKCS1_v1_5.new(private_key)
```

### Comparing `MandiriUtils-0.2/MandiriUtils.egg-info/PKG-INFO` & `MandiriUtils-0.4/MandiriUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.2
+Version: 0.4
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_03.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_04.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.2/PKG-INFO` & `MandiriUtils-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MandiriUtils
-Version: 0.2
+Version: 0.4
 Summary: Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API
 Home-page: https://github.com/har07
-Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_03.tar.gz
+Download-URL: https://github.com/har07/mandiri-utils/archive/refs/tags/v_04.tar.gz
 Author: Hanif Amal Robbani
 Author-email: dev.har07@gmail.com
 License: MIT
 Keywords: banking,signature,token,mandiri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `MandiriUtils-0.2/setup.py` & `MandiriUtils-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'MandiriUtils',         
   packages = ['MandiriUtils'],   
-  version = '0.2',      
+  version = '0.4',      
   license='MIT',        
   description = 'Helper package for requesting token and generating request signatures to be used for consuming Bank Mandiri API',
   author = 'Hanif Amal Robbani',       
   author_email = 'dev.har07@gmail.com',
   url = 'https://github.com/har07',
-  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_03.tar.gz', 
+  download_url = 'https://github.com/har07/mandiri-utils/archive/refs/tags/v_04.tar.gz', 
   keywords = ['banking', 'signature', 'token', 'mandiri'], 
   install_requires=[
           'pycryptodome==3.17.0',
           'requests==2.22.0',
           'pyjks==20.0.0',
       ],
   classifiers=[
```

