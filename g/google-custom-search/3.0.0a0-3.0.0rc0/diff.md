# Comparing `tmp/google-custom-search-3.0.0a0.tar.gz` & `tmp/google-custom-search-3.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-custom-search-3.0.0a0.tar", last modified: Sat Oct 29 06:14:02 2022, max compression
+gzip compressed data, was "google-custom-search-3.0.0rc0.tar", last modified: Tue May 23 15:55:44 2023, max compression
```

## Comparing `google-custom-search-3.0.0a0.tar` & `google-custom-search-3.0.0rc0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:14:02.423434 google-custom-search-3.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2022-10-29 06:14:02.423434 google-custom-search-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:14:02.423434 google-custom-search-3.0.0a0/google_custom_search/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/google_custom_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/google_custom_search/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/google_custom_search/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/google_custom_search/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/google_custom_search/search.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/google_custom_search/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 06:14:02.423434 google-custom-search-3.0.0a0/google_custom_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3009 2022-10-29 06:14:02.000000 google-custom-search-3.0.0a0/google_custom_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-29 06:14:02.000000 google-custom-search-3.0.0a0/google_custom_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 06:14:02.000000 google-custom-search-3.0.0a0/google_custom_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-29 06:14:02.000000 google-custom-search-3.0.0a0/google_custom_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-29 06:14:02.000000 google-custom-search-3.0.0a0/google_custom_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 06:14:02.423434 google-custom-search-3.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-10-29 06:13:55.000000 google-custom-search-3.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:55:44.886177 google-custom-search-3.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-23 15:55:44.886177 google-custom-search-3.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:55:44.886177 google-custom-search-3.0.0rc0/google_custom_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/google_custom_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/google_custom_search/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/google_custom_search/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/google_custom_search/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/google_custom_search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/google_custom_search/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:55:44.886177 google-custom-search-3.0.0rc0/google_custom_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-23 15:55:44.000000 google-custom-search-3.0.0rc0/google_custom_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-23 15:55:44.000000 google-custom-search-3.0.0rc0/google_custom_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:55:44.000000 google-custom-search-3.0.0rc0/google_custom_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 15:55:44.000000 google-custom-search-3.0.0rc0/google_custom_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 15:55:44.000000 google-custom-search-3.0.0rc0/google_custom_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:55:44.886177 google-custom-search-3.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 15:55:33.000000 google-custom-search-3.0.0rc0/setup.py
```

### Comparing `google-custom-search-3.0.0a0/LICENSE` & `google-custom-search-3.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-custom-search-3.0.0a0/PKG-INFO` & `google-custom-search-3.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-custom-search
-Version: 3.0.0a0
+Version: 3.0.0rc0
 Summary: This is for google custom search api.
 Home-page: https://github.com/mc-fdc-dev/google-custom-search
 Author: mc-fdc-dev
 Author-email: masato190411@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `google-custom-search-3.0.0a0/README.md` & `google-custom-search-3.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `google-custom-search-3.0.0a0/google_custom_search/adapter.py` & `google-custom-search-3.0.0rc0/google_custom_search/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,18 +67,18 @@
 
 
 class RequestsAdapter(BaseAdapter):
     "This class is requestsadapter for sync mode."
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.session = Session()
+        self.__session = Session()
 
     def request(self, method: str, path: str, *args, **kwargs) -> dict:
-        return self.session.request(
+        return self.__session.request(
             method, self.APIURL + path, *args, **kwargs
         ).json()
 
     def search(self, *args, **kwargs) -> List[Item]:
         return self._from_dict(
             self.request(
                 "GET", "/", params=self._payload_maker(*args, **kwargs)
@@ -90,18 +90,18 @@
     "This class is aiohttpadapter for async mode."
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if not async_mode:
             raise AsyncError(
                 "This adapter use aiohttp, so please install aiohttp")
-        self.session = ClientSession(*args, **kwargs)
+        self.__session = ClientSession(*args, **kwargs)
 
     async def request(self, method: str, path: str, *args, **kwargs) -> dict:
-        async with self.session.request(
+        async with self.__session.request(
             method, self.APIURL + path, *args, **kwargs
         ) as r:
             return await r.json()
 
     async def search(self, *args, **kwargs) -> List[Item]:
         r = await self.request(
             "GET", "/", params=self._payload_maker(*args, **kwargs)
```

### Comparing `google-custom-search-3.0.0a0/google_custom_search/enums.py` & `google-custom-search-3.0.0rc0/google_custom_search/enums.py`

 * *Files identical despite different names*

### Comparing `google-custom-search-3.0.0a0/google_custom_search/search.py` & `google-custom-search-3.0.0rc0/google_custom_search/search.py`

 * *Files identical despite different names*

### Comparing `google-custom-search-3.0.0a0/google_custom_search/types.py` & `google-custom-search-3.0.0rc0/google_custom_search/types.py`

 * *Files identical despite different names*

### Comparing `google-custom-search-3.0.0a0/google_custom_search.egg-info/PKG-INFO` & `google-custom-search-3.0.0rc0/google_custom_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-custom-search
-Version: 3.0.0a0
+Version: 3.0.0rc0
 Summary: This is for google custom search api.
 Home-page: https://github.com/mc-fdc-dev/google-custom-search
 Author: mc-fdc-dev
 Author-email: masato190411@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `google-custom-search-3.0.0a0/setup.py` & `google-custom-search-3.0.0rc0/setup.py`

 * *Files identical despite different names*

