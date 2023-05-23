# Comparing `tmp/vantage6-common-3.8.8rc3.tar.gz` & `tmp/vantage6-common-3.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-3.8.8rc3.tar", last modified: Mon May 22 13:38:28 2023, max compression
+gzip compressed data, was "vantage6-common-3.9.0rc2.tar", last modified: Tue May  9 13:37:04 2023, max compression
```

## Comparing `vantage6-common-3.8.8rc3.tar` & `vantage6-common-3.9.0rc2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.168110 vantage6-common-3.8.8rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-22 13:38:28.168110 vantage6-common-3.8.8rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:38:28.168110 vantage6-common-3.8.8rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.164109 vantage6-common-3.8.8rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.168110 vantage6-common-3.8.8rc3/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.168110 vantage6-common-3.8.8rc3/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-22 13:38:16.000000 vantage6-common-3.8.8rc3/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.168110 vantage6-common-3.8.8rc3/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-22 13:38:28.000000 vantage6-common-3.8.8rc3/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 13:38:28.000000 vantage6-common-3.8.8rc3/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:28.000000 vantage6-common-3.8.8rc3/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-22 13:38:28.000000 vantage6-common-3.8.8rc3/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 13:38:28.000000 vantage6-common-3.8.8rc3/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-09 13:36:37.000000 vantage6-common-3.9.0rc2/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.050815 vantage6-common-3.9.0rc2/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 13:37:04.000000 vantage6-common-3.9.0rc2/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-3.8.8rc3/PKG-INFO` & `vantage6-common-3.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.8rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc2 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.8.8rc3/setup.py` & `vantage6-common-3.9.0rc2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'appdirs==1.4.4',
         'click==8.1.3',
         'colorama==0.4.6',
         'cryptography==39.0.1',
