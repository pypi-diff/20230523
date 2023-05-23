# Comparing `tmp/jwt_validate-0.3.4.tar.gz` & `tmp/jwt_validate-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwt_validate-0.3.4.tar", max compression
+gzip compressed data, was "jwt_validate-0.3.5.tar", max compression
```

## Comparing `jwt_validate-0.3.4.tar` & `jwt_validate-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.4/index.md
--rw-r--r--   0        0        0     2112 2023-05-19 14:38:52.702124 jwt_validate-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.4/src/__init__.py
--rw-r--r--   0        0        0      773 2023-05-19 12:36:44.634536 jwt_validate-0.3.4/src/config.py
--rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.4/src/constants.py
--rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.4/src/exceptions.py
--rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.4/src/generate/generate_jwt.py
--rw-r--r--   0        0        0      432 2023-05-16 22:18:03.768247 jwt_validate-0.3.4/src/main.py
--rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.4/src/utils.py
--rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.4/src/validate/__init__.py
--rw-r--r--   0        0        0     2960 2023-05-19 14:38:04.506439 jwt_validate-0.3.4/src/validate/validate_jwt.py
--rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 jwt_validate-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1663 2023-05-19 12:12:52.897568 jwt_validate-0.3.5/index.md
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152260 jwt_validate-0.3.5/jwt_validate/__init__.py
+-rw-r--r--   0        0        0      492 2023-05-19 17:00:39.522115 jwt_validate-0.3.5/jwt_validate/config.py
+-rw-r--r--   0        0        0      437 2023-05-16 20:05:04.152451 jwt_validate-0.3.5/jwt_validate/constants.py
+-rw-r--r--   0        0        0      934 2023-05-16 20:05:04.152530 jwt_validate-0.3.5/jwt_validate/exceptions.py
+-rw-r--r--   0        0        0      395 2023-05-16 20:05:04.152650 jwt_validate-0.3.5/jwt_validate/generate/generate_jwt.py
+-rw-r--r--   0        0        0      243 2023-05-16 20:05:04.152823 jwt_validate-0.3.5/jwt_validate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:05:04.152895 jwt_validate-0.3.5/jwt_validate/validate/__init__.py
+-rw-r--r--   0        0        0     3362 2023-05-19 17:03:52.093642 jwt_validate-0.3.5/jwt_validate/validate/validate_jwt.py
+-rw-r--r--   0        0        0     2122 2023-05-23 11:59:22.547719 jwt_validate-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 jwt_validate-0.3.5/PKG-INFO
```

### Comparing `jwt_validate-0.3.4/index.md` & `jwt_validate-0.3.5/index.md`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.4/pyproject.toml` & `jwt_validate-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "jwt-validate"
-version = "0.3.4"
+version = "0.3.5"
 description = "Library for validation token JWT"
 authors = ["Reinaldo Saraiva do Carmo <reinaldo.carmo@luizalabs.com>"]
 license = "BeerWare"
 readme = "index.md"
-packages = [{include = "src"}]
+packages = [{include = "jwt_validate"}]
 
 classifiers = [
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware",
     "Development Status :: 5 - Production/Stable",
     "Natural Language :: English",
     "Framework :: FastAPI",
     "Intended Audience :: Developers",
@@ -53,14 +53,15 @@
 
 [tool.pytest.ini_options]
 pythonpath = "."
 log_level = "DEBUG"
 addopts = "-ra --doctest-modules"
 
 
+
 [tool.coverage.run]
 omit = ["*/*/tests/*", "*/*/settings/*", "**/tests/*", "**/conftest.py", "**/db.py", "**/base_class.py"]
 
 
 [tool.isort]
 profile = "black"
 line_length = 79
```

### Comparing `jwt_validate-0.3.4/src/exceptions.py` & `jwt_validate-0.3.5/jwt_validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwt_validate-0.3.4/src/validate/validate_jwt.py` & `jwt_validate-0.3.5/jwt_validate/validate/validate_jwt.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,44 +3,57 @@
 
 import jwt
 from fastapi import (
     Depends,
     HTTPException,
 )
 from fastapi.security import (
-    HTTPAuthorizationCredentials,
     HTTPBearer,
+    OAuth2PasswordBearer,
+    SecurityScopes,
 )
 from jwt.exceptions import (
     DecodeError,
     ExpiredSignatureError,
 )
 
-from src.config import settings
+from jwt_validate.config import settings
 
 security = HTTPBearer()
-jwks = jwt.PyJWKClient(settings.IDPA_URL)
+jwks = jwt.PyJWKClient(
+    settings.IDPA_URL, lifespan=settings.IDPA_JWKS_CACHE_TIME_SECONDS
+)
+
+oauth2_scheme = OAuth2PasswordBearer(
+    tokenUrl=f'{settings.IDPA_URL}/oauth/token',
+    scopes={
+        'usr:user-standing:admin': 'Interact with administrative routes.',
+        'openid': 'Default OpenID scope.',
+    },
+)
 
 
 def validate_jwt(token: str, required_scopes: list) -> dict:
-    """The method that receives a JWT token generated by IDMAGALU and its scope
+    """This method receives a JWT token generated by ID Magalu and a list of
+       scopes for validating the token signature using ID Magalu certificate
+       and the existency of the parameterized scopes.
 
     Parameters:
         token (str): A JWT token generated from the RS256 algorithm is expected as a parameter.
         required_scopes (list): As a parameter, the scope of the action for which the JWT token was authorized is expected.
     Returns:
-        dict: Checked the signature on the JWT token and return its claims.
+        dict: The decoded JWT token with the claims.
     Raises:
         ExpiredSignatureError: Signature has expired
         DecodeError: Invalid token
         HTTPException: Insufficient permissions, missing scope "{scope}"
 
 
     Examples:
-        >>> from src.generate.generate_jwt import generate_jwt
+        >>> from jwt_validate.generate.generate_jwt import generate_jwt
         >>> token = generate_jwt()['token']
         >>> validate_jwt(token=token,required_scopes=['block-storage.read']) # doctest: +ELLIPSIS
         {'iss': '...', 'iat': ..., 'jti': '...', 'aud': '...', 'scope': '...', 'pid': '...', 'tenant': '...', 'email': '...', 'sub': '...', 'exp': ...}
     """
     try:
         signing_key = jwks.get_signing_key_from_jwt(token)
         decoded_token = jwt.decode(
@@ -73,15 +86,15 @@
         )
 
 
 def validate_jwt_scopes(required_scopes: list = []):
     def decorator(func):
         @wraps(func)
         async def wrapper(
-            credentials: HTTPAuthorizationCredentials = Depends(security),
+            credentials: oauth2_scheme = Depends(security),
             *args,
             **kwargs,
         ):
             validate_jwt(
                 token=credentials.credentials, required_scopes=required_scopes
             )
             return await func(*args, **kwargs)
```

### Comparing `jwt_validate-0.3.4/PKG-INFO` & `jwt_validate-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwt-validate
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library for validation token JWT
 License: Beerware
 Author: Reinaldo Saraiva do Carmo
 Author-email: reinaldo.carmo@luizalabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
```

