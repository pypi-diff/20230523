# Comparing `tmp/unitlab-1.8.4.tar.gz` & `tmp/unitlab-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.8.4.tar", last modified: Fri May 19 07:14:11 2023, max compression
+gzip compressed data, was "unitlab-1.8.5.tar", last modified: Tue May 23 13:15:54 2023, max compression
```

## Comparing `unitlab-1.8.4.tar` & `unitlab-1.8.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.219713 unitlab-1.8.4/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.4/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.4/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-19 07:14:11.219713 unitlab-1.8.4/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      812 2023-05-16 06:53:44.000000 unitlab-1.8.4/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-19 07:14:11.219713 unitlab-1.8.4/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1131 2023-05-19 07:12:49.000000 unitlab-1.8.4/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.215713 unitlab-1.8.4/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.215713 unitlab-1.8.4/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)       63 2023-05-17 08:58:29.000000 unitlab-1.8.4/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)    11120 2023-05-17 13:54:30.000000 unitlab-1.8.4/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      746 2023-05-17 08:50:07.000000 unitlab-1.8.4/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4572 2023-05-17 13:51:47.000000 unitlab-1.8.4/src/unitlab/pretty.py
--rw-rw-r--   0 me        (1000) me        (1000)     2311 2023-05-17 13:50:32.000000 unitlab-1.8.4/src/unitlab/run.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-19 07:14:11.219713 unitlab-1.8.4/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      376 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       67 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-19 07:14:11.000000 unitlab-1.8.4/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.5/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.5/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-23 13:15:54.121113 unitlab-1.8.5/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1439 2023-05-23 07:41:41.000000 unitlab-1.8.5/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-23 13:15:54.125113 unitlab-1.8.5/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-05-23 13:04:53.000000 unitlab-1.8.5/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.5/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2084 2023-05-23 11:11:24.000000 unitlab-1.8.5/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    10963 2023-05-23 13:05:44.000000 unitlab-1.8.5/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-05-23 07:35:04.000000 unitlab-1.8.5/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-05-23 13:06:10.000000 unitlab-1.8.5/src/unitlab/run.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-23 13:15:54.121113 unitlab-1.8.5/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      373 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-23 13:15:54.000000 unitlab-1.8.5/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.4/LICENSE.md` & `unitlab-1.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.4/PKG-INFO` & `unitlab-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.4
+Version: 1.8.5
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-1.8.4/setup.py` & `unitlab-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.4",
+    version="1.8.5",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
@@ -24,15 +24,14 @@
     url="https://github.com/teamunitlab/unitlab-sdk",
     keywords="unitlab-sdk",
     install_requires=[
         "aiohttp",
         "numpy",
         "opencv-python",
         "Pillow",
-        "prettytable",
         "requests",
         "tqdm",
         "typer",
     ],
     entry_points={
         "console_scripts": ["unitlab=unitlab.run:app"],
     },
```

### Comparing `unitlab-1.8.4/src/unitlab/client.py` & `unitlab-1.8.5/src/unitlab/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 import os
 import re
 
 import aiohttp
 import requests
 import tqdm
 
-from .exceptions import AuthenticationError, NetworkError
+from .exceptions import AuthenticationError
 
-BASE_URL = "https://api-dev.unitlab.ai/api/cli"
+BASE_URL = "https://api.unitlab.ai/api/cli/"
+SDK_URL = BASE_URL + "/api/sdk/"
 
-ENPOINTS = {
-    "ai_model_list": BASE_URL + "/task-parent/",
-    "ai_model_detail": BASE_URL + "/task-parent/{}/",
-    "task_list": BASE_URL + "/task/",
-    "task_detail": BASE_URL + "/task/{}/",
-    "task_data_sources": BASE_URL + "/task/{}/datasource/",
-    "task_members": BASE_URL + "/task/{}/members/",
-    "task_statistics": BASE_URL + "/task/{}/statistics/",
-    "task_upload_datasources": BASE_URL + "/task/upload-datasource/",
-    "task_download_data": BASE_URL + "/task/{}/download-data/",
-    "datasource_result": BASE_URL + "/datasource/{}/result/",
-    "datasets": BASE_URL + "/datasets/",
-    "dataset_detail": BASE_URL + "/datasets/{}/",
-}
 
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger(__name__)
+SDK_ENPOINTS = {
+    "ai_models": SDK_URL + "ai-models/",
+    "ai_model": SDK_URL + "ai-model/{}/",
+    "tasks": SDK_URL + "tasks/",
+    "task": SDK_URL + "tasks/{}/",
+    "task_datasources": SDK_URL + "tasks/{}/datasources/",
+    "task_members": SDK_URL + "tasks/{}/members/",
+    "task_statistics": SDK_URL + "tasks/{}/statistics/",
+    "upload_data": SDK_URL + "upload-data/",
+    "download_data": SDK_URL + "tasks/{}/download-data/",
+    "datasets": SDK_URL + "datasets/",
+    "dataset": SDK_URL + "datasets/{}/",
+}
 
 
 class UnitlabClient:
     """A client with a connection to the Unitlab.ai platform.
 
     Note:
         Please refer to the `Python SDK quickstart <https://docs.unitlab.ai/tutorials/python-sdk-quickstart>`__ for a full example of working with the Python SDK.
@@ -60,141 +58,128 @@
 
     Args:
         api_key: Your Unitlab.ai API key. If no API key given, reads ``UNITLAB_API_KEY`` from the environment. Defaults to :obj:`None`.
     Raises:
         :exc:`~unitlab.exceptions.AuthenticationError`: If an invalid API key is used or (when not passing the API key directly) if ``UNITLAB_API_KEY`` is not found in your environment.
     """
 
