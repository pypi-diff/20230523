# Comparing `tmp/pysmsboxnet-2023.2.1.tar.gz` & `tmp/pysmsboxnet-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmsboxnet-2023.2.1.tar", last modified: Fri Feb 10 12:58:35 2023, max compression
+gzip compressed data, was "pysmsboxnet-2023.5.0.tar", last modified: Tue May 23 12:24:47 2023, max compression
```

## Comparing `pysmsboxnet-2023.2.1.tar` & `pysmsboxnet-2023.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 12:58:35.225142 pysmsboxnet-2023.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-02-10 12:58:35.225142 pysmsboxnet-2023.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 12:58:35.225142 pysmsboxnet-2023.2.1/pysmsboxnet/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/pysmsboxnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/pysmsboxnet/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/pysmsboxnet/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 12:58:35.225142 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-02-10 12:58:35.000000 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-10 12:58:35.000000 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 12:58:35.000000 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 12:58:34.000000 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-10 12:58:35.000000 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-10 12:58:35.000000 pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-10 12:58:35.229142 pysmsboxnet-2023.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 12:58:35.225142 pysmsboxnet-2023.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-02-10 12:58:04.000000 pysmsboxnet-2023.2.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:24:47.514714 pysmsboxnet-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-23 12:24:47.514714 pysmsboxnet-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:24:47.514714 pysmsboxnet-2023.5.0/pysmsboxnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/pysmsboxnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/pysmsboxnet/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/pysmsboxnet/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:24:47.514714 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-23 12:24:47.000000 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 12:24:47.000000 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:24:47.000000 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:24:47.000000 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 12:24:47.000000 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 12:24:47.000000 pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 12:24:47.514714 pysmsboxnet-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:24:47.514714 pysmsboxnet-2023.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-23 12:24:30.000000 pysmsboxnet-2023.5.0/tests/test_api.py
```

### Comparing `pysmsboxnet-2023.2.1/LICENSE` & `pysmsboxnet-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmsboxnet-2023.2.1/PKG-INFO` & `pysmsboxnet-2023.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmsboxnet
-Version: 2023.2.1
+Version: 2023.5.0
 Summary: Client to send SMS using www.smsbox.net API
 Author-email: Patrick ZAJDA <patrick@zajda.fr>
 License: MIT license
 Project-URL: Source code, https://github.com/Nardol/pysmsboxnet
 Project-URL: Bug tracker, https://github.com/Nardol/pysmsboxnet/issues
 Project-URL: Documentation, https://nardol.github.io/pysmsboxnet/stable
 Project-URL: SMSBox API 1.1 doc, https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.html
