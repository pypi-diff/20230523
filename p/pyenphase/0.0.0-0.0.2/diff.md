# Comparing `tmp/pyenphase-0.0.0.tar.gz` & `tmp/pyenphase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.0.0.tar", max compression
+gzip compressed data, was "pyenphase-0.0.2.tar", max compression
```

## Comparing `pyenphase-0.0.0.tar` & `pyenphase-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-05-23 14:45:58.481011 pyenphase-0.0.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-05-23 14:45:58.475854 pyenphase-0.0.0/README.md
--rw-r--r--   0        0        0     2225 2023-05-23 14:47:44.974919 pyenphase-0.0.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-23 14:46:16.272879 pyenphase-0.0.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     2847 2023-05-23 14:48:16.553003 pyenphase-0.0.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0     1271 2023-05-23 14:48:16.553625 pyenphase-0.0.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0      415 2023-05-23 14:46:16.273712 pyenphase-0.0.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1130 2023-05-23 14:48:16.554311 pyenphase-0.0.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-05-23 14:45:58.501807 pyenphase-0.0.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-05-23 14:45:58.501248 pyenphase-0.0.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 pyenphase-0.0.0/setup.py
--rw-r--r--   0        0        0     4757 1970-01-01 00:00:00.000000 pyenphase-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 14:45:58.481011 pyenphase-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3476 2023-05-23 14:45:58.475854 pyenphase-0.0.2/README.md
+-rw-r--r--   0        0        0     2226 2023-05-23 15:13:56.980875 pyenphase-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-23 14:46:16.272879 pyenphase-0.0.2/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-23 14:59:20.964327 pyenphase-0.0.2/src/pyenphase/auth.py
+-rw-r--r--   0        0        0     2404 2023-05-23 15:04:01.936595 pyenphase-0.0.2/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0      446 2023-05-23 14:53:58.015119 pyenphase-0.0.2/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1321 2023-05-23 15:05:28.214252 pyenphase-0.0.2/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-05-23 14:45:58.501807 pyenphase-0.0.2/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:45:58.501248 pyenphase-0.0.2/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-05-23 15:05:18.328813 pyenphase-0.0.2/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 pyenphase-0.0.2/setup.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 pyenphase-0.0.2/PKG-INFO
```

### Comparing `pyenphase-0.0.0/LICENSE` & `pyenphase-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.0/README.md` & `pyenphase-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.0.0/pyproject.toml` & `pyenphase-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.0.0"
+version = "0.0.2"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pyenphase/pyenphase/issues"
 "Changelog" = "https://github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10"
 httpx = ">=0.24.0"
 lxml = ">=4.9.2"
 pyjwt = ">=2.7.0"
 awesomeversion = ">=22.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
```

### Comparing `pyenphase-0.0.0/src/pyenphase/auth.py` & `pyenphase-0.0.2/src/pyenphase/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,92 @@
-import asyncio
+"""Envoy authentication methods."""
+
 import json
 
 import httpx
 
 from .exceptions import EnvoyAuthenticationError
-from .firmware import EnvoyFirmware
-
-"""Envoy authentication methods."""
 
 
 class EnvoyTokenAuth:
     def __init__(
         self,
-        client,
-        cloud_username=None,
-        cloud_password=None,
-        envoy_serial=None,
-        token=None,
-    ):
+        client: httpx.AsyncClient | None = None,
+        cloud_username: str | None = None,
+        cloud_password: str | None = None,
+        envoy_serial: str | None = None,
+        token: str | None = None,
+    ) -> None:
         self.cloud_client = client or httpx.AsyncClient()
         self.cloud_username = cloud_username
         self.cloud_password = cloud_password
         self.envoy_serial = envoy_serial
         self._token = token
 
-        async def fetch_token(self):
-            # Login to Enlighten to obtain a session ID
-            data = {"user[email]": cloud_username, "user[password]": cloud_password}
-            req = await self.cloud_client.post(
-                "https://enlighten.enphaseenergy.com/login.json?", data=data
-            )
-            response = json.loads(req.text)
-
-            # Obtain the token
-            data = {
-                "session_id": response["session_id"],
-                "serial_num": envoy_serial,
-                "username": cloud_username,
-            }
-            req = await self.cloud_client.post(
-                "https://entrez.enphaseenrgy.com/tokens", json=data
-            )
-            self._token = req.text
+    async def setup(self) -> None:
+        """Obtain the token for Envoy authentication."""
+        # Login to Enlighten to obtain a session ID
+        data = {
+            "user[email]": self.cloud_username,
+            "user[password]": self.cloud_password,
+        }
+        req = await self.cloud_client.post(
+            "https://enlighten.enphaseenergy.com/login.json?", data=data
+        )
+        response = json.loads(req.text)
+
+        # Obtain the token
+        data = {
+            "session_id": response["session_id"],
+            "serial_num": self.envoy_serial,
+            "username": self.cloud_username,
+        }
+        req = await self.cloud_client.post(
+            "https://entrez.enphaseenrgy.com/tokens", json=data
+        )
+        self._token = req.text
 
         # If a token wasn't provided, fetch it from the cloud API
         if not self._token:
             # Raise if we don't have cloud credentials
             if not self.cloud_username or not self.cloud_password:
                 raise EnvoyAuthenticationError(
                     "Your firmware requires token authentication, but no cloud credentials were provided to obtain the token."
                 )
             # Raise if we are missing the envoy serial number
             if not self.envoy_serial:
                 raise EnvoyAuthenticationError(
                     "Your firmware requires token authentication, but no envoy serial number was provided to obtain the token."
                 )
 
