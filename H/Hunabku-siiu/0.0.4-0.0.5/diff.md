# Comparing `tmp/Hunabku_siiu-0.0.4.tar.gz` & `tmp/Hunabku_siiu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_siiu-0.0.4.tar", last modified: Tue May  9 22:54:38 2023, max compression
+gzip compressed data, was "Hunabku_siiu-0.0.5.tar", last modified: Tue May 23 19:49:17 2023, max compression
```

## Comparing `Hunabku_siiu-0.0.4.tar` & `Hunabku_siiu-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/hunabku_siiu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/hunabku_siiu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/hunabku_siiu/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/hunabku_siiu/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/hunabku_siiu/endpoints/SIIU.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:49:17.897001 Hunabku_siiu-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:49:17.893001 Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 19:49:17.000000 Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-23 19:49:17.000000 Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:49:17.000000 Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 19:49:17.000000 Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 19:49:17.000000 Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 19:49:01.000000 Hunabku_siiu-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 19:49:17.893001 Hunabku_siiu-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 19:49:01.000000 Hunabku_siiu-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:49:17.893001 Hunabku_siiu-0.0.5/hunabku_siiu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:49:01.000000 Hunabku_siiu-0.0.5/hunabku_siiu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 19:49:01.000000 Hunabku_siiu-0.0.5/hunabku_siiu/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:49:17.893001 Hunabku_siiu-0.0.5/hunabku_siiu/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-23 19:49:01.000000 Hunabku_siiu-0.0.5/hunabku_siiu/endpoints/SIIU.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:49:17.897001 Hunabku_siiu-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-23 19:49:01.000000 Hunabku_siiu-0.0.5/setup.py
```

### Comparing `Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/PKG-INFO` & `Hunabku_siiu-0.0.5/Hunabku_siiu.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-siiu
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.4/PKG-INFO` & `Hunabku_siiu-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_siiu
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.4/README.md` & `Hunabku_siiu-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_siiu-0.0.4/hunabku_siiu/endpoints/SIIU.py` & `Hunabku_siiu-0.0.5/hunabku_siiu/endpoints/SIIU.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
-from elasticsearch import Elasticsearch, helpers, __version__ as es_version
+from elasticsearch import Elasticsearch, __version__ as es_version
 from elasticsearch_dsl import Search
 import time
 
 
 class SIIU(HunabkuPluginBase):
     config = Config()
     config += Param(mdb_uri="mongodb://localhost:27017/",
@@ -26,14 +26,25 @@
         self.dbclient = MongoClient(self.config.mdb_uri)
         auth = (self.config.es_user, self.config.es_pass)
         if es_version[0] < 8:
             self.es = Elasticsearch(self.config.es_uri, http_auth=auth)
         else:
             self.es = Elasticsearch(self.config.es_uri, basic_auth=auth)
 
+    def check_index(self):
+        if not self.es.indices.exists(index=self.config.es_project_index):
+            response = self.app.response_class(
+                response=self.json.dumps(
+                    {"msg": f"Internal error, index {self.config.es_project_index} not found in Elastic Search"}),
+                status=500,
+                mimetype='application/json'
+            )
+            return response
+        return None
+
     @endpoint('/siiu/project', methods=['GET'])
     def siiu_project(self):
         """
         @api {get} /siiu/project Project
         @apiName Project
         @apiGroup SIIU
         @apiDescription Allows to perform queries for projects,
@@ -43,14 +54,16 @@
                         lots of text where indexed for this search.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} search  keyword for text search.
         @apiParam {String} CODIGO  project id.
         @apiParam {String} group_code  Colciencias Group ID ex:"COL0008423"
         @apiParam {String} group_name  name of the research group (returns the projects for this group)
+        @apiParam {String} participant_name  name of the project participant (returns the projects for this participant)
+        @apiParam {String} participant_id  id of the participant (returns the projects for this participant)
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
@@ -58,35 +71,38 @@
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&search=keyword
             # An specific product
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&CODIGO=2013-86
             # An projects given a group id
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&group_code=COL0008423
             # An projects given a group name
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&group_name="psicologia cognitiva"
+            # An projects given a participant name
+            curl -i http://apis.colav.co/siiu/project?apikey=XXXX&participant_name="Diego Alejandro Restrepo Quintero"
+            # An projects given a participant id
+            curl -i http://apis.colav.co/siiu/project?apikey=XXXX&participant_id="xxxx"
 
         """
         if self.valid_apikey():
 
             keyword = self.request.args.get('search')
             codigo = self.request.args.get('CODIGO')
             grp_codigo = self.request.args.get('group_code')
             group_name = self.request.args.get('group_name')
+            participant_name = self.request.args.get('participant_name')
+            participant_id = self.request.args.get('participant_id')
+
             if keyword:
-                if not self.es.indices.exists(index=self.config.es_project_index):
-                    response = self.app.response_class(
-                        response=self.json.dumps(
-                            {"msg": f"Internal error, index {self.config.es_project_index} not found in Elastic Search"}),
-                        status=500,
-                        mimetype='application/json'
-                    )
-                    return response
+                check = self.check_index()
+                if check is not None:
+                    return check
+
                 body = {"query": {
                     "bool": {
                         "should": [
-                            {"match": {"NOMBRE_CORTO":  keyword}},
+                            {"match": {"NOMBRE_CORTO": keyword}},
                             {"match": {"NOMBRE_COMPLETO": keyword}},
                             {"match": {"PALABRAS_CLAVES": keyword}},
                             {"match": {"descriptive_text.TEXTO_INGRESADO": keyword}}
                         ]
                     }
                 }
                 }
@@ -123,30 +139,69 @@
                             ["project"].find({"project_participant.group.CODIGO_COLCIENCIAS": grp_codigo}, {"_id": 0}))
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=200,
                     mimetype='application/json'
                 )
                 return response
