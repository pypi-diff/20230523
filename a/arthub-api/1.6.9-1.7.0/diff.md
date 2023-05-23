# Comparing `tmp/arthub_api-1.6.9.tar.gz` & `tmp/arthub_api-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.9.tar", last modified: Fri May 19 06:21:27 2023, max compression
+gzip compressed data, was "arthub_api-1.7.0.tar", last modified: Tue May 23 10:47:51 2023, max compression
```

## Comparing `arthub_api-1.6.9.tar` & `arthub_api-1.7.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.691635 arthub_api-1.6.9/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.9/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-19 06:21:27.691131 arthub_api-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.6.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.666960 arthub_api-1.6.9/arthub_api/
--rw-rw-rw-   0        0        0      645 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3483 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.9/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.9/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    42964 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2070 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    26625 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.9/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.9/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.9/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.9/arthub_api/models.py
--rw-rw-rw-   0        0        0    42130 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.9/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-19 06:20:15.000000 arthub_api-1.6.9/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.679145 arthub_api-1.6.9/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.9/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-19 06:21:26.000000 arthub_api-1.6.9/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.9/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 06:21:27.691635 arthub_api-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0     3079 2023-05-19 06:20:15.000000 arthub_api-1.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:21:27.689424 arthub_api-1.6.9/tests/
--rw-rw-rw-   0        0        0      139 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/_utils.py
--rw-rw-rw-   0        0        0      280 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/conftest.py
--rw-rw-rw-   0        0        0     6110 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_open_api.py
--rw-rw-rw-   0        0        0    17906 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3647 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_storage.py
--rw-rw-rw-   0        0        0     7255 2023-05-19 06:20:15.000000 arthub_api-1.6.9/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:47:51.975453 arthub_api-1.7.0/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-23 10:47:51.974454 arthub_api-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 10:47:51.891678 arthub_api-1.7.0/arthub_api/
+-rw-rw-rw-   0        0        0      675 2023-05-22 10:07:06.000000 arthub_api-1.7.0/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3730 2023-05-22 10:07:06.000000 arthub_api-1.7.0/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-23 10:45:39.000000 arthub_api-1.7.0/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.7.0/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      104 2023-05-22 10:07:06.000000 arthub_api-1.7.0/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-05-22 10:07:06.000000 arthub_api-1.7.0/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-05-22 10:07:06.000000 arthub_api-1.7.0/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2070 2023-05-19 06:20:15.000000 arthub_api-1.7.0/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28363 2023-05-23 10:45:39.000000 arthub_api-1.7.0/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.7.0/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1443 2023-05-23 10:45:39.000000 arthub_api-1.7.0/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.7.0/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.7.0/arthub_api/models.py
+-rw-rw-rw-   0        0        0    42924 2023-05-23 10:45:39.000000 arthub_api-1.7.0/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41836 2023-05-22 10:07:06.000000 arthub_api-1.7.0/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     9100 2023-05-23 10:45:39.000000 arthub_api-1.7.0/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:47:51.922592 arthub_api-1.7.0/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-23 10:47:51.000000 arthub_api-1.7.0/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-23 10:47:51.000000 arthub_api-1.7.0/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 10:47:51.000000 arthub_api-1.7.0/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-23 10:47:51.000000 arthub_api-1.7.0/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.7.0/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2023-05-23 10:47:51.000000 arthub_api-1.7.0/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 10:47:51.000000 arthub_api-1.7.0/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.7.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 10:47:51.975453 arthub_api-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3079 2023-05-19 06:20:15.000000 arthub_api-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 10:47:51.972460 arthub_api-1.7.0/tests/
+-rw-rw-rw-   0        0        0      176 2023-05-22 10:07:06.000000 arthub_api-1.7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.7.0/tests/_utils.py
+-rw-rw-rw-   0        0        0      280 2023-05-19 06:20:15.000000 arthub_api-1.7.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     6110 2023-05-19 06:20:15.000000 arthub_api-1.7.0/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    18818 2023-05-22 10:07:06.000000 arthub_api-1.7.0/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3647 2023-05-19 06:20:15.000000 arthub_api-1.7.0/tests/test_storage.py
+-rw-rw-rw-   0        0        0     8450 2023-05-23 10:45:39.000000 arthub_api-1.7.0/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.9/LICENSE` & `arthub_api-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/PKG-INFO` & `arthub_api-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.9
+Version: 1.7.0
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.9/README.md` & `arthub_api-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/arthub_api/__init__.py` & `arthub_api-1.7.0/arthub_api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,18 @@
     __copyright__,
     __description__,
     __license__,
     __title__,
     __url__,
     __version__,
 )
