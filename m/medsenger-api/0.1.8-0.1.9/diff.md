# Comparing `tmp/medsenger_api-0.1.8.tar.gz` & `tmp/medsenger_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/roctbb/PycharmProjects/medsenger_api/dist/tmpg3ukjcu_/medsenger_api-0.1.8.tar", last modified: Tue Aug 31 13:55:23 2021, max compression
+gzip compressed data, was "/Users/roctbb/PycharmProjects/medsenger_api/dist/tmpi7m0pxaw/medsenger_api-0.1.9.tar", last modified: Tue Aug 31 14:03:26 2021, max compression
```

## Comparing `medsenger_api-0.1.8.tar` & `medsenger_api-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 roctbb     (501) staff       (20)        0 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/
--rw-r--r--   0 roctbb     (501) staff       (20)     1313 2021-08-27 09:03:19.000000 medsenger_api-0.1.8/LICENSE
--rw-r--r--   0 roctbb     (501) staff       (20)      379 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/PKG-INFO
--rw-r--r--   0 roctbb     (501) staff       (20)       18 2021-08-27 09:03:19.000000 medsenger_api-0.1.8/README.md
-drwxr-xr-x   0 roctbb     (501) staff       (20)        0 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api/
--rw-r--r--   0 roctbb     (501) staff       (20)    10703 2021-08-31 13:55:04.000000 medsenger_api-0.1.8/medsenger_api/__init__.py
-drwxr-xr-x   0 roctbb     (501) staff       (20)        0 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api.egg-info/
--rw-r--r--   0 roctbb     (501) staff       (20)      379 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api.egg-info/PKG-INFO
--rw-r--r--   0 roctbb     (501) staff       (20)      251 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api.egg-info/SOURCES.txt
--rw-r--r--   0 roctbb     (501) staff       (20)        1 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api.egg-info/dependency_links.txt
--rw-r--r--   0 roctbb     (501) staff       (20)        9 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api.egg-info/requires.txt
--rw-r--r--   0 roctbb     (501) staff       (20)       14 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/medsenger_api.egg-info/top_level.txt
--rw-r--r--   0 roctbb     (501) staff       (20)      119 2021-08-27 09:03:19.000000 medsenger_api-0.1.8/pyproject.toml
--rw-r--r--   0 roctbb     (501) staff       (20)       38 2021-08-31 13:55:23.000000 medsenger_api-0.1.8/setup.cfg
--rw-r--r--   0 roctbb     (501) staff       (20)      476 2021-08-31 13:55:04.000000 medsenger_api-0.1.8/setup.py
+drwxr-xr-x   0 roctbb     (501) staff       (20)        0 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/
+-rw-r--r--   0 roctbb     (501) staff       (20)     1313 2021-08-27 09:03:19.000000 medsenger_api-0.1.9/LICENSE
+-rw-r--r--   0 roctbb     (501) staff       (20)      379 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/PKG-INFO
+-rw-r--r--   0 roctbb     (501) staff       (20)       18 2021-08-27 09:03:19.000000 medsenger_api-0.1.9/README.md
+drwxr-xr-x   0 roctbb     (501) staff       (20)        0 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api/
+-rw-r--r--   0 roctbb     (501) staff       (20)    10875 2021-08-31 14:03:05.000000 medsenger_api-0.1.9/medsenger_api/__init__.py
+drwxr-xr-x   0 roctbb     (501) staff       (20)        0 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api.egg-info/
+-rw-r--r--   0 roctbb     (501) staff       (20)      379 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api.egg-info/PKG-INFO
+-rw-r--r--   0 roctbb     (501) staff       (20)      251 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api.egg-info/SOURCES.txt
+-rw-r--r--   0 roctbb     (501) staff       (20)        1 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api.egg-info/dependency_links.txt
+-rw-r--r--   0 roctbb     (501) staff       (20)       22 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api.egg-info/requires.txt
+-rw-r--r--   0 roctbb     (501) staff       (20)       14 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/medsenger_api.egg-info/top_level.txt
+-rw-r--r--   0 roctbb     (501) staff       (20)      119 2021-08-27 09:03:19.000000 medsenger_api-0.1.9/pyproject.toml
+-rw-r--r--   0 roctbb     (501) staff       (20)       38 2021-08-31 14:03:26.000000 medsenger_api-0.1.9/setup.cfg
+-rw-r--r--   0 roctbb     (501) staff       (20)      492 2021-08-31 14:03:00.000000 medsenger_api-0.1.9/setup.py
```

### Comparing `medsenger_api-0.1.8/LICENSE` & `medsenger_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `medsenger_api-0.1.8/medsenger_api/__init__.py` & `medsenger_api-0.1.9/medsenger_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 medsenger_api.
 Python SDK for Medsenger.AI
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = 'Rostislav Borodin'
 __credits__ = 'TelePat LLC'
 
 import base64
 import uuid
 from copy import copy
 import requests
@@ -146,15 +146,14 @@
 
         if record_time:
             data['time'] = record_time
 
         if files:
             data['files'] = files
 
-
         return self.__send_request__('/api/agents/records/add', data)
 
     def add_records(self, contract_id, values, record_time=None, params={}):
         data = {"contract_id": contract_id, "api_key": self.api_key, 'values': []}
 
         for record in values:
             record_params = copy(params)
@@ -170,16 +169,15 @@
                 category_name = record['category_name']
                 value = record['value']
                 custom_params = record.get('params', {})
                 record_params.update(custom_params)
                 files = record.get('files', [])
 
             data['values'].append(
-                    {"category_name": category_name, "value": value, "params": files, "files": files, "time": record_time})
-
+                {"category_name": category_name, "value": value, "params": files, "files": files, "time": record_time})
 
         return self.__send_request__('/api/agents/records/add', data)
 
     def send_message(self, contract_id, text, action_link=None, action_name=None, action_onetime=True,
                      only_doctor=False,
                      only_patient=False, action_deadline=None, is_urgent=False, need_answer=False,
                      attachments=None, action_big=True, send_from=None, forward_to_doctor=True):
@@ -218,19 +216,22 @@
         if is_urgent:
             message['is_urgent'] = is_urgent
 
         if attachments:
             message['attachments'] = []
 
             for attachment in attachments:
-                message['attachments'].append({
-                    "name": attachment[0],
-                    "type": attachment[1],
-                    "base64": attachment[2],
-                })
+                if isinstance(attachment, (list, tuple)):
+                    message['attachments'].append({
+                        "name": attachment[0],
+                        "type": attachment[1],
+                        "base64": attachment[2],
+                    })
+                elif isinstance(attachment, (dict)):
+                    message['attachments'].append(attachment)
 
         data = {
             "contract_id": contract_id,
             "api_key": self.api_key,
             "message": message
         }
 
@@ -296,24 +297,24 @@
 
     def ajax_url(self, action, contract_id, agent_token):
         # TODO fix
         return self.host.replace('8001',
                                  '8000') + "/api/client/agents/{agent_id}/?action={action}&contract_id={contract_id}&agent_token={agent_token}".format(
             agent_id=self.agent_id, action=action, contract_id=contract_id, agent_token=agent_token
         )
-    
+
     def download_file(self, *args, **kwargs):
         return self.get_file(*args, **kwargs)
-    
+
     def download_attachment(self, *args, **kwargs):
         return self.get_attachment(*args, **kwargs)
-    
+
     def download_image(self, *args, **kwargs):
         return self.get_image(*args, **kwargs)
-    
+
     def get_file(self, contract_id, file_id):
         data = {
             "api_key": self.api_key,
             "file_id": file_id,
             "contract_id": contract_id
         }
 
@@ -332,32 +333,33 @@
             "api_key": self.api_key,
             "attachment_id": image_id,
             "size": size
         }
 
         return self.__send_request__('/api/agents/image', data)
 
+
 def prepare_binary(name, data):
     import magic
     type = magic.from_buffer(data, mime=True)
 
     return {
         "name": name,
         "base64": base64.b64encode(data).decode('utf-8'),
         "type": type
     }
 
+
 def prepare_file(filename):
     import magic
     import os
 
     type = magic.from_file(filename, mime=True)
 
     with open(filename, 'rb') as file:
         answer = {
             "name": filename.split(os.sep)[-1],
             "base64": base64.b64encode(file.read()).decode('utf-8'),
             "type": type
         }
 
     return answer
-
```

