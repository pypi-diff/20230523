# Comparing `tmp/robotcloud-client-0.0.5.tar.gz` & `tmp/robotcloud-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robotcloud-client-0.0.5.tar", last modified: Wed Mar 22 07:02:13 2023, max compression
+gzip compressed data, was "dist/robotcloud-client-0.0.6.tar", last modified: Tue May 23 09:15:44 2023, max compression
```

## Comparing `robotcloud-client-0.0.5.tar` & `robotcloud-client-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      948 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/PKG-INFO
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      571 2023-03-16 11:05:19.000000 robotcloud-client-0.0.5/README.md
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-22 07:02:13.887336 robotcloud-client-0.0.5/robotcloud/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-16 08:53:35.000000 robotcloud-client-0.0.5/robotcloud/__init__.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     5103 2022-07-08 06:05:41.000000 robotcloud-client-0.0.5/robotcloud/api.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      765 2022-03-22 07:09:51.000000 robotcloud-client-0.0.5/robotcloud/authenticator.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      261 2022-07-08 06:21:11.000000 robotcloud-client-0.0.5/robotcloud/constants.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/robotcloud/endpoints/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      306 2022-07-08 10:10:07.000000 robotcloud-client-0.0.5/robotcloud/endpoints/__init__.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2760 2022-04-21 07:37:05.000000 robotcloud-client-0.0.5/robotcloud/endpoints/configurationtypes.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2199 2023-03-16 07:43:25.000000 robotcloud-client-0.0.5/robotcloud/endpoints/devices.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1157 2023-03-20 11:23:25.000000 robotcloud-client-0.0.5/robotcloud/endpoints/locations.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      630 2023-03-16 08:34:00.000000 robotcloud-client-0.0.5/robotcloud/endpoints/login.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1935 2022-07-08 06:51:48.000000 robotcloud-client-0.0.5/robotcloud/endpoints/organizations.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1919 2022-07-08 08:24:23.000000 robotcloud-client-0.0.5/robotcloud/endpoints/projects.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     6937 2023-03-16 08:09:02.000000 robotcloud-client-0.0.5/robotcloud/endpoints/services.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3705 2022-06-06 05:41:10.000000 robotcloud-client-0.0.5/robotcloud/endpoints/services_data.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1167 2022-04-08 09:23:38.000000 robotcloud-client-0.0.5/robotcloud/endpoints/subsystems.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1141 2022-07-08 05:52:20.000000 robotcloud-client-0.0.5/robotcloud/endpoints/tags.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2347 2023-03-16 08:37:33.000000 robotcloud-client-0.0.5/robotcloud/endpoints/users.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1255 2022-07-08 08:22:31.000000 robotcloud-client-0.0.5/robotcloud/exceptions.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/robotcloud/utils/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      117 2022-07-08 08:22:45.000000 robotcloud-client-0.0.5/robotcloud/utils/__init__.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/robotcloud/utils/datatables/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2022-05-10 13:46:31.000000 robotcloud-client-0.0.5/robotcloud/utils/datatables/__init__.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      428 2022-07-08 06:17:40.000000 robotcloud-client-0.0.5/robotcloud/utils/datatables/request.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      551 2022-07-08 06:17:51.000000 robotcloud-client-0.0.5/robotcloud/utils/datatables/response.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      235 2022-05-10 13:46:31.000000 robotcloud-client-0.0.5/robotcloud/utils/paginated_response.py
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      286 2023-03-16 08:04:55.000000 robotcloud-client-0.0.5/robotcloud/utils/pagination.py
-drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/robotcloud_client.egg-info/
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      948 2023-03-22 07:02:13.000000 robotcloud-client-0.0.5/robotcloud_client.egg-info/PKG-INFO
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      976 2023-03-22 07:02:13.000000 robotcloud-client-0.0.5/robotcloud_client.egg-info/SOURCES.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        1 2023-03-22 07:02:13.000000 robotcloud-client-0.0.5/robotcloud_client.egg-info/dependency_links.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       15 2023-03-22 07:02:13.000000 robotcloud-client-0.0.5/robotcloud_client.egg-info/requires.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       11 2023-03-22 07:02:13.000000 robotcloud-client-0.0.5/robotcloud_client.egg-info/top_level.txt
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      157 2023-03-22 07:02:13.891336 robotcloud-client-0.0.5/setup.cfg
--rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1408 2023-03-21 14:00:34.000000 robotcloud-client-0.0.5/setup.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-05-23 09:15:44.762324 robotcloud-client-0.0.6/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      959 2023-05-23 09:15:44.762324 robotcloud-client-0.0.6/PKG-INFO
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      582 2023-03-22 07:06:52.000000 robotcloud-client-0.0.6/README.md
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-05-23 09:15:44.758324 robotcloud-client-0.0.6/robotcloud/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-03-16 08:53:35.000000 robotcloud-client-0.0.6/robotcloud/__init__.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     5103 2022-07-08 06:05:41.000000 robotcloud-client-0.0.6/robotcloud/api.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      765 2022-03-22 07:09:51.000000 robotcloud-client-0.0.6/robotcloud/authenticator.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      261 2022-07-08 06:21:11.000000 robotcloud-client-0.0.6/robotcloud/constants.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-05-23 09:15:44.762324 robotcloud-client-0.0.6/robotcloud/endpoints/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      306 2022-07-08 10:10:07.000000 robotcloud-client-0.0.6/robotcloud/endpoints/__init__.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1100 2023-03-27 10:21:54.000000 robotcloud-client-0.0.6/robotcloud/endpoints/applications.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2760 2022-04-21 07:37:05.000000 robotcloud-client-0.0.6/robotcloud/endpoints/configurationtypes.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2199 2023-03-16 07:43:25.000000 robotcloud-client-0.0.6/robotcloud/endpoints/devices.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1157 2023-03-20 11:23:25.000000 robotcloud-client-0.0.6/robotcloud/endpoints/locations.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      630 2023-03-16 08:34:00.000000 robotcloud-client-0.0.6/robotcloud/endpoints/login.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1935 2022-07-08 06:51:48.000000 robotcloud-client-0.0.6/robotcloud/endpoints/organizations.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3036 2023-03-31 05:38:34.000000 robotcloud-client-0.0.6/robotcloud/endpoints/projects.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     6937 2023-03-16 08:09:02.000000 robotcloud-client-0.0.6/robotcloud/endpoints/services.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     3705 2022-06-06 05:41:10.000000 robotcloud-client-0.0.6/robotcloud/endpoints/services_data.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1167 2022-04-08 09:23:38.000000 robotcloud-client-0.0.6/robotcloud/endpoints/subsystems.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1141 2022-07-08 05:52:20.000000 robotcloud-client-0.0.6/robotcloud/endpoints/tags.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     2347 2023-03-16 08:37:33.000000 robotcloud-client-0.0.6/robotcloud/endpoints/users.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1255 2022-07-08 08:22:31.000000 robotcloud-client-0.0.6/robotcloud/exceptions.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-05-23 09:15:44.762324 robotcloud-client-0.0.6/robotcloud/utils/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      117 2022-07-08 08:22:45.000000 robotcloud-client-0.0.6/robotcloud/utils/__init__.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-05-23 09:15:44.762324 robotcloud-client-0.0.6/robotcloud/utils/datatables/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        0 2022-05-10 13:46:31.000000 robotcloud-client-0.0.6/robotcloud/utils/datatables/__init__.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      428 2022-07-08 06:17:40.000000 robotcloud-client-0.0.6/robotcloud/utils/datatables/request.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      551 2022-07-08 06:17:51.000000 robotcloud-client-0.0.6/robotcloud/utils/datatables/response.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      235 2022-05-10 13:46:31.000000 robotcloud-client-0.0.6/robotcloud/utils/paginated_response.py
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      286 2023-03-16 08:04:55.000000 robotcloud-client-0.0.6/robotcloud/utils/pagination.py
+drwxrwxr-x   0 bernat-robot  (1000) bernat-robot  (1000)        0 2023-05-23 09:15:44.762324 robotcloud-client-0.0.6/robotcloud_client.egg-info/
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      959 2023-05-23 09:15:44.000000 robotcloud-client-0.0.6/robotcloud_client.egg-info/PKG-INFO
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1013 2023-05-23 09:15:44.000000 robotcloud-client-0.0.6/robotcloud_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)        1 2023-05-23 09:15:44.000000 robotcloud-client-0.0.6/robotcloud_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       15 2023-05-23 09:15:44.000000 robotcloud-client-0.0.6/robotcloud_client.egg-info/requires.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)       11 2023-05-23 09:15:44.000000 robotcloud-client-0.0.6/robotcloud_client.egg-info/top_level.txt
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)      157 2023-05-23 09:15:44.766324 robotcloud-client-0.0.6/setup.cfg
+-rw-rw-r--   0 bernat-robot  (1000) bernat-robot  (1000)     1408 2023-05-23 09:10:47.000000 robotcloud-client-0.0.6/setup.py
```

### Comparing `robotcloud-client-0.0.5/PKG-INFO` & `robotcloud-client-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcloud-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client to interact with robotcloud API from a python project.
 Home-page: https://github.com/robotmallorca/sw.module.python.robotcloud.client
 Author: Bernat Galmés Rubert
 Author-email: bernat.galmes@robotbas.com
 Keywords: client,robotcloud
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -19,9 +19,9 @@
 pip install robotcloud-client
 ```
 ### Environment variables
 
 The environment where your application is running must define the next environment variables
 to be able to interact with robotcloud:
 - **ROBOTCLOUD_API_KEY**: Should contain the api key of the robotcloud instance you want to interact.  
-- **ROOT_URL**: Should contain the base URL which point to the robotcloud instance. 
+- **ROBOTCLOUD_ROOT_URL**: Should contain the base URL which point to the robotcloud instance. 
 In a local environment can be something like "http://127.0.0.1:8080/robotcloud/1.2"
```

