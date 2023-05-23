# Comparing `tmp/vantage6-client-3.8.8rc3.tar.gz` & `tmp/vantage6-client-3.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-3.8.8rc3.tar", last modified: Mon May 22 13:38:28 2023, max compression
+gzip compressed data, was "vantage6-client-3.9.0rc2.tar", last modified: Tue May  9 13:37:04 2023, max compression
```

## Comparing `vantage6-client-3.8.8rc3.tar` & `vantage6-client-3.9.0rc2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.672125 vantage6-client-3.8.8rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-22 13:38:28.672125 vantage6-client-3.8.8rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:38:28.672125 vantage6-client-3.8.8rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.664124 vantage6-client-3.8.8rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.664124 vantage6-client-3.8.8rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.668125 vantage6-client-3.8.8rc3/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    81449 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.672125 vantage6-client-3.8.8rc3/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/dispatch_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-05-22 13:38:16.000000 vantage6-client-3.8.8rc3/vantage6/tools/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:28.672125 vantage6-client-3.8.8rc3/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-22 13:38:28.000000 vantage6-client-3.8.8rc3/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-22 13:38:28.000000 vantage6-client-3.8.8rc3/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:28.000000 vantage6-client-3.8.8rc3/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 13:38:28.000000 vantage6-client-3.8.8rc3/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 13:38:28.000000 vantage6-client-3.8.8rc3/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:04.810855 vantage6-client-3.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    83897 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/algorithm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/dispatch_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19081 2023-05-09 13:36:37.000000 vantage6-client-3.9.0rc2/vantage6/tools/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:04.806855 vantage6-client-3.9.0rc2/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 13:37:04.000000 vantage6-client-3.9.0rc2/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-3.8.8rc3/PKG-INFO` & `vantage6-client-3.9.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.8rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc2 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.8.8rc3/setup.py` & `vantage6-client-3.9.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/tests/test_client.py` & `vantage6-client-3.9.0rc2/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import json
 import pickle
-from typing import Dict
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 
 from vantage6.client import Client
 from vantage6.common.globals import STRING_ENCODING
 
 # Mock server
@@ -64,15 +63,15 @@
         mock_result = b'pickle.' + pickle.dumps([1, 2, 3, 4, 5])
 
         results = TestClient._receive_results_on_mock_client(mock_result)
 
         assert results == [{'result': [1, 2, 3, 4, 5]}]
 
     @staticmethod
-    def post_task_on_mock_client(input_, serialization: str) -> Dict[str, any]:
+    def post_task_on_mock_client(input_, serialization: str) -> dict[str, any]:
         mock_requests = MagicMock()
         mock_requests.get.return_value.status_code = 200
         mock_requests.post.return_value.status_code = 200
 
         mock_jwt = TestClient._create_mock_jwt()
         with patch.multiple('vantage6.client', requests=mock_requests, jwt=mock_jwt):
             client = TestClient.setup_client()
```

### Comparing `vantage6-client-3.8.8rc3/tests/test_deserialization.py` & `vantage6-client-3.9.0rc2/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/tests/test_docker_wrapper.py` & `vantage6-client-3.9.0rc2/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/tests/test_serialization.py` & `vantage6-client-3.9.0rc2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/vantage6/client/__init__.py` & `vantage6-client-3.9.0rc2/vantage6/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import pyfiglet
 import json as json_lib
 import itertools
 import sys
 import traceback
 
 from pathlib import Path
-from typing import Dict, Tuple, Union
 
 from vantage6.common.exceptions import AuthenticationException
 from vantage6.common import bytes_to_base64s, base64s_to_bytes
 from vantage6.common.globals import APPNAME
 from vantage6.common.encryption import RSACryptor, DummyCryptor
 from vantage6.common import WhoAmI
 from vantage6.client import serialization, deserialization
@@ -31,28 +30,40 @@
 
 module_name = __name__.split('.')[1]
 
 LEGACY = 'legacy'
 
 
 class ServerInfo(typing.NamedTuple):
-    """Data-class to store the server info."""
+    """
+    Data-class to store the server info.
+
+    Attributes
+    ----------
+    host : str
+        Adress (including protocol, e.g. `https://`) of the vantage6 server
+    port : int
+        Port numer to which the server listens
+    path : str
+        Path of the api, e.g. '/api'
+    """
     host: str
     port: int
     path: str
 
 
 class ClientBase(object):
     """Common interface to the central server.
 
-    Contains the basis for all other clients. This includes a basic interface
-    to authenticate, generic request, creating tasks and result retrieval.
+    Contains the basis for all other clients, e.g. UserClient, NodeClient and
+    AlgorithmClient. This includes a basic interface to authenticate, send
+    generic requests, create tasks and retrieve results.
     """
 
