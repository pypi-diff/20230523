# Comparing `tmp/aniwrap-1.0.0.tar.gz` & `tmp/aniwrap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aniwrap-1.0.0.tar", max compression
+gzip compressed data, was "aniwrap-1.0.1.tar", max compression
```

## Comparing `aniwrap-1.0.0.tar` & `aniwrap-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-05-15 16:44:34.756159 aniwrap-1.0.0/LICENSE
--rw-r--r--   0        0        0     2429 2023-05-15 16:44:34.756159 aniwrap-1.0.0/README.md
--rw-r--r--   0        0        0     1476 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/__init__.py
--rw-r--r--   0        0        0     2535 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/client.py
--rw-r--r--   0        0        0     1570 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/endpoints.py
--rw-r--r--   0        0        0      541 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/__init__.py
--rw-r--r--   0        0        0     2159 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/anime.py
--rw-r--r--   0        0        0      989 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/base.py
--rw-r--r--   0        0        0      272 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/common.py
--rw-r--r--   0        0        0      281 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/http.py
--rw-r--r--   0        0        0     1354 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/manga.py
--rw-r--r--   0        0        0     2320 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/enums/user.py
--rw-r--r--   0        0        0     1023 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/__init__.py
--rw-r--r--   0        0        0     6116 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/anime.py
--rw-r--r--   0        0        0      206 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/base.py
--rw-r--r--   0        0        0     2902 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/common.py
--rw-r--r--   0        0        0     2977 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/forum.py
--rw-r--r--   0        0        0      632 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/http.py
--rw-r--r--   0        0        0     4175 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/manga.py
--rw-r--r--   0        0        0     2041 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/route.py
--rw-r--r--   0        0        0     4201 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/models/user.py
--rw-r--r--   0        0        0        0 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/py.typed
--rw-r--r--   0        0        0     1990 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/result.py
--rw-r--r--   0        0        0    20166 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/serializer.py
--rw-r--r--   0        0        0      359 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/services/__init__.py
--rw-r--r--   0        0        0     7670 2023-05-15 16:44:34.756159 aniwrap-1.0.0/aniwrap/services/anime.py
--rw-r--r--   0        0        0      569 2023-05-15 16:44:34.760159 aniwrap-1.0.0/aniwrap/services/base.py
--rw-r--r--   0        0        0     6109 2023-05-15 16:44:34.760159 aniwrap-1.0.0/aniwrap/services/forum.py
--rw-r--r--   0        0        0     3320 2023-05-15 16:44:34.760159 aniwrap-1.0.0/aniwrap/services/http.py
--rw-r--r--   0        0        0     5378 2023-05-15 16:44:34.760159 aniwrap-1.0.0/aniwrap/services/manga.py
--rw-r--r--   0        0        0    14949 2023-05-15 16:44:34.760159 aniwrap-1.0.0/aniwrap/services/user.py
--rw-r--r--   0        0        0      842 2023-05-15 16:44:34.760159 aniwrap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 aniwrap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-23 17:15:05.446475 aniwrap-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2457 2023-05-23 17:15:05.446475 aniwrap-1.0.1/README.md
+-rw-r--r--   0        0        0     1476 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/__init__.py
+-rw-r--r--   0        0        0     2535 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/client.py
+-rw-r--r--   0        0        0     1570 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/endpoints.py
+-rw-r--r--   0        0        0      541 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/__init__.py
+-rw-r--r--   0        0        0     2159 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/anime.py
+-rw-r--r--   0        0        0      989 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/base.py
+-rw-r--r--   0        0        0      272 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/common.py
+-rw-r--r--   0        0        0      281 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/http.py
+-rw-r--r--   0        0        0     1354 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/manga.py
+-rw-r--r--   0        0        0     2320 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/enums/user.py
+-rw-r--r--   0        0        0     1023 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/__init__.py
+-rw-r--r--   0        0        0     6116 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/anime.py
+-rw-r--r--   0        0        0      206 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/base.py
+-rw-r--r--   0        0        0     2902 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/common.py
+-rw-r--r--   0        0        0     2977 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/forum.py
+-rw-r--r--   0        0        0      632 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/http.py
+-rw-r--r--   0        0        0     4175 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/manga.py
+-rw-r--r--   0        0        0     2041 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/route.py
+-rw-r--r--   0        0        0     4201 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/models/user.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/py.typed
+-rw-r--r--   0        0        0     1990 2023-05-23 17:15:05.446475 aniwrap-1.0.1/aniwrap/result.py
+-rw-r--r--   0        0        0    20166 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/serializer.py
+-rw-r--r--   0        0        0      359 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/__init__.py
+-rw-r--r--   0        0        0     7670 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/anime.py
+-rw-r--r--   0        0        0      569 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/base.py
+-rw-r--r--   0        0        0     6109 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/forum.py
+-rw-r--r--   0        0        0     3318 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/http.py
+-rw-r--r--   0        0        0     5378 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/manga.py
+-rw-r--r--   0        0        0    14949 2023-05-23 17:15:05.450475 aniwrap-1.0.1/aniwrap/services/user.py
+-rw-r--r--   0        0        0      899 2023-05-23 17:15:05.450475 aniwrap-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 aniwrap-1.0.1/PKG-INFO
```

### Comparing `aniwrap-1.0.0/LICENSE` & `aniwrap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/README.md` & `aniwrap-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     error = anime_list_result.error
 
 if manga_list_result.is_success:
     manga_list = manga_list_result.value
 
 if manga_list_result.is_error:
     error = manga_list_result.error
