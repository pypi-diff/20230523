# Comparing `tmp/os2mo-fastapi-utils-1.3.0.tar.gz` & `tmp/os2mo_fastapi_utils-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/rammearkitektur/os2mo-fastapi-utils/dist/.tmp-z79elq4h/os2mo-fastapi-utils-1.3.0.tar", last modified: Wed Jan 18 12:18:58 2023, max compression
+gzip compressed data, was "os2mo_fastapi_utils-1.3.3.tar", max compression
```

## Comparing `os2mo-fastapi-utils-1.3.0.tar` & `os2mo_fastapi_utils-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    16725 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2021 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/oidc.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/test_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/pydantic_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4613 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/tracing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2021 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      366 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-01-18 12:16:55.000000 os2mo-fastapi-utils-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 12:18:58.000000 os2mo-fastapi-utils-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-01-18 12:06:31.000000 os2mo-fastapi-utils-1.3.0/setup.py
+drwxr-xr-x   0        0        0        0 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/LICENSES/
+-rw-r--r--   0        0        0    16725 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     1426 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/README.md
+-rw-r--r--   0        0        0       75 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:28:30.139873 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-23 15:28:30.077868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/exceptions.py
+-rw-r--r--   0        0        0      537 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/models.py
+-rw-r--r--   0        0        0     4937 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/oidc.py
+-rw-r--r--   0        0        0     2203 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/test_helper.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:28:30.141873 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/py.typed
+-rw-r--r--   0        0        0     2396 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/pydantic_types.py
+-rw-r--r--   0        0        0     4678 2023-05-23 15:28:30.078868 os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/tracing.py
+-rw-r--r--   0        0        0     1332 2023-05-23 15:28:30.809929 os2mo_fastapi_utils-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 os2mo_fastapi_utils-1.3.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `os2mo-fastapi-utils-1.3.0/LICENSE` & `os2mo_fastapi_utils-1.3.3/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `os2mo-fastapi-utils-1.3.0/PKG-INFO` & `os2mo_fastapi_utils-1.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: os2mo-fastapi-utils
-Version: 1.3.0
-Summary: Utility library with various reusable FastAPI components
-Home-page: https://git.magenta.dk/rammearkitektur/os2mo-data-import-and-export
-Author: Magenta ApS
+Version: 1.3.3
+Summary: FastAPI utils for os2mo
+Home-page: https://magenta.dk/
+License: MPL-2.0
+Keywords: os2mo-fastapi-utils,os2mo,fastapi,utils
+Author: Magenta
 Author-email: info@magenta.dk
