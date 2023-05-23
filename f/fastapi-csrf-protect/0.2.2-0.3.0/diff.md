# Comparing `tmp/fastapi-csrf-protect-0.2.2.tar.gz` & `tmp/fastapi-csrf-protect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-csrf-protect-0.2.2.tar", max compression
+gzip compressed data, was "fastapi-csrf-protect-0.3.0.tar", max compression
```

## Comparing `fastapi-csrf-protect-0.2.2.tar` & `fastapi-csrf-protect-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2022-05-16 14:56:34.276540 fastapi-csrf-protect-0.2.2/LICENSE
--rw-r--r--   0        0        0     4748 2022-05-16 14:56:34.276789 fastapi-csrf-protect-0.2.2/README.md
--rw-r--r--   0        0        0      411 2022-05-16 15:15:39.097812 fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/__init__.py
--rw-r--r--   0        0        0     6407 2022-05-16 15:15:39.097834 fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/core.py
--rw-r--r--   0        0        0     2315 2022-05-16 15:15:39.097850 fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/csrf_config.py
--rw-r--r--   0        0        0      765 2022-05-16 15:15:39.098556 fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/exceptions.py
--rw-r--r--   0        0        0     2028 2022-05-16 15:15:39.097821 fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/load_config.py
--rw-r--r--   0        0        0     1660 2022-05-16 15:15:21.959037 fastapi-csrf-protect-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5900 2022-05-16 15:16:48.614933 fastapi-csrf-protect-0.2.2/setup.py
--rw-r--r--   0        0        0     6270 2022-05-16 15:16:48.615146 fastapi-csrf-protect-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-05-16 14:56:34.276540 fastapi-csrf-protect-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3647 2023-05-23 13:37:59.268734 fastapi-csrf-protect-0.3.0/README.md
+-rw-r--r--   0        0        0      443 2023-05-23 14:09:10.000718 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/__init__.py
+-rw-r--r--   0        0        0     6620 2023-05-23 14:09:10.000696 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/core.py
+-rw-r--r--   0        0        0     1941 2023-05-23 14:09:10.000710 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/csrf_config.py
+-rw-r--r--   0        0        0      825 2023-05-23 14:09:10.000832 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/exceptions.py
+-rw-r--r--   0        0        0     1867 2023-05-23 14:09:10.000763 fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/load_config.py
+-rw-r--r--   0        0        0     1768 2023-05-23 14:09:05.224543 fastapi-csrf-protect-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4590 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.0/setup.py
+-rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 fastapi-csrf-protect-0.3.0/PKG-INFO
```

### Comparing `fastapi-csrf-protect-0.2.2/LICENSE` & `fastapi-csrf-protect-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-csrf-protect-0.2.2/README.md` & `fastapi-csrf-protect-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 [![Package Vesion](https://img.shields.io/pypi/v/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 [![Format](https://img.shields.io/pypi/format/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 [![Python Version](https://img.shields.io/pypi/pyversions/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 [![License](https://img.shields.io/pypi/l/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 
 ## Features
 
-FastAPI extension that provides Cross-Site Request Forgery (XSRF) Protection support (easy to use and lightweight).
+FastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.
+Aimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.
 If you were familiar with `flask-wtf` library this extension suitable for you.
 This extension inspired by `fastapi-jwt-auth` 😀
 
 - Storing `fastapi-csrf-token` in cookies or serve it in template's context
 
 ## Installation
 
@@ -24,104 +25,58 @@
 poetry add fastapi-csrf-protect
 ```
 
 ## Getting Started
 
 The following examples show you how to integrate this extension to a FastAPI App
 
-### With Context and Headers
+### Example Login Form
 
 ```python
 from fastapi import FastAPI, Request, Depends
 from fastapi.responses import JSONResponse
 from fastapi.templating import Jinja2Templates
 from fastapi_csrf_protect import CsrfProtect
 from fastapi_csrf_protect.exceptions import CsrfProtectError
 from pydantic import BaseModel
 
 app = FastAPI()
-templates = Jinja2Templates(directory='templates')
+templates = Jinja2Templates(directory="templates")
 
 class CsrfSettings(BaseModel):
-  secret_key:str = 'asecrettoeverybody'
+  secret_key: str = "asecrettoeverybody"
+  cookie_samesite: str = "none"
 
 @CsrfProtect.load_config
 def get_csrf_config():
   return CsrfSettings()
 
-@app.get('/form')
-def form(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
+@app.get("/login")
+def form(request: Request, csrf_protect: CsrfProtect = Depends()):
+  """
   Returns form template.
-  '''
+  """
   csrf_token = csrf_protect.generate_csrf()
-  response = templates.TemplateResponse('form.html', {
-    'request': request, 'csrf_token': csrf_token
-  })
-  return response
-
-@app.post('/posts', response_class=JSONResponse)
-def create_post(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
-  Creates a new Post
-  '''
-  csrf_token = csrf_protect.get_csrf_from_headers(request.headers)
-  csrf_protect.validate_csrf(csrf_token)
-  # Do stuff
-
-@app.exception_handler(CsrfProtectError)
-def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
-  return JSONResponse(
-    status_code=exc.status_code,
-      content={ 'detail':  exc.message
-    }
+  response = templates.TemplateResponse(
+    "form.html", {"request": request, "csrf_token": csrf_token}
   )
-
-```
-
-### With Cookies
-
-```python
-from fastapi import FastAPI, Request, Depends
-from fastapi.responses import JSONResponse
-from fastapi.templating import Jinja2Templates
-from fastapi_csrf_protect import CsrfProtect
-from fastapi_csrf_protect.exceptions import CsrfProtectError
-from pydantic import BaseModel
-
-app = FastAPI()
-templates = Jinja2Templates(directory='templates')
-
-class CsrfSettings(BaseModel):
-  secret_key:str = 'asecrettoeverybody'
-
-@CsrfProtect.load_config
-def get_csrf_config():
-  return CsrfSettings()
-
-@app.get('/form')
-def form(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
-  Returns form template.
-  '''
-  response = templates.TemplateResponse('form.html', { 'request': request })
-  csrf_protect.set_csrf_cookie(response)
+  csrf_protect.set_csrf_cookie(csrf_token, response)
   return response
 
-@app.post('/posts', response_class=JSONResponse)
-def create_post(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
+@app.post("/login", response_class=JSONResponse)
+def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
+  """
   Creates a new Post
-  '''
-  csrf_protect.validate_csrf_in_cookies(request)
+  """
+  csrf_protect.validate_csrf(request)
   # Do stuff
 
 @app.exception_handler(CsrfProtectError)
 def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
-  return JSONResponse(status_code=exc.status_code, content={ 'detail':  exc.message })
+  return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})
 
 ```
 
 ## Contributions
 
 To contribute to the project, fork the repository and clone to your local device and install preferred testing dependency [pytest](https://github.com/pytest-dev/pytest)
 Alternatively, run the following command on your terminal to do so:
@@ -130,34 +85,29 @@
 pip install -U poetry
 poetry install
 ```
 
 Testing can be done by the following command post-installation:
 
 ```bash
+poetry install --with test
 pytest
 ```
 
 ### Run Examples
 
 To run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)
 Alternatively, run the following command on your terminal to do so
 
 ```bash
-poetry install --extras examples
+poetry install --with examples
 ```
 
-1. Running the example utilizing Context and Headers
+Running the example utilizing Context and Headers
 
-    ```bash
-    uvicorn examples.context:app
-    ```
-
-2. Running the example utilizing Cookies
-
-    ```bash
-    uvicorn examples.cookies:app
-    ```
+```bash
+uvicorn examples.login:app
+```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/core.py` & `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,166 @@
 #!/usr/bin/env python3
-# Copyright (C) 2019-2020 All rights reserved.
+# Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  core.py
-# VERSION: 	 0.2.2
+# VERSION: 	 0.3.0
 # CREATED: 	 2020-11-25 14:35
-# AUTHOR: 	 Aekasitt Guruvanich <aekazitt@gmail.com>
+# AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
-#*************************************************************
+# *************************************************************
 import re
 from os import urandom
 from hashlib import sha1
 from typing import Optional
 from fastapi.requests import Request
 from fastapi.responses import Response
 from starlette.datastructures import Headers
 from itsdangerous import BadData, SignatureExpired, URLSafeTimedSerializer
 from fastapi_csrf_protect.csrf_config import CsrfConfig
-from fastapi_csrf_protect.exceptions import InvalidHeaderError, MissingTokenError, TokenValidationError
+from fastapi_csrf_protect.exceptions import (
+    InvalidHeaderError,
+    MissingTokenError,
+    TokenValidationError,
+)
 
-class CsrfProtect(CsrfConfig):
 
-  def __init__(self, request: Request = None, response: Response = None):
-    '''
-    Retrieve response object if jwt in the cookie
-
-    ---
-    :param request: all incoming request  
-    :type request: fastapi.requests.Request  
-    :param response: response from endpoint  
-    :type response: fastapi.responses.Response  
-    '''
-    if response and self.token_in_cookies:
-      self._response = response
-
-  def generate_csrf(self, secret_key: Optional[str] = None):
-    '''
-    Generate a CSRF token.
-    TODO: The token should be cached for a request, so multiple
-    calls to this function will generate the same token.
-
-    ---
-    :param secret_key: (Optional) the secret key used when generating a new token for users
-    :type secret_key: str
-    '''
-    secret_key = secret_key or self._secret_key
-    if secret_key is None: raise RuntimeError('A secret key is required to use CSRF.')
-    serializer = URLSafeTimedSerializer(secret_key, salt='fastapi-csrf-token')
-    token = serializer.dumps(sha1(urandom(64)).hexdigest())
-    return token
-
-  def get_csrf_from_headers(self, headers: Headers) -> str:
-    '''
-    Get token from the headers
-
-    ---
-    :param headers: Headers containing header with configured `csrf_header_name`
-    :type headers: starlette.datastructures.Headers
-    '''
-    header_name, header_type = self._csrf_header_name, self._csrf_header_type
-    header_parts = None
-    try:
-      header_parts = headers[header_name].split()
-    except KeyError:
-      raise InvalidHeaderError(f'Bad headers. Expected "{header_name}" in headers')
-    token = None
-    # Make sure the header is in a valid format that we are expecting, ie
-    if not header_type:
-      # <HeaderName>: <Token>
-      if len(header_parts) != 1:
-        raise InvalidHeaderError(f'Bad {header_name} header. Expected value "<Token>"')
-      token = header_parts[0]
-    else:
-      # <HeaderName>: <HeaderType> <Token>
-      if not re.match(r"{}\s".format(header_type), headers[header_name]) or len(header_parts) != 2:
-        raise InvalidHeaderError(f'Bad {header_name} header. Expected value "{header_type} <Token>"')
-      token = header_parts[1]
-    return token
-
-  def set_csrf_cookie(self, response: Optional[Response] = None) -> None:
-    '''
-    Sets Csrf Protection token to the response cookies
-
-    ---
-    :param response: The FastAPI response object to sets the access cookies in.
-    :type response: fastapi.responses.Response
-    '''
-    if response and not isinstance(response,Response):
-      raise TypeError('The response must be an object response FastAPI')
-    response = response or self._response
-    response.set_cookie(
-      self._cookie_key,
-      self.generate_csrf(self._secret_key),
-      max_age=self._max_age,
-      path=self._cookie_path,
-      domain=self._cookie_domain,
-      secure=self._cookie_secure,
-      httponly=self._httponly,
-      samesite=self._cookie_samesite
-    )
-
-  def unset_csrf_cookie(self, response: Optional[Response] = None) -> None:
-    '''
-    Remove Csrf Protection token from the response cookies
-
-    ---
-    :param response: (Optional) The FastAPI response object to delete the access cookies in.
-    :type response: fastapi.responses.Response
-    '''
-    if response and not isinstance(response, Response):
-      raise TypeError('The response must be an object response FastAPI')
-    response = response or self._response
-    response.delete_cookie(
-      self._cookie_key,
-      path=self._cookie_path,
-      domain=self._cookie_domain
-    )
-
-  def validate_csrf(self, data, secret_key: Optional[str] = None, time_limit: Optional[int] = None):
-    '''
-    Check if the given data is a valid CSRF token. This compares the given
-    signed token to the one stored in the session.
-
-    ---
-    :param data: The signed CSRF token to be checked.
-    :type data: Any
-    :param secret_key: (Optional) secret key used to decrypt the token
-        Default is set in CsrfConfig when `load_config` was called;
-    :type secret_key: str
-    :param time_limit: (Optional) Number of seconds that the token is valid.
-        Default is set in CsrfConfig when `load_config` was called;
-    :type time_limit: int
-    :raises TokenValidationError: Contains the reason that validation failed.
-    '''
-    secret_key = secret_key or self._secret_key
-    if secret_key is None: raise RuntimeError('A secret key is required to use CSRF.')
-    time_limit = time_limit or self._max_age
-    if not data:
-      raise TokenValidationError('The CSRF token is missing.')
-    serializer = URLSafeTimedSerializer(secret_key, salt='fastapi-csrf-token')
-    try:
-      token = serializer.loads(data, max_age=time_limit)
-    except SignatureExpired:
-      raise TokenValidationError('The CSRF token has expired.')
-    except BadData:
-      raise TokenValidationError('The CSRF token is invalid.')
-
-  def validate_csrf_in_cookies(self, request: Request, secret_key: Optional[str] = None, field_name: Optional[str] = None):
-    '''
-    Check if the given Request with its Cookies contains a valid CSRF token.  
-    Once extracted, off-loads logic to `validate_csrf` method.  
-
-    ---
-    :param request: all incoming request  
-    :type request: fastapi.requests.Request
-    :param secret_key: (Optional) secret key used to decrypt the token
-    :type secret_key: str
-    :param field_name: (Optional)
-        Default is set in CsrfConfig when `load_config` was called;
-    :type field_name: str
-    '''
-    field_name = field_name or self._cookie_key
-    cookie = request.cookies.get(field_name)
-    if cookie is None: raise MissingTokenError(f'Missing Cookie {field_name}')
-    self.validate_csrf(cookie, secret_key)
+class CsrfProtect(CsrfConfig):
+    def generate_csrf(self, secret_key: Optional[str] = None):
+        """
+        Generate a CSRF token.
+        TODO: The token should be cached for a request, so multiple
+        calls to this function will generate the same token.
+
+        ---
+        :param secret_key: (Optional) the secret key used when generating a new token for users
+        :type secret_key: str
+        """
+        secret_key = secret_key or self._secret_key
+        if secret_key is None:
+            raise RuntimeError("A secret key is required to use CsrfProtect extension.")
+        serializer = URLSafeTimedSerializer(secret_key, salt="fastapi-csrf-token")
+        token = serializer.dumps(sha1(urandom(64)).hexdigest())
+        return token
+
+    def get_csrf_from_headers(self, headers: Headers) -> str:
+        """
+        Get token from the headers
+
+        ---
+        :param headers: Headers containing header with configured `header_name`
+        :type headers: starlette.datastructures.Headers
+        """
+        header_name, header_type = self._header_name, self._header_type
+        header_parts = None
+        try:
+            header_parts = headers[header_name].split()
+        except KeyError:
+            raise InvalidHeaderError(
+                f'Bad headers. Expected "{header_name}" in headers'
+            )
+        token = None
+        # Make sure the header is in a valid format that we are expecting, ie
+        if not header_type:
+            # <HeaderName>: <Token>
+            if len(header_parts) != 1:
+                raise InvalidHeaderError(
+                    f'Bad {header_name} header. Expected value "<Token>"'
+                )
+            token = header_parts[0]
+        else:
+            # <HeaderName>: <HeaderType> <Token>
+            if (
+                not re.match(r"{}\s".format(header_type), headers[header_name])
+                or len(header_parts) != 2
+            ):
+                raise InvalidHeaderError(
+                    f'Bad {header_name} header. Expected value "{header_type} <Token>"'
+                )
+            token = header_parts[1]
+        return token
+
+    def set_csrf_cookie(
+        self, csrf_token: Optional[str] = None, response: Optional[Response] = None
+    ) -> None:
+        """
+        Sets Csrf Protection token to the response cookies
+
+        ---
+        :param csrf_token: (Optional) pre-determined token data
+        :type csrf_token: str
+        :param response: The FastAPI response object to sets the access cookies in.
+        :type response: fastapi.responses.Response
+        """
+        csrf_token = csrf_token or self.generate_csrf(self._secret_key)
+        if response and not isinstance(response, Response):
+            raise TypeError("The response must be an object response FastAPI")
+        response = response or self._response
+        response.set_cookie(
+            self._cookie_key,
+            csrf_token,
+            max_age=self._max_age,
+            path=self._cookie_path,
+            domain=self._cookie_domain,
+            secure=self._cookie_secure,
+            httponly=self._httponly,
+            samesite=self._cookie_samesite,
+        )
+
+    def unset_csrf_cookie(self, response: Optional[Response] = None) -> None:
+        """
+        Remove Csrf Protection token from the response cookies
+
+        ---
+        :param response: (Optional) The FastAPI response object to delete the access cookies in.
+        :type response: fastapi.responses.Response
+        """
+        if response and not isinstance(response, Response):
+            raise TypeError("The response must be an object response FastAPI")
+        response = response or self._response
+        response.delete_cookie(
+            self._cookie_key, path=self._cookie_path, domain=self._cookie_domain
+        )
+
+    def validate_csrf(
+        self,
+        request: Request,
+        cookie_key: Optional[str] = None,
+        secret_key: Optional[str] = None,
+        time_limit: Optional[int] = None,
+    ):
+        """
+        Check if the given data is a valid CSRF token. This compares the given
+        signed token to the one stored in the session.
+
+        ---
+        :param request: incoming Request instance
+        :type request: fastapi.requests.Request
+        :param cookie_key: (Optional) field name for the CSRF token field stored in cookies
+            Default is set in CsrfConfig when `load_config` was called;
+        :type cookie_key: str
+        :param secret_key: (Optional) secret key used to decrypt the token
+            Default is set in CsrfConfig when `load_config` was called;
+        :type secret_key: str
+        :param time_limit: (Optional) Number of seconds that the token is valid.
+            Default is set in CsrfConfig when `load_config` was called;
+        :type time_limit: int
+        :raises TokenValidationError: Contains the reason that validation failed.
+        """
+        secret_key = secret_key or self._secret_key
+        if secret_key is None:
+            raise RuntimeError("A secret key is required to use CsrfProtect extension.")
+        cookie_key = cookie_key or self._cookie_key
+        cookie_token = request.cookies.get(cookie_key)
+        if cookie_token is None:
+            raise MissingTokenError(f"Missing Cookie: `{cookie_key}`.")
+        time_limit = time_limit or self._max_age
+        token: str = self.get_csrf_from_headers(request.headers)
+        if token != cookie_token:
+            raise TokenValidationError("The CSRF token pair submitted do not match.")
+        serializer = URLSafeTimedSerializer(secret_key, salt="fastapi-csrf-token")
+        try:
+            serializer.loads(token, max_age=time_limit)
+        except SignatureExpired:
+            raise TokenValidationError("The CSRF token has expired.")
+        except BadData:
+            raise TokenValidationError("The CSRF token is invalid.")
```

### Comparing `fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/csrf_config.py` & `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/csrf_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 #!/usr/bin/env python3
-# Copyright (C) 2019-2020 All rights reserved.
+# Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  fastapi_csrf_config.py
-# VERSION: 	 0.2.2
+# VERSION: 	 0.3.0
 # CREATED: 	 2020-11-25 14:35
-# AUTHOR: 	 Aekasitt Guruvanich <aekazitt@gmail.com>
+# AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
-#*************************************************************
-from typing import Callable, List, Sequence
+# *************************************************************
+### Standard Packages ###
+from typing import Callable, List, Literal, Optional, Sequence
+
+### Third-Party Modules ###
 from pydantic import ValidationError
-from fastapi_csrf_protect.load_config import LoadConfig
 
-class CsrfConfig(object):
-  _csrf_header_name: str          = 'X-CSRF-Token'
-  _csrf_header_type: str          = None
-  _csrf_in_cookies: bool          = True
-  _csrf_methods: Sequence[str]    = { 'POST', 'PUT', 'PATCH', 'DELETE' }
-  _max_age: int                   = 3600
-  _secret_key: str                = None
-  _token_locations: Sequence[str] = { 'headers' }
-  # In case of using cookies
-  _cookie_key: str                = 'fastapi-csrf-token'
-  _cookie_path: str               = '/'
-  _cookie_domain: str             = None
-  _cookie_secure: bool            = False
-  _cookie_samesite: bool          = None
-  _cookie_csrf_protect: bool      = True
-  _httponly: bool                 = True
+### Local Modules ###
+from fastapi_csrf_protect.load_config import LoadConfig
 
-  @property
-  def token_in_headers(self) -> bool:
-    return 'headers' in self._token_locations
 
-  @property
-  def token_in_cookies(self) -> bool:
-    return 'cookies' in self._token_locations
+class CsrfConfig(object):
+    _cookie_key: str = "fastapi-csrf-token"
+    _cookie_path: str = "/"
+    _cookie_domain: str = None
+    _cookie_samesite: Optional[Literal["lax", "strict", "none"]] = None
+    _cookie_secure: bool = False
+    _header_name: str = "X-CSRF-Token"
+    _header_type: str = None
+    _httponly: bool = True
+    _max_age: int = 3600
+    _methods: Sequence[str] = {"POST", "PUT", "PATCH", "DELETE"}
+    _secret_key: str = None
 
-  @classmethod
-  def load_config(cls, settings: Callable[..., List[tuple]]) -> 'CsrfConfig':
-    try:
-      config = LoadConfig(**{key.lower():value for key,value in settings()})
-      cls._csrf_header_name = config.csrf_header_name
-      cls._csrf_header_type = config.csrf_header_type
-      cls._csrf_in_cookies = config.csrf_in_cookies
-      cls._csrf_methods = config.csrf_methods
-      cls._max_age = config.max_age
-      cls._secret_key = config.secret_key
-      cls._token_locations = config.token_locations
-      cls._cookie_key = config.cookie_key
-      cls._cookie_path = config.cookie_path
-      cls._cookie_domain = config.cookie_domain
-      cls._cookie_secure = config.cookie_secure
-      cls._cookie_samesite = config.cookie_samesite
-      cls._cookie_csrf_protect = config.cookie_csrf_protect
-      cls._httponly = config.httponly
-    except ValidationError: raise
-    except Exception:
-      raise TypeError('CsrfConfig must be pydantic "BaseSettings" or list of tuple')
+    @classmethod
+    def load_config(cls, settings: Callable[..., List[tuple]]) -> None:
+        try:
+            config = LoadConfig(**{key.lower(): value for key, value in settings()})
+            cls._cookie_key = config.cookie_key
+            cls._cookie_path = config.cookie_path
+            cls._cookie_domain = config.cookie_domain
+            cls._cookie_samesite = config.cookie_samesite
+            cls._cookie_secure = config.cookie_secure
+            cls._header_name = config.header_name
+            cls._header_type = config.header_type
+            cls._httponly = config.httponly
+            cls._max_age = config.max_age
+            cls._methods = config.methods
+            cls._secret_key = config.secret_key
+        except ValidationError:
+            raise
+        except Exception as err:
+            print(err)
+            raise TypeError(
+                'CsrfConfig must be pydantic "BaseSettings" or list of tuple'
+            )
```

### Comparing `fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/exceptions.py` & `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #!/usr/bin/env python3
-# Copyright (C) 2019-2020 All rights reserved.
+# Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  exceptions.py
-# VERSION: 	 0.2.2
+# VERSION: 	 0.3.0
 # CREATED: 	 2020-11-25 14:35
-# AUTHOR: 	 Aekasitt Guruvanich <aekazitt@gmail.com>
+# AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
-#*************************************************************
+# *************************************************************
 class CsrfProtectError(Exception):
-  def __init__(self, status_code, message):
-    self.status_code = status_code
-    self.message = message
+    def __init__(self, status_code: int, message: str):
+        self.status_code = status_code
+        self.message = message
+
 
 class InvalidHeaderError(CsrfProtectError):
-  def __init__(self, message):
-    super().__init__(422, message)
+    def __init__(self, message: str):
+        super().__init__(422, message)
+
 
 class MissingTokenError(CsrfProtectError):
-  def __init__(self, message):
-    super().__init__(400, message)
+    def __init__(self, message: str):
+        super().__init__(400, message)
+
 
 class TokenValidationError(CsrfProtectError):
-  def __init__(self, message):
-    super().__init__(401, message)
+    def __init__(self, message: str):
+        super().__init__(401, message)
```

### Comparing `fastapi-csrf-protect-0.2.2/fastapi_csrf_protect/load_config.py` & `fastapi-csrf-protect-0.3.0/fastapi_csrf_protect/load_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 #!/usr/bin/env python3
-# Copyright (C) 2019-2020 All rights reserved.
+# Copyright (C) 2021-2023 All rights reserved.
 # FILENAME:  load_config.py
-# VERSION: 	 0.2.2
+# VERSION: 	 0.3.0
 # CREATED: 	 2020-11-25 14:35
-# AUTHOR: 	 Aekasitt Guruvanich <aekazitt@gmail.com>
+# AUTHOR: 	 Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
-#*************************************************************
+# *************************************************************
 from typing import Optional, Sequence
 from pydantic import BaseModel, validator, StrictBool, StrictInt, StrictStr
 
+
 class LoadConfig(BaseModel):
-  csrf_header_name: Optional[StrictStr]          = 'X-CSRF-Token'
-  csrf_header_type: Optional[StrictStr]          = None
-  csrf_in_cookies: Optional[StrictBool]          = True
-  csrf_methods: Optional[Sequence[StrictStr]]    = { 'POST', 'PUT', 'PATCH', 'DELETE' }
-  max_age: Optional[StrictInt]                   = 3600
-  secret_key: Optional[StrictStr]                = None
-  token_locations: Optional[Sequence[StrictStr]] = { 'headers' }
-  # In case of using cookies
-  cookie_key: Optional[StrictStr]                = 'fastapi-csrf-token'
-  cookie_path: Optional[StrictStr]               = '/'
-  cookie_domain: Optional[StrictStr]             = None
-  cookie_secure: Optional[StrictBool]            = False
-  cookie_samesite: Optional[StrictStr]           = 'lax'
-  cookie_csrf_protect: Optional[StrictBool]      = True
-  httponly: Optional[StrictBool]                 = True
+    cookie_key: Optional[StrictStr] = "fastapi-csrf-token"
+    cookie_path: Optional[StrictStr] = "/"
+    cookie_domain: Optional[StrictStr] = None
+    # NOTE: `cookie_secure` must be placed before `cookie_samesite`
+    cookie_secure: Optional[StrictBool] = False
+    cookie_samesite: Optional[StrictStr] = "lax"
+    header_name: Optional[StrictStr] = "X-CSRF-Token"
+    header_type: Optional[StrictStr] = None
+    httponly: Optional[StrictBool] = True
+    max_age: Optional[StrictInt] = 3600
+    methods: Optional[Sequence[StrictStr]] = {"POST", "PUT", "PATCH", "DELETE"}
+    secret_key: Optional[StrictStr] = None
 
-  @validator('csrf_methods', each_item=True)
-  def validate_csrf_methods(cls, value):
-    if value.upper() not in {'GET', 'HEAD', 'POST', 'PUT', 'DELETE', 'PATCH'}:
-      raise ValueError('The "csrf_methods" must be between http request methods')
-    return value.upper()
+    @validator("methods", each_item=True)
+    def validate_csrf_methods(cls, value):
+        if value.upper() not in {"GET", "HEAD", "POST", "PUT", "DELETE", "PATCH"}:
+            raise ValueError('The "csrf_methods" must be between http request methods')
+        return value.upper()
 
-  @validator('cookie_samesite', always=True)
-  def validate_cookie_samesite(cls, value: str, values: dict):
-    if value not in { 'strict', 'lax', 'none' }:
-      raise ValueError('The "cookie_samesite" must be between "strict", "lax", or "none".')
-    elif value == 'none' and values.get('cookie_secure', False) is not True:
-      raise ValueError('The "cookie_secure" must be True if "cookie_samesite" set to "none".')
-    return value
+    @validator("cookie_samesite", always=True)
+    def validate_cookie_samesite(cls, value: str, values: dict):
+        if value not in {"strict", "lax", "none"}:
+            raise ValueError(
+                'The "cookie_samesite" must be between "strict", "lax", or "none".'
+            )
+        elif value == "none" and values.get("cookie_secure", False) is not True:
+            raise ValueError(
+                'The "cookie_secure" must be True if "cookie_samesite" set to "none".'
+            )
+        return value
```

### Comparing `fastapi-csrf-protect-0.2.2/pyproject.toml` & `fastapi-csrf-protect-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 [tool.poetry]
 name = "fastapi-csrf-protect"
-version = "0.2.2"
-description = "Simple integration of Cross-Site Request Forgery (XSRF) Protection by using either Cookies or Context combined with Headers"
+version = "0.3.0"
+description = "Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern"
 authors = ["Sitt Guruvanich <aekazitt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aekasitt/fastapi-csrf-protect"
 repository = "https://github.com/aekasitt/fastapi-csrf-protect"
 keywords = ["starlette", "fastapi", "csrf", "xsrf", "cross-site request forgery", "samesite", "asynchronous"]
 classifiers = [
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Operating System :: OS Independent",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
   "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
+python = "^3.7"
 fastapi = "^0"
 itsdangerous = ">=2.0.1,<3.0.0"
 pydantic = ">=1.7.2,<2.0.0"
-uvicorn = {version = "^0.15.0", optional = true, extras = ["examples"]}
-Jinja2 = {version = "^3.0.1", optional = true, extras = ["examples"]}
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+mypy = "^1.3.0"
 
-[tool.poetry.extras]
-examples = [ "uvicorn", "jinja2" ]
+[tool.poetry.group.examples]
+optional = true
+
+[tool.poetry.group.examples.dependencies]
+Jinja2 = "^3.0.1"
+uvicorn = "^0.15.0"
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+httpx = "^0.24.1"
+pytest = "^7.3.1"
 
 [tool.pytest.ini_options]
 addopts = "--strict-markers --tb=short -s"
 testpaths = [ "tests" ]
 python_files = "*.py"
 
 [build-system]
```

### Comparing `fastapi-csrf-protect-0.2.2/PKG-INFO` & `fastapi-csrf-protect-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: fastapi-csrf-protect
-Version: 0.2.2
-Summary: Simple integration of Cross-Site Request Forgery (XSRF) Protection by using either Cookies or Context combined with Headers
+Version: 0.3.0
+Summary: Stateless implementation of Cross-Site Request Forgery (XSRF) Protection by using Double Submit Cookie mitigation pattern
 Home-page: https://github.com/aekasitt/fastapi-csrf-protect
 License: MIT
 Keywords: starlette,fastapi,csrf,xsrf,cross-site request forgery,samesite,asynchronous
 Author: Sitt Guruvanich
 Author-email: aekazitt@gmail.com
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: examples
-Requires-Dist: Jinja2[examples] (>=3.0.1,<4.0.0); extra == "examples"
 Requires-Dist: fastapi (>=0,<1)
 Requires-Dist: itsdangerous (>=2.0.1,<3.0.0)
 Requires-Dist: pydantic (>=1.7.2,<2.0.0)
-Requires-Dist: uvicorn[examples] (>=0.15.0,<0.16.0); extra == "examples"
 Project-URL: Repository, https://github.com/aekasitt/fastapi-csrf-protect
 Description-Content-Type: text/markdown
 
 # FastAPI CSRF Protect
 
 [![Build Status](https://travis-ci.com/aekasitt/fastapi-csrf-protect.svg?branch=master)](https://app.travis-ci.com/github/aekasitt/fastapi-csrf-protect)
 [![Package Vesion](https://img.shields.io/pypi/v/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 [![Format](https://img.shields.io/pypi/format/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 [![Python Version](https://img.shields.io/pypi/pyversions/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 [![License](https://img.shields.io/pypi/l/fastapi-csrf-protect)](https://pypi.org/project/fastapi-csrf-protect)
 
 ## Features
 
-FastAPI extension that provides Cross-Site Request Forgery (XSRF) Protection support (easy to use and lightweight).
+FastAPI extension that provides stateless Cross-Site Request Forgery (XSRF) Protection support.
+Aimed to be easy to use and lightweight, we adopt [Double Submit Cookie](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie) mitigation pattern.
 If you were familiar with `flask-wtf` library this extension suitable for you.
 This extension inspired by `fastapi-jwt-auth` 😀
 
 - Storing `fastapi-csrf-token` in cookies or serve it in template's context
 
 ## Installation
 
@@ -56,104 +59,58 @@
 poetry add fastapi-csrf-protect
 ```
 
 ## Getting Started
 
 The following examples show you how to integrate this extension to a FastAPI App
 
-### With Context and Headers
+### Example Login Form
 
 ```python
 from fastapi import FastAPI, Request, Depends
 from fastapi.responses import JSONResponse
 from fastapi.templating import Jinja2Templates
 from fastapi_csrf_protect import CsrfProtect
 from fastapi_csrf_protect.exceptions import CsrfProtectError
 from pydantic import BaseModel
 
 app = FastAPI()
-templates = Jinja2Templates(directory='templates')
+templates = Jinja2Templates(directory="templates")
 
 class CsrfSettings(BaseModel):
-  secret_key:str = 'asecrettoeverybody'
+  secret_key: str = "asecrettoeverybody"
+  cookie_samesite: str = "none"
 
 @CsrfProtect.load_config
 def get_csrf_config():
   return CsrfSettings()
 
-@app.get('/form')
-def form(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
+@app.get("/login")
+def form(request: Request, csrf_protect: CsrfProtect = Depends()):
+  """
   Returns form template.
-  '''
+  """
   csrf_token = csrf_protect.generate_csrf()
-  response = templates.TemplateResponse('form.html', {
-    'request': request, 'csrf_token': csrf_token
-  })
-  return response
-
-@app.post('/posts', response_class=JSONResponse)
-def create_post(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
-  Creates a new Post
-  '''
-  csrf_token = csrf_protect.get_csrf_from_headers(request.headers)
-  csrf_protect.validate_csrf(csrf_token)
-  # Do stuff
-
-@app.exception_handler(CsrfProtectError)
-def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
-  return JSONResponse(
-    status_code=exc.status_code,
-      content={ 'detail':  exc.message
-    }
+  response = templates.TemplateResponse(
+    "form.html", {"request": request, "csrf_token": csrf_token}
   )
-
-```
-
-### With Cookies
-
-```python
-from fastapi import FastAPI, Request, Depends
-from fastapi.responses import JSONResponse
-from fastapi.templating import Jinja2Templates
-from fastapi_csrf_protect import CsrfProtect
-from fastapi_csrf_protect.exceptions import CsrfProtectError
-from pydantic import BaseModel
-
-app = FastAPI()
-templates = Jinja2Templates(directory='templates')
-
-class CsrfSettings(BaseModel):
-  secret_key:str = 'asecrettoeverybody'
-
-@CsrfProtect.load_config
-def get_csrf_config():
-  return CsrfSettings()
-
-@app.get('/form')
-def form(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
-  Returns form template.
-  '''
-  response = templates.TemplateResponse('form.html', { 'request': request })
-  csrf_protect.set_csrf_cookie(response)
+  csrf_protect.set_csrf_cookie(csrf_token, response)
   return response
 
-@app.post('/posts', response_class=JSONResponse)
-def create_post(request: Request, csrf_protect:CsrfProtect = Depends()):
-  '''
+@app.post("/login", response_class=JSONResponse)
+def create_post(request: Request, csrf_protect: CsrfProtect = Depends()):
+  """
   Creates a new Post
-  '''
-  csrf_protect.validate_csrf_in_cookies(request)
+  """
+  csrf_protect.validate_csrf(request)
   # Do stuff
 
 @app.exception_handler(CsrfProtectError)
 def csrf_protect_exception_handler(request: Request, exc: CsrfProtectError):
-  return JSONResponse(status_code=exc.status_code, content={ 'detail':  exc.message })
+  return JSONResponse(status_code=exc.status_code, content={"detail": exc.message})
 
 ```
 
 ## Contributions
 
 To contribute to the project, fork the repository and clone to your local device and install preferred testing dependency [pytest](https://github.com/pytest-dev/pytest)
 Alternatively, run the following command on your terminal to do so:
@@ -162,35 +119,30 @@
 pip install -U poetry
 poetry install
 ```
 
 Testing can be done by the following command post-installation:
 
 ```bash
+poetry install --with test
 pytest
 ```
 
 ### Run Examples
 
 To run the provided examples, first you must install extra dependencies [uvicorn](https://github.com/encode/uvicorn) and [jinja2](https://github.com/pallets/jinja/)
 Alternatively, run the following command on your terminal to do so
 
 ```bash
-poetry install --extras examples
+poetry install --with examples
 ```
 
-1. Running the example utilizing Context and Headers
+Running the example utilizing Context and Headers
 
-    ```bash
-    uvicorn examples.context:app
-    ```
-
-2. Running the example utilizing Cookies
-
-    ```bash
-    uvicorn examples.cookies:app
-    ```
+```bash
+uvicorn examples.login:app
+```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

