# Comparing `tmp/lcacollect_config-1.4.0.tar.gz` & `tmp/lcacollect_config-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcacollect_config-1.4.0.tar", max compression
+gzip compressed data, was "lcacollect_config-1.5.0.tar", max compression
```

## Comparing `lcacollect_config-1.4.0.tar` & `lcacollect_config-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1030 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/README.md
--rw-r--r--   0        0        0     2220 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/__init__.py
--rw-r--r--   0        0        0     1882 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/config.py
--rw-r--r--   0        0        0     1507 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/connection.py
--rw-r--r--   0        0        0      372 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/context.py
--rw-r--r--   0        0        0      217 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/exceptions.py
--rw-r--r--   0        0        0      637 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/fastapi.py
--rw-r--r--   0        0        0      597 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/formatting.py
--rw-r--r--   0        0        0        0 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/graphql/__init__.py
--rw-r--r--   0        0        0     2772 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/graphql/input_filters.py
--rw-r--r--   0        0        0     1270 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/graphql/pagination.py
--rw-r--r--   0        0        0      400 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/permissions.py
--rw-r--r--   0        0        0     1043 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/router.py
--rw-r--r--   0        0        0      535 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/security.py
--rw-r--r--   0        0        0     2634 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/validate.py
--rw-r--r--   0        0        0     2038 1970-01-01 00:00:00.000000 lcacollect_config-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1030 2023-05-22 10:03:18.376158 lcacollect_config-1.5.0/README.md
+-rw-r--r--   0        0        0     2506 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/__init__.py
+-rw-r--r--   0        0        0     2346 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/config.py
+-rw-r--r--   0        0        0     1507 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/connection.py
+-rw-r--r--   0        0        0      372 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/context.py
+-rw-r--r--   0        0        0     2835 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/email.py
+-rw-r--r--   0        0        0      263 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/exceptions.py
+-rw-r--r--   0        0        0      637 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/fastapi.py
+-rw-r--r--   0        0        0      597 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/formatting.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/graphql/__init__.py
+-rw-r--r--   0        0        0     2772 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/graphql/input_filters.py
+-rw-r--r--   0        0        0     1270 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/graphql/pagination.py
+-rw-r--r--   0        0        0      400 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/permissions.py
+-rw-r--r--   0        0        0     1043 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/router.py
+-rw-r--r--   0        0        0      535 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/security.py
+-rw-r--r--   0        0        0     5079 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/user.py
+-rw-r--r--   0        0        0     2634 2023-05-22 10:03:18.380158 lcacollect_config-1.5.0/src/lcacollect_config/validate.py
+-rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 lcacollect_config-1.5.0/PKG-INFO
```

### Comparing `lcacollect_config-1.4.0/README.md` & `lcacollect_config-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/pyproject.toml` & `lcacollect_config-1.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lcacollect-config"
-version = "1.4.0"
+version = "1.5.0"
 description = "This package contains shared config and utils to be used across LCAcollect backends."
 authors = ["Christian Kongsgaard <chrk@arkitema.com>"]
 repository = "https://github.com/lcacollect/shared-config-backend"
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -12,14 +12,17 @@
 pydantic = "*"
 strawberry-graphql = {extras = ["fastapi"], version = ">=0.164.0"}
 fastapi-azure-auth = ">=4.0.0"
 aiocache = "*"
 SQLAlchemy = {version = ">=1.4.35", extras = ["asyncio"], optional = true}
 sqlmodel = {version = ">=0.0.8", optional = true }
 asyncpg = {version = "^0.26.0", optional = true }
+msgraph-core = "*"
+sendgrid = "*"
+requests = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-env = "*"
 pytest_httpx = "*"
 pytest-asyncio = "*"
 psycopg2-binary = "^2.9.3"
@@ -71,11 +74,16 @@
     "AAD_TEST_CLIENT_SECRET=PALCEHOLDER",
     "STORAGE_ACCOUNT_URL=PALCEHOLDER",
     "ROUTER_URL=http://router.url",
     "STORAGE_CONTAINER_NAME=PALCEHOLDER",
     "STORAGE_ACCESS_KEY=PLACEHOLDER",
     "STORAGE_BASE_PATH=test",
     "SPECKLE_TOKEN=PALCEHOLDER",
+    "AAD_GRAPH_SECRET=PLACEHOLDER",
+    "DEFAULT_AD_FQDN=PLACEHOLDER",
+    "SENDGRID_SECRET=c2VjcmV0",
+    "EMAIL_NOTIFICATION_FROM=no-reply@arkitema.com",  # no-reply@molio.com
+    "INTERNAL_EMAIL_DOMAINS_LIST=arkitema,cowi,cowicloud",
 ]
 
 [tool.coverage.run]
 omit=["src/exceptions/*.py"]