-from .__main__ import init_config
+from .__main__ import (
+    init_config,
+    setup_logging
+)
 
 from .open_api import (
     OpenAPI,
     APIResponse
 )
 
 from .blade_api import (
```

### Comparing `arthub_api-1.6.9/arthub_api/__main__.py` & `arthub_api-1.7.0/arthub_api/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 @environ.config(prefix="AH_BLADE")
 class DefaultEnvConfig(object):
     """This creates a env config loads from AH_XXXXX and AH_BLADE_XXXX."""
     api_config_name = environ.var(os.getenv("AH_API_CONFIG_NAME"), help="Api config name. one of ['oa', 'qq']")
     public_token = environ.var("",  help="Value for blade public token auth method.")
     account_email = environ.var(os.getenv("AH_ACCOUNT_NAME"),  help="User name for login auth method.")
     password = environ.var(os.getenv("AH_PASSWORD"),  help="User password for login auth method.")
+    log_level= environ.var(os.getenv('AH_LOG_LEVEL', 'INFO'), help="Log level for arthub_api", converter=lambda x:x.upper())
 
 
 def load_config(file_path=None):
     UserError = type("UserError", (Exception,), {})
 
     file_path = file_path or os.getenv("ARTHUB_API_CONFIG",
                                        os.path.expanduser("~/Documents/ArtHub/arthub_api_config.py"))
@@ -57,32 +58,32 @@
         if member.startswith("__"):
             continue
 
         setattr(arthub_api_config, "_%s" % member,
                 getattr(arthub_api_config, member))
 
 
-def setup_logging():
-    logger = logging.getLogger()
-    logger.setLevel(logging.DEBUG)
+def setup_logging(log_level=logging.INFO):
+    logger = utils.logger
+    logger.setLevel(log_level)
 
     # to file
     log_dir = os.path.expanduser("~/Documents/ArtHub/sdk_log")
     if utils.mkdir(log_dir):
         f_handler = logging.handlers.TimedRotatingFileHandler(os.path.join(log_dir, "arthub_api.log"),
                                                               when='midnight', interval=1,
                                                               backupCount=7)
-        f_handler.setLevel(logging.INFO)
+        f_handler.setLevel(log_level)
         f_handler.setFormatter(
             logging.Formatter("%(asctime)s - %(levelname)s - %(filename)s[:%(lineno)d] - %(message)s"))
         logger.addHandler(f_handler)
 
     # to stdout
     s_handler = logging.StreamHandler()
-    s_handler.setLevel(logging.DEBUG)
+    s_handler.setLevel(log_level)
     s_handler.setFormatter(logging.Formatter("%(message)s"))
     logger.addHandler(s_handler)
 
 
 def apply_environ_to_config():
     """This loads config from env and set into arthub_api_config."""
     ENV_CONFIG = environ.to_config(DefaultEnvConfig)
@@ -90,23 +91,25 @@
         arthub_api_config.api_config_name = ENV_CONFIG.api_config_name
     if ENV_CONFIG.public_token:
         arthub_api_config.blade_public_token = ENV_CONFIG.public_token
     if ENV_CONFIG.account_email:
         arthub_api_config.account_email = ENV_CONFIG.account_email
     if ENV_CONFIG.password:
         arthub_api_config.password = ENV_CONFIG.password
+    if ENV_CONFIG.log_level:
+        arthub_api_config.log_level = ENV_CONFIG.log_level
 
 
 def init_config():
-    setup_logging()
     patch_config()
     load_config()
     apply_environ_to_config()
 
 
 def main():
     init_config()
+    setup_logging(arthub_api_config.log_level)
     cli.cli()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `arthub_api-1.6.9/arthub_api/_internal_utils.py` & `arthub_api-1.7.0/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/arthub_api/blade_api.py` & `arthub_api-1.7.0/arthub_api/blade_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 """
 arthub_api.blade_api
 ~~~~~~~~~~~~~~
 
 This module encapsulates the API for blade tool system.
 """
-import logging
+import copy
+from contextlib import contextmanager
 from .open_api import (
     OpenAPI
 )
 from . import arthub_api_config
+from .config import api_config_oa
+from .utils import get_config_by_name
 
 
 class BladeAPI(OpenAPI):
-    def __init__(self, config, get_token_from_cache=True, blade_public_token=""):
+    def __init__(self, config=api_config_oa, get_token_from_cache=True, blade_public_token="", api_config_name=None):
         r"""Used to call Blade openapi.
 
         :param config: from arthub_api.config.
         :param get_token_from_cache: read token from local cache.
         """
-        super(BladeAPI, self).__init__(config, get_token_from_cache)
+        super(BladeAPI, self).__init__(config, get_token_from_cache, api_config_name=api_config_name)
         self._api_version_blade = "v1"
         self.blade_public_token = blade_public_token
+        
+    @contextmanager
+    def switch_config(self, api_config_name, get_token_from_cache=True, blade_public_token=""):
+        config = get_config_by_name(api_config_name, api_config_oa)
+        old__dict = copy.copy(self.__dict__)
+        self.__dict__ = BladeAPI(config, get_token_from_cache, blade_public_token).__dict__.copy()
+        yield
+        self.__dict__ = old__dict
 
     def init_from_config(self):
         super(BladeAPI, self).init_from_config()
         self.blade_public_token = arthub_api_config.blade_public_token
 
     def _blade_url(self, api_method):
         return "%s//%s/blade/blade/openapi/%s/core/%s" % (
```

### Comparing `arthub_api-1.6.9/arthub_api/blade_api_instance.py` & `arthub_api-1.7.0/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/arthub_api/blade_storage.py` & `arthub_api-1.7.0/arthub_api/blade_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """internal COS API can be used to upload and download files from COS."""
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 # Import built-in modules
-import six
 import logging
+import six
 import socket
 import os
 import time
 import threading
 import requests
 import concurrent
 import json
@@ -22,24 +22,33 @@
 
 # Import third-party modules
 from tenacity import retry as tenacity_retry
 from tenacity import retry_if_exception_type
 from tenacity import stop_after_attempt
 from tenacity import wait_fixed
 from tenacity import RetryError
+from tenacity.before import before_log
 from xml.etree import ElementTree
 
+from arthub_api.open_api import APIError
 # Import local modules
-from arthub_api.__version__ import __title__
-from arthub_api.blade_api import BladeAPI
+from arthub_api.utils import logger
 import arthub_api.utils as utils
 import arthub_api._internal_utils as _internal_utils
 
 
-logger = logging.getLogger(__title__)
+allowed_schemes = ["http", "https"]
+
+
+def normalize_scheme(scheme):
+    scheme = scheme.rstrip(":")
+    if scheme not in allowed_schemes:
+        scheme = "https"
+    return scheme
+
 
 if six.PY2:
     class PermissionError(OSError):
         pass
     class FileNotFoundError(IOError):
         pass
 
@@ -50,15 +59,19 @@
     pass
 
 # signer for blade api
 class RemoteSignerForPackage(object):    
     def __init__(self, blade_backend, force=False):
         self.cli = blade_backend
         self.force = force
-        
+        self.scheme = "https"
+
+    def set_scheme(self, scheme):
+        self.scheme = normalize_scheme(scheme)
+
     @classmethod
     def _remove_suffix(cls, s, sf):
         if s.endswith(sf):
             return s[:len(s)-len(sf)]
         return s
 
     @classmethod
@@ -74,15 +87,15 @@
         return {"name": result[2], "version": result[3]}
     
     def _take_signed_url(self, arthub_response, type_of_sign=""):
         arthub_response.raise_for_err()
         logger.debug('{0} sign-url rsp is {1}'.format(type_of_sign, arthub_response.result))
         if len(arthub_response.result) == 0:
             raise SignerError("arthub api: result is empty")
-        return "https:" + arthub_response.result[0].get('signed_url')
+        return self.scheme + ":" + arthub_response.result[0].get('signed_url')
         
     # we use bucket + key to identify a file. 
     # however bucket might be fixed for ArtHub condition, so bucket input is ignored
     # pkg do not supports for expired argument
     def _get_package_download_sign(self, bucket, key, expired=1200):
         pkg = self._key_to_pkg(key)
         # this will return a url expires in 10 minutes
@@ -92,15 +105,15 @@
             raise SignerError("arthub api: result is empty")
         logger.debug("download sign-url rsp is {0}".format(signed.result))
         return signed.result
     
     # pkg do not supports for expired argument
     def get_download_url(self, bucket, key, expired=1200):
         signed = self._get_package_download_sign(bucket, key, expired)
-        return "https:" + signed[0].get('signed_url')
+        return self.scheme + ":" + signed[0].get('signed_url')
         
     def get_file_size(self, bucket, key):
         signed = self._get_package_download_sign(bucket, key)
         return signed[0].get('size')
     
     def get_upload_url(self, bucket, key, expired=1200):
         pkg = self._key_to_pkg(key)
@@ -121,39 +134,43 @@
     def get_complete_multipart_upload_url(self, bucket, key, upload_id, expired=1200):
         pkg = self._key_to_pkg(key)
         pkg.update({"upload_id": upload_id})
         signed = self.cli.blade_complete_multipart_package_upload([pkg], self.force)
         return self._take_signed_url(signed, "end multipart upload")
 
 class RemoteSigner(object):    
-    def __init__(self, blade_backend, force=False):
+    def __init__(self, blade_backend, force=True):
         self.cli = blade_backend
         self.force = force
+        self.scheme = "https"
+
+    def set_scheme(self, scheme):
+        self.scheme = normalize_scheme(scheme)
 
     def _take_signed_url(self, arthub_response, type_of_sign=""):
         arthub_response.raise_for_err()
         logger.debug('{0} sign-url rsp is {1}'.format(type_of_sign, arthub_response.result))
         if len(arthub_response.result) == 0:
             raise SignerError("arthub api: result is empty")
-        return "https:" + arthub_response.result[0].get('signed_url')
+        return self.scheme + ":" + arthub_response.result[0].get('signed_url')
         
     # we use bucket + key to identify a file. 
     # however bucket might be fixed for ArtHub condition, so bucket input is ignored
     def _get_download_sign(self, bucket, key, expired=1200):
         # this will return a url expires in 10 minutes
         signed = self.cli.blade_download_sign([{"cos_key": key, "expired": expired}])
         signed.raise_for_err()
         if len(signed.result) == 0:
             raise SignerError("arthub api: result is empty")
         logger.debug("download sign-url rsp is {0}".format(signed.result))
         return signed.result
     
     def get_download_url(self, bucket, key, expired=1200):
         signed = self._get_download_sign(bucket, key, expired)
-        return "https:" + signed[0].get('signed_url')
+        return self.scheme + ":" + signed[0].get('signed_url')
         
     def get_file_size(self, bucket, key):
         signed = self._get_download_sign(bucket, key)
         size = signed[0].get('size')
         if not size:
             return 0
         return size
@@ -195,30 +212,31 @@
         return self.__finished_size, self.__file_size
             
     def get_percent(self):
         return self.__finished_size / self.__file_size
 
 
 class Client(object):
-    def __init__(self, signer=None):
+    def __init__(self, signer=None, timeout=5):
         if signer is None:
             raise ReferenceError("signer is None: must provide signer arg")
         self.remote_signer = signer
+        self.timeout = timeout
         
     def download_file(self, Bucket, Key, DestFilePath, PartSize=20, MAXThread=5, EnableCRC=False, progress_callback=None):
         if EnableCRC:
             warnings.warn("EnableCRC is not supported")
         part_size = PartSize * 1024 * 1024
         file_size = self.remote_signer.get_file_size(Bucket, Key)
         if file_size is None:
             raise RetryError('failed to get file_size for {0}, file might not exist'.format(Key))
         callback = None
         if progress_callback:
             callback = ProgressCallback(file_size, progress_callback)
-        resumable_downloader = ResumableDownLoader(self.remote_signer, Bucket, Key, DestFilePath, file_size, part_size, MAXThread, callback)
+        resumable_downloader = ResumableDownLoader(self.remote_signer, Bucket, Key, DestFilePath, file_size, part_size, MAXThread, callback, self.timeout)
         if file_size < 20 * 1024 * 1024:
             resumable_downloader.simple_download()
             return
             
         resumable_downloader.download()
         
     def upload_file(self, Bucket, Key, LocalFilePath, PartSize=20, MAXThread=5, EnableCRC=False, progress_callback=None):
@@ -227,49 +245,50 @@
         if not os.path.isfile(LocalFilePath):
             raise OSError("not found file: {0}".format(LocalFilePath))
         file_size = os.path.getsize(LocalFilePath)
         part_size = PartSize * 1024 * 1024
         callback = None
         if progress_callback:
             callback = ProgressCallback(file_size, progress_callback)
-        resumableUploader = ResumableUploader(self.remote_signer, Bucket, Key, LocalFilePath, file_size, part_size, MAXThread, callback)
+        resumableUploader = ResumableUploader(self.remote_signer, Bucket, Key, LocalFilePath, file_size, part_size, MAXThread, callback, self.timeout)
         if file_size < 20 * 1024 * 1024:
             resumableUploader.simple_upload()
             return
             
         resumableUploader.upload()
 
     def get_download_url(self, Bucket, Key, Expired=1200):
         return self.remote_signer.get_download_url(Bucket, Key, Expired)
 
     # check file exists with http-get method
     def check_exists(self, bucket, key):
         headers = {'Range': 'bytes=0-0'}
         self.download_url = self.remote_signer.get_download_url(bucket, key)
-        response = requests.get(self.download_url, headers=headers)
+        response = requests.get(self.download_url, headers=headers, timeout=self.timeout)
         if response.status_code == 404:
             return False
         if response.status_code == 416:
             return True
         response.raise_for_status()
         return True
 
 
 class ResumableDownLoader(object):
-    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None):
+    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None, timeout=5):
         self.remote_signer = remote_signer
         self.bucket = bucket
         self.key = key
         self.local_path = local_path
         self.part_size = part_size
         self.thread_num = thread_num
         self.progress_callback = progress_callback
         self.file_size = file_size
         self.download_url = None
         self.expired = 600