-License: MPL 2.0
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: opentelemetry-api (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-jaeger (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation-aiohttp-client (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-instrumentation-httpx (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-instrumentation-requests (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-sdk (>=1.18.0,<2.0.0)
+Requires-Dist: pydantic[email] (>=1.10.7,<2.0.0)
+Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Project-URL: Repository, https://git.magenta.dk/rammearkitektur/os2mo-fastapi-utils
 Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: test
-Provides-Extra: dist
-License-File: LICENSE
 
 <!--
 SPDX-FileCopyrightText: Magenta ApS
 
 SPDX-License-Identifier: MPL-2.0
 -->
 
@@ -77,7 +90,8 @@
     get_auth_exception_handler(logger)
 )
 
 @app.get("/")
 async def root(token: Token = Depends(auth)):
     return {"message": "Hello World"}
 ```
+
```

### Comparing `os2mo-fastapi-utils-1.3.0/README.md` & `os2mo_fastapi_utils-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/exceptions.py` & `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/oidc.py` & `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/oidc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
-
-from typing import Any, List, Type, TypeVar, Union
+from typing import Any
+from typing import List
+from typing import Type
+from typing import TypeVar
+from typing import Union
 
 import jwt.exceptions
-from fastapi import Depends, Request
+from fastapi import Depends
+from fastapi import Request
 from fastapi.security import OAuth2PasswordBearer
 from starlette.responses import JSONResponse
-from starlette.status import HTTP_401_UNAUTHORIZED, HTTP_500_INTERNAL_SERVER_ERROR
+from starlette.status import HTTP_401_UNAUTHORIZED
+from starlette.status import HTTP_500_INTERNAL_SERVER_ERROR
 
 from os2mo_fastapi_utils.auth.exceptions import AuthenticationError
 from os2mo_fastapi_utils.auth.models import Token
 
 TokenModel = TypeVar("TokenModel", bound=Token)
 
 
@@ -119,23 +124,21 @@
     :param logger: any logger for logging auth errors
     """
 
     def authentication_exception_handler(
         request: Request, err: AuthenticationError
     ) -> JSONResponse:
         if err.is_client_side_error():
-            logger.exception("Client side authentication error", exception=err.exc)
+            logger.exception("Client side authentication error", exc_info=err)
             return JSONResponse(
                 status_code=HTTP_401_UNAUTHORIZED,
                 content={"status": "Unauthorized", "msg": str(err.exc)},
             )
 
-        logger.exception(
-            "Problem communicating with the Keycloak server", exception=err.exc
-        )
+        logger.exception("Problem communicating with the Keycloak server", exc_info=err)
 
         return JSONResponse(
             status_code=HTTP_500_INTERNAL_SERVER_ERROR,
             content={"msg": "A server side authentication error occurred"},
         )
 
     return authentication_exception_handler
```

### Comparing `os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/auth/test_helper.py` & `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/auth/test_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
-
 from fastapi.routing import APIRoute
 
 
 def lookup_auth_dependency(route, auth_coro):
     # Check if auth dependency exists
     return any(d.dependency == auth_coro for d in route.dependencies)
```

### Comparing `os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/pydantic_types.py` & `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/pydantic_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # SPDX-FileCopyrightText: Magenta ApS
 #
 # SPDX-License-Identifier: MPL-2.0
+from typing import Any
+from typing import no_type_check
+from typing import Optional
+from typing import TYPE_CHECKING
 
-from typing import TYPE_CHECKING, Any, Optional, no_type_check
-
-from pydantic.errors import UrlHostError, UrlPortError
-from pydantic.fields import ModelField
-from pydantic.main import BaseConfig
-from pydantic.networks import ascii_domain_regex, int_domain_regex
+from pydantic.errors import UrlHostError
+from pydantic.errors import UrlPortError
+from pydantic.networks import ascii_domain_regex
+from pydantic.networks import int_domain_regex
 from pydantic.validators import str_validator
 
 if TYPE_CHECKING:  # pragma: no cover
     from pydantic.typing import CallableGenerator
 
 
 class Port(int):
```

### Comparing `os2mo-fastapi-utils-1.3.0/os2mo_fastapi_utils/tracing.py` & `os2mo_fastapi_utils-1.3.3/os2mo_fastapi_utils/tracing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # SPDX-FileCopyrightText: Magenta ApS
 #
 # SPDX-License-Identifier: MPL-2.0
-
 from contextlib import contextmanager
-from typing import List, Optional
-from uuid import UUID
+from typing import Optional
 
 import structlog
-from fastapi import Request, Response
+from fastapi import Request
+from fastapi import Response
 from opentelemetry import trace
 from opentelemetry.exporter.jaeger.thrift import JaegerExporter
 from opentelemetry.instrumentation.aiohttp_client import AioHttpClientInstrumentor
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
-from pydantic import BaseSettings, HttpUrl
-from pydantic.tools import parse_obj_as
+from pydantic import BaseSettings
 from structlog import get_logger
-from structlog.contextvars import (
-    bind_contextvars,
-    clear_contextvars,
-    merge_contextvars,
-    unbind_contextvars,
-)
+from structlog.contextvars import bind_contextvars
+from structlog.contextvars import clear_contextvars
+from structlog.contextvars import merge_contextvars
+from structlog.contextvars import unbind_contextvars
 
-from os2mo_fastapi_utils.pydantic_types import Domain, Port
+from os2mo_fastapi_utils.pydantic_types import Domain
+from os2mo_fastapi_utils.pydantic_types import Port
 
 
 class TracingSettings(BaseSettings):
     jaeger_service: str = "OS2mo_fastapi_utils"
     jaeger_hostname: Optional[Domain] = None
     jaeger_port: Port = Port(6831)
```