### Comparing `robotcloud-client-0.0.5/README.md` & `robotcloud-client-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 pip install robotcloud-client
 ```
 ### Environment variables
 
 The environment where your application is running must define the next environment variables
 to be able to interact with robotcloud:
 - **ROBOTCLOUD_API_KEY**: Should contain the api key of the robotcloud instance you want to interact.  
-- **ROOT_URL**: Should contain the base URL which point to the robotcloud instance. 
+- **ROBOTCLOUD_ROOT_URL**: Should contain the base URL which point to the robotcloud instance. 
 In a local environment can be something like "http://127.0.0.1:8080/robotcloud/1.2"
```

### Comparing `robotcloud-client-0.0.5/robotcloud/api.py` & `robotcloud-client-0.0.6/robotcloud/api.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/authenticator.py` & `robotcloud-client-0.0.6/robotcloud/authenticator.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/configurationtypes.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/configurationtypes.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/devices.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/devices.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/locations.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/locations.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/login.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/organizations.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/organizations.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/projects.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/projects.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,33 @@
         self.project_id = project_id
         super().__init__(token)
 
     def get_endpoint(self):
         return f"projects/{self.project_id}/devices"
 
 
+class ProjectApplicationsListAPIEndpoint(APIEndPointAuthenticated):
+    def __init__(self, token: str, project_id: str):
+        self.project_id = project_id
+        super().__init__(token)
+
+    def get_endpoint(self):
+        return f"projects/{self.project_id}/applications"
+
+
+class ProjectApplicationsItemAPIEndpoint(APIEndPointAuthenticated):
+    def __init__(self, token: str, project_id: str, application_id: str):
+        self.project_id = project_id
+        self.application_id = application_id
+        super().__init__(token)
+
+    def get_endpoint(self):
+        return f"projects/{self.project_id}/applications/{self.application_id}"
+
+
 def get_project(token, project_id):
     return APICallProjects(token, project_id).get()
 
 
 def get_projects(token):
     return APICallProjects(token).get()
 
