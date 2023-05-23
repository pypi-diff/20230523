# Comparing `tmp/mythic-0.1.1.tar.gz` & `tmp/mythic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.1.tar", last modified: Wed May 17 21:07:29 2023, max compression
+gzip compressed data, was "mythic-0.1.2.tar", last modified: Tue May 23 19:10:52 2023, max compression
```

## Comparing `mythic-0.1.1.tar` & `mythic-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-17 21:07:29.893484 mythic-0.1.1/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-17 21:07:29.893108 mythic-0.1.1/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1707 2023-05-10 02:44:23.000000 mythic-0.1.1/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-17 21:07:29.891115 mythic-0.1.1/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.1/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.1/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    99712 2023-05-17 20:24:46.000000 mythic-0.1.1/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3373 2023-05-17 19:32:31.000000 mythic-0.1.1/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.1/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7607 2023-05-17 19:28:56.000000 mythic-0.1.1/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-17 21:07:29.892671 mythic-0.1.1/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-05-17 21:07:29.000000 mythic-0.1.1/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-17 21:07:29.893586 mythic-0.1.1/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      818 2023-05-17 20:38:50.000000 mythic-0.1.1/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 19:10:51.999088 mythic-0.1.2/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-23 19:10:51.998706 mythic-0.1.2/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1707 2023-05-10 02:44:23.000000 mythic-0.1.2/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 19:10:51.996771 mythic-0.1.2/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.2/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.2/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    99712 2023-05-17 20:24:46.000000 mythic-0.1.2/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3373 2023-05-23 19:10:45.000000 mythic-0.1.2/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.2/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7731 2023-05-23 19:09:57.000000 mythic-0.1.2/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 19:10:51.998289 mythic-0.1.2/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2052 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-05-23 19:10:51.000000 mythic-0.1.2/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-23 19:10:51.999186 mythic-0.1.2/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      818 2023-05-23 19:10:30.000000 mythic-0.1.2/setup.py
```

### Comparing `mythic-0.1.1/PKG-INFO` & `mythic-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.1/README.md` & `mythic-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.1/mythic/graphql_queries.py` & `mythic-0.1.2/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.1/mythic/mythic.py` & `mythic-0.1.2/mythic/mythic.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.1/mythic/mythic_classes.py` & `mythic-0.1.2/mythic/mythic_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.refresh_token = refresh_token
         self.server_ip = server_ip
         self.server_port = server_port
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.1"
+        self.scripting_version = "0.1.2"
         self.current_operation_id = 0
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
             {
                 "username": self.username,
```

### Comparing `mythic-0.1.1/mythic/mythic_utilities.py` & `mythic-0.1.2/mythic/mythic_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     try:
         query_data = gql(query) if query is not None else gql_query
         if query_data is None:
             raise Exception("No data or gql_data passed into graphql_post function")
         async with Client(
             transport=await get_http_transport(mythic=mythic),
             fetch_schema_from_transport=False,
+            execute_timeout=None if mythic.global_timeout < 0 else mythic.global_timeout,
             schema=mythic.schema,
         ) as session:
             result = await session.execute(query_data, variable_values=variables)
             return result
     except Exception as e:
         raise e
 
@@ -167,14 +168,15 @@
             raise Exception(
                 "No data or gql_data passed into graphql_subscription function"
             )
 
         async with Client(
             transport=await get_ws_transport(mythic=mythic),
             fetch_schema_from_transport=False,
+            execute_timeout=None,
         ) as session:
             logging.debug(f"Started subscription for {query}")
             async for result in timeout_generator(
                 it=session.subscribe(query_data, variable_values=variables),
                 timeout=local_timeout,
             ):
                 yield result
```

### Comparing `mythic-0.1.1/mythic.egg-info/PKG-INFO` & `mythic-0.1.2/mythic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.1/setup.py` & `mythic-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.1",
+    version="0.1.2",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