+
+await  user_client.close()
 ```
 
 You can find information on generating Client Id and user's access token used in the above examples on [MAL documentation](https://myanimelist.net/apiconfig/references/authorization).
 
 ## Issues
 
 If you're facing any problems with the library, please open an issue [here](https://github.com/thevenuz/aniwrap.py/issues).
```

### Comparing `aniwrap-1.0.0/aniwrap/__init__.py` & `aniwrap-1.0.1/aniwrap/__init__.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/client.py` & `aniwrap-1.0.1/aniwrap/client.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/endpoints.py` & `aniwrap-1.0.1/aniwrap/endpoints.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/enums/__init__.py` & `aniwrap-1.0.1/aniwrap/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/enums/anime.py` & `aniwrap-1.0.1/aniwrap/enums/anime.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/enums/base.py` & `aniwrap-1.0.1/aniwrap/enums/base.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/enums/manga.py` & `aniwrap-1.0.1/aniwrap/enums/manga.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/enums/user.py` & `aniwrap-1.0.1/aniwrap/enums/user.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/__init__.py` & `aniwrap-1.0.1/aniwrap/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/anime.py` & `aniwrap-1.0.1/aniwrap/models/anime.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/common.py` & `aniwrap-1.0.1/aniwrap/models/common.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/forum.py` & `aniwrap-1.0.1/aniwrap/models/forum.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/http.py` & `aniwrap-1.0.1/aniwrap/models/http.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/manga.py` & `aniwrap-1.0.1/aniwrap/models/manga.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/route.py` & `aniwrap-1.0.1/aniwrap/models/route.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/models/user.py` & `aniwrap-1.0.1/aniwrap/models/user.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/result.py` & `aniwrap-1.0.1/aniwrap/result.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/serializer.py` & `aniwrap-1.0.1/aniwrap/serializer.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/services/anime.py` & `aniwrap-1.0.1/aniwrap/services/anime.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/services/base.py` & `aniwrap-1.0.1/aniwrap/services/base.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/services/forum.py` & `aniwrap-1.0.1/aniwrap/services/forum.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/services/http.py` & `aniwrap-1.0.1/aniwrap/services/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             async with session(
                 uri, headers=self._headers, params=params, data=data
             ) as r:
                 response = await r.json()
                 if r.status == 200:
                     return HttpSuccessResponse(r.status, "Success.", response)
 
-                return HttpErrorResponse(r.status, response.get("message"))
+                return HttpErrorResponse(r.status, response.get("error"))
 
         except Exception as e:
             return HttpErrorResponse(500, str(e))
 
     async def fetch(
         self, route: GenerateRoute, method: HttpMethod
     ) -> HttpErrorResponse | HttpSuccessResponse:
```

### Comparing `aniwrap-1.0.0/aniwrap/services/manga.py` & `aniwrap-1.0.1/aniwrap/services/manga.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/aniwrap/services/user.py` & `aniwrap-1.0.1/aniwrap/services/user.py`

 * *Files identical despite different names*

### Comparing `aniwrap-1.0.0/pyproject.toml` & `aniwrap-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "aniwrap"
-version = "1.0.0"
+version = "1.0.1"
 description = "An Asynchronous API wrapper for My Anime List API."
 authors = ["thevenuz"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thevenuz/aniwrap.py"
 repository = "https://github.com/thevenuz/aniwrap.py"
+documentation = "https://thevenuz.github.io/aniwrap.py/"
 packages = [{include = "aniwrap"},
 { include = "aniwrap/py.typed" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 aiohttp = ">=3.8.4"
 attrs = ">=22"
```

### Comparing `aniwrap-1.0.0/PKG-INFO` & `aniwrap-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: aniwrap
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Asynchronous API wrapper for My Anime List API.
 Home-page: https://github.com/thevenuz/aniwrap.py
 License: MIT
 Author: thevenuz
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4)
 Requires-Dist: attrs (>=22)
+Project-URL: Documentation, https://thevenuz.github.io/aniwrap.py/
 Project-URL: Repository, https://github.com/thevenuz/aniwrap.py
 Description-Content-Type: text/markdown
 
 # aniwrap
 
 An asynchronous wrapper for the [MyAnimeList V2 API](https://myanimelist.net/apiconfig/references/api/v2).
 
@@ -86,14 +87,16 @@
     error = anime_list_result.error
 
 if manga_list_result.is_success:
     manga_list = manga_list_result.value
 
 if manga_list_result.is_error:
     error = manga_list_result.error
+
+await  user_client.close()
 ```
 
 You can find information on generating Client Id and user's access token used in the above examples on [MAL documentation](https://myanimelist.net/apiconfig/references/authorization).
 
 ## Issues
 
 If you're facing any problems with the library, please open an issue [here](https://github.com/thevenuz/aniwrap.py/issues).
```