+        self.timeout = timeout
         self.url_expire_time = None
         self.tmp_file = '{0}_ahtmp'.format(local_path)
         self.record_file = '{0}_dl_ahrecord'.format(local_path)
 
     def _refresh_download_url(self):
         current_time = time.time()
         if self.download_url is None or current_time >= self.url_expire_time:
@@ -286,26 +305,32 @@
         with threading.Lock():  
             with open(self.record_file, 'a') as f:
                 f.write('{start}-{end}-{part_size}\n'.format(start=start, end=end, part_size=self.part_size))  # Save part_size along with the progress, part_size is not current chunk_length
 
     def _download_part(self, start, end):
         self._refresh_download_url()
         headers = {'Range': 'bytes={start}-{end}'.format(start=start, end=end)}
-        response = requests.get(self.download_url, headers=headers, stream=True)
+        try:
+            response = requests.get(self.download_url, headers=headers, stream=True, timeout=self.timeout)
+        except Exception as e:
+            raise COSHttpError("error with requests {0}".format(e))
         with open(self.tmp_file, 'rb+') as f:
             f.seek(start)
             for chunk in response.iter_content(chunk_size=8192):
                 f.write(chunk)
                 if self.progress_callback:
                     self.progress_callback.report(len(chunk))
         self._save_progress(start, end)  # Save progress after part is downloaded
 
     def simple_download(self):
         self._refresh_download_url()