@@ -59,7 +78,19 @@
     org_id = data['organization_id']
     data.pop('organization_id')
     return APICallOrganizationProjects(token, org_id).post(data)
 
 
 def delete_project(token, project_id) -> dict:
     return APICallProjects(token, project_id).delete()
+
+
+def get_project_applications(token, project_id) -> list:
+    return ProjectApplicationsListAPIEndpoint(token, project_id).get()
+
+
+def get_project_application(token, project_id, application_id) -> list:
+    return ProjectApplicationsItemAPIEndpoint(token, project_id, application_id).get()
+
+
+def update_project_application(token, project_id, application_id, data: dict) -> list:
+    return ProjectApplicationsItemAPIEndpoint(token, project_id, application_id).put(data)
```

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/services.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/services.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/services_data.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/services_data.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/subsystems.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/subsystems.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/tags.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/endpoints/users.py` & `robotcloud-client-0.0.6/robotcloud/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/exceptions.py` & `robotcloud-client-0.0.6/robotcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud/utils/datatables/response.py` & `robotcloud-client-0.0.6/robotcloud/utils/datatables/response.py`

 * *Files identical despite different names*

### Comparing `robotcloud-client-0.0.5/robotcloud_client.egg-info/PKG-INFO` & `robotcloud-client-0.0.6/robotcloud_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcloud-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client to interact with robotcloud API from a python project.
 Home-page: https://github.com/robotmallorca/sw.module.python.robotcloud.client
 Author: Bernat Galmés Rubert
 Author-email: bernat.galmes@robotbas.com
 Keywords: client,robotcloud
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -19,9 +19,9 @@
 pip install robotcloud-client
 ```
 ### Environment variables
 
 The environment where your application is running must define the next environment variables
 to be able to interact with robotcloud:
 - **ROBOTCLOUD_API_KEY**: Should contain the api key of the robotcloud instance you want to interact.  
-- **ROOT_URL**: Should contain the base URL which point to the robotcloud instance. 
+- **ROBOTCLOUD_ROOT_URL**: Should contain the base URL which point to the robotcloud instance. 
 In a local environment can be something like "http://127.0.0.1:8080/robotcloud/1.2"
```