-    def __init__(self, host: str, port: int, path: str = '/api'):
+    def __init__(self, host: str, port: int, path: str = '/api') -> None:
         """Basic setup for the client
 
         Parameters
         ----------
         host : str
             Adress (including protocol, e.g. `https://`) of the vantage6 server
         port : int
@@ -74,48 +85,98 @@
         self.__refresh_url = None
 
         self.cryptor = None
         self.whoami = None
 
     @property
     def name(self) -> str:
-        """Return the node's/client's name"""
+        """
+        Return the node's/client's name
+
+        Returns
+        -------
+        str
+            Name of the user or node
+        """
         return self.whoami.name
 
     @property
     def headers(self) -> dict:
-        """Headers that are send with each request"""
+        """
+        Defines headers that are sent with each request. This includes the
+        authorization token.
+
+        Returns
+        -------
+        dict
+            Headers
+        """
         if self._access_token:
             return {'Authorization': 'Bearer ' + self._access_token}
         else:
             return {}
 
     @property
     def token(self) -> str:
-        """JWT Authorization token"""
+        """
+        JWT Authorization token
+
+        Returns
+        -------
+        str
+            JWT token
+        """
         return self._access_token
 
     @property
     def host(self) -> str:
-        """Host including protocol (HTTP/HTTPS)"""
+        """
+        Host including protocol (HTTP/HTTPS)
+
+        Returns
+        -------
+        str
+            Host address of the vantage6 server
+        """
         return self.__host
 
     @property
     def port(self) -> int:
-        """Port to vantage6-server listens"""
+        """
+        Port on which vantage6 server listens
+
+        Returns
+        -------
+        int
+            Port number
+        """
         return self.__port
 
     @property
     def path(self) -> str:
-        """Path/endpoint at the server where the api resides"""
+        """
+        Path/endpoint at the server where the api resides
+
+        Returns
+        -------
+        str
+            Path to the api
+        """
         return self.__api_path
 
     @property
     def base_path(self) -> str:
-        """Combination of host, port and api-path"""
+        """
+        Full path to the server URL. Combination of host, port and api-path
+
+        Returns
+        -------
+        str
+            Server URL
+        """
         if self.__port:
             return f"{self.host}:{self.port}{self.__api_path}"
 
         return f"{self.host}{self.__api_path}"
 
     def generate_path_to(self, endpoint: str) -> str:
         """Generate URL to endpoint using host, port and endpoint
@@ -216,14 +277,18 @@
         to the server.
 
         Parameters
         ----------
         private_key_file : str
             File path of the private key file
 
+        Raises
+        ------
+        AssertionError
+            If the client is not authenticated
         """
         assert self._access_token, \
             "Encryption can only be setup after authentication"
         assert self.whoami.organization_id, \
             "Organization unknown... Did you authenticate?"
 
         if private_key_file is None:
@@ -338,20 +403,22 @@
     def refresh_token(self) -> None:
         """Refresh an expired token using the refresh token
 
         Raises
         ------
         Exception
             Authentication Error!
+        AssertionError
+            Refresh URL not found
         """
         self.log.info("Refreshing token")
         assert self.__refresh_url, \
             "Refresh URL not found, did you authenticate?"
 
-        # if no port is specified explicit, then it should be omit the
+        # if no port is specified explicit, then it should be omnit the
         # colon : in the path. Similar (but different) to the property
         # base_path
         if self.__port:
             url = f"{self.__host}:{self.__port}{self.__refresh_url}"
         else:
             url = f"{self.__host}{self.__refresh_url}"
 
@@ -395,19 +462,26 @@
             Ids of organizations (within the collaboration) that need to
             execute this task, by default None
         data_format : str, optional
             Type of data format to use to send and receive
             data. possible values: 'json', 'pickle', 'legacy'. 'legacy'
             will use pickle serialization. Default is 'legacy'., by default
             LEGACY
+        database : str, optional
+            Database label to use for the task, by default 'default'
 
         Returns
         -------
         dict
             Containing the task meta-data
+
+        Raises
+        ------
+        AssertionError
+            Encryption has not yet been setup.
         """
         assert self.cryptor, "Encryption has not yet been setup!"
 
         if organization_ids is None:
             organization_ids = []
 
         if data_format == LEGACY:
@@ -437,15 +511,15 @@
             "description": description,
             "organizations": organization_json_list,
             'database': database
         })
 
     # TODO BvB 23-01-23 remove this method in v4+ (or make it private?). It is
     # only here for backwards compatibility.