```

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/config.py` & `lcacollect_config-1.5.0/src/lcacollect_config/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import Any
 
 from pydantic import AnyHttpUrl, BaseSettings, PostgresDsn, validator
 
 
+def convert_env_to_list(cls, v: str | list[str]) -> list[str] | str:
+    if isinstance(v, str) and not v.startswith("["):
+        return [i.strip() for i in v.split(",")]
+    elif isinstance(v, list):
+        return v
+    raise ValueError(v)
+
+
 class ServerSettings(BaseSettings):
     API_STR: str = "/api"
     SERVER_NAME: str
     SERVER_HOST: AnyHttpUrl
     BACKEND_CORS_ORIGINS: list[AnyHttpUrl] = [
         "http://localhost:3000",
         "http://0.0.0.0:3000",
     ]
 
-    @validator("BACKEND_CORS_ORIGINS", pre=True)
-    def assemble_cors_origins(cls, v: str | list[str]) -> list[str] | str:
-        if isinstance(v, str) and not v.startswith("["):
-            return [i.strip() for i in v.split(",")]
-        elif isinstance(v, (list, str)):
-            return v
-        raise ValueError(v)
+    # validators
+    _convert_to_list = validator("BACKEND_CORS_ORIGINS", allow_reuse=True)(convert_env_to_list)
 
     class Config:
         case_sensitive = True
 
 
 class AzureSettings(BaseSettings):
     AAD_APP_CLIENT_ID: str
@@ -58,9 +61,26 @@
             port=values.get("POSTGRES_PORT"),
         )
 
     class Config:
         case_sensitive = True
 
 
-class Settings(ServerSettings, AzureSettings, PostgresSettings):
+class EmailSettings(BaseSettings):
+    SENDGRID_SECRET: str
+    EMAIL_NOTIFICATION_FROM: str
+    INTERNAL_EMAIL_DOMAINS_LIST: str | None = None
+    DEFAULT_AD_FQDN: str
+
+    # validators
+    _convert_to_list = validator("INTERNAL_EMAIL_DOMAINS_LIST", allow_reuse=True)(convert_env_to_list)
+
+    class Config:
+        case_sensitive = True
+
+
+class Settings(ServerSettings, AzureSettings, PostgresSettings, EmailSettings):
     ROUTER_URL: AnyHttpUrl
+    AAD_GRAPH_SECRET: str
+
+    class Config:
+        case_sensitive = True
```

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/connection.py` & `lcacollect_config-1.5.0/src/lcacollect_config/connection.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/fastapi.py` & `lcacollect_config-1.5.0/src/lcacollect_config/fastapi.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/formatting.py` & `lcacollect_config-1.5.0/src/lcacollect_config/formatting.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/graphql/input_filters.py` & `lcacollect_config-1.5.0/src/lcacollect_config/graphql/input_filters.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/graphql/pagination.py` & `lcacollect_config-1.5.0/src/lcacollect_config/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/router.py` & `lcacollect_config-1.5.0/src/lcacollect_config/router.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/security.py` & `lcacollect_config-1.5.0/src/lcacollect_config/security.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/src/lcacollect_config/validate.py` & `lcacollect_config-1.5.0/src/lcacollect_config/validate.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.4.0/PKG-INFO` & `lcacollect_config-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: lcacollect-config
-Version: 1.4.0
+Version: 1.5.0
 Summary: This package contains shared config and utils to be used across LCAcollect backends.
 Home-page: https://github.com/lcacollect/shared-config-backend
 License: LGPL-3.0-or-later
 Author: Christian Kongsgaard
 Author-email: chrk@arkitema.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: database
 Requires-Dist: SQLAlchemy[asyncio] (>=1.4.35) ; extra == "database"
 Requires-Dist: aiocache
 Requires-Dist: asyncpg (>=0.26.0,<0.27.0) ; extra == "database"
 Requires-Dist: fastapi-azure-auth (>=4.0.0)
+Requires-Dist: msgraph-core
 Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sendgrid
 Requires-Dist: sqlmodel (>=0.0.8) ; extra == "database"
 Requires-Dist: strawberry-graphql[fastapi] (>=0.164.0)
 Project-URL: Repository, https://github.com/lcacollect/shared-config-backend
 Description-Content-Type: text/markdown
 
 # LCAcollect Shared Config Package
```