-        response = requests.get(self.download_url, stream=True)
+        try:
+            response = requests.get(self.download_url, stream=True, timeout=self.timeout)
+        except Exception as e:
+            raise COSHttpError("error with requests {0}".format(e))
         response.raise_for_status()
         with open(self.tmp_file, 'wb') as f:
             for chunk in response.iter_content(chunk_size=8192):
                 f.write(chunk)
                 if self.progress_callback:
                     self.progress_callback.report(len(chunk))
         try:
@@ -362,87 +387,88 @@
             end = min((i + 1) * self.part_size - 1, self.file_size - 1)
             part_ranges.append((start, end))
 
         return part_ranges
     
 
 class ResumableUploader(object):
-    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None):
+    def __init__(self, remote_signer, bucket, key, local_path, file_size, part_size=5*1024*1024, thread_num=4, progress_callback=None, timeout=5):
         self.remote_signer = remote_signer
         self.bucket = bucket
         self.key = key
         self.local_path = local_path
         self.part_size = part_size
         self.thread_num = thread_num
         self.progress_callback = progress_callback
         self.file_size = file_size
         self.upload_url = None
         self.url_expire_time = None
+        self.timeout = timeout
         self.record_file = '{0}_ul_ahrecord'.format(local_path)
         
     def _begin_multipart_upload(self, bucket, key, file_name):
         begin_url = self.remote_signer.get_begin_multipart_upload_url(bucket, key)
         # req
         try:
             res = requests.post(begin_url,
-                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)})
+                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)}, timeout=self.timeout)
         except Exception as e:
             error_message = "request S3 multipart by url %s upload id exception: %s" % (begin_url, e)
-            logging.error("[API] %s" % error_message)
-            raise
+            logger.error("[API] %s" % error_message)
+            raise COSHttpError(error_message)
         if not res or not res.ok:
             error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (begin_url, res.status_code)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             raise COSHttpError(error_message)
         # parse
         try:
             xml_tree = ElementTree.fromstring(res.content)
             upload_id = xml_tree.find("UploadId").text
-            logging.info("[API] get multipart upload id: %s" % upload_id)
+            logger.debug("[API] get multipart upload id: %s" % upload_id)
             return upload_id
         except Exception as e:
             error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             raise COSHttpError(error_message)
         
     def _upload_part(self, bucket, key, start, end, upload_id, part_number, disable_record=False):
         upload_url = self.remote_signer.get_upload_part_url(bucket, key, upload_id, part_number)
-        res = utils.upload_part_of_file(upload_url, self.local_path, start, end-start+1, self._report)
+        res = utils.upload_part_of_file(upload_url, self.local_path, start, end-start+1, self._report, self.timeout)
         if not res.is_succeeded():
             err = "upload \"{0}\"th part failed, {1}".format(part_number, res.error_message())
-            logging.error("[API] %s" % err)
+            logger.error("[API] %s" % err)
             raise COSHttpError(err)
         etag = res.data.headers.get("etag").strip('"')
         if not disable_record:
             self._save_progress(start, end, upload_id, part_number, etag)  # Save progress after part is uploaded
         return (part_number, etag)
     
     def _complete_multipart_upload(self, bucket, key, upload_id, etags):
         complete_url = self.remote_signer.get_complete_multipart_upload_url(bucket, key, upload_id)
         etag_data = self._generate_etags_xml(etags)
         # req
         try:
             res = requests.post(complete_url,
-                                headers={"content-type": "application/xml"}, data=etag_data)
+                                headers={"content-type": "application/xml"}, data=etag_data, timeout=self.timeout)
         except Exception as e:
             error_message = "request complete S3 multipart by url %s upload id exception: %s" % (complete_url, e)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             raise
         if not res or not res.ok:
             error_message = "request complete S3 multipart upload id failed, url: %s, code: %d" % (complete_url, res.status_code)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             raise COSHttpError(error_message)
         return
         
     def _upload(self, bucket, key):
         upload_url = self.remote_signer.get_upload_url(bucket, key)
-        res = utils.upload_file(upload_url, self.local_path, self._report)
+        res = utils.upload_file(upload_url, self.local_path, self._report, self.timeout)
         if not res.is_succeeded():
             err = "upload failed, {0}".format(res.error_message())