-    def get_results(self, id_: int = None, state: str = None,
+    def get_results(self, id: int = None, state: str = None,
                     include_task: bool = False, task_id: int = None,
                     node_id: int = None, params: dict = {}) -> dict:
         """Get task result(s) from the central server
 
         Depending if a `id` is specified or not, either a single or a
         list of results is returned. The input and result field of the
         result are attempted te be decrypted. This fails if the public
@@ -455,74 +529,86 @@
         Parameters
         ----------
         id : int, optional
             Id of the result, by default None
         state : str, optional
             The state of the task (e.g. `open`), by default None
         include_task : bool, optional
-            Whenever to include the originating task, by default False
+            Whenever to include the orginating task, by default False
         task_id : int, optional
             The id of the originating task, this will return all results
             belonging to this task, by default None
         node_id : int, optional
             The id of the node at which this result has been produced,
             this will return all results from this node, by default None
+        params : dict, optional
+            Additional query parameters, by default {}
 
         Returns
         -------
         dict
             Containing the result(s)
         """
         # Determine endpoint and create dict with query parameters
-        endpoint = 'result' if not id_ else f'result/{id_}'
+        endpoint = 'result' if not id else f'result/{id}'
 
-        extended_params = params.copy()
         if state:
-            extended_params['state'] = state
+            params['state'] = state
         if include_task:
-            extended_params['include'] = 'task'
+            params['include'] = 'task'
         if task_id:
-            extended_params['task_id'] = task_id
+            params['task_id'] = task_id
         if node_id:
-            extended_params['node_id'] = node_id
+            params['node_id'] = node_id
 
         # self.log.debug(f"Retrieving results using query parameters:{params}")
-        results = self.request(endpoint=endpoint, params=extended_params)
+        results = self.request(endpoint=endpoint, params=params)
 
         if isinstance(results, str):
             self.log.warn("Requesting results failed")
             self.log.debug(f"Results message: {results}")
             return {}
 
         # hack: in the case that the pagination metadata is included we
         # need to strip that for decrypting
         if isinstance(results, dict) and 'data' in results:
             wrapper = results
             results = results['data']
 
-        if id_:
+        if id:
             # Single result
             self._decrypt_result(results)
 
         else:
             # Multiple results
             for result in results:
                 self._decrypt_result(result)
 
         if 'wrapper' in locals():
             wrapper['data'] = results
             results = wrapper
 
         return results
 
-    def _decrypt_result(self, result):
-        """Helper to decrypt the keys 'input' and 'result' in dict.
+    def _decrypt_result(self, result: dict) -> None:
+        """
+        Helper to decrypt the keys 'input' and 'result' in dict.
 
         Keys are replaced, but object reference remains intact: changes are
         made *in-place*.
+
+        Parameters
+        ----------
+        result : dict
+            The result dict to decrypt
+
+        Raises
+        ------
+        AssertionError
+            Encryption has not been initialized
         """
         assert self.cryptor, "Encryption has not been initialized"
         cryptor = self.cryptor
         try:
             self.log.info('Decrypting input')
             # TODO this only works when the results belong to the
             # same organization... We should make different implementation
@@ -540,37 +626,47 @@
 
         except ValueError as e:
             self.log.error("Could not decrypt/decode input or result.")
             self.log.error(e)
             # raise
 
     class SubClient:
-        """Create sub groups of commands using this SubClient"""
-        def __init__(self, parent):
+        """
+        Create sub groups of commands using this SubClient
+
+        Parameters
+        ----------
+        parent : UserClient
+            The parent client
+        """
+        def __init__(self, parent) -> None:
             self.parent: UserClient = parent
 
 
 class UserClient(ClientBase):
     """User interface to the vantage6-server"""
 
-    def __init__(self, *args, verbose=False, log_level='debug', **kwargs):
+    def __init__(self, *args, verbose=False, log_level='debug',
+                 **kwargs) -> None:
         """Create user client
 
         All paramters from `ClientBase` can be used here.
 
         Parameters
         ----------
         verbose : bool, optional
             Whenever to print (info) messages, by default False
+        log_level : str, optional
+            The log level to use, by default 'debug'
         """
         super(UserClient, self).__init__(*args, **kwargs)
 
         # Replace logger by print logger
         # TODO in v4+, remove the verbose option and only keep log_level
-        self.log = self.get_logger(verbose, log_level)
+        self.log = self._get_logger(verbose, log_level)
 
         # attach sub-clients
         self.util = self.Util(self)
         self.collaboration = self.Collaboration(self)
         self.organization = self.Organization(self)
         self.user = self.User(self)
         self.result = self.Result(self)
@@ -590,15 +686,15 @@
         self.log.info("Cite us!")
         self.log.info("If you publish your findings obtained using vantage6, ")
         self.log.info("please cite the proper sources as mentioned in:")
         self.log.info("https://vantage6.ai/vantage6/references")
         self.log.info("-" * 60)
 
     @staticmethod
-    def get_logger(enabled: bool, level: str) -> logging.Logger:
+    def _get_logger(enabled: bool, level: str) -> logging.Logger:
         """
         Create print-logger
 
         Parameters
         ----------
         enabled: bool
             If true, logging at most detailed level
@@ -627,26 +723,26 @@
                 f"{', '.join([lvl.value for lvl in LogLevel])}. ")
             logger.warn(f"Log level now set to {default_lvl}.")
         else:
             logger.setLevel(level)
         return logger
 
     def authenticate(self, username: str, password: str,
-                     mfa_code: Union[int, str] = None) -> None:
+                     mfa_code: int | str = None) -> None:
         """Authenticate as a user
 
         It also collects some additional info about your user.
 
         Parameters
         ----------
         username : str
             Username used to authenticate
         password : str
             Password used to authenticate
-        mfa_token: str or int
+        mfa_token: str | int
             Six-digit two-factor authentication code
         """
         auth_json = {
             "username": username,
             "password": password,
         }
         if mfa_code:
@@ -690,29 +786,29 @@
             self.log.info(f" --> Name: {name} (id={id_})")
             self.log.info(f" --> Organization: {organization_name} "
                           f"(id={organization_id})")
         except Exception:
             self.log.info('--> Retrieving additional user info failed!')
             self.log.error(traceback.format_exc())
 
-    def wait_for_results(self, task_id: int, sleep: float = 1) -> Dict:
+    def wait_for_results(self, task_id: int, sleep: float = 1) -> dict:
         """
         Polls the server to check when results are ready, and returns the
         results when the task is completed.
 
         Parameters
         ----------
         task_id: int
             ID of the task that you are waiting for
         sleep: float
             Interval in seconds between checks if task is finished. Default 1.
 
         Returns
         -------
-        Dict
+        dict
             A dictionary with the results of the task, after it has completed.
         """
         # Disable logging (additional logging would prevent the 'wait' message
         # from being printed on a single line)
         if isinstance(self.log, logging.Logger):
             prev_level = self.log.level
             self.log.setLevel(logging.WARN)
@@ -740,15 +836,15 @@
 
         return self.get_results(task_id=task_id)
 
     class Util(ClientBase.SubClient):
         """Collection of general utilities"""
 
         def get_server_version(self) -> dict:
-            r"""View the version number of the vantage6-server
+            """View the version number of the vantage6-server
 
             Returns
             -------
             dict
                 A dict containing the version number
             """
             return self.parent.request('version')
@@ -900,22 +996,19 @@
                 msg = result.get('msg')
                 self.parent.log.info(f'--> {msg}')
             return result
 
         def generate_private_key(self, file_: str = None) -> None:
             """Generate new private key
 
-            ....
-
             Parameters
             ----------
             file_ : str, optional
                 Path where to store the private key, by default None
             """
-
             if not file_:
                 self.parent.log.info('--> Using current directory')
                 file_ = "private_key.pem"
 
             if isinstance(file_, str):
                 file_ = Path(file_).absolute()
 
@@ -965,15 +1058,15 @@
             Returns
             -------
             list of dicts
                 Containing collabotation information
 
             Notes
             -----
-            - pagination does not work in combination with scope
+            - Pagination does not work in combination with scope
               `organization` as pagination is missing at endpoint
               /organization/<id>/collaboration
             """
             includes = ['metadata'] if include_metadata else []
             params = {
                 'page': page, 'per_page': per_page, 'include': includes,
                 'name': name, 'encrypted': encrypted,
@@ -1056,15 +1149,15 @@
 
         @post_filtering()
         def list(self, name: str = None, organization: int = None,
                  collaboration: int = None, is_online: bool = None,
                  ip: str = None, last_seen_from: str = None,
                  last_seen_till: str = None, page: int = 1, per_page: int = 20,
                  include_metadata: bool = True,
-                 ) -> list:
+                 ) -> list[dict]:
             """List nodes
 
             Parameters
             ----------
             name: str, optional
                 Filter by name (with LIKE operator)
             organization: int, optional
@@ -1198,17 +1291,19 @@
                 'kill/node/tasks', method='post', json={'id': id_}
             )
 
     class Organization(ClientBase.SubClient):
         """Collection of organization requests"""
 
         @post_filtering()
-        def list(self, name: str = None, country: int = None,
-                 collaboration: int = None, page: int = None,
-                 per_page: int = None, include_metadata: bool = True) -> list:
+        def list(
+            self, name: str = None, country: int = None,
+            collaboration: int = None, page: int = None, per_page: int = None,
+            include_metadata: bool = True
+        ) -> list[dict]:
             """List organizations
 
             Parameters
             ----------
             name: str, optional
                 Filter by name (with LIKE operator)
             country: str, optional
@@ -1222,15 +1317,15 @@
             include_metadata: bool, optional
                 Whenever to include the pagination metadata. If this is
                 set to False the output is no longer wrapped in a
                 dictonairy, by default True
 
             Returns
             -------