### Comparing `robotcloud-client-0.0.5/robotcloud_client.egg-info/SOURCES.txt` & `robotcloud-client-0.0.6/robotcloud_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 robotcloud/__init__.py
 robotcloud/api.py
 robotcloud/authenticator.py
 robotcloud/constants.py
 robotcloud/exceptions.py
 robotcloud/endpoints/__init__.py
+robotcloud/endpoints/applications.py
 robotcloud/endpoints/configurationtypes.py
 robotcloud/endpoints/devices.py
 robotcloud/endpoints/locations.py
 robotcloud/endpoints/login.py
 robotcloud/endpoints/organizations.py
 robotcloud/endpoints/projects.py
 robotcloud/endpoints/services.py
```

### Comparing `robotcloud-client-0.0.5/setup.py` & `robotcloud-client-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='robotcloud-client',
-    version='0.0.5',
+    version='0.0.6',
     author="Bernat Galmés Rubert",
     author_email="bernat.galmes@robotbas.com",
     description="Client to interact with robotcloud API from a python project.",
     url='https://github.com/robotmallorca/sw.module.python.robotcloud.client',
     keywords="client,robotcloud",
     packages=find_packages(include=['robotcloud', 'robotcloud.endpoints', 'robotcloud.utils', 'robotcloud.utils.datatables']),
     long_description=read('README.md'),
```

