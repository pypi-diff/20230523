# Comparing `tmp/gandai-1.1.8.tar.gz` & `tmp/gandai-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.8.tar", last modified: Mon May 15 00:34:47 2023, max compression
+gzip compressed data, was "gandai-1.1.9.tar", last modified: Tue May 16 10:29:15 2023, max compression
```

## Comparing `gandai-1.1.8.tar` & `gandai-1.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.389003 gandai-1.1.8/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.8/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-15 00:34:47.388872 gandai-1.1.8/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.384188 gandai-1.1.8/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.8/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.386850 gandai-1.1.8/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.8/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.8/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-15 00:21:53.000000 gandai-1.1.8/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-14 00:47:34.000000 gandai-1.1.8/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.8/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.8/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5474 2023-05-15 00:13:44.000000 gandai-1.1.8/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6137 2023-05-14 03:30:02.000000 gandai-1.1.8/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17744 2023-05-15 00:13:44.000000 gandai-1.1.8/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.8/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8074 2023-05-15 00:13:44.000000 gandai-1.1.8/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1703 2023-05-15 00:33:20.000000 gandai-1.1.8/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-15 00:33:21.000000 gandai-1.1.8/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.8/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     3443 2023-05-15 00:05:22.000000 gandai-1.1.8/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.387754 gandai-1.1.8/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.8/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.388321 gandai-1.1.8/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.8/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-14 19:49:36.000000 gandai-1.1.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.8/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1655 2023-05-14 20:47:34.000000 gandai-1.1.8/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-14 17:36:57.000000 gandai-1.1.8/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.388606 gandai-1.1.8/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)     2920 2023-05-15 00:05:33.000000 gandai-1.1.8/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2642 2023-05-14 03:28:36.000000 gandai-1.1.8/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)     9337 2023-05-15 00:00:59.000000 gandai-1.1.8/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5497 2023-05-14 21:00:02.000000 gandai-1.1.8/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-15 00:34:47.384717 gandai-1.1.8/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-15 00:34:47.000000 gandai-1.1.8/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2023-05-15 00:34:23.000000 gandai-1.1.8/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-15 00:34:47.389036 gandai-1.1.8/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.8/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.128274 gandai-1.1.9/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.9/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-16 10:29:15.128153 gandai-1.1.9/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.122682 gandai-1.1.9/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       45 2023-05-13 19:24:50.000000 gandai-1.1.9/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.126221 gandai-1.1.9/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-05-13 19:25:52.000000 gandai-1.1.9/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.9/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-15 00:21:53.000000 gandai-1.1.9/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4064 2023-05-15 02:35:18.000000 gandai-1.1.9/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2075 2023-05-13 19:36:23.000000 gandai-1.1.9/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.9/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5474 2023-05-15 00:13:44.000000 gandai-1.1.9/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6137 2023-05-14 03:30:02.000000 gandai-1.1.9/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17744 2023-05-15 00:13:44.000000 gandai-1.1.9/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.9/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8074 2023-05-15 00:13:44.000000 gandai-1.1.9/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1703 2023-05-16 10:28:54.000000 gandai-1.1.9/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1583 2023-05-15 00:33:21.000000 gandai-1.1.9/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     2451 2023-05-13 19:35:44.000000 gandai-1.1.9/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     3526 2023-05-16 10:26:58.000000 gandai-1.1.9/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.127116 gandai-1.1.9/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.9/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.127631 gandai-1.1.9/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.1.9/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-14 19:49:36.000000 gandai-1.1.9/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      409 2023-05-13 19:26:13.000000 gandai-1.1.9/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1655 2023-05-15 12:42:15.000000 gandai-1.1.9/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3257 2023-05-14 17:36:57.000000 gandai-1.1.9/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.127900 gandai-1.1.9/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)     2913 2023-05-15 21:05:11.000000 gandai-1.1.9/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2642 2023-05-14 03:28:36.000000 gandai-1.1.9/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)     9337 2023-05-15 00:00:59.000000 gandai-1.1.9/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5554 2023-05-16 10:27:56.000000 gandai-1.1.9/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-16 10:29:15.123356 gandai-1.1.9/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1015 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-16 10:29:15.000000 gandai-1.1.9/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2023-05-16 10:29:01.000000 gandai-1.1.9/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-16 10:29:15.128305 gandai-1.1.9/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.9/setup.py
```

### Comparing `gandai-1.1.8/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8b2f6064 (Sun May 14 00:47:07 2023 UTC)
+moddate:  0xd17d6164 (Mon May 15 00:33:21 2023 UTC)
 files sz: 1583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.1.8/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.9/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/auth.py` & `gandai-1.1.9/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/datastore.py` & `gandai-1.1.9/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/db.py` & `gandai-1.1.9/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/main.py` & `gandai-1.1.9/gandai/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,11 +94,14 @@
     """
 
     events = query.event(search_uid=search_uid)
     checkpoints = query.checkpoint(search_uid=search_uid)
 
     q = list(set(events["id"].tolist()) - set(checkpoints["event_id"].tolist()))
     
-    with ThreadPoolExecutor(max_workers=4) as executor:
-        executor.map(process_event, q)
+    for event_id in q:
+        print(event_id)
+        process_event(event_id)
+    # with ThreadPoolExecutor(max_workers=4) as executor:
+    #     executor.map(process_event, q)
     
     return len(q)
```

### Comparing `gandai-1.1.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.1.9/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/migrations/db_seed.py` & `gandai-1.1.9/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/migrations/dealcloud.py` & `gandai-1.1.9/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/migrations/sql/schema.sql` & `gandai-1.1.9/gandai/migrations/sql/schema.sql`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     e.type AS last_event_type, 
     e.created AS last_event_dt,
     c.name as name,
     c.uid as dealcloud_id,
     c.description as description,
     c.meta as meta,
     (c.meta->>'employees') AS employees,
-    (c.meta->>'ownership_status') AS ownership_status,
+    (c.meta->>'ownership_status') AS ownership,
     (c.meta->>'linkedin') AS linkedin,    
     (r.data->>'rating') AS rating
 FROM (
     SELECT 
         domain, 
         MAX(created) AS max_created
     FROM
```

### Comparing `gandai-1.1.8/gandai/models.py` & `gandai-1.1.9/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/query.py` & `gandai-1.1.9/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.8/gandai/sources.py` & `gandai-1.1.9/gandai/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         response = requests.post(
             "https://search.grata.com/api/v1/enrich/",
             headers=GrataWrapper.HEADERS,
             json={"domain": domain},
         )
         data = response.json()
         data['linkedin'] = data.get('social_linkedin')
+        data['ownership'] = data.get('ownership_status')
         return data
 
     def _get_api_filter(search: Search) -> dict:
         STATES = {
             "AL": "Alabama",
             "AK": "Alaska",
             "AZ": "Arizona",
```

### Comparing `gandai-1.1.8/gandai.egg-info/SOURCES.txt` & `gandai-1.1.9/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

