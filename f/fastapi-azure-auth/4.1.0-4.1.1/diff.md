# Comparing `tmp/fastapi_azure_auth-4.1.0.tar.gz` & `tmp/fastapi_azure_auth-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_azure_auth-4.1.0.tar", max compression
+gzip compressed data, was "fastapi_azure_auth-4.1.1.tar", max compression
```

## Comparing `fastapi_azure_auth-4.1.0.tar` & `fastapi_azure_auth-4.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-05-19 15:56:38.807537 fastapi_azure_auth-4.1.0/LICENSE
--rw-r--r--   0        0        0     6468 2023-05-19 15:56:38.807537 fastapi_azure_auth-4.1.0/README.md
--rw-r--r--   0        0        0      339 2023-05-19 15:56:38.823537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/__init__.py
--rw-r--r--   0        0        0    19735 2023-05-19 15:56:38.823537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/auth.py
--rw-r--r--   0        0        0      337 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/exceptions.py
--rw-r--r--   0        0        0     4451 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/openid_config.py
--rw-r--r--   0        0        0        0 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/py.typed
--rw-r--r--   0        0        0     9000 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/user.py
--rw-r--r--   0        0        0      457 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/fastapi_azure_auth/utils.py
--rw-r--r--   0        0        0     2365 2023-05-19 15:56:38.827537 fastapi_azure_auth-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     8033 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-23 07:03:48.960938 fastapi_azure_auth-4.1.1/LICENSE
+-rw-r--r--   0        0        0     6468 2023-05-23 07:03:48.960938 fastapi_azure_auth-4.1.1/README.md
+-rw-r--r--   0        0        0      339 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/__init__.py
+-rw-r--r--   0        0        0    19735 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/auth.py
+-rw-r--r--   0        0        0      337 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/exceptions.py
+-rw-r--r--   0        0        0     4451 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/openid_config.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/py.typed
+-rw-r--r--   0        0        0     9337 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/user.py
+-rw-r--r--   0        0        0      457 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/fastapi_azure_auth/utils.py
+-rw-r--r--   0        0        0     2365 2023-05-23 07:03:48.976939 fastapi_azure_auth-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8033 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.1.1/PKG-INFO
```

### Comparing `fastapi_azure_auth-4.1.0/LICENSE` & `fastapi_azure_auth-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.0/README.md` & `fastapi_azure_auth-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.0/fastapi_azure_auth/auth.py` & `fastapi_azure_auth-4.1.1/fastapi_azure_auth/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.0/fastapi_azure_auth/openid_config.py` & `fastapi_azure_auth-4.1.1/fastapi_azure_auth/openid_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.0/fastapi_azure_auth/user.py` & `fastapi_azure_auth-4.1.1/fastapi_azure_auth/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List, Literal, Optional
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, validator
 
 
 class Claims(BaseModel):
     """
     A more complete overview of the claims available in an access token can be found here:
     https://learn.microsoft.com/en-us/azure/active-directory/develop/access-tokens#payload-claims
     """
@@ -41,16 +41,16 @@
         ...,
         description='An internal claim used by Azure AD to record data for token reuse. Resources should not use this claim.',
     )
     name: Optional[str] = Field(
         default=None,
         description='Provides a human-readable value that identifies the subject of the token.',
     )
-    scp: str = Field(
-        ...,
+    scp: List[str] = Field(
+        default=[],
         description='The set of scopes exposed by the application for which the client application has requested (and received) consent. Only included for user tokens.',
     )
     roles: List[str] = Field(
         default=[],
         description='The set of permissions exposed by the application that the requesting application or user has been given permission to call.',
     )
     wids: List[str] = Field(
@@ -227,14 +227,24 @@
     )
     # V2.0 only
     preferred_username: Optional[str] = Field(
         default=None,
         description='The primary username that represents the user. Only available in V2.0 tokens',
     )
 
+    @validator('scp', pre=True)
+    def scopes_to_list(cls, v: object) -> object:
+        """
+        Validator on the scope attribute that convert the space separated list
+        of scope into an actual list of scope.
+        """
+        if isinstance(v, str):
+            return v.split(' ')
+        return v
+
 
 class User(Claims):
     claims: Dict[str, Any] = Field(
         ...,
         description='The entire decoded token',
     )
     access_token: str = Field(
```

### Comparing `fastapi_azure_auth-4.1.0/pyproject.toml` & `fastapi_azure_auth-4.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-azure-auth"
-version = "4.1.0"  # Remember to change in __init__.py as well
+version = "4.1.1"  # Remember to change in __init__.py as well
 description = "Easy and secure implementation of Azure AD for your FastAPI APIs"
 authors = ["Jonas Krüger Svensson <jonas.svensson@intility.no>"]
 readme = "README.md"
 homepage = "https://github.com/intility/fastapi-azure-auth"
 repository = "https://github.com/intility/fastapi-azure-auth"
 documentation = "https://github.com/intility/fastapi-azure-auth"
 keywords = [
```

### Comparing `fastapi_azure_auth-4.1.0/PKG-INFO` & `fastapi_azure_auth-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-azure-auth
-Version: 4.1.0
+Version: 4.1.1
 Summary: Easy and secure implementation of Azure AD for your FastAPI APIs
 Home-page: https://github.com/intility/fastapi-azure-auth
 Keywords: ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi tenant,oauth2,oidc,security,single tenant,starlette,trio
 Author: Jonas Krüger Svensson
 Author-email: jonas.svensson@intility.no
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.1.0 Summary: Easy and
+Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.1.1 Summary: Easy and
 secure implementation of Azure AD for your FastAPI APIs Home-page: https://
 github.com/intility/fastapi-azure-auth Keywords:
 ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi
 tenant,oauth2,oidc,security,single tenant,starlette,trio Author: Jonas KrÃ¼ger
 Svensson Author-email: jonas.svensson@intility.no Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
```

