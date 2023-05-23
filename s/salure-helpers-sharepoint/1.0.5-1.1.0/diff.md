# Comparing `tmp/salure_helpers_sharepoint-1.0.5.tar.gz` & `tmp/salure_helpers_sharepoint-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_sharepoint-1.0.5.tar", last modified: Wed Jan 18 15:53:09 2023, max compression
+gzip compressed data, was "dist/salure_helpers_sharepoint-1.1.0.tar", last modified: Tue May 23 16:07:43 2023, max compression
```

## Comparing `salure_helpers_sharepoint-1.0.5.tar` & `salure_helpers_sharepoint-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      274 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers/sharepoint/
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-01-18 15:52:54.000000 salure_helpers_sharepoint-1.0.5/salure_helpers/sharepoint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9583 2023-01-18 15:52:54.000000 salure_helpers_sharepoint-1.0.5/salure_helpers/sharepoint/sharepoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      378 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/salure_helpers_sharepoint.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 15:53:09.000000 salure_helpers_sharepoint-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-01-18 15:52:54.000000 salure_helpers_sharepoint-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers/sharepoint/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-23 16:07:28.000000 salure_helpers_sharepoint-1.1.0/salure_helpers/sharepoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10735 2023-05-23 16:07:28.000000 salure_helpers_sharepoint-1.1.0/salure_helpers/sharepoint/sharepoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/salure_helpers_sharepoint.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 16:07:43.000000 salure_helpers_sharepoint-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-05-23 16:07:28.000000 salure_helpers_sharepoint-1.1.0/setup.py
```

### Comparing `salure_helpers_sharepoint-1.0.5/salure_helpers/sharepoint/sharepoint.py` & `salure_helpers_sharepoint-1.1.0/salure_helpers/sharepoint/sharepoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from typing import List, Union
 import requests
 import json
 from io import BytesIO
+
+import typing
 from salure_helpers.salureconnect import SalureConnect
 
 
 class Sharepoint(SalureConnect):
     def __init__(self, label: Union[str, List], site: str = None, site_id: str = None, json_subset: int = None, site_name: str = None, debug: bool = False):
         """
         :param label: label of the sharepoint system in salureconnect
@@ -159,30 +161,42 @@
             download_url = response.json()['@microsoft.graph.downloadUrl']
             response_download = requests.get(url=download_url, headers=headers)
             with open(file=f'{local_folder_path}{file["name"]}', mode='wb') as f:
                 f.write(BytesIO(response_download.content).read())
             filecount += 1
         print(f'{filecount} files downloaded')
 
-    def list_dir(self, remote_folder_path: str) -> json:
+    def list_dir(self, remote_folder_path: str, get_files_from_nested_folders: bool = False) -> [json, typing.Generator]:
         """
         Fetch the contents of the API and return the "children"
         which has the information of all the items under that folder
         remote_folder_path: folder path you want to list
         :return: all the contents of the folder items
         """
+        if get_files_from_nested_folders:
+            return list(self._get_all_files_in_folder(folder_path=remote_folder_path))
+
         drive_id = self.get_driveid()
         url = f'https://graph.microsoft.com/v1.0/sites/{self.site_id}/drives/{drive_id}/root:/{remote_folder_path}?expand=children'
         if self.debug:
             print(f"url: {url}")
         response = requests.get(url, headers=self._get_headers(), timeout=120)
         response.raise_for_status()
 
         return response.json()['children']
 
+    # helpers function to get all files in a nested directory
+    def _get_all_files_in_folder(self, folder_path) -> typing.Generator:
+        children = self.list_dir(remote_folder_path=folder_path)
+        for child in children:
+            if 'file' in child:
+                yield {"folder": folder_path, "file": child['name'], "id": child['id']}
+            else:
+                yield from self._get_all_files_in_folder(folder_path=f"{folder_path}/{child['name']}")
+
     def remove_file(self, remote_file_path: str):
         """
         Remove a file from Sharepoint
         remote_file_path: complete path including filename
         :return: response from Sharepoint
         """
         drive_id = self.get_driveid()
@@ -201,7 +215,19 @@
         folder_content = self.list_dir(remote_folder_path=remote_folder_path)
         for file in folder_content:
             url = f'https://graph.microsoft.com/v1.0/sites/{self.site_id}/drives/{drive_id}/root:/{remote_folder_path}{file["name"]}'
             if self.debug:
                 print(f"url: {url}")
             response = requests.delete(url=url, headers=self._get_headers())
             response.raise_for_status()
+
+    def remove_folder(self, folder_id: str):
+        """
+        Remove a folder from Sharepoint
+        folder: folder id that you want to delete
+        """
+        drive_id = self.get_driveid()
+        url = f'https://graph.microsoft.com/v1.0/sites/{self.site_id}/drives/{drive_id}/items/{folder_id}'
+        if self.debug:
+            print(f"url: {url}")
+        response = requests.delete(url=url, headers=self._get_headers())
+        response.raise_for_status()
```

