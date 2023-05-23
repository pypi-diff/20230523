# Comparing `tmp/elementapi-0.4.tar.gz` & `tmp/elementapi-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elementapi-0.4.tar", last modified: Tue Mar 14 10:26:44 2023, max compression
+gzip compressed data, was "elementapi-0.5.tar", last modified: Tue May 23 09:31:49 2023, max compression
```

## Comparing `elementapi-0.4.tar` & `elementapi-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 scratch   (1000) scratch   (1000)        0 2023-03-14 10:26:44.024557 elementapi-0.4/
--rw-rw-r--   0 scratch   (1000) scratch   (1000)      551 2023-03-14 10:26:44.024557 elementapi-0.4/PKG-INFO
-drwxrwxr-x   0 scratch   (1000) scratch   (1000)        0 2023-03-14 10:26:44.024557 elementapi-0.4/elementapi/
--rw-rw-r--   0 scratch   (1000) scratch   (1000)    12613 2023-03-14 09:42:42.000000 elementapi-0.4/elementapi/__init__.py
-drwxrwxr-x   0 scratch   (1000) scratch   (1000)        0 2023-03-14 10:26:44.024557 elementapi-0.4/elementapi.egg-info/
--rw-rw-r--   0 scratch   (1000) scratch   (1000)      551 2023-03-14 10:26:44.000000 elementapi-0.4/elementapi.egg-info/PKG-INFO
--rw-rw-r--   0 scratch   (1000) scratch   (1000)      200 2023-03-14 10:26:44.000000 elementapi-0.4/elementapi.egg-info/SOURCES.txt
--rw-rw-r--   0 scratch   (1000) scratch   (1000)        1 2023-03-14 10:26:44.000000 elementapi-0.4/elementapi.egg-info/dependency_links.txt
--rw-rw-r--   0 scratch   (1000) scratch   (1000)        9 2023-03-14 10:26:44.000000 elementapi-0.4/elementapi.egg-info/requires.txt
--rw-rw-r--   0 scratch   (1000) scratch   (1000)       11 2023-03-14 10:26:44.000000 elementapi-0.4/elementapi.egg-info/top_level.txt
--rw-rw-r--   0 scratch   (1000) scratch   (1000)       38 2023-03-14 10:26:44.024557 elementapi-0.4/setup.cfg
--rw-rw-r--   0 scratch   (1000) scratch   (1000)      666 2023-03-14 10:00:24.000000 elementapi-0.4/setup.py
+drwxrwxr-x   0 scratch   (1000) scratch   (1000)        0 2023-05-23 09:31:49.910418 elementapi-0.5/
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)      551 2023-05-23 09:31:49.910418 elementapi-0.5/PKG-INFO
+drwxrwxr-x   0 scratch   (1000) scratch   (1000)        0 2023-05-23 09:31:49.910418 elementapi-0.5/elementapi/
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)    13059 2023-05-23 09:29:34.000000 elementapi-0.5/elementapi/__init__.py
+drwxrwxr-x   0 scratch   (1000) scratch   (1000)        0 2023-05-23 09:31:49.910418 elementapi-0.5/elementapi.egg-info/
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)      551 2023-05-23 09:31:49.000000 elementapi-0.5/elementapi.egg-info/PKG-INFO
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)      200 2023-05-23 09:31:49.000000 elementapi-0.5/elementapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)        1 2023-05-23 09:31:49.000000 elementapi-0.5/elementapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)        9 2023-05-23 09:31:49.000000 elementapi-0.5/elementapi.egg-info/requires.txt
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)       11 2023-05-23 09:31:49.000000 elementapi-0.5/elementapi.egg-info/top_level.txt
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)       38 2023-05-23 09:31:49.910418 elementapi-0.5/setup.cfg
+-rw-rw-r--   0 scratch   (1000) scratch   (1000)      666 2023-05-23 09:31:28.000000 elementapi-0.5/setup.py
```

### Comparing `elementapi-0.4/PKG-INFO` & `elementapi-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementapi
-Version: 0.4
+Version: 0.5
 Summary: element-iot api client lib
 Home-page: https://github.com/ZennerIoT/python-elementapi
 Download-URL: https://github.com/ZennerIoT/python-elementapi/archive/master.zip
 Author: Stefan Reiser
 Author-email: sr@zenner-iot.com
 Keywords: client,rest,element-iot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elementapi-0.4/elementapi/__init__.py` & `elementapi-0.5/elementapi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return 'ELEMENTAPI Exception, caused by `%s` %s : %s' % (
             str(self.cause),
             "with status code %s" % self.status_code if self.status_code else '',
             self.msg
         )
 
     def __repr__(self):