-            logging.error("[API] %s" % err)
+            logger.error("[API] %s" % err)
             raise COSHttpError(err)
         return 
         
     def _report(self, new_read_size):
         if self.progress_callback:
             self.progress_callback.report(new_read_size)
 
@@ -541,36 +567,46 @@
             part_number = ElementTree.SubElement(part, 'PartNumber')
             part_number.text = str(item[0])
         return ElementTree.tostring(root)
 
 class BladeCOSApi(object):
     """API to access THM pipeline installers on Blade storage."""
     # user input:
-    def __init__(self, api, force=False, retry=3, cli=None, signer=None):
+    def __init__(self, api, force=False, retry=3, cli=None, signer=None, scheme=None, timeout=None):
         self.force = force
         self.retry = retry
         self.signer = signer
         self.cli = cli
-        self.logger = logging.getLogger(__name__)
+        if scheme is None:
+            scheme = api.http_scheme
+        if timeout is None:
+            timeout = api.timeout
+        self.timeout = timeout
+        # signer
         if signer is None:
             signer = RemoteSignerForPackage(api, force)
+        signer.set_scheme(scheme)
         self.signer = signer
+        # cli
         if cli is None:
-            cli = Client(signer)
+            cli = Client(signer, timeout=timeout)
         self.cli = cli
 
     def check_file_exist(self, server_path):
         try:
             return self.cli.check_exists("", server_path)
         except ValueError:
             return False
 
     def get_file_object(self, server_path):
         url = self.get_download_url(server_path)
-        r = requests.get(url, stream=True)
+        try:
+            r = requests.get(url, stream=True, timeout=self.timeout)
+        except Exception as e:
+            raise COSHttpError("error requests {0}".format(e))
         if r.status_code >= 400:
             msg = r.text
             if msg == u'':
                 msg = r.headers
             raise COSHttpError("message: {0}, status code: {1}".format(msg, r.status_code))
         obj = dict(r.headers)
         obj.update({"Response": r})