@@ -33,15 +33,15 @@
 
 # pysmsboxnet
 
 Asynchronous Python library for [smsbox.net](https://www.smsbox.net) API.
 Currently it allows to send a SMS, using the [v1.1 API](https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.html).
 You can also [download the documentation](https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.pdf).
 Future version might allow to use other [account features](https://en.smsbox.net/docs/doc-APIFunctions-SMSBOX-FR.html), this doc is in French.
-The exception is the credits async property which allows getting remaining credits.
+The exception is `get_credits()` which allows getting remaining credits.
 
 ## Installing
 
 You can install using pip.
 
 ## How to use
```

### Comparing `pysmsboxnet-2023.2.1/README.md` & `pysmsboxnet-2023.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pysmsboxnet
 
 Asynchronous Python library for [smsbox.net](https://www.smsbox.net) API.
 Currently it allows to send a SMS, using the [v1.1 API](https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.html).
 You can also [download the documentation](https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.pdf).
 Future version might allow to use other [account features](https://en.smsbox.net/docs/doc-APIFunctions-SMSBOX-FR.html), this doc is in French.
-The exception is the credits async property which allows getting remaining credits.
+The exception is `get_credits()` which allows getting remaining credits.
 
 ## Installing
 
 You can install using pip.
 
 ## How to use
```

### Comparing `pysmsboxnet-2023.2.1/pyproject.toml` & `pysmsboxnet-2023.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = [ "setuptools>=41", "wheel", "setuptools-git-versioning<2", ]
+requires = [ "setuptools==67.2.0", "wheel==0.38.4", "setuptools-git-versioning==1.13.1", ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysmsboxnet"
 dynamic=["version"]
 authors = [
     {name = "Patrick ZAJDA", email = "patrick@zajda.fr"}
@@ -29,15 +29,14 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Communications",
     "Topic :: Communications :: Telephony",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "aiohttp>=3.8.0,<4.0",
-    "async-property==0.2.1",
 ]
 
 [project.urls]
 "Source code" = "https://github.com/Nardol/pysmsboxnet"
 "Bug tracker" = "https://github.com/Nardol/pysmsboxnet/issues"
 "Documentation" = "https://nardol.github.io/pysmsboxnet/stable"
 "SMSBox API 1.1 doc" = "https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.html"
```

### Comparing `pysmsboxnet-2023.2.1/pysmsboxnet/api.py` & `pysmsboxnet-2023.5.0/pysmsboxnet/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """smsbox.net api client module."""
-
 from __future__ import annotations
 
+import logging
+
 from aiohttp import ClientSession
-from async_property import async_property
 
 from . import exceptions
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class Client:
     """API client class.
 
     :param aiohttp.ClientSession session: the aiohttp session to use
     :param str host: the API endpoint host, for example api.smsbox.pro (https is forced)
     :param str cleApi: the SMSBox API key, name is in French to reflect the documentation
@@ -18,15 +20,15 @@
 
     def __init__(self, session: ClientSession, host: str, cleApi: str):
         """Initialize the SMS."""
         self.host = host
         self.cleApi = cleApi
         self.session = session
 
-    async def __smsbox_request(self, uri: str, parameters: dict) -> str:
+    async def __smsbox_request(self, uri: str, parameters: dict[str, str]) -> str:
         """Private method to send a request to the API.
 
         :param str uri: the host API endpoint, for example api.php or 1.1/api.php
         :param dict parameters: parameters to pass to the API
 
         :returns: SMSBox API response
         :rtype: str
@@ -39,22 +41,30 @@
         :raises pysmsboxnet.exceptions.WrongRecipientException: recipient format is wrong
         :raises pysmsboxnet.exceptions.InternalErrorException: SMSBox API internal error
         """
         headers = {
             "authorization": f"App {self.cleApi}",
         }
 
+        _LOGGER.debug(
+            "Sending request to SMSBox API using host %s with URI %s and parameters %s",
+            self.host,
+            uri,
+            parameters,
+        )
         async with self.session.post(
             url=f"https://{self.host}/{uri}",
             headers=headers,
             data=parameters,
         ) as resp:
+            _LOGGER.debug("HTTP response: %s", resp.status)
             if resp.status != 200:
                 raise exceptions.HTTPException(resp.status)
             respText = await resp.text()
+            _LOGGER.debug("API response: %s", respText)
             if respText == "ERROR":
                 raise exceptions.SMSBoxException
             elif respText == "ERROR 01":
                 raise exceptions.ParameterErrorException
             elif respText == "ERROR 02":
                 raise exceptions.AuthException
             elif respText == "ERROR 03":
@@ -62,15 +72,17 @@
             elif respText == "ERROR 04":
                 raise exceptions.WrongRecipientException
             elif respText == "ERROR 05":
                 raise exceptions.InternalErrorException
             else:
                 return respText
 
-    async def send(self, dest: str, msg: str, mode: str, parameters: dict = []) -> int:
+    async def send(
+        self, dest: str, msg: str, mode: str, parameters: dict[str, str] | None = None
+    ) -> int:
         """Send a SMS.
 
         :param str dest: SMS recipient(s), see API documentation about how to format
         :param str msg: the SMS message
         :param str mode: send mode,  mode API parameter
         :param dict parameters: other API parameter as strategy or if other charset than UTF8 is needed
 
@@ -79,26 +91,25 @@
         """
         postData = {
             "dest": dest,
             "msg": msg,
             "mode": mode,
             "charset": "utf-8",
         }
-        postData.update(parameters)
+        if parameters:
+            postData.update(parameters)
 
         respText = await self.__smsbox_request("1.1/api.php", postData)
 
-        if respText.startswith("OK"):
-            respOK = respText.split(" ")
-            if len(respOK) == 1:
-                return 0
-            return int(respOK[1])
+        respOK = respText.split(" ")
+        if len(respOK) == 1:
+            return 0
+        return int(respOK[1])
 
-    @async_property
-    async def credits(self) -> float:
+    async def get_credits(self) -> float:
         """Return float number of credits.
 
         :raises pysmsboxnet.exceptions.SMSBoxException: result is not OK
         """
         postData = {
             "action": "credit",
         }
```

### Comparing `pysmsboxnet-2023.2.1/pysmsboxnet/exceptions.py` & `pysmsboxnet-2023.5.0/pysmsboxnet/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,50 +11,50 @@
         """
         super().__init__(message)
 
 
 class ParameterErrorException(SMSBoxException):
     """Exception when API returns ERROR 01."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize for bad parameters exception."""
         super().__init__("Some parameters are invalid or missing")
 
 
 class AuthException(SMSBoxException):
     """Exception when API returns ERROR 02."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize authorization error, no message to specify."""
         super().__init__(
             "Unable to authenticate,"
             " check if your API key is valid or not suspended."
         )
 
 
 class BillingException(SMSBoxException):
     """Exception when API returns ERROR 03."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize when no enough SMS credits, no message to specify."""
         super().__init__("No enough credits, please buy some")
 
 
 class WrongRecipientException(SMSBoxException):
     """Exception when API returns ERROR 04."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize when recipient is bad, no message to specify."""
         super().__init__("Wrong recipient(s), not valid or missformated")
 
 
 class InternalErrorException(SMSBoxException):
     """Exception when API returns ERROR 05."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize internal error."""
         super().__init__("SMSBox.net internal error, try again later")
 
 
 class HTTPException(SMSBoxException):
     """Exception when API returns ERROR 03."""
```

### Comparing `pysmsboxnet-2023.2.1/pysmsboxnet.egg-info/PKG-INFO` & `pysmsboxnet-2023.5.0/pysmsboxnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmsboxnet
-Version: 2023.2.1
+Version: 2023.5.0
 Summary: Client to send SMS using www.smsbox.net API
 Author-email: Patrick ZAJDA <patrick@zajda.fr>
 License: MIT license
 Project-URL: Source code, https://github.com/Nardol/pysmsboxnet
 Project-URL: Bug tracker, https://github.com/Nardol/pysmsboxnet/issues
 Project-URL: Documentation, https://nardol.github.io/pysmsboxnet/stable
 Project-URL: SMSBox API 1.1 doc, https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.html
@@ -33,15 +33,15 @@
 
 # pysmsboxnet
 
 Asynchronous Python library for [smsbox.net](https://www.smsbox.net) API.
 Currently it allows to send a SMS, using the [v1.1 API](https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.html).
 You can also [download the documentation](https://en.smsbox.net/docs/doc-API-SMSBOX-1.1-EN.pdf).
 Future version might allow to use other [account features](https://en.smsbox.net/docs/doc-APIFunctions-SMSBOX-FR.html), this doc is in French.
-The exception is the credits async property which allows getting remaining credits.
+The exception is `get_credits()` which allows getting remaining credits.
 
 ## Installing
 
 You can install using pip.
 
 ## How to use
```

### Comparing `pysmsboxnet-2023.2.1/tests/test_api.py` & `pysmsboxnet-2023.5.0/tests/test_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for pysmsboxnet."""
 
 from __future__ import annotations
 
 import random
+from typing import Any
 
 import aiohttp
 import pytest
 
 from pysmsboxnet import exceptions
 from pysmsboxnet.api import Client
 
@@ -16,15 +17,15 @@
 SMS_RECIPIENT = "9999001"
 SMS_MSG = "Test d'un message ! En plus il va être envoyé."
 SEND_MODE = "expert"
 SMSBOX_STRATEGY = "2"
 
 
 @pytest.mark.asyncio
-async def test_parameters_error(aresponses):
+async def test_parameters_error(aresponses: Any) -> None:
     """Test if exception is raised if web server returns ERROR 01."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="ERROR 01",
@@ -40,15 +41,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_bad_auth(aresponses):
+async def test_bad_auth(aresponses: Any) -> None:
     """Test if exception is raised in case of wrong authentication ERROR 02."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="ERROR 02",
@@ -68,15 +69,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_billing(aresponses):
+async def test_billing(aresponses: Any) -> None:
     """Test if BillingException is raised in case of ERROR 03."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="ERROR 03",
@@ -96,15 +97,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_bad_dest(aresponses):
+async def test_bad_dest(aresponses: Any) -> None:
     """Test if WrongRecipientException is raised on ERROR 04."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="ERROR 04",
@@ -124,15 +125,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_internal_error(aresponses):
+async def test_internal_error(aresponses: Any) -> None:
     """Test if right exception is raised on ERROR 05."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="ERROR 05",
@@ -152,15 +153,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_other_error(aresponses):
+async def test_other_error(aresponses: Any) -> None:
     """Test unknown error."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="ERROR",
@@ -180,15 +181,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_http_error(aresponses):
+async def test_http_error(aresponses: Any) -> None:
     """Test if HTTP status is not 200."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="",
@@ -208,15 +209,15 @@
                 SEND_MODE,
                 {"strategy": SMSBOX_STRATEGY},
             )
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_ok(aresponses):
+async def test_ok(aresponses: Any) -> None:
     """Test result OK without ID."""
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
         aresponses.Response(
             text="OK",
@@ -236,15 +237,15 @@
             {"strategy": SMSBOX_STRATEGY},
         )
         assert 0 == result
         await session.close()
 
 
 @pytest.mark.asyncio
-async def test_ok_with_id(aresponses):
+async def test_ok_with_id(aresponses: Any) -> None:
     """Test result OK with a random ID."""
     # Get a random integer which will serv as the message ID
     MSG_ID = random.randint(100000000000, 999999999999)
     aresponses.add(
         "api.smsbox.pro",
         "/1.1/api.php",
         "post",
@@ -266,15 +267,15 @@
             {"strategy": SMSBOX_STRATEGY, "id": "1"},
         )
         assert MSG_ID == result
         await session.close()
 
 
 @pytest.mark.asyncio
-async def test_credits(aresponses):
+async def test_credits(aresponses: Any) -> None:
     """Test credits async property returning a random number."""
     # Get a random float which will serv as the number of credits
     CREDITS = round(random.uniform(0, 9999), 1)
     aresponses.add(
         "api.smsbox.pro",
         "/api.php",
         "post",
@@ -285,21 +286,21 @@
     )
     async with aiohttp.ClientSession() as session:
         sms = Client(
             session,
             SMSBOX_HOST,
             SMSBOX_API_KEY,
         )
-        result = await sms.credits
+        result = await sms.get_credits()
         assert CREDITS == result
         await session.close()
 
 
 @pytest.mark.asyncio
-async def test_exception_credits(aresponses):
+async def test_exception_credits(aresponses: Any) -> None:
     """Test get credits async property raising exception."""
     aresponses.add(
         "api.smsbox.pro",
         "/api.php",
         "post",
         aresponses.Response(
             text="ERROR 02",
@@ -309,20 +310,20 @@
     async with aiohttp.ClientSession() as session:
         sms = Client(
             session,
             SMSBOX_HOST,
             SMSBOX_API_KEY,
         )
         with pytest.raises(exceptions.SMSBoxException):
-            await sms.credits
+            await sms.get_credits()
             await session.close()
 
 
 @pytest.mark.asyncio
-async def test_error_credits(aresponses):
+async def test_error_credits(aresponses: Any) -> None:
     """Test get credits async property returning strange string."""
     aresponses.add(
         "api.smsbox.pro",
         "/api.php",
         "post",
         aresponses.Response(
             text="FFF",
@@ -332,9 +333,9 @@
     async with aiohttp.ClientSession() as session:
         sms = Client(
             session,
             SMSBOX_HOST,
             SMSBOX_API_KEY,
         )
         with pytest.raises(exceptions.SMSBoxException):
-            await sms.credits
+            await sms.get_credits()
             await session.close()
```