-       return self._str()
+        return self._str()
 
     def __str__(self):
         return self._str()
 
 
 def get_body(resp):
     try:
@@ -50,26 +50,38 @@
                 r = resp.text
         else:
             r = resp.text
 
     return r
 
 
-
 class ElementAPI:
     apitoken = None
     baseurl = "element-iot.com"
     https = True
     port = 443
     apiversion = "/"
     sync = False
     proxies = None
+    custom_ca = None
+    https_no_verify = False
     headers = {'Accept': 'application/json'}
 
-    def __init__(self, apitoken, baseurl=None, https=True, port=None, apiversion=1, sync=False, proxies=None):
+    def __init__(
+            self,
+            apitoken,
+            baseurl=None,
+            https=True,
+            port=None,
+            apiversion=1,
+            sync=False,
+            proxies=None,
+            custom_ca=None,
+            https_no_verify=False
+    ):
         if baseurl:
             self.baseurl = baseurl
 
         self.https = https
         if port:
             self.port = port
         elif not port and https:
@@ -83,20 +95,28 @@
 
         if proxies:
             if type(proxies) is dict:
                 self.proxies = proxies
             elif type(proxies) is str:
                 # TODO: check if string ?
                 self.proxies = {'http%s' % ('s' if https else ''): proxies}
-                
+
+        self.custom_ca = custom_ca
+        self.https_no_verify = https_no_verify
+
         self.requestargs = {
             'headers': self.headers,
             'proxies': self.proxies
         }
 
+        if self.custom_ca:
+            self.requestargs['verify'] = self.custom_ca
+
+        if self.https_no_verify:
+            self.requestargs['verify'] = False
 
     # TODO: allow plain string paths !
     def genurl(self, _path=None, **opts):
         if 'limit' not in opts or not opts['limit'] or opts['limit'] > 100:
             opts['limit'] = 100
 
         if opts.get('nolimit', False):
@@ -163,15 +183,15 @@
                 )
                 self._log_request("GET", url)
                 last_response = resp
                 resp = requests.get(url, **self.requestargs)
 
                 if resp.status_code >= 400:
                     if resp.status_code == 429 and not raise_rl:
-                        # hit reate-limit
+                        # hit create-limit
 
                         # sleep|block
 
                         rl_s = int(resp.headers.get('x-ratelimit-reset', 0))
                         logger.info('hit rate limit, blocking further requests for %s ms' % rl_s)
 
                         # keep last
```

### Comparing `elementapi-0.4/elementapi.egg-info/PKG-INFO` & `elementapi-0.5/elementapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementapi
-Version: 0.4
+Version: 0.5
 Summary: element-iot api client lib
 Home-page: https://github.com/ZennerIoT/python-elementapi
 Download-URL: https://github.com/ZennerIoT/python-elementapi/archive/master.zip
 Author: Stefan Reiser
 Author-email: sr@zenner-iot.com
 Keywords: client,rest,element-iot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elementapi-0.4/setup.py` & `elementapi-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
   name='elementapi',
   packages=['elementapi'],
-  version='0.4',
+  version='0.5',
   description='element-iot api client lib',
   author='Stefan Reiser',
   author_email='sr@zenner-iot.com',
   url='https://github.com/ZennerIoT/python-elementapi',
   download_url='https://github.com/ZennerIoT/python-elementapi/archive/master.zip',
   keywords=['client', 'rest', 'element-iot'],
   classifiers =[
```