@@ -580,36 +616,44 @@
         return self.cli.get_download_url(
             Bucket="",
             Key=server_path,
             Expired=expired_time,
         )
 
     @tenacity_retry(
-        stop=stop_after_attempt(5),
+        before=before_log(logger, logging.WARN),
+        stop=stop_after_attempt(3),
         wait=wait_fixed(0.5),
         retry=retry_if_exception_type(OSError)
         | retry_if_exception_type(PermissionError)
         | retry_if_exception_type(FileNotFoundError)
+        | retry_if_exception_type(APIError)
+        | retry_if_exception_type(SignerError)
+        | retry_if_exception_type(COSHttpError)
     )
     def download_file(self, server_path, local_path, progress_callback=None):
         """Download file by given server path."""
         return self.cli.download_file(
             Bucket="",
             Key=server_path,
             DestFilePath=local_path,
             MAXThread=10,
             progress_callback=progress_callback,
         )
 
     @tenacity_retry(
-        stop=stop_after_attempt(5),
+        before=before_log(logger, logging.WARN),
+        stop=stop_after_attempt(3),
         wait=wait_fixed(0.5),
         retry=retry_if_exception_type(OSError)
         | retry_if_exception_type(PermissionError)
         | retry_if_exception_type(FileNotFoundError)
+        | retry_if_exception_type(APIError)
+        | retry_if_exception_type(SignerError)
+        | retry_if_exception_type(COSHttpError)
     )
     def upload_file(self, server_path, local_path, progress_callback=None):
         """Upload file by given server path."""
         return self.cli.upload_file(
             Bucket="",
             Key=server_path,
             LocalFilePath=local_path,
```

### Comparing `arthub_api-1.6.9/arthub_api/config.py` & `arthub_api-1.7.0/arthub_api/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,32 +17,36 @@
 
 # config for access ArtHub intranet domain
 api_config_oa = {
     "http_scheme": "http:",
     "web_socket_scheme": "ws:",
     "host": _api_host_oa,
     "client_proxy_host": _client_proxy_host_oa,
+    "timeout": 5,
 }
 
 # config for access ArtHub extranet domain
 api_config_qq = {
     "http_scheme": "https:",
     "web_socket_scheme": "wss:",
     "host": _api_host_qq,
     "client_proxy_host": _client_proxy_host_qq,
+    "timeout": 10,
 }
 
 # config for internal test
 api_config_oa_test = {
     "http_scheme": "http:",
     "web_socket_scheme": "ws:",
     "host": _api_host_oa_test,
     "client_proxy_host": _client_proxy_host_oa_test,
+    "timeout": 5,
 }
 
 # config for internal test
 api_config_qq_test = {
     "http_scheme": "https:",
     "web_socket_scheme": "wss:",
     "host": _api_host_qq_test,
     "client_proxy_host": _client_proxy_host_qq_test,
+    "timeout": 10,
 }
```

### Comparing `arthub_api-1.6.9/arthub_api/exception.py` & `arthub_api-1.7.0/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/arthub_api/models.py` & `arthub_api-1.7.0/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/arthub_api/open_api.py` & `arthub_api-1.7.0/arthub_api/open_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 arthub_api.open_api
 ~~~~~~~~~~~~~~
 
 This module encapsulates the ArtHub OpenAPI.
 For detailed interface doc: "https://arthub.aa.com/user_manual/index.html"
 """
-import logging
+from contextlib import contextmanager
+import copy
 import requests
 from . import utils
 from . import models
 from . import _internal_utils
 from . import exception
 from xml.etree import ElementTree
 from . import arthub_api_config
+from .config import api_config_oa
+from .utils import get_config_by_name, logger
 
 
 def _node_query_metas(simplified_meta=True):
     metas = [
         "name",
         "file_format",
         "node_type",
@@ -69,15 +72,15 @@
 
     def _preprocess(self):
         if self._network_connection_failed:
             return
         if self._http_response is None:
             return
         if not self._http_response.ok:
-            logging.error("[API] request \"%s\" failed, code: %d" % (
+            logger.error("[API] request \"%s\" failed, code: %d" % (
                 self._http_response.url, self._http_response.status_code))
             return
         try:
             # parse api response
             _data = self._http_response.json()
             # parse result code
             self.api_result_code = _data["code"]
@@ -88,15 +91,15 @@
             # parse error message
             self._parse_error()
             if type(self.results) == dict:
                 self._direct_result = list(self.results.values())
 
         except Exception as e:
             self.exception = e
-            logging.error("[API] parsing response exception, \"%s\"" % self._http_response.text)
+            logger.error("[API] parsing response exception, \"%s\"" % self._http_response.text)
 
     def _parse_error(self):
         if not self.errors:
             return
         e = self.errors.get(next(iter(self.errors)))
         if e is None:
             return
@@ -257,34 +260,43 @@
                 raise NotLoginError("authentication failed")
             if res.is_no_permission():
                 raise NoPermissionError("no permission")
             raise APIError("err from api {0}".format(res.api_error_message))
 
 
 class OpenAPI(object):
-    def __init__(self, config, get_token_from_cache=True):
+    def __init__(self, config=api_config_oa, get_token_from_cache=True, api_config_name=None):
         r"""Used to call ArtHub openapi.
         for detailed interface doc: "https://arthub.qq.com/user_manual/index.html"
 
         :param config: from arthub_api.config.
         :param get_token_from_cache: read token from local cache.
         """
-
+        if api_config_name:
+            config = get_config_by_name(api_config_name)
         self._config = config
         self._token = ""
         self._public_token = ""
         self._cookies = None
         self._api_version_depot = "v2"
         self._api_version_gateway = "v2"
         self._api_version_account = "v3"
         self._cached_account_name = ""
         self._cached_password = ""
         self._auto_login = False
         if get_token_from_cache:
             self.get_token_from_cache()
+            
+    @contextmanager
+    def switch_config(self, api_config_name, get_token_from_cache):
+        config = get_config_by_name(api_config_name, api_config_oa)
+        old__dict = copy.copy(self.__dict__)
+        self.__dict__ = OpenAPI(config, get_token_from_cache).__dict__.copy()
+        yield
+        self.__dict__ = old__dict
 
     @property
     def config(self):
         return self._config
 
     @property
     def api_host(self):
@@ -294,14 +306,20 @@
 
     @property
     def http_scheme(self):
         if self.config:
             return self.config["http_scheme"]
         return ""
 
+    @property
+    def timeout(self):
+        if self.config:
+            return self.config["timeout"]
+        return None
+
     @staticmethod
     def get_node_permission_group(node_brief):
         p = node_brief.get("permission_mask")
         if p is None:
             raise exception.Error(value="node brief does not contain field \"permission_mask\"")
         permission_group = []
         if p & (1 << 2) > 0:
@@ -424,17 +442,17 @@
         if self._public_token:
             headers["publictoken"] = self._public_token
         headers["content-type"] = content_type
         self.add_headers(headers)
 
         # send request
         try:
-            res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies)
+            res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies, timeout=self.timeout)
         except Exception as e:
-            logging.error("[API] send request \"%s\" exception: %s" % (url, e))
+            logger.error("[API] send request \"%s\" exception: %s" % (url, e))
             response = APIResponse(None, True)
             response.exception = e
             return response
 
         response = APIResponse(res)
         if response.is_api_authentication_failed() and try_login_on_expired:
             # Try to log in again due to authentication failure
@@ -657,15 +675,15 @@
             return models.failure_result("get upload signature url of %d to create empty file failed, %s" % (
                 asset_id, api_res.error_message()))
         signed_upload_url = api_res.direct_result
         origin_url = api_res.first_result()["origin_url"]
 
         # send signature url
         try:
-            upload_res = requests.put(url=signed_upload_url, headers={"content-length": str(0)})
+            upload_res = requests.put(url=signed_upload_url, headers={"content-length": str(0)}, timeout=self.timeout)
         except Exception as e:
             return models.failure_result("request \"%s\" exception, %s" % (
                 signed_upload_url, e))
         if not upload_res.ok:
             return models.failure_result("upload to \"%s\" failed, status code: %d" % (
                 signed_upload_url, upload_res.status_code))
 
@@ -712,38 +730,38 @@
             "file_name": file_name
         }])
         if not api_res.is_succeeded():
             return models.failure_result("get create multipart upload signature url of %d failed, %s" % (
                 asset_id, api_res.error_message()))
         signed_url = api_res.direct_result
         origin_url = api_res.first_result()["origin_url"]
-        logging.info("[API] get begin multipart upload signed url: %s" % signed_url)
+        logger.info("[API] get begin multipart upload signed url: %s" % signed_url)
 
         # send signature url
         try:
             res = requests.post(signed_url,
-                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)})
+                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)}, timeout=self.timeout)
         except Exception as e:
             error_message = "request S3 multipart by url %s upload id exception: %s" % (signed_url, e)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
 
         if not res or not res.ok:
             error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (signed_url, res.status_code)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
 
         try:
             xml_tree = ElementTree.fromstring(res.content)
             upload_id = xml_tree.find("UploadId").text
 
-            logging.info("[API] get multipart upload id: %s" % upload_id)
+            logger.info("[API] get multipart upload id: %s" % upload_id)
         except Exception as e:
             error_message = "parsing S3 multipart upload id from \"%s\" exception, %s" % (res.text, e)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
         return models.success_result({
             "origin_url": origin_url,
             "upload_id": upload_id
         })
 
     def depot_get_part_upload_signature(self, asset_hub, nodes):
@@ -765,15 +783,15 @@
         url = self._depot_url(asset_hub, "upload-part-signature")
         req_payload = {
             "items": nodes
         }
         res = self._make_api_request(url, req_payload)
         signed_url = "%s%s" % (self.http_scheme, res.first_result("signed_url"))
 
-        logging.info("[API] get multipart upload signed url: %s" % signed_url)
+        logger.info("[API] get multipart upload signed url: %s" % signed_url)
 
         res.set_result(signed_url)
         return res
 
     def depot_get_complete_multipart_upload_signature(self, asset_hub, nodes):
         r"""Get the multipart upload url to visit S3 in depot.
 
@@ -822,24 +840,24 @@
             return models.failure_result("get complete multipart upload signature url of %d failed, %s" % (
                 asset_id, api_res.error_message()))
         signed_url = api_res.direct_result
 
         # send signature url
         try:
             res = requests.post(signed_url,
-                                headers={"content-type": "application/xml"}, data=etag_data)
+                                headers={"content-type": "application/xml"}, data=etag_data, timeout=self.timeout)
         except Exception as e:
             error_message = "request complete S3 multipart upload by url %s exception: %s" % (signed_url, e)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
 
         if not res or not res.ok:
             error_message = "request complete S3 multipart upload failed, url: %s, code: %d" % (
                 signed_url, res.status_code)