+            if participant_id:
+                data = list(self.dbclient[self.config.mdb_name]
+                            ["project"].find({"project_participant.PERSONA_NATURAL": participant_id}, {"_id": 0}))
+                response = self.app.response_class(
+                    response=self.json.dumps(data),
+                    status=200,
+                    mimetype='application/json'
+                )
+                return response
 
             if group_name:
-                if not self.es.indices.exists(index=self.config.es_project_index):
-                    response = self.app.response_class(
-                        response=self.json.dumps(
-                            {"msg": f"Internal error, index {self.config.es_project_index} not found in Elastic Search"}),
-                        status=500,
-                        mimetype='application/json'
-                    )
-                    return response
+                check = self.check_index()
+                if check is not None:
+                    return check
+                body = {
+                    "query": {
+                        "bool": {
+                            "must": [
+                                {"match_phrase": {
+                                    "project_participant.group.NOMBRE_COMPLETO": group_name}},
+                            ]
+                        }
+                    }
+                }
+
+                # get the start time
+                st = time.time()
+                s = Search(using=self.es, index=self.config.es_project_index)
+                s = s.update_from_dict(body)
+                s = s.extra(track_total_hits=True)
+                s.execute()
+                data = [hit.to_dict() for hit in s.scan()]
+                response = self.app.response_class(
+                    response=self.json.dumps(data),
+                    status=200,
+                    mimetype='application/json'
+                )
+                # get the end time
+                et = time.time()
+                # get the execution time
+                elapsed_time = et - st
+                print(f'Search for "{group_name}" Execution time:',
+                      elapsed_time, 'seconds')
+                return response
+
+            if participant_name:
+                check = self.check_index()
+                if check is not None:
+                    return check
                 body = {
                     "query": {
                         "bool": {
                             "must": [
                                 {"match_phrase": {
-                                    "project_participant.group.NOMBRE_COMPLETO":  group_name}},
+                                    "project_participant.NOMBRE_COMPLETO": participant_name}},
                             ]
                         }
                     }
                 }
 
                 # get the start time
                 st = time.time()
```

### Comparing `Hunabku_siiu-0.0.4/setup.py` & `Hunabku_siiu-0.0.5/setup.py`

 * *Files identical despite different names*