-    def __init__(self, api_key: str = None, check_connection: bool = True):
+    def __init__(self, api_key: str = None):
         if api_key is None:
             api_key = os.getenv("UNITLAB_API_KEY")
             if api_key is None:
                 raise AuthenticationError(
                     message="Please provide the api_key argument or set UNITLAB_API_KEY in your environment."
                 )
-            logger.info("Found a Unitlab API key in your environment.")
-
+            logging.info("Found a Unitlab API key in your environment.")
         self.api_key = api_key
         self.api_session = requests.Session()
         adapter = requests.adapters.HTTPAdapter(max_retries=3)
         self.api_session.mount("http://", adapter)
         self.api_session.mount("https://", adapter)
-        if check_connection:
-            try:
-                r = self.api_session.get(
-                    f"{BASE_URL}/api-status/", headers=self._get_auth_header()
-                )
-                r.raise_for_status()
-                if r.status_code == 200:
-                    logger.info("Successfully connected to the Unitlab.ai API.")
-            except NetworkError:
-                raise AuthenticationError(
-                    message="Something went wrong. Did you use the right API key?"
-                )
 
     def close(self) -> None:
         """Close :class:`UnitlabClient` connections.
 
         You can manually close the Unitlab client's connections:
 
         .. code-block:: python
 
             client = UnitlabClient()
-            client.task_list()
+            client.tasks()
             client.close()
 
         Or use the client as a context manager:
 
         .. code-block:: python
 
             with UnitlabClient() as client:
-                client.task_list()
+                client.tasks()
         """
         self.api_session.close()
 
     def __enter__(self):
         return self
 
     def __exit__(
         self,
         exc_type,
         exc_value,
         traceback,
     ) -> None:
         self.close()
 
-    def _get_auth_header(self):
+    def _get_headers(self):
         return {"Authorization": f"Api-Key {self.api_key}"} if self.api_key else None
 
-    def task_list(self):
+    def tasks(self):
         """Get a list of all tasks.
 
         Returns:
             A list of all tasks.
         """
-        r = self.api_session.get(ENPOINTS["task_list"], headers=self._get_auth_header())
+        r = self.api_session.get(SDK_ENPOINTS["tasks"], headers=self._get_headers())
         r.raise_for_status()
         return r.json()
 