-        'docker==6.1.2',
+        'docker==6.0.1',
         'pyfiglet==0.8.post1',
         'PyYAML==6.0',
         'python-dateutil==2.8.2',
         'schema==0.7.5',
     ],
     package_data={
         'vantage6.common': [
```

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/_version.py` & `vantage6-common-3.9.0rc2/vantage6/common/_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 8, 'candidate', __build__, 0)))
+version_info = (3, 9, 0, 'candidate', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
-pre_release = f'' if version_info[3] == 'final' else \
+pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
-post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
+post_release = '' if not version_info[5] else f'.post{version_info[5]}'
 
 # Module version accessible using thomas.__version__
 __version__ = f'{version}{pre_release}{post_release}'
```

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/docker/addons.py` & `vantage6-common-3.9.0rc2/vantage6/common/docker/addons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,89 @@
+from datetime import datetime
 import logging
 import re
 import docker
 import requests
 import base64
 import json
 import signal
 import pathlib
 
 from dateutil.parser import parse
 from docker.client import DockerClient
 from docker.models.containers import Container
 from docker.models.networks import Network
-from typing import Dict, Union
 
 from vantage6.common import logger_name
 from vantage6.common import ClickLogger
 from vantage6.common.globals import APPNAME
 
 log = logging.getLogger(logger_name(__name__))
 
 docker_client = docker.from_env()
 
 
 class ContainerKillListener:
     """Listen for signals that the docker container should be shut down """
     kill_now = False
 
-    def __init__(self):
+    def __init__(self) -> None:
         signal.signal(signal.SIGINT, self.exit_gracefully)
         signal.signal(signal.SIGTERM, self.exit_gracefully)
 
-    def exit_gracefully(self, *args):
+    def exit_gracefully(self, *args) -> None:
+        """Set kill_now to True. This will trigger the container to stop"""
         self.kill_now = True
 
 
-def check_docker_running():
-    """Return True if docker engine is running"""
+def check_docker_running() -> None:
+    """
+    Check if docker engine is running. If not, exit the program.
+    """
     try:
         docker_client.ping()
     except Exception as e:
         log.error("Cannot reach the Docker engine! Please make sure Docker "
                   "is running.")
         log.warn("Exiting...")
         log.debug(e)
         exit(1)
 
 
 def running_in_docker() -> bool:
-    """Return True if this code is executed within a Docker container."""
+    """
+    Check if this code is executed within a Docker container.
+
+    Returns
+    -------
+    bool
+        True if the code is executed within a Docker container, False otherwise
+    """
     return pathlib.Path('/.dockerenv').exists()
 
 
-def registry_basic_auth_header(docker_client, registry):
-    """Obtain credentials for registry
+def registry_basic_auth_header(
+        docker_client: DockerClient, registry: str) -> dict[str, str]:
+    """
+    Obtain credentials for registry
 
     This is a wrapper around docker-py to obtain the credentials used
     to access a registry. Normally communication to the registry goes
     through the Docker deamon API (locally), therefore we have to take
     extra steps in order to communicate with the (Harbor) registry
     directly.
 
     Note that this has only been tested for the harbor registries.
 
     Parameters
     ----------
+    docker_client: DockerClient
+        Docker client
     registry : str
-        registry name (e.g. harbor.vantage6.ai)
+        registry name (e.g. harbor2.vantage6.ai)
 
     Returns
     -------
     dict
         Containing a basic authorization header
     """
 
@@ -95,33 +109,35 @@
     # Encode them back to base64 and as a dict
     bytes_basic_auth = basic_auth.encode("utf-8")
     b64_basic_auth = base64.b64encode(bytes_basic_auth).decode("utf-8")
 
     return {'authorization': f'Basic {b64_basic_auth}'}
 
 
-def inspect_remote_image_timestamp(docker_client, image: str, log=ClickLogger):
+def inspect_remote_image_timestamp(
+    docker_client: DockerClient, image: str,
+    log: logging.Logger | ClickLogger = ClickLogger
+) -> tuple[datetime, str] | None:
     """
     Obtain creation timestamp object from remote image.
 
     Parameters
     ----------
-    reg : str
-        registry where the image is hosted
-    rep : str
-        repository in the registry
-    img : str
-        image name
-    tag : str, optional
-        image tag to be used, by default "latest"
+    docker_client: DockerClient
+        Docker client
+    image: str
+        Image name
+    log: logging.Logger | ClickLogger
+        Logger
 
     Returns
     -------
-    datetime
-        timestamp object containing the creation date and time of the image
+    tuple[datetime, str] | None
+        Timestamp containing the creation date of the image and its digest, or
+        None if the remote image could not be found.
     """
     # check if a tag has been profided
 
     image_tag = re.split(":", image)
     img = image_tag[0]
     tag = image_tag[1] if len(image_tag) == 2 else "latest"
 
@@ -129,29 +145,29 @@
         reg, rep, img_ = re.split("/", img)
     except ValueError:
         log.warn("Could not construct remote URL, "
                  "are you using a local image?")
         log.warn("Or an image from docker hub?")
         log.warn("We'll make a final attempt when running the image to pull"
                  " it without any checks...")
-        return
+        return None, None
 
     # figure out API of the docker repo
     v1_check = requests.get(f"https://{reg}/api/health")
     v1 = v1_check.status_code == 200
     v2 = False
     if not v1:
         v2_check = requests.get(f"https://{reg}/api/v2.0/health")
         v2 = v2_check.status_code == 200
 
     if not v1 and not v2:
         log.error(f"Could not determine version of the registry! {reg}")
         log.error("Is this a Harbor registry?")
         log.error("Or is the harbor server offline?")
-        return
+        return None, None
 
     if v1:
         image = f"https://{reg}/api/repositories/{rep}/{img_}/tags/{tag}"
     else:
         image = f"https://{reg}/api/v2.0/projects/{rep}/repositories/" \
                 f"{img_}/artifacts/{tag}"
 
@@ -159,97 +175,114 @@
     result = requests.get(
         image, headers=registry_basic_auth_header(docker_client, reg)
     )
 
     # verify that we got an result
     if result.status_code == 404:
         log.warn(f"Remote image not found! {image}")
-        return
+        return None, None
 
     if result.status_code != 200:
         log.warn(f"Remote info could not be fetched! ({result.status_code}) "
                  f"{image}")
-        return
+        return None, None
 
     if v1:
         timestamp = parse(result.json().get("created"))
+        digest = None
     else:
         timestamp = parse(result.json().get("push_time"))
-    return timestamp
+        digest = result.json().get("digest")
+    return timestamp, digest
 
 
-def inspect_local_image_timestamp(docker_client, image: str, log=ClickLogger):
+def inspect_local_image_timestamp(
+    docker_client: DockerClient, image: str,
+    log: logging.Logger | ClickLogger = ClickLogger
+) -> tuple[datetime, str] | None:
     """
     Obtain creation timestamp object from local image.
 
     Parameters
     ----------
-    reg : str
-        registry where the image is hosted
-    rep : str
-        repository in the registry
-    img : str
-        image name
-    tag : str, optional
-        image tag to be used, by default "latest"
+    docker_client: DockerClient
+        Docker client
+    image: str
+        Image name
+    log: logging.Logger | ClickLogger
+        Logger
 
     Returns
     -------
-    datetime
-        timestamp object containing the creation date and time of the image
+    tuple[datetime, str] | None
+        Timestamp containing the creation date and time of the local image and
+        the image digest. If the image does not exist, None is returned.
     """
-    # p = re.split(r"[/:]", image)
-    # if len(p) == 4:
-    #     image = f"{p[0]}/{p[1]}/{p[2]}:{p[3]}"
-
     try:
         img = docker_client.images.get(image)
     except docker.errors.ImageNotFound:
         log.debug(f"Local image does not exist! {image}")
-        return None
+        return None, None
     except docker.errors.APIError:
         log.debug(f"Local info not available! {image}")
-        return None
+        return None, None
 
+    try:
+        digest = img.attrs.get("RepoDigests")[0].split("@")[1]
+    except Exception:
+        digest = None
     timestamp = img.attrs.get("Created")
     timestamp = parse(timestamp)
-    return timestamp
+    return timestamp, digest
 
 
-def pull_if_newer(docker_client: DockerClient, image: str,
-                  log: Union[logging.Logger, ClickLogger] = ClickLogger):
+def pull_if_newer(
+    docker_client: DockerClient, image: str,
+    log: logging.Logger | ClickLogger = ClickLogger
+) -> None:
     """
     Docker pull only if the remote image is newer.
 
     Parameters
     ----------
     docker_client: DockerClient
         A Docker client instance
     image: str
         Image to be pulled
     log: logger.Logger or ClickLogger
         Logger class
+
+    Raises
+    ------
+    docker.errors.APIError
+        If the image cannot be pulled
     """
-    local_ = inspect_local_image_timestamp(docker_client, image, log=log)
-    remote_ = inspect_remote_image_timestamp(docker_client, image, log=log)
+    local_time, local_digest = inspect_local_image_timestamp(
+        docker_client, image, log=log
+    )
+    remote_time, remote_digest = inspect_remote_image_timestamp(
+        docker_client, image, log=log
+    )
     pull = False
-    if local_ and remote_:
-        if remote_ > local_:
+    if local_time and remote_time:
+        if remote_digest == local_digest:
+            log.debug(f"Local image is up-to-date: {image}")
+        elif remote_time > local_time:
             log.debug(f"Remote image is newer: {image}")
             pull = True
-        elif remote_ == local_:
+        elif remote_time == local_time:
             log.debug(f"Local image is up-to-date: {image}")
-        elif remote_ < local_:
+        elif remote_time < local_time:
             log.warn(f"Local image is newer! Are you testing? {image}")
-    elif local_:
+    elif local_time:
         log.warn(f"Only a local image has been found! {image}")
-    elif remote_:
+    elif remote_time:
         log.debug("No local image found, pulling from remote!")
         pull = True
-    elif not local_ and not remote_:
+    elif not local_time and not remote_time:
         log.warn(f"Cannot locate image {image} locally or remotely. Will try "
                  "to pull it from Docker Hub...")
         # we will try to pull it from the docker hub
         pull = True
 
     if pull:
         try:
@@ -301,15 +334,15 @@
     container = get_container(docker_client, **filters)
     if container:
         log.warn("Removing container that was already running: "
                  f"{container.name}")
         remove_container(container, kill=True)
 
 
-def remove_container(container: Container, kill=False) -> None:
+def remove_container(container: Container, kill: bool = False) -> None:
     """
     Removes a docker container
 
     Parameters
     ----------
     container: Container
         The container that should be removed
@@ -378,15 +411,15 @@
     # remove the network
     try:
         network.remove()
     except Exception:
         log.warn(f"Could not delete existing network {network.name}")
 
 
-def get_networks_of_container(container: Container) -> Dict:
+def get_networks_of_container(container: Container) -> dict:
     """
     Get list of networks the container is in
 
     Parameters
     ----------
     container: Container
         The container in which we are interested
@@ -426,15 +459,15 @@
             continue
         containers = network_obj.attrs['Containers']
         if len(containers) > 1:
             count_non_empty_networks += 1
     return count_non_empty_networks
 
 
-def get_server_config_name(container_name: str, scope: str):
+def get_server_config_name(container_name: str, scope: str) -> str:
     """
     Get the configuration name of a server from its docker container name
 
     Docker container name of the server is formatted as
     f"{APPNAME}-{self.name}-{self.scope}-server". This will return {self.name}
 
     Parameters
```

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/docker/network_manager.py` & `vantage6-common-3.9.0rc2/vantage6/common/docker/network_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import docker
 import logging
 
-from typing import List, Union
 from docker.models.containers import Container
 
 from vantage6.common.docker.addons import delete_network
 from vantage6.common import logger_name
 
 
 # TODO maybe move following to utils?
 def remove_subnet_mask(ip: str) -> str:
     """
     Remove the subnet mask of an ip address, e.g. 172.1.0.0/16 -> 172.1.0.0
+
+    Parameters
+    ----------
+    ip: str
+        IP subnet, potentially including a mask
+
+    Returns
+    -------
+    str
+        IP subnet address without the subnet mask
     """
     return ip[0:ip.find('/')]
 
 
 class NetworkManager(object):
     """
     Handle a Docker network
@@ -109,35 +118,35 @@
         -------
         bool
             Whether or not container is in the network
         """
         self.network.reload()
         return container in self.network.containers
 
-    def connect(self, container_name: str, aliases: List[str] = [],
-                ipv4: Union[str, None] = None) -> None:
+    def connect(self, container_name: str, aliases: list[str] = None,
+                ipv4: str | None = None) -> None:
         """
         Connect a container to the network.
 
         Parameters
         ----------
         container_name: str
             Name of the container that should be connected to the network
-        aliases: List[str]
+        aliases: list[str]
             A list of aliases for the container in the network
-        ipv4: str
+        ipv4: str | None
             An IP address to assign to the container in the network
         """
         self.log.debug(
             f"Connecting {container_name} to network '{self.network_name}'")
         self.network.connect(
             container_name, aliases=aliases, ipv4_address=ipv4
         )
 
-    def disconnect(self, container_name: str):
+    def disconnect(self, container_name: str) -> None:
         """
         Disconnect a container from the network.
 
         Parameters
         ----------
         container:
             Name of the container to disconnect
```

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/encryption.py` & `vantage6-common-3.9.0rc2/vantage6/common/encryption.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 All incomming messages (input/results) should be encrypted using the
 public key of this organization. This way we can decrypt them using our
 private key.
 
 In the case we are sending messages (input/results) we need to encrypt
 it using the public key of the receiving organization. (retreiving
 these public keys is outside the scope of this module).
-
-TODO handle no public key from other organization (should that happen here)
 """
+# TODO handle no public key from other organization (should that happen here?)
 import os
 import logging
 
 from pathlib import Path
+from typing import Any
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
@@ -45,81 +45,171 @@
     """Base class/interface for encryption implementations."""
     def __init__(self):
         """Create a new CryptorBase instance."""
         self.log = logging.getLogger(logger_name(__name__))
 
     @staticmethod
     def bytes_to_str(data: bytes) -> str:
-        """Encode bytes as base64 encoded string."""
+        """
+        Encode bytes as base64 encoded string.
+
+        Parameters
+        ----------
+        data: bytes
+            The data to encode.
+
+        Returns
+        -------
+        str
+            The base64 encoded string.
+        """
         return bytes_to_base64s(data)
 
     @staticmethod
     def str_to_bytes(data: str) -> bytes:
-        """Decode base64 encoded string to bytes."""
+        """
+        Decode base64 encoded string to bytes.
+
+        Parameters
+        ----------
+        data: str
+            The base64 encoded string.
+
+        Returns
+        -------
+        bytes
+            The encoded string converted to bytes.
+        """
         return base64s_to_bytes(data)
 
     def encrypt_bytes_to_str(self, data: bytes, pubkey_base64: str) -> str:
-        """Encrypt bytes in `data` using a (base64 encoded) public key."""
+        """
+        Encrypt bytes in `data` using a (base64 encoded) public key.
+
+        Note that the public key is ignored in this base class. If you want
+        to encode your data with a public key, use the `RSACryptor` class.
+
+        Parameters
+        ----------
+        data: bytes
+            The data to encrypt.
+        pubkey_base64: str
+            The public key to use for encryption. This is ignored in this
+            base class.
+
+        Returns
+        -------
+        str
+            The encrypted data encoded as base64 string.
+        """
         return self.bytes_to_str(data)
 
     def decrypt_str_to_bytes(self, data: str) -> bytes:
-        """Decrypt base64 encoded *string* `data."""
+        """
+        Decrypt base64 encoded *string* `data.
+
+        Parameters
+        ----------
+        data: str
+            The data to decrypt.
+
+        Returns
+        -------
+        bytes
+            The decrypted data.
+        """
         return self.str_to_bytes(data)
 
 
 # ------------------------------------------------------------------------------
 # DummyCryptor
 # ------------------------------------------------------------------------------
 class DummyCryptor(CryptorBase):
-    """Does absolutely nothing."""
+    """Does absolutely nothing to encrypt the data."""
 
 
 # ------------------------------------------------------------------------------
 # RSACryptor
 # ------------------------------------------------------------------------------
 class RSACryptor(CryptorBase):
-    """Wrapper class for the cryptography package.
+    """
+    Wrapper class for the cryptography package.
 
-        It loads the private key, and has an interface to encrypt en decrypt
-        messages. If no private key is found, it can generate one, and store
-        it at the default location. The encrpytion can be done via a public
-        key from another organization, make sure the key is in the right
-        data-type.
-
-        Communication between node and server requires serialization (and
-        deserialization) of the encrypted messages (which are in bytes).
-        The API can not communicate bytes, therefore a base64 conversion
-        needs to be executed (and also a utf-8 encoding needs to be applied
-        because of the way python implemented base64). The same goed for
-        sending and receiving the public_key.
+    It loads the private key, and has an interface to encrypt en decrypt
+    messages. If no private key is found, it can generate one, and store
+    it at the default location. The encrpytion can be done via a public
+    key from another organization, make sure the key is in the right
+    data-type.
+
+    Communication between node and server requires serialization (and
+    deserialization) of the encrypted messages (which are in bytes).
+    The API can not communicate bytes, therefore a base64 conversion
+    needs to be executed (and also a utf-8 encoding needs to be applied
+    because of the way python implemented base64). The same goes for
+    sending and receiving the public_key.
+
+    Parameters
+    ----------
+    private_key_file: Path
+        The path to the private key file.
     """
 
-    def __init__(self, private_key_file):
-        """Create a new RSACryptor instance."""
+    def __init__(self, private_key_file: Path) -> None:
+        """
+        Create a new RSACryptor instance.
+
+        Parameters
+        ----------
+        private_key_file: Path
+            The path to the private key file.
+        """
         super().__init__()
         self.private_key = self.__load_private_key(private_key_file)
 
-    def __load_private_key(self, private_key_file):
-        """ Load a private key file into this instance."""
+    def __load_private_key(self, private_key_file: Path) -> Any:
+        """
+        Load a private key file into this instance.
+
+        Parameters
+        ----------
+        private_key_file: Path
+            The path to the private key file.
+
+        Returns
+        -------
+        Any
+            The loaded private key.
+        """
 
         if not private_key_file.exists():
             raise FileNotFoundError(
                 f"Private key file {private_key_file} not found.")
 
         self.log.debug("Loading private key")
 
         return load_pem_private_key(
             private_key_file.read_bytes(),
             password=None,
             backend=default_backend()
         )
 
     @staticmethod
-    def create_new_rsa_key(path: Path):
-        """ Creates a new RSA key for E2EE.
+    def create_new_rsa_key(path: Path) -> rsa.RSAPrivateKey:
+        """
+        Creates a new RSA key for E2EE.
+
+        Parameters
+        ----------
+        path: Path
+            The path to the private key file.
+
+        Returns
+        -------
+        RSAPrivateKey
+            The newly created private key.
         """
         private_key = rsa.generate_private_key(
             backend=default_backend(),
             key_size=4096,
             public_exponent=65537
         )
 
@@ -129,32 +219,73 @@
                 format=serialization.PrivateFormat.TraditionalOpenSSL,
                 encryption_algorithm=serialization.NoEncryption()
             )
         )
         return private_key
 
     @property
-    def public_key_bytes(self):
-        """ Returns the public key bytes from the organization."""
+    def public_key_bytes(self) -> bytes:
+        """
+        Returns the public key bytes from the organization.
+
+        Returns
+        -------
+        bytes
+            The public key as bytes.
+        """
         return self.create_public_key_bytes(self.private_key)
 
     @staticmethod
-    def create_public_key_bytes(private_key):
+    def create_public_key_bytes(private_key: rsa.RSAPrivateKey) -> bytes:
+        """
+        Create a public key from a private key.
+
+        Parameters
+        ----------
+        private_key: RSAPrivateKey
+            The private key to use.
+
+        Returns
+        -------
+        bytes
+            The public key as bytes.
+        """
         return private_key.public_key().public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo
         )
 
     @property
-    def public_key_str(self):
-        """ Returns a JSON safe public key, used for the API."""
+    def public_key_str(self) -> str:
+        """
+        Returns a JSON safe public key, used for the API.
+
+        Returns
+        -------
+        str
+            The public key as base64 encoded string.
+        """
         return bytes_to_base64s(self.public_key_bytes)
 
     def encrypt_bytes_to_str(self, data: bytes, pubkey_base64s: str) -> str:
-        """Encrypt bytes in `data` using a (base64 encoded) public key."""
+        """
+        Encrypt bytes in `data` using a (base64 encoded) public key.
+
+        Parameters
+        ----------
+        data: bytes
+            The data to encrypt.
+        pubkey_base64s: str
+            The public key to use for encryption.
+
+        Returns
+        -------
+        str
+            The encrypted data encoded as base64 string.
+        """
 
         # Use the shared key for symmetric encryption/decryption of the payload
         shared_key = os.urandom(32)
         iv_bytes = os.urandom(16)
 
         cipher = Cipher(
             algorithms.AES(shared_key),
@@ -179,15 +310,27 @@
         encrypted_key = self.bytes_to_str(encrypted_key_bytes)
         iv = self.bytes_to_str(iv_bytes)
         encrypted_msg = self.bytes_to_str(encrypted_msg_bytes)
 
         return SEPARATOR.join([encrypted_key, iv, encrypted_msg])
 
     def decrypt_str_to_bytes(self, data: str) -> bytes:
-        """Decrypt base64 encoded *string* `data."""
+        """
+        Decrypt base64 encoded *string* `data.
+
+        Parameters
+        ----------
+        data: str
+            The data to decrypt.
+
+        Returns
+        -------
+        bytes
+            The decrypted data.
+        """
 
         (encrypted_key, iv, encrypted_msg) = data.split(SEPARATOR)
 
         # Yes, this can be done more efficiently.
         encrypted_key_bytes = self.str_to_bytes(encrypted_key)
         iv_bytes = self.str_to_bytes(iv)
         encrypted_msg_bytes = self.str_to_bytes(encrypted_msg)
@@ -208,20 +351,28 @@
         )
 
         decryptor = cipher.decryptor()
         result = decryptor.update(encrypted_msg_bytes) + decryptor.finalize()
 
         return result
 
-    def verify_public_key(self, pubkey_base64) -> bool:
-        """Verifies the public key.
-
-            Compare a public key with the generated public key from
-            the private key that is stored in this instance. This is
-            usefull for verifying that the public key stored on the
-            server is derived from the currently used private key.
+    def verify_public_key(self, pubkey_base64: str) -> bool:
+        """
+        Verifies the public key.
 
-            :param pubkey_base64: public_key as returned from the
-                server (still base64 encoded)
+        Compare a public key with the generated public key from the private key
+        that is stored in this instance. This is usefull for verifying that the
+        public key stored on the server is derived from the currently used
+        private key.
+
+        Parameters
+        ----------
+        pubkey_base64: str
+            The public key to verify as returned from the server.
+
+        Returns
+        -------
+        bool
+            True if the public key is valid, False otherwise.
         """
         public_key_server = base64s_to_bytes(pubkey_base64)
         return self.public_key_bytes == public_key_server
```

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/globals.py` & `vantage6-common-3.9.0rc2/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/task_status.py` & `vantage6-common-3.9.0rc2/vantage6/common/task_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from enum import Enum
 
 
 class TaskStatus(str, Enum):
+    """ Enum to represent the status of a task """
     # Task has not yet been started (usually, node is offline)
     PENDING = 'pending'
     # Task is being started
     INITIALIZING = 'initializing'
     # Container started without exceptions
     ACTIVE = 'active'
     # Container exited and had zero exit code
```

### Comparing `vantage6-common-3.8.8rc3/vantage6/common/utest.py` & `vantage6-common-3.9.0rc2/vantage6/common/utest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 import os
 
 import logging
 import unittest
 from datetime import datetime
 
+
 class TestResult(unittest.TextTestResult):
 
     def __init__(self, stream, descriptions, verbosity, log):
         super(TestResult, self).__init__(stream, descriptions, verbosity)
         self.log = log
 
     def startTest(self, test):
```

### Comparing `vantage6-common-3.8.8rc3/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-3.9.0rc2/vantage6_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.8rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc2 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.8.8rc3/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-3.9.0rc2/vantage6_common.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 vantage6/common/_version.py
 vantage6/common/colors.py
 vantage6/common/configuration_manager.py
 vantage6/common/context.py
 vantage6/common/encryption.py
 vantage6/common/exceptions.py
 vantage6/common/globals.py
+vantage6/common/log.py
 vantage6/common/task_status.py
 vantage6/common/utest.py
 vantage6/common/docker/__init__.py
 vantage6/common/docker/addons.py
 vantage6/common/docker/network_manager.py
 vantage6_common.egg-info/PKG-INFO
 vantage6_common.egg-info/SOURCES.txt
```