-            list of dicts
+            list[dict]
                 Containing meta-data information of the organizations
             """
             includes = ['metadata'] if include_metadata else []
             params = {
                 'page': page, 'per_page': per_page, 'include': includes,
                 'name': name, 'country': country,
                 'collaboration_id': collaboration
@@ -1503,16 +1598,16 @@
                 Role ids that are assigned to this user. Note that you
                 can only assign roles if you own the rules within this
                 role.
             rules : list of ints
                 Rule ids that are assigned to this user. Note that you
                 can only assign rules that you own
 
-            Return
-            ----------
+            Returns
+            -------
             dict
                 Containing data of the new user
             """
             user_data = {
                 'username': username,
                 'firstname': firstname,
                 'lastname': lastname,
@@ -1526,15 +1621,15 @@
 
     class Role(ClientBase.SubClient):
 
         @post_filtering()
         def list(self, name: str = None, description: str = None,
                  organization: int = None, rule: int = None, user: int = None,
                  include_root: bool = None, page: int = 1, per_page: int = 20,
-                 include_metadata: bool = True) -> list:
+                 include_metadata: bool = True) -> list[dict]:
             """List of roles
 
             Parameters
             ----------
             name: str, optional
                 Filter by name (with LIKE operator)
             description: str, optional
@@ -1555,15 +1650,15 @@
             include_metadata: bool, optional
                 Whenever to include the pagination metadata. If this is
                 set to False the output is no longer wrapped in a
                 dictonairy, by default True
 
             Returns
             -------
-            list of dicts
+            list[dict]
                 Containing roles meta-data
             """
             includes = ['metadata'] if include_metadata else []
             params = {
                 'page': page, 'per_page': per_page, 'include': includes,
                 'name': name, 'description': description,
                 'organization_id': organization, 'rule_id': rule,
@@ -1864,31 +1959,31 @@
             -------
             dict
                 Containing the result data
             """
             self.parent.log.info('--> Attempting to decrypt results!')
 
             # get_results also handles decryption
-            result = self.parent.get_results(id_=id_, include_task=include_task)
+            result = self.parent.get_results(id=id_, include_task=include_task)
             result_data = result.get('result')
             if result_data:
                 try:
                     result['result'] = deserialization.load_data(result_data)
                 except Exception as e:
                     self.parent.log.warn('--> Failed to deserialize')
                     self.parent.log.debug(e)
 
             return result
 
         @post_filtering()
         def list(self, task: int = None, organization: int = None,
                  state: str = None, node: int = None,
-                 include_task: bool = False, started: Tuple[str, str] = None,
-                 assigned: Tuple[str, str] = None,
-                 finished: Tuple[str, str] = None, port: int = None,
+                 include_task: bool = False, started: tuple[str, str] = None,
+                 assigned: tuple[str, str] = None,
+                 finished: tuple[str, str] = None, port: int = None,
                  page: int = None, per_page: int = None,
                  include_metadata: bool = True) -> list:
             """List results
 
             Parameters
             ----------
             task: int, optional
@@ -1897,41 +1992,38 @@
                 Filter by organization id
             state: int, optional
                 Filter by state: ('open',)
             node: int, optional
                 Filter by node id
             include_task : bool, optional
                 Whenever to include the task or not, by default False
-            started: Tuple[str, str], optional
+            started: tuple[str, str], optional
                 Filter on a range of start times (format: yyyy-mm-dd)
-            assigned: Tuple[str, str], optional
+            assigned: tuple[str, str], optional
                 Filter on a range of assign times (format: yyyy-mm-dd)
-            finished: Tuple[str, str], optional
+            finished: tuple[str, str], optional
                 Filter on a range of finished times (format: yyyy-mm-dd)
             port: int, optional
                 Port on which result was computed
             page: int, optional
                 Pagination page number, defaults to 1
             per_page: int, optional
                 Number of items per page, defaults to 20
             include_metedata: bool, optional
                 Whenevet to include pagination metadata, defaults to
                 True
 
             Returns
             -------
-            dict
-                Containing the key 'data' which contains a list of
+            dict | list[dict]
+                If include_metadata is True, a dictionary is returned
+                containing the key 'data' which contains a list of
                 results, and a key 'links' which contains the pagination
-                metadata
-
-            OR
-
-            list of dicts
-                When include_metadata is set to False, the metadata wrapper
+                metadata.
+                When include_metadata is False, the metadata wrapper
                 is stripped and only a list of results is returned
             """
             includes = []
             if include_metadata:
                 includes.append('metadata')
             if include_task:
                 includes.append('task')
@@ -1974,15 +2066,34 @@
 
             if 'wrapper' in locals():
                 wrapper['data'] = cleaned_results
                 cleaned_results = wrapper
 
             return cleaned_results
 
-        def from_task(self, task_id: int, include_task: bool = False):
+        # note: using typing.List instead of `list` to prevent referring
+        # to the list() function in an incorrect manner
+        def from_task(
+            self, task_id: int, include_task: bool = False
+        ) -> typing.List[dict]:
+            """
+            Get all results from a specific task
+
+            Parameters
+            ----------
+            task_id : int
+                Id of the task to get results from
+            include_task : bool, optional
+                Whenever to include the task or not, by default False
+
+            Returns
+            -------
+            list[dict]
+                Containing the results
+            """
             self.parent.log.info('--> Attempting to decrypt results!')
 
             # get_results also handles decryption
             results = self.parent.get_results(task_id=task_id,
                                               include_task=include_task)
             cleaned_results = []
             for result in results:
```

### Comparing `vantage6-client-3.8.8rc3/vantage6/client/_version.py` & `vantage6-client-3.9.0rc2/vantage6/client/_version.py`

 * *Files 10% similar despite different names*

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

### Comparing `vantage6-client-3.8.8rc3/vantage6/client/algorithm_client.py` & `vantage6-client-3.9.0rc2/vantage6/client/algorithm_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import jwt
 import pickle
 
-from typing import List, Union
-
 from vantage6.client import ClientBase
 from vantage6.client import base64s_to_bytes, bytes_to_base64s
 
 
 class AlgorithmClient(ClientBase):
     """
     Interface to communicate between the algorithm container and the central
@@ -26,15 +24,15 @@
     token: str
         JWT (container) token, generated by the node the algorithm container
         runs on
     *args, **kwargs
         Arguments passed to the parent ClientBase class.
     """
 
-    def __init__(self, token: str, *args, **kwargs):
+    def __init__(self, token: str, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         # obtain the identity from the token
         jwt_payload = jwt.decode(
             token, options={"verify_signature": False})
 
         # FIXME: 'identity' is no longer needed in version 4+. So this if
@@ -65,26 +63,36 @@
         self._access_token = token
 
     def request(self, *args, **kwargs) -> dict:
         """
         Make a request to the central server. This overwrites the parent
         function so that containers will not try to refresh their token, which
         they would be unable to do.
+
+        Parameters
+        ----------
+        *args, **kwargs
+            Arguments passed to the parent ClientBase.request function.
+
+        Returns
+        -------
+        dict
+            Response from the central server.
         """
         return super().request(*args, **kwargs, retry=False)
 
     class Result(ClientBase.SubClient):
         """
         Result client for the algorithm container.
 
         This client is used to obtain results of tasks with the same run_id
         from the central server.
         """
 
-        def get(self, task_id: int) -> List:
+        def get(self, task_id: int) -> list:
             """
             Obtain results from a specific task at the server.
 
             Containers are allowed to obtain the results of their children
             (having the same run_id at the server). The permissions are checked
             at te central server.
 
@@ -94,15 +102,15 @@
             Parameters
             ----------
             task_id: int
                 ID of the task from which you want to obtain the results
 
             Returns
             -------
-            List
+            list
                 List of results. The type of the results depends on the
                 algorithm.
             """
             results = self.parent.request(
                 f"task/{task_id}/result"
             )
 
@@ -142,30 +150,30 @@
                 Dictionary containing the task information
             """
             return self.parent.request(
                 f"task/{task_id}"
             )
 
         def create(
-            self, input_: bytes, organization_ids: List[int] = None,
+            self, input_: bytes, organization_ids: list[int] = None,
             name: str = "subtask", description: str = None
         ) -> dict:
             """
             Create a new (child) task at the central server.
 
             Containers are allowed to create child tasks (having the
             same run_id) at the central server. The docker image must
             be the same as the docker image of this container self.
 
             Parameters
             ----------
             input_ : bytes
                 Input to the task. Should be b64 encoded.
-            organization_ids : List[int], optional
-                List of organization IDs that should execute the task
+            organization_ids : list[int]
+                List of organization IDs that should execute the task.
             name: str, optional
                 Name of the subtask
             description : str, optional
                 Description of the subtask
 
             Returns
             -------
@@ -206,81 +214,127 @@
     class VPN(ClientBase.SubClient):
         """
         A VPN client for the algorithm container.
 
         It provides functions to obtain the IP addresses of other containers.
         """
         def get_addresses(
-            self, include_children: bool = False, include_parent: bool = False,
+            self, only_children: bool = False, only_parent: bool = False,
+            include_children: bool = False, include_parent: bool = False,
             label: str = None
-        ) -> Union[List[dict], dict]:
+        ) -> list[dict] | dict:
             """
             Get information about the VPN IP addresses and ports of other
             algorithm containers involved in the current task. These addresses
             can be used to send VPN communication to.
 
             Parameters
             ----------
+            only_children : bool, optional
+                Only return the IP addresses of the children of the current
+                task, by default False. Incompatible with only_parent.
+            only_parent : bool, optional
+                Only return the IP address of the parent of the current task,
+                by default False. Incompatible with only_children.
             include_children : bool, optional
                 Include the IP addresses of the children of the current task,
-                by default False.
+                by default False. Incompatible with only_parent, superseded
+                by only_children.
             include_parent : bool, optional
                 Include the IP address of the parent of the current task, by
-                default False.
+                default False. Incompatible with only_children, superseded by
+                only_parent.
             label : str, optional
                 The label of the port you are interested in, which is set
                 in the algorithm Dockerfile. If this parameter is set, only
                 the ports with this label will be returned.
 
             Returns
             -------
-            List[dict] or dict
+            list[dict] | dict
                 List of dictionaries containing the IP address and port number,
                 and other information to identify the containers. If obtaining
                 the VPN addresses from the server fails, a dictionary with a
                 'message' key is returned instead.
             """
             results = self.parent.request("vpn/algorithm/addresses", params={
+                "only_children": only_children,
+                "only_parent": only_parent,
                 "include_children": include_children,
                 "include_parent": include_parent,
                 "label": label
             })
 
             if 'addresses' not in results:
                 return {'message': 'Obtaining VPN addresses failed!'}
 
             return results['addresses']
 
+        def get_parent_address(self) -> dict:
+            """
+            Get the IP address and port number of the parent of the current
+            task.
+
+            Returns
+            -------
+            dict
+                Dictionary containing the IP address and port number, and other
+                information to identify the containers. If obtaining the VPN
+                addresses from the server fails, a dictionary with a 'message'
+                key is returned instead.
+            """
+            return self.get_addresses(only_parent=True)
+
+        def get_child_addresses(self) -> list[dict]:
+            """
+            Get the IP addresses and port numbers of the children of the
+            current task.
+
+            Returns
+            -------
+            List[dict]
+                List of dictionaries containing the IP address and port number,
+                and other information to identify the containers. If obtaining
+                the VPN addresses from the server fails, a dictionary with a
+                'message' key is returned instead.
+            """
+            return self.get_addresses(only_children=True)
+
     class Organization(ClientBase.SubClient):
         """
         Get information about organizations in the collaboration.
         """
         def get(self, id_: int) -> dict:
             """
             Get an organization by ID.
 
             Parameters
             ----------
             id: int
                 ID of the organization to retrieve
+
+            Returns
+            -------
+            dict
+                Dictionary containing the organization data.
             """
             return self.parent.request(f"organization/{id_}")
 
-        def list(self) -> List[dict]:
+        def list(self) -> list[dict]:
             """
             Obtain all organization in the collaboration.
 
             The container runs in a Node which is part of a single
             collaboration. This method retrieves all organization data that are
             within that collaboration. This can be used to target specific
             organizations in a collaboration.
 
             Returns
             -------
-            List[dict]
+            list[dict]
                 List of organizations in the collaboration.
             """
             organizations = self.parent.request(
                 "organization",
                 params={"collaboration_id": self.parent.collaboration_id}
             )
             return organizations
@@ -308,10 +362,11 @@
         def get(self) -> dict:
             """
             Get the node data.
 
             Returns
             -------
             dict
-                Dictionary containing the node data.
+                Dictionary containing data on the node this algorithm is
+                running on.
             """
             return self.parent.request(f"node/{self.parent.host_node_id}")
```

### Comparing `vantage6-client-3.8.8rc3/vantage6/client/deserialization.py` & `vantage6-client-3.9.0rc2/vantage6/client/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/vantage6/client/serialization.py` & `vantage6-client-3.9.0rc2/vantage6/client/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/vantage6/client/utils.py` & `vantage6-client-3.9.0rc2/vantage6/client/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import qrcode
 
 from enum import Enum
-from typing import Dict
 
 
-def print_qr_code(json_data: Dict) -> None:
+def print_qr_code(json_data: dict) -> None:
     """
     Print the QR code for 2fa with additional info of how to use it.
 
     This function should work in any terminal or Python scripting environment.
     Therefore, all is printed regardless of log level
 
     Parameters
     ----------
-    json_data: Dict
+    json_data: dict
         A dictionary containing the secret and URI to generate the QR code
     """
     print("This server has obligatory two-factor authentication. Please scan "
           "the QR code below with your favorite authenticator app (we "
           "recommend the LastPass or Google Authenticator).")
     print("After you have authenticated, please log in again.")
     show_qr_code_image(json_data.get('qr_uri'))
@@ -43,12 +42,28 @@
     )
     qr.add_data(qr_uri)
     qr.make(fit=True)
     qr.print_ascii()
 
 
 class LogLevel(Enum):
+    """
+    Enum for the different log levels
+
+    Attributes
+    ----------
+    DEBUG: str
+        The debug log level
+    INFO: str
+        The info log level
+    WARN: str
+        The warn log level
+    ERROR: str
+        The error log level
+    CRITICAL: str
+        The critical log level
+    """
     DEBUG = 'DEBUG'
     INFO = 'INFO'
     WARN = 'WARN'
     ERROR = 'ERROR'
     CRITICAL = 'CRITICAL'
```

### Comparing `vantage6-client-3.8.8rc3/vantage6/tools/deserialization.py` & `vantage6-client-3.9.0rc2/vantage6/tools/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/vantage6/tools/serialization.py` & `vantage6-client-3.9.0rc2/vantage6/tools/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/vantage6/tools/util.py` & `vantage6-client-3.9.0rc2/vantage6/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.8rc3/vantage6/tools/wrapper.py` & `vantage6-client-3.9.0rc2/vantage6/tools/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """
-Wrapper
-
 This module contains algorithm wrappers. These wrappers are used to provide
 different data adapters to the algorithms. This way we ony need to write the
 algorithm once and can use it with different data adapters.
 
 Currently the following wrappers are available:
     - ``DockerWrapper`` (= ``CSVWrapper``)
     - ``SparqlDockerWrapper``
@@ -78,15 +76,15 @@
     database_type = os.environ.get(f"{label.upper()}_DATABASE_TYPE", "csv")\
         .lower()
 
     # Create the correct wrapper based on the database type, note that the
     # multi database wrapper is not available.
     if database_type == "csv":
         wrapper = CSVWrapper()
-    elif database_type == "excel":
+    if database_type == "excel":
         wrapper = ExcelWrapper()
     elif database_type == "sparql":
         wrapper = SparqlDockerWrapper()
     elif database_type == "parquet":
         wrapper = ParquetWrapper()
     elif database_type == "sql":
         wrapper = SQLWrapper()
@@ -173,14 +171,15 @@
                        use_new_client: bool = False) -> None:
         """
         Wrap an algorithm module to provide input and output handling for the
         vantage6 infrastructure.
 
         Data is received in the form of files, whose location should be
         specified in the following environment variables:
+
         - ``INPUT_FILE``: input arguments for the algorithm
         - ``OUTPUT_FILE``: location where the results of the algorithm should
           be stored
         - ``TOKEN_FILE``: access token for the vantage6 server REST api
         - ``DATABASE_URI``: either a database endpoint or path to a csv file.
 
         The wrapper is able to parse a number of input file formats. The
@@ -287,14 +286,15 @@
         pandas.DataFrame
             The data from the csv file
         """
         return pandas.read_csv(database_uri)
 
 
 # for backwards compatibility