-            logging.error("[API] %s" % error_message)
+            logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
         return models.success_result(None)
 
     def depot_get_child_node_count(self, asset_hub, ids, query_filters=[], is_recursive=False):
         r"""Get the child node count of node in depot.
 
         :param asset_hub: str. Example: "trial".
```

### Comparing `arthub_api-1.6.9/arthub_api/storage.py` & `arthub_api-1.7.0/arthub_api/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 arthub_api.storage
 ~~~~~~~~~~~~~~
 
 This module provides the operation interface of the ArtHub asset storage module
 To visit the page of the asset storage module: "https://arthub.qq.com/trial/pan?node=304942678017"
 """
-import logging
-
 from . import utils
 from . import models
+from .utils import logger
 import os
 from xml.etree import ElementTree
 from multiprocessing.pool import ThreadPool
 import threading
 
 
 class _TransferTaskScheduler(object):
@@ -198,15 +197,15 @@
             "origin_url": self._origin_url,
             "part_number": chunk.part_num
         }])
         if not res.is_succeeded():
             return models.failure_result("get \"%d\"th part upload url failed, %s" % (
                 chunk.part_num, res.error_message()))
         upload_url = res.direct_result
-        logging.info("get multipart upload url: %s" % upload_url)
+        logger.info("get multipart upload url: %s" % upload_url)
 
         # upload
         res = utils.upload_part_of_file(upload_url, self._local_path, chunk.offset, chunk.length)
         if not res.is_succeeded():
             return models.failure_result("upload \"%d\"th part failed, %s" % (
                 chunk.part_num, res.error_message()))
```

### Comparing `arthub_api-1.6.9/arthub_api/utils.py` & `arthub_api-1.7.0/arthub_api/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 from platformdirs import user_cache_dir
 from .config import (
     api_config_oa,
     api_config_qq,
     api_config_oa_test,
     api_config_qq_test
 )
+from .__version__ import __title__
+
+
+logger = logging.getLogger(__title__)
 
 
 def _path_preprocess(path):
     path = path.strip()
     path = path.rstrip("\\/")
     return path
 
@@ -91,32 +95,32 @@
         content = self._file.read(size_to_read)
         self._completed_size += len(content)
         if self._callback:
             self._callback(len(content))
         return content
 
 
-def upload_part_of_file(url, file_path, offset, length, callback=None):
+def upload_part_of_file(url, file_path, offset, length, callback=None, timeout=5):
     try:
         if not os.path.isfile(file_path):
             return models.Result(False, error_message="file \"%s\" not exist" % file_path)
         with open(file_path, 'rb') as file_:
             res = requests.put(url, data=UploadFilePartReader(file_, offset, length, callback), headers={
                 "Accept": "application/json",
                 "Accept-Encoding": "gzip, deflate, br",
                 "Connection": "keep-alive",
                 "Content-Type": "application/octet-stream",
                 "Content-Length": str(length)
-            })
+            }, timeout=timeout)
             if not res.ok:
                 return models.Result(False, error_message="status code: %d" % res.status_code)
             return models.Result(True, data=res)
     except Exception as e:
         error_message = "send request \"%s\" exception" % url
-        logging.error("[UploadFilePart] %s" % error_message)
+        logger.error("[UploadFilePart] %s" % error_message)
         return models.Result(False, error_message=error_message)
 
 
 class UploadFileReader(object):
     def __init__(self, file_, callback):
         self._file = file_
         self._file.seek(0)
@@ -132,48 +136,48 @@
         content = self._file.read(size)
         self._completed_size += len(content)
         if self._callback:
             self._callback(len(content))
         return content
 
 
-def upload_file(url, file_path, callback=None):
+def upload_file(url, file_path, callback=None, timeout=5):
     try:
         if not os.path.isfile(file_path):
             return models.Result(False, error_message="file \"%s\" not exist" % file_path)
         with open(file_path, 'rb') as file_:
             res = requests.put(url, data=UploadFileReader(file_, callback), headers={
                 "Accept-Encoding": "gzip, deflate, br",
                 "Connection": "keep-alive",
                 "Content-Type": "application/octet-stream",
                 "Content-Length": str(os.path.getsize(file_path))
-            })
+            }, timeout=timeout)
             if not res.ok:
                 return models.Result(False, error_message="status code: %d" % res.status_code)
             return models.Result(True, data=res)
     except Exception as e:
         error_message = "send request \"%s\" exception \"%s\"" % (url, str(e))
-        logging.error("[UploadFile] %s" % error_message)
+        logger.error("[UploadFile] %s" % error_message)
         return models.Result(False, error_message=error_message)
 
 
-def download_file(url, file_path):
+def download_file(url, file_path, timeout=5):
     try:
         if os.path.exists(file_path):
             remove(file_path)
 
         if not create_empty_file(file_path):
             return models.Result(False, error_message="create \"%s\" failed" % file_path)
 
         # download file
         download_dir_path = os.path.dirname(file_path)
         if not mkdir(download_dir_path):
             return models.Result(False, error_message="create directory \"%s\" failed" % download_dir_path)
 
-        res_download = requests.get(url, stream=True)
+        res_download = requests.get(url, stream=True, timeout=timeout)
 
         if not res_download:
             return models.Result(False, error_message="request \"%s\" failed" % url)
         with open(file_path, "ab") as f:
             for chunk in res_download.iter_content(chunk_size=1024):
                 f.write(chunk)
                 f.flush()