-            asyncio.run(fetch_token(self))
-
         # Verify we have adequate credentials
         if not self.token:
             raise EnvoyAuthenticationError(
                 "Unable to obtain token for Envoy authentication."
             )
 
     @property
     def token(self) -> str:
+        assert self._token is not None  # nosec
         return self._token
 
     @property
-    def token_header(self) -> str:
+    def token_header(self) -> str | None:
         if not self._token:
             return None
         return f"Bearer {self._token}"
 
 
 class EnvoyLegacyAuth:
-    def __init__(self, host, username, password):
+    """Class for legacy Envoy authentication."""
+
+    def __init__(self, host: str, username: str, password: str) -> None:
         self.host = host
-        self.username = username
-        self.password = password
+        self.local_username = username
+        self.local_password = password
 
     @property
     def local_auth(self) -> httpx.DigestAuth:
+        """Digest authentication for local Envoy."""
         if not self.local_username or not self.local_password:
             return None
         return httpx.DigestAuth(self.local_username, self.local_password)
```

### Comparing `pyenphase-0.0.0/src/pyenphase/firmware.py` & `pyenphase-0.0.2/src/pyenphase/firmware.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import httpx
 from awesomeversion import AwesomeVersion
-from lxml import etree
+from lxml import etree  # nosec
 
 from .exceptions import EnvoyFirmwareCheckError
+from .ssl import NO_VERIFY_SSL_CONTEXT
 
 
 class EnvoyFirmware:
     """Class for querying and determining the Envoy firmware version."""
 
-    async def __init__(self, host) -> str:
-        self._client = httpx.AsyncClient(verify=False)
+    def __init__(self, host: str) -> None:
+        self._client = httpx.AsyncClient(verify=NO_VERIFY_SSL_CONTEXT)  # nosec
         self._host = host
 
+    async def setup(self) -> None:
+        """Obtain the firmware version for Envoy authentication."""
         # <envoy>/info will return XML with the firmware version
         try:
-            result = await self._client.get(f"{self.host}/info")
+            result = await self._client.get(f"{self._host}/info")
         except httpx.HTTPError:
-            raise EnvoyFirmwareCheckError("Unable to query firmware version")
+            raise EnvoyFirmwareCheckError(500, "Unable to query firmware version")
 
         if result.status_code == 200:
-            xml = etree.fromstring(result.content)
+            xml = etree.fromstring(result.content)  # nosec
             self.firmware_version = xml.findtext("package[@nameW='app']/version")
 
         # If we get a different status code, raise an exception
         raise EnvoyFirmwareCheckError(result.status_code, result.text)
 
     @property
     def requires_token_auth(self) -> bool:
```

### Comparing `pyenphase-0.0.0/setup.py` & `pyenphase-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {'': ['*']}
 
 install_requires = \
 ['awesomeversion>=22.9.0', 'httpx>=0.24.0', 'lxml>=4.9.2', 'pyjwt>=2.7.0']
 
 setup_kwargs = {
     'name': 'pyenphase',
-    'version': '0.0.0',
+    'version': '0.0.2',
     'description': 'Library to control enphase envoy',
     'long_description': '# pyenphase\n\n<p align="center">\n  <a href="https://github.com/pyenphase/pyenphase/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/pyenphase/pyenphase/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://pyenphase.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/pyenphase.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/pyenphase/pyenphase">\n    <img src="https://img.shields.io/codecov/c/github/pyenphase/pyenphase.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/pyenphase/">\n    <img src="https://img.shields.io/pypi/v/pyenphase.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/pyenphase.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/pyenphase.svg?style=flat-square" alt="License">\n</p>\n\nLibrary to control enphase envoy\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install pyenphase`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'pyenphase',
     'author_email': 'cgarwood@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pyenphase/pyenphase',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['pyenphase'] package_data = \ {'': ['*']} install_requires
 = \ ['awesomeversion>=22.9.0', 'httpx>=0.24.0', 'lxml>=4.9.2', 'pyjwt>=2.7.0']
-setup_kwargs = { 'name': 'pyenphase', 'version': '0.0.0', 'description':
+setup_kwargs = { 'name': 'pyenphase', 'version': '0.0.2', 'description':
 'Library to control enphase envoy', 'long_description': '# pyenphase\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
@@ -17,8 +17,8 @@
 specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package
 was created with\n[Copier](https://copier.readthedocs.io/) and the\n
 [browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
 template)\nproject template.\n', 'author': 'pyenphase', 'author_email':
 'cgarwood@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
 'https://github.com/pyenphase/pyenphase', 'package_dir': package_dir,
 'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+install_requires, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `pyenphase-0.0.0/PKG-INFO` & `pyenphase-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.0.0
+Version: 0.0.2
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: awesomeversion (>=22.9.0)
 Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: lxml (>=4.9.2)
 Requires-Dist: pyjwt (>=2.7.0)
```

#### html2text {}

```diff
@@ -1,16 +1,14 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 0.0.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.0.2 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
-Python: >=3.7,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
 Dist: awesomeversion (>=22.9.0) Requires-Dist: httpx (>=0.24.0) Requires-Dist:
 lxml (>=4.9.2) Requires-Dist: pyjwt (>=2.7.0) Project-URL: Bug Tracker, https:/
 /github.com/pyenphase/pyenphase/issues Project-URL: Changelog, https://
 github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://pyenphase.readthedocs.io Project-URL: Repository, https:
```