+# TODO BvB 2023-03-02 remove in v5+?
 CsvWrapper = CSVWrapper
 DockerWrapper = CSVWrapper
 
 
 class ExcelWrapper(WrapperBase):
     @staticmethod
     def load_data(database_uri: str, input_data: dict) -> pandas.DataFrame:
@@ -341,14 +341,30 @@
         if 'query' not in input_data:
             error("No query in the input specified. Exiting ...")
         query = input_data['query']
         return SparqlDockerWrapper._query_triplestore(database_uri, query)
 
     @staticmethod
     def _query_triplestore(endpoint: str, query: str) -> pandas.DataFrame:
+        """
+        Send a query to a triplestore and return the result as a pandas
+        DataFrame.
+
+        Parameters
+        ----------
+        endpoint : str
+            URI of the triplestore
+        query : str
+            The query to send to the triplestore
+
+        Returns
+        -------
+        pandas.DataFrame
+            The result of the query
+        """
         sparql = SPARQLWrapper(endpoint, returnFormat=_SPARQL_RETURN_FORMAT)
         sparql.setQuery(query)
 
         result = sparql.query().convert().decode()
 
         return pandas.read_csv(io.StringIO(result))
 
@@ -509,14 +525,27 @@
                 input_data = pickle.load(fp)
             except pickle.UnpicklingError:
                 raise DeserializationException('Could not deserialize input')
     return input_data
 
 
 def _read_formatted(file: BinaryIO) -> Any:
+    """
+    Try to read the prescribed data format.
+
+    Parameters
+    ----------
+    file : BinaryIO
+        Input file received from the user.
+
+    Returns
+    -------
+    Any
+        Deserialized input data
+    """
     data_format = str.join('', list(_read_data_format(file)))
     data_format = DataFormat(data_format.lower())
     return deserialization.deserialize(file, data_format)
 
 
 def _read_data_format(file: BinaryIO) -> Generator:
     """
```

### Comparing `vantage6-client-3.8.8rc3/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-3.9.0rc2/vantage6_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.8rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc2 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.8.8rc3/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-3.9.0rc2/vantage6_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

