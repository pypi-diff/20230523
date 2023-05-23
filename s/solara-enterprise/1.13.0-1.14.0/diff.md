# Comparing `tmp/solara_enterprise-1.13.0.tar.gz` & `tmp/solara_enterprise-1.14.0.tar.gz`

## Comparing `solara_enterprise-1.13.0.tar` & `solara_enterprise-1.14.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/RELEASE.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/license.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/ssg.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/auth/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/auth/components.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/auth/flask.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/auth/middleware.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/auth/starlette.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/auth/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/cache/__init__.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/cache/base.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/cache/disk.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/cache/memory_size.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/cache/multi_level.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/cache/redis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/search/__init__.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/search/index.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/search/search.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/solara_enterprise/search/search.vue
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/LICENSE
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/pyproject.toml
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 solara_enterprise-1.13.0/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/RELEASE.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/license.py
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/ssg.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/auth/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/auth/components.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/auth/flask.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/auth/middleware.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/auth/starlette.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/auth/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/cache/__init__.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/cache/base.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/cache/disk.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/cache/memory_size.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/cache/multi_level.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/cache/redis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/search/__init__.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/search/index.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/search/search.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/solara_enterprise/search/search.vue
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/pyproject.toml
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 solara_enterprise-1.14.0/PKG-INFO
```

### Comparing `solara_enterprise-1.13.0/solara_enterprise/ssg.py` & `solara_enterprise-1.14.0/solara_enterprise/ssg.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/auth/components.py` & `solara_enterprise-1.14.0/solara_enterprise/auth/components.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/auth/flask.py` & `solara_enterprise-1.14.0/solara_enterprise/auth/flask.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/auth/middleware.py` & `solara_enterprise-1.14.0/solara_enterprise/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/auth/starlette.py` & `solara_enterprise-1.14.0/solara_enterprise/auth/starlette.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/auth/utils.py` & `solara_enterprise-1.14.0/solara_enterprise/auth/utils.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/cache/base.py` & `solara_enterprise-1.14.0/solara_enterprise/cache/base.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/cache/disk.py` & `solara_enterprise-1.14.0/solara_enterprise/cache/disk.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/cache/memory_size.py` & `solara_enterprise-1.14.0/solara_enterprise/cache/memory_size.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/cache/multi_level.py` & `solara_enterprise-1.14.0/solara_enterprise/cache/multi_level.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/cache/redis.py` & `solara_enterprise-1.14.0/solara_enterprise/cache/redis.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/search/index.py` & `solara_enterprise-1.14.0/solara_enterprise/search/index.py`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/solara_enterprise/search/search.vue` & `solara_enterprise-1.14.0/solara_enterprise/search/search.vue`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/.gitignore` & `solara_enterprise-1.14.0/.gitignore`

 * *Files identical despite different names*

### Comparing `solara_enterprise-1.13.0/pyproject.toml` & `solara_enterprise-1.14.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     {name = "Maarten A. Breddels", email = "maartenbreddels@gmail.com"},
     {name = "Mario Buikhuizen", email = "mariobuikhuizen@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: Free for non-commercial use"]
 dynamic = ["version", "description"]
 dependencies = [
-    "solara==1.13.0",
+    "solara==1.14.0",
 ]
 
 [project.optional-dependencies]
 ssg = [
     "beautifulsoup4",
     "playwright; python_version > '3.6'",
 ]
```

### Comparing `solara_enterprise-1.13.0/PKG-INFO` & `solara_enterprise-1.14.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: solara-enterprise
-Version: 1.13.0
+Version: 1.14.0
 Project-URL: Home, https://www.github.com/widgetti/solara
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>, Mario Buikhuizen <mariobuikhuizen@gmail.com>
 License: Not open source, contact contact@solara.dev for licencing.
 License-File: LICENSE
 Classifier: License :: Free for non-commercial use
-Requires-Dist: solara==1.13.0
+Requires-Dist: solara==1.14.0
 Provides-Extra: all
 Requires-Dist: solara-enterprise[auth]; extra == 'all'
 Requires-Dist: solara-enterprise[ssg]; extra == 'all'
 Provides-Extra: auth
 Requires-Dist: authlib; extra == 'auth'
 Requires-Dist: httpx; extra == 'auth'
 Requires-Dist: itsdangerous; extra == 'auth'
```