@@ -270,25 +274,25 @@
 
 def get_token_from_cache(api_host):
     token_file = get_token_cache_file(api_host)
     try:
         if os.path.exists(token_file):
             return read_file(token_file)
     except Exception:
-        logging.warning("[TokenCache] get token from file \"%s\" error: %s",
+        logger.warning("[TokenCache] get token from file \"%s\" error: %s",
                         token_file, str(e))
     return ""
 
 
 def save_token_to_cache(token, api_host):
     token_file = get_token_cache_file(api_host)
     try:
         write_file(token_file, token)
     except Exception:
-        logging.warning("[TokenCache] save token to file \"%s\" error: %s",
+        logger.warning("[TokenCache] save token to file \"%s\" error: %s",
                         token_file, str(e))
 
 
 def remove_token_cache_file(api_host):
     remove(get_token_cache_file(api_host))
```

### Comparing `arthub_api-1.6.9/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.7.0/arthub_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.9
+Version: 1.7.0
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.9/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.7.0/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/setup.py` & `arthub_api-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/tests/test_open_api.py` & `arthub_api-1.7.0/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/tests/test_open_api_blade.py` & `arthub_api-1.7.0/tests/test_open_api_blade.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from arthub_api.open_api import NotLoginError
 from . import _utils
 from arthub_api import (
     arthub_api_config,
     BladeAPI, init_config,
 )
 from arthub_api.blade_api_instance import BladeInstance
+from arthub_api.utils import get_config_by_name
 
 
 @contextmanager
 def set_env_var(name, value):
     original_value = os.environ.get(name)
     os.environ[name] = value
     try:
@@ -581,8 +582,30 @@
         init_config()
         assert arthub_api_config.blade_public_token == "test_input2"
     with set_env_var("AH_BLADE_ACCOUNT_EMAIL", "email1"):
         init_config()
         assert arthub_api_config.account_email == "email1"
     with set_env_var("AH_BLADE_PASSWORD", "password1"):
         init_config()
-        assert arthub_api_config.password == "password1"
+        assert arthub_api_config.password == "password1"
+        
+        
+def test_switch_between_configs(env):
+    o1 = BladeAPI(get_config_by_name("oa"), False, "1234")
+    assert o1.config.get("host") == "service.arthub.woa.com"
+    assert o1.blade_public_token == "1234"
+    with o1.switch_config("qq", False, "456"):
+        assert o1.config.get("host") == "service.arthub.qq.com"
+        assert o1.blade_public_token == "456"
+    assert o1.config.get("host") == "service.arthub.woa.com"
+    assert o1.blade_public_token == "1234"
+    
+    cfg = {
+        "api_config_name": "oa_test",
+        "blade_public_token": "789",
+    }
+    with o1.switch_config(**cfg):
+        assert o1.config.get("host") == "arthub-service-test.woa.com"
+        assert o1.blade_public_token == "789"
+    assert o1.config.get("host") == "service.arthub.woa.com"
+    assert o1.blade_public_token == "1234"
+
```

### Comparing `arthub_api-1.6.9/tests/test_storage.py` & `arthub_api-1.7.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.9/tests/test_storage_blade.py` & `arthub_api-1.7.0/tests/test_storage_blade.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding:utf-8 -*-
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
+from tenacity import RetryError
+
 import arthub_api
 import pytest
 import sys
 import logging
 from arthub_api import arthub_api_config
 from arthub_api.blade_storage import RemoteSigner
 from arthub_api.open_api import APIError
@@ -78,15 +80,15 @@
     target = "pkg_distribution/7z/arthub_test_pkg/0.0.1/arthub_test_pkg.7z"
     source = os.path.join(str(tmp_path), "tmp.7z")
         
     cli = BladeCOSApi(api=blade_api)
     cli.download_file(target,source)
     try:
         cli.upload_file(target, source)
-    except APIError:
+    except RetryError:
         # expected condition:
         return
     # package should already uploaded, an error should be raised
     assert False 
 
 def test_blade_check_exists(env, tmp_path):
     blade_api = init_api(env)
@@ -145,20 +147,20 @@
     cli.download_file(target, local)
     
 def test_blade_uploader_fail_general_signer(env, tmp_path):
     blade_api = init_api(env)
     target = "pkg_distribution/7z/arthub_test_pkg/0.0.1/arthub_test_pkg.7z"
     source = os.path.join(str(tmp_path), "tmp.7z")
         
-    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api))
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=False))
     cli.download_file(target,source)
     try:
         target = "test_space/7z/arthub_test_pkg-0.0.1.7z"
         cli.upload_file(target, source)
-    except APIError:
+    except RetryError:
         # expected condition:
         return
     # package should already uploaded, an error should be raised
     assert False 
 
 def test_blade_check_exists_general_signer(env, tmp_path):
     blade_api = init_api(env)
@@ -191,8 +193,33 @@
     
     target = "test_space/7z/arthub_test_pkg-0.0.2.7z"
     def print_percent1(a, b):
         print_percent(a, b)
         if a > b/2:
             import os
             os.exit(1)
+    cli.upload_file(target, source, print_percent)
+        
+def test_blade_sign_scheme(env):
+    blade_api = init_api(env)
+    
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=True), scheme="http")
+    assert cli.signer.get_download_url('', 'any-key').startswith("http://")
+    
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=True), scheme="https")
+    assert cli.signer.get_download_url('', 'any-key').startswith("https://")
+    
+    target = "pkg_distribution/7z/pyqt/5.15.2-ng.1/pyqt.7z"
+    cli = BladeCOSApi(api=blade_api, scheme="http")
+    assert cli.signer.get_download_url('', target).startswith("http://")
+    
+    cli = BladeCOSApi(api=blade_api, scheme="https")
+    assert cli.signer.get_download_url('', target).startswith("https://")
+    
+def test_blade_uploader_http(env, tmp_path):
+    blade_api = init_api(env)
+    target = "pkg_distribution/7z/arthub_test_pkg/0.0.2/arthub_test_pkg.7z"
+    source = os.path.join(str(tmp_path), "tmp.7z")
+        
+    cli = BladeCOSApi(api=blade_api, force=True, scheme="http")
+    cli.download_file(target,source)
     cli.upload_file(target, source, print_percent)
```

