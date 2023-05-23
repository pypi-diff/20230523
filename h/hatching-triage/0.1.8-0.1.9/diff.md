# Comparing `tmp/hatching-triage-0.1.8.tar.gz` & `tmp/hatching-triage-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatching-triage-0.1.8.tar", last modified: Wed Nov 16 09:52:06 2022, max compression
+gzip compressed data, was "hatching-triage-0.1.9.tar", last modified: Thu Mar 16 15:01:38 2023, max compression
```

## Comparing `hatching-triage-0.1.8.tar` & `hatching-triage-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2022-11-16 09:52:06.696663 hatching-triage-0.1.8/
--rw-rw-r--   0 jbr       (1000) jbr       (1000)     4181 2022-11-16 09:52:06.696663 hatching-triage-0.1.8/PKG-INFO
--rw-rw-r--   0 jbr       (1000) jbr       (1000)     2445 2021-11-04 19:43:17.000000 hatching-triage-0.1.8/README.md
-drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2022-11-16 09:52:06.692663 hatching-triage-0.1.8/cli/
--rw-rw-r--   0 jbr       (1000) jbr       (1000)       58 2021-11-04 19:43:17.000000 hatching-triage-0.1.8/cli/__init__.py
--rw-rw-r--   0 jbr       (1000) jbr       (1000)    12229 2022-11-15 14:43:43.000000 hatching-triage-0.1.8/cli/triage.py
--rw-rw-r--   0 jbr       (1000) jbr       (1000)     1124 2022-01-18 00:44:08.000000 hatching-triage-0.1.8/cli/tui.py
-drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2022-11-16 09:52:06.692663 hatching-triage-0.1.8/hatching_triage.egg-info/
--rw-rw-r--   0 jbr       (1000) jbr       (1000)     4181 2022-11-16 09:52:06.000000 hatching-triage-0.1.8/hatching_triage.egg-info/PKG-INFO
--rw-rw-r--   0 jbr       (1000) jbr       (1000)      352 2022-11-16 09:52:06.000000 hatching-triage-0.1.8/hatching_triage.egg-info/SOURCES.txt
--rw-rw-r--   0 jbr       (1000) jbr       (1000)        1 2022-11-16 09:52:06.000000 hatching-triage-0.1.8/hatching_triage.egg-info/dependency_links.txt
--rw-rw-r--   0 jbr       (1000) jbr       (1000)       43 2022-11-16 09:52:06.000000 hatching-triage-0.1.8/hatching_triage.egg-info/entry_points.txt
--rw-rw-r--   0 jbr       (1000) jbr       (1000)       48 2022-11-16 09:52:06.000000 hatching-triage-0.1.8/hatching_triage.egg-info/requires.txt
--rw-rw-r--   0 jbr       (1000) jbr       (1000)       11 2022-11-16 09:52:06.000000 hatching-triage-0.1.8/hatching_triage.egg-info/top_level.txt
--rw-rw-r--   0 jbr       (1000) jbr       (1000)       38 2022-11-16 09:52:06.696663 hatching-triage-0.1.8/setup.cfg
--rw-rw-r--   0 jbr       (1000) jbr       (1000)      752 2022-11-15 14:43:43.000000 hatching-triage-0.1.8/setup.py
-drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2022-11-16 09:52:06.692663 hatching-triage-0.1.8/triage/
--rw-rw-r--   0 jbr       (1000) jbr       (1000)      110 2021-11-04 19:43:17.000000 hatching-triage-0.1.8/triage/__init__.py
--rw-rw-r--   0 jbr       (1000) jbr       (1000)    17433 2022-11-15 14:43:43.000000 hatching-triage-0.1.8/triage/client.py
--rw-rw-r--   0 jbr       (1000) jbr       (1000)     1400 2022-01-18 00:44:08.000000 hatching-triage-0.1.8/triage/pagination.py
+drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2023-03-16 15:01:38.708245 hatching-triage-0.1.9/
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)     4181 2023-03-16 15:01:38.708245 hatching-triage-0.1.9/PKG-INFO
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)     2445 2021-11-04 19:43:17.000000 hatching-triage-0.1.9/README.md
+drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2023-03-16 15:01:38.708245 hatching-triage-0.1.9/cli/
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)       58 2021-11-04 19:43:17.000000 hatching-triage-0.1.9/cli/__init__.py
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)    12229 2022-11-15 14:43:43.000000 hatching-triage-0.1.9/cli/triage.py
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)     1124 2022-01-18 00:44:08.000000 hatching-triage-0.1.9/cli/tui.py
+drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2023-03-16 15:01:38.708245 hatching-triage-0.1.9/hatching_triage.egg-info/
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)     4181 2023-03-16 15:01:38.000000 hatching-triage-0.1.9/hatching_triage.egg-info/PKG-INFO
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)      352 2023-03-16 15:01:38.000000 hatching-triage-0.1.9/hatching_triage.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)        1 2023-03-16 15:01:38.000000 hatching-triage-0.1.9/hatching_triage.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)       43 2023-03-16 15:01:38.000000 hatching-triage-0.1.9/hatching_triage.egg-info/entry_points.txt
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)       48 2023-03-16 15:01:38.000000 hatching-triage-0.1.9/hatching_triage.egg-info/requires.txt
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)       11 2023-03-16 15:01:38.000000 hatching-triage-0.1.9/hatching_triage.egg-info/top_level.txt
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)       38 2023-03-16 15:01:38.708245 hatching-triage-0.1.9/setup.cfg
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)      752 2023-03-16 15:01:03.000000 hatching-triage-0.1.9/setup.py
+drwxrwxr-x   0 jbr       (1000) jbr       (1000)        0 2023-03-16 15:01:38.708245 hatching-triage-0.1.9/triage/
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)      110 2021-11-04 19:43:17.000000 hatching-triage-0.1.9/triage/__init__.py
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)    18155 2023-03-16 15:01:03.000000 hatching-triage-0.1.9/triage/client.py
+-rw-rw-r--   0 jbr       (1000) jbr       (1000)     1405 2023-03-16 15:01:03.000000 hatching-triage-0.1.9/triage/pagination.py
```

### Comparing `hatching-triage-0.1.8/PKG-INFO` & `hatching-triage-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatching-triage
-Version: 0.1.8
+Version: 0.1.9
 Summary: API client and CLI for Hatching Triage
 Home-page: https://hatching.io/
 Author: Hatching B.V.
 Author-email: info@hatching.io
 License: UNKNOWN
 Description: 
         # Usage