-    def task_detail(self, task_id):
+    def task(self, task_id):
         """Get a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             A task.
         """
         r = self.api_session.get(
-            ENPOINTS["task_detail"].format(task_id),
-            headers=self._get_auth_header(),
+            SDK_ENPOINTS["task"].format(task_id),
+            headers=self._get_headers(),
         )
         r.raise_for_status()
         return r.json()
 
     def task_data(self, task_id):
         """Get the data of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             The data of a task.
         """
         r = self.api_session.get(
-            ENPOINTS["task_data_sources"].format(task_id),
-            headers=self._get_auth_header(),
+            SDK_ENPOINTS["task_datasources"].format(task_id),
+            headers=self._get_headers(),
         )
         r.raise_for_status()
         return r.json()
 
     def task_members(self, task_id):
         """Get the members of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             The members of a task.
         """
         r = self.api_session.get(
-            ENPOINTS["task_members"].format(task_id),
-            headers=self._get_auth_header(),
+            SDK_ENPOINTS["task_members"].format(task_id),
+            headers=self._get_headers(),
         )
         r.raise_for_status()
         return r.json()
 
     def task_statistics(self, task_id):
         """Get the statistics of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             The statistics of a task.
         """
         r = self.api_session.get(
-            ENPOINTS["task_statistics"].format(task_id),
-            headers=self._get_auth_header(),
+            SDK_ENPOINTS["task_statistics"].format(task_id),
+            headers=self._get_headers(),
         )
         r.raise_for_status()
         return r.json()
 
     def upload_data(self, task_id, directory, batch_size=100):
         """Upload data to a task by id.
 
@@ -210,20 +195,20 @@
             raise ValueError(f"Directory {directory} does not exist")
 
         async def post_image(session: aiohttp.ClientSession, image: str, task_id: str):
             with open(image, "rb") as img:
                 try:
                     response = await session.request(
                         "POST",
-                        url=ENPOINTS["task_upload_datasources"],
+                        url=SDK_ENPOINTS["upload_data"],
                         data=aiohttp.FormData(fields={"task": task_id, "image": img}),
                     )
                     return 1 if response.status == 201 else 0
                 except Exception as e:
-                    logger.error(f"Error uploading image {image} - {e}")
+                    logging.error(f"Error uploading image {image} - {e}")
                     return 0
 
         async def batch_upload(
             session: aiohttp.ClientSession, batch: list, task_id: str, pbar: tqdm.tqdm
         ):
             tasks = []
             for image in batch:
@@ -239,18 +224,18 @@
                     for extension in ["*jpg", "*png"]
                 )
                 for image in images_list
             ]
             num_images = len(images)
             num_batches = (num_images + batch_size - 1) // batch_size
 
-            logger.info(f"Uploading {num_images} images to task {task_id}")
+            logging.info(f"Uploading {num_images} images to task {task_id}")
             with tqdm.tqdm(total=num_images, ncols=80) as pbar:
                 async with aiohttp.ClientSession(
-                    headers=self._get_auth_header()
+                    headers=self._get_headers()
                 ) as session:
                     for i in range(num_batches):
                         await batch_upload(
                             session,
                             images[
                                 i * batch_size : min((i + 1) * batch_size, num_images)
                             ],
@@ -265,16 +250,16 @@
 
         Args:
             task_id: The id of the task.
         Returns:
             Writes the data to a json file.
         """
         response = self.api_session.get(
-            url=ENPOINTS["task_download_data"].format(task_id),
-            headers=self._get_auth_header(),
+            url=SDK_ENPOINTS["download_data"].format(task_id),
+            headers=self._get_headers(),
         )
         response.raise_for_status()
         with self.api_session.get(
             url=response.json()["file"],
             stream=True,
         ) as r:
             r.raise_for_status()
@@ -287,63 +272,75 @@
                     filename = f"task-data-{task_id}.json"
             else:
                 filename = f"task-data-{task_id}.json"
 
             with open(filename, "wb") as f:
                 for chunk in r.iter_content(chunk_size=1024 * 1024):
                     f.write(chunk)
-            return os.path.abspath(filename)
 
     def ai_models(self):
         """Get a list of all ai models.
 
         Returns:
             A list of all ai models.
         """
-        r = self.api_session.get(
-            ENPOINTS["ai_model_list"], headers=self._get_auth_header()
-        )
+        r = self.api_session.get(SDK_ENPOINTS["ai_models"], headers=self._get_headers())
         r.raise_for_status()
         return r.json()
 
     def ai_model(self, ai_model_id):
         """Get an ai model by id.
 
         Args:
             ai_model_id: The id of the ai model.
         Returns:
             An ai model.
         """
         r = self.api_session.get(
-            ENPOINTS["ai_model_detail"].format(ai_model_id),
-            headers=self._get_auth_header(),
+            SDK_ENPOINTS["ai_model"].format(ai_model_id),
+            headers=self._get_headers(),
         )
         r.raise_for_status()
         return r.json()
 
     def datasets(self):
         """Get a list of all datasets.
 
         Returns:
             A list of all datasets.
         """
-        r = self.api_session.get(ENPOINTS["datasets"], headers=self._get_auth_header())
+        r = self.api_session.get(SDK_ENPOINTS["datasets"], headers=self._get_headers())
         r.raise_for_status()
         return r.json()
 
     def dataset(self, dataset_id):
-        """Get a dataset by id.
+        """Download a dataset by id.
 
         Args:
             dataset_id: The id of the dataset.
         Returns:
-            A dataset.
+            Writes the data to a json file.
         """
-        r = self.api_session.get(
-            ENPOINTS["dataset_detail"].format(dataset_id),
-            headers=self._get_auth_header(),
+        response = self.api_session.get(
+            url=SDK_ENPOINTS["dataset"].format(dataset_id),
+            headers=self._get_headers(),
         )
-        r.raise_for_status()
-        return r.json()["file"]
+        response.raise_for_status()
+        with self.api_session.get(
+            url=response.json()["file"],
+            stream=True,
+        ) as r:
+            r.raise_for_status()
+            if "Content-Disposition" in r.headers.keys():
+                content_disposition = r.headers["Content-Disposition"]
+                filename_match = re.search('filename="(.+)"', content_disposition)
+                if filename_match:
+                    filename = filename_match.group(1)
+                else:
+                    filename = f"dataset-{dataset_id}.json"
+            else:
+                filename = f"dataset-{dataset_id}.json"
 
-    def datasource_result(self, datasource_id):
-        raise NotImplementedError
+            with open(filename, "wb") as f:
+                for chunk in r.iter_content(chunk_size=1024 * 1024):
+                    f.write(chunk)
+        return os.path.abspath(filename)
```

### Comparing `unitlab-1.8.4/src/unitlab/exceptions.py` & `unitlab-1.8.5/src/unitlab/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,13 +19,7 @@
         return self.message
 
 
 class AuthenticationError(UnitlabError):
     """Raised when an API key fails authentication."""
 
     pass
-
-
-class NetworkError(UnitlabError):
-    """Raised when an HTTP error occurs."""
-
-    pass
```

### Comparing `unitlab-1.8.4/src/unitlab/run.py` & `unitlab-1.8.5/src/unitlab/run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,82 @@
-import os
+import logging
 from pathlib import Path
 from uuid import UUID
 
 import typer
 from typing_extensions import Annotated
 
-from . import pretty
+from . import cli
 from .client import UnitlabClient
 
 app = typer.Typer()
 
 API_KEY = Annotated[str, typer.Option(help="The api-key obtained from unitlab.ai")]
 
 
 def get_client(api_key: str) -> UnitlabClient:
-    return UnitlabClient(api_key=api_key, check_connection=False)
+    return UnitlabClient(api_key=api_key)
 
 
 @app.command(help="Task list")
 def tasks(api_key: API_KEY):
-    pretty.print_task(get_client(api_key).task_list(), many=True)
+    cli.tasks(api_key)
 
 
 @app.command(help="Task detail")
-def task(task_id: UUID, api_key: API_KEY):
-    pretty.print_task(get_client(api_key).task_detail(task_id=task_id), many=False)
+def task(pk: UUID, api_key: API_KEY):
+    cli.task(api_key, pk)
 
 
 @app.command(help="Task datasources")
-def task_data(task_id: UUID, api_key: API_KEY):
-    pretty.print_data_sources(get_client(api_key).task_data(task_id=task_id))
+def task_data(pk: UUID, api_key: API_KEY):
+    cli.task_data(api_key, pk)
 
 
 @app.command(help="Task members")
-def task_members(task_id: UUID, api_key: API_KEY):
-    pretty.print_members(get_client(api_key).task_members(task_id=task_id))
+def task_members(pk: UUID, api_key: API_KEY):
+    cli.task_members(api_key, pk)
 
 
 @app.command(help="Task statistics")
 def task_statistics(pk: UUID, api_key: API_KEY):
-    pretty.print_task_statistics(get_client(api_key).task_statistics(task_id=pk))
+    cli.task_statistics(api_key, pk)
 
 
 @app.command(help="Upload data")
 def upload_data(
     pk: UUID,
     api_key: API_KEY,
     directory: Annotated[
         Path, typer.Option(help="Directory containing the data to be uploaded")
     ],
 ):
-    get_client(api_key).upload_data(task_id=str(pk), directory=directory)
+    get_client(api_key).upload_data(str(pk), directory=directory)
 
 
 @app.command(help="Download data")
 def download_data(pk: UUID, api_key: API_KEY):
-    print("File:", get_client(api_key).download_data(task_id=pk))
-
-
-@app.command(help="Datasource result")
-def datasource_result(pk: UUID, api_key: API_KEY):
-    get_client(api_key).datasource_result(pk)
+    logging.info(f"File: {get_client(api_key).download_data(pk)}")
 
 
 @app.command(help="AI models")
 def ai_models(api_key: API_KEY):
-    pretty.print_ai_model(get_client(api_key).ai_models(), many=True)
+    cli.ai_models(api_key)
 
 
 @app.command(help="AI model")
 def ai_model(pk: UUID, api_key: API_KEY):
-    pretty.print_ai_model(get_client(api_key).ai_model(pk), many=False)
+    cli.ai_model(api_key, pk)
 
 
 @app.command(help="Datasets")
 def datasets(api_key: API_KEY):
-    pretty.print_datasets(get_client(api_key).datasets())
+    cli.datasets(api_key)
 
 
 @app.command(help="Dataset")
 def dataset(pk: UUID, api_key: API_KEY):
-    print("File: ", get_client(api_key).dataset(pk))
+    logging.info(f"File: {get_client(api_key).dataset(pk)}")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `unitlab-1.8.4/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.8.5/src/unitlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.4
+Version: 1.8.5
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