```

### Comparing `hatching-triage-0.1.8/README.md` & `hatching-triage-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hatching-triage-0.1.8/cli/triage.py` & `hatching-triage-0.1.9/cli/triage.py`

 * *Files identical despite different names*

### Comparing `hatching-triage-0.1.8/cli/tui.py` & `hatching-triage-0.1.9/cli/tui.py`

 * *Files identical despite different names*

### Comparing `hatching-triage-0.1.8/hatching_triage.egg-info/PKG-INFO` & `hatching-triage-0.1.9/hatching_triage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatching-triage
-Version: 0.1.8
+Version: 0.1.9
 Summary: API client and CLI for Hatching Triage
 Home-page: https://hatching.io/
 Author: Hatching B.V.
 Author-email: info@hatching.io
 License: UNKNOWN
 Description: 
         # Usage
```

### Comparing `hatching-triage-0.1.8/setup.py` & `hatching-triage-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hatching-triage",
-    version="0.1.8",
+    version="0.1.9",
     author="Hatching B.V.",
     author_email="info@hatching.io",
     description="API client and CLI for Hatching Triage",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://hatching.io/",
     packages=setuptools.find_packages(),
```

### Comparing `hatching-triage-0.1.8/triage/client.py` & `hatching-triage-0.1.9/triage/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 settings = s.merge_environment_settings(r.url, {}, None, False, None)
                 res = s.send(r.prepare(), **settings)
                 res.raise_for_status()
                 return res.json()
         except exceptions.HTTPError as err:
             raise ServerError(err)
 
-    def submit_sample_file(self, filename, file, interactive=False, profiles=None, password=None):
+    def submit_sample_file(self, filename, file, interactive=False, profiles=None, password=None, timeout=150, network="internet"):
         """
         Submit a file for analysis on Triage.
 
         Parameters:
             filename (str):
                 The name of the file
             file (file):
@@ -72,14 +72,18 @@
                     {
                         "pick": "file1.exe", // for archives
                         "profile": "w7_long"
                     }
                 ]
             password (str):
                 Password for the archive sample
+            timeout: (int):
+                Timeout of the analysis
+            network (str):
+                Type of network routing to use ("internet" | "drop" | "tor" | "sim200" | "sim404" | "simnx")
         Returns:
             response (dict):
                 {
                     'id': '200923-4zhlr84m42',
                     'status': 'pending',
                     'kind': 'file',
                     'filename': 'test.exe',
@@ -89,14 +93,18 @@
         """
         if profiles is None:
             profiles = []
         d = {
             'kind': 'file',
             'interactive': interactive,
             'profiles': profiles,
+            'defaults': {
+                'timeout': timeout,
+                'network': network
+            }
         }
         if password:
             d['password'] = password
         body, content_type = encode_multipart_formdata({
             '_json': json.dumps(d),
             'file': (filename, file),
         })
@@ -191,14 +199,27 @@
         if pick is None:
             pick = []
         return self._req_json('POST', '/v0/samples/%s/profile' % sample_id, {
             'auto': True,
             'pick': pick,
         })
 
+    def org_samples(self, max=20):
+        """
+        Returns a Paginator object with organisation samples.
+
+        Parameters:
+            max (int): The maximum amount of samples to return
+
+        Returns:
+            Paginator (object):
+                Loop over this object to get the samples
+        """
+        return Paginator(self, '/v0/samples?subset=org', max)
+
     def owned_samples(self, max=20):
         """
         Returns a Paginator object with owned samples.
 
         Parameters:
             max (int): The maximum amount of samples to return
 
@@ -461,15 +482,15 @@
     def create_profile(self, name, tags, network, timeout):
         """
         Create a new profile.
 
         Parameters:
             name (str): The name of the profile
             tags (list): Tags for the profile, list of strings
-            network (list): network used when running the sample (Currently available : "", "drop", "internet")
+            network (str): network used when running the sample (Currently available : "", "drop", "internet")
             timeout (int): The timeout of the profile
 
         Returns:
             response (dict):
                 {}, empty dict
         """
         return self._req_json("POST", "/v0/profiles", data={
```

### Comparing `hatching-triage-0.1.8/triage/pagination.py` & `hatching-triage-0.1.9/triage/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __init__(self, client, path, max):
         self._client = client
         self._path = path
         self._offset = None
         self._limit = 200
         self._current_page = []
         self._eof = False
-        self._max = max
+        self._max = int(max)
         self._counter = 0
 
     def __iter__(self):
         return self
 
     def _fetch_next_page(self):
         if '?' in self._path:
```

