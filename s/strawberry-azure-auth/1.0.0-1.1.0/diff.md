# Comparing `tmp/strawberry_azure_auth-1.0.0.tar.gz` & `tmp/strawberry_azure_auth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_azure_auth-1.0.0.tar", max compression
+gzip compressed data, was "strawberry_azure_auth-1.1.0.tar", max compression
```

## Comparing `strawberry_azure_auth-1.0.0.tar` & `strawberry_azure_auth-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/LICENSE
--rw-r--r--   0        0        0     3418 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/README.md
--rw-r--r--   0        0        0      890 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      167 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/__init__.py
--rw-r--r--   0        0        0      154 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/__init__.py
--rw-r--r--   0        0        0     1234 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/context.py
--rw-r--r--   0        0        0     1851 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/handlers.py
--rw-r--r--   0        0        0     7092 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/schema.py
--rw-r--r--   0        0        0        0 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/django/__init__.py
--rw-r--r--   0        0        0      836 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/django/context.py
--rw-r--r--   0        0        0     9552 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/extension.py
--rw-r--r--   0        0        0     5416 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/openid.py
--rw-r--r--   0        0        0     1085 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/permissions.py
--rw-r--r--   0        0        0      519 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/types.py
--rw-r--r--   0        0        0     1585 2023-05-22 13:10:49.339111 strawberry_azure_auth-1.0.0/strawberry_azure_auth/utils.py
--rw-r--r--   0        0        0     4038 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3418 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/README.md
+-rw-r--r--   0        0        0      955 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/__init__.py
+-rw-r--r--   0        0        0     1318 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/context.py
+-rw-r--r--   0        0        0     1851 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/handlers.py
+-rw-r--r--   0        0        0     7097 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/schema.py
+-rw-r--r--   0        0        0        0 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/django/__init__.py
+-rw-r--r--   0        0        0      920 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/django/context.py
+-rw-r--r--   0        0        0    10627 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/extension.py
+-rw-r--r--   0        0        0     5416 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/openid.py
+-rw-r--r--   0        0        0     1164 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/permissions.py
+-rw-r--r--   0        0        0      519 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/types.py
+-rw-r--r--   0        0        0     1585 2023-05-23 10:28:24.979394 strawberry_azure_auth-1.1.0/strawberry_azure_auth/utils.py
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.1.0/PKG-INFO
```

### Comparing `strawberry_azure_auth-1.0.0/LICENSE` & `strawberry_azure_auth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.0.0/README.md` & `strawberry_azure_auth-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.0.0/pyproject.toml` & `strawberry_azure_auth-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "strawberry-azure-auth"
-version = "1.0.0"
+version = "1.1.0"
 description = "Azure AD authentication for Strawberry GraphQL"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/skarre-r/strawberry-azure-auth"
 packages = [{include = "strawberry_azure_auth"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.24.1"
 pyjwt = { version = "^2.7.0", extras = ["crypto"] }
 strawberry-graphql = { version = "^0.177.3", extras = ["channels"] }
```

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/context.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 __all__ = ["ChannelsContext", "ChannelsExecutionContext"]
 
-from dataclasses import dataclass
+import dataclasses
 from strawberry.channels.context import StrawberryChannelsContext
 from strawberry.types.execution import ExecutionContext
 
 
-@dataclass
+@dataclasses.dataclass
 class ChannelsContext(StrawberryChannelsContext):
     upn: str | None = None
-    roles: list[str] = list  # type: ignore[assignment]
+    roles: list[str] = dataclasses.field(default_factory=list)
     authorized: bool = False
 
+    _handle_authentication: bool = True
+    _handle_authorization: bool = True
+
     @property
     def access_token(self) -> str | None:
         # check connection params
         authorization_param: str | None = (
             self.connection_params.get("Authorization") if self.connection_params else None
         )
         if authorization_param and authorization_param.lower().startswith("bearer "):
```

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/handlers.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/handlers.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/channels/schema.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/channels/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     GraphQLFieldResolver,
     parse,
     subscribe,
 )
 
 from .context import ChannelsExecutionContext
 
-logger: logging.Logger = logging.getLogger(name="strawberry.auth")
+logger: logging.Logger = logging.getLogger(name="strawberry.execution")
 
 
 async def _subscribe(
     schema: GraphQLSchema,
     document: DocumentNode,
     extensions: list[type[SchemaExtension] | SchemaExtension],  # !
     execution_context: ChannelsExecutionContext,  # !
```

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/django/context.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/django/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 __all__ = ["DjangoContext", "DjangoExecutionContext"]
 
 
-from dataclasses import dataclass
+import dataclasses
 from strawberry.django.context import StrawberryDjangoContext
 from strawberry.types.execution import ExecutionContext
 
 
-@dataclass
+@dataclasses.dataclass
 class DjangoContext(StrawberryDjangoContext):
     upn: str | None = None
-    roles: list[str] = list  # type: ignore[assignment]
+    roles: list[str] = dataclasses.field(default_factory=list)
     authorized: bool = False
 
+    _handle_authentication: bool = True
+    _handle_authorization: bool = True
+
     @property
     def access_token(self) -> str | None:
         authorization_header: str | None = self.request.headers.get("Authorization")
         if authorization_header and authorization_header.lower().startswith("bearer "):
             _, access_token = authorization_header.split(" ")
             return access_token
         return None
```

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/extension.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         *,
         client_id: str,
         tenant_id: str,
         scopes: str | list[str],
         roles: list[str] | None = None,
         enable_caching: bool = False,
         allow_introspection: bool = True,
-        allow_unauthorized_operations: bool = False,
+        allow_unauthenticated: bool = False,
+        allow_unauthorized: bool = False,
         execution_context: ExecutionContext | None = None,
     ) -> None:
         """
         :param client_id: Your Azure application's client ID.
         :param tenant_id: Your Azure tenant ID.
         :param scopes: Scope(s) defined by your Azure application.
             The provided scopes are used to validate the 'scp' claim
@@ -63,37 +64,50 @@
         :param roles: Optional role(s) defined by your Azure application.
             If any are provided, they will be used to validate the 'roles' claim
             which means that all access tokens must include at least one of them.
             Does nothing if the `allow_unauthorized_operations` param is set to `True`.
         :param enable_caching: Whether to cache the OpenID configuration using Django's built-in cache framework or not.
             Useful during development to avoid re-fetching the OpenID document every time the application restarts.
             Off by default.
-        :param allow_introspection: Whether to allow unauthenticated 'introspection queries' or not.
+        :param allow_introspection: Whether to allow introspection queries or not.
             Enabled by default.
-        :param allow_unauthorized_operations: Whether to 'allow' unauthorized requests or not.
-            By default, all unauthorized operations will be stopped before they're executed.
-            If you have any operations that should not require authentication, set this to `True`.
-            Permission classes will still handle authorization on operations where they're configured.
+        :param allow_unauthenticated: Whether to allow unauthenticated requests or not.
+            By default, all unauthenticated requests will be stopped before they're executed.
+            Settings this to `True` will let those requests through, leaving it up to the permission classes to
+            allow or block operations.
+            Useful if you have *any* operations that should not require authentication.
+            WARNING: Using this in conjunction with the 'allow_unauthorized' flag
+            will disable the authentication completely!
+        :param allow_unauthorized: Whether to allow unauthorized requests or not.
+            By default, all unauthorized requests will be stopped by the extension (when using the 'roles' flag)
+            or by any permission classes that inherit from
+            the :class:`RoleBasedPermission<strawberry_azure_auth.permissions.RoleBasedPermission>` class.
+            WARNING: Settings this to `True` will disable the permission handling, and
+            using it in conjunction with the 'allow_unauthenticated' flag will disable the authentication completely!
         """
         super().__init__(execution_context=execution_context)  # type: ignore[arg-type]
         self._client_id: str = client_id
         self._tenant_id: str = tenant_id
         self._scopes: list[str] = scopes.split(" ") if isinstance(scopes, str) else scopes
         self._roles: list[str] | None = roles
         self._allow_introspection: bool = allow_introspection
-        self._allow_unauthorized: bool = allow_unauthorized_operations
+        self._allow_unauthenticated: bool = allow_unauthenticated
+        self._allow_unauthorized: bool = allow_unauthorized
         self._openid: OpenIDConfig = OpenIDConfig(
             client_id=client_id, tenant_id=tenant_id, enable_caching=enable_caching
         )
 
     async def on_operation(self) -> AsyncIteratorOrIterator[None]:
         """
         Hook that runs at the start/ end of every request/ operation:
         Authenticate incoming requests by validating the provided access tokens.
         """
+        self.execution_context.context._handle_authentication = not self._allow_unauthenticated
+        self.execution_context.context._handle_authorization = not self._allow_unauthorized
+
         if not self.execution_context.context.authorized and (
             access_token := self.execution_context.context.access_token
         ):
             header: dict[str, str] = jwt.get_unverified_header(jwt=access_token)
             if kid := header.get("kid"):
                 await self._openid.load_config()
                 if (issuer := self._openid.issuer) and (signing_key := self._openid.signing_keys.get(kid)):
@@ -106,34 +120,35 @@
                         self.execution_context.context.roles = claims.get("roles", [])
         yield
 
     async def on_execute(self) -> AsyncIteratorOrIterator[None]:
         """
         Hook that runs before / after the 'GraphQL execution step':
         Stop the execution of unauthorized requests by manually setting the execution result.
-        This behaviour can be controlled using the 'roles', 'allow_introspection', and 'allow_unauthorized_operations'
-        parameters.
+        This behaviour can be controlled using the 'roles', 'allow_introspection', 'allow_unauthenticated',
+        and 'allow_unauthorized' parameters.
         """
-        if not self._allow_unauthorized and not bool(
+        if not bool(
             self._allow_introspection
             and is_introspection_query(graphql_document=self.execution_context.graphql_document)
         ):
-            if not self.execution_context.context.authorized:
+            if not self._allow_unauthenticated and not self.execution_context.context.authorized:
                 self.execution_context.result = ExecutionResult(
                     data=None, errors=[GraphQLError(message="Unauthorized")]
                 )
-                if hasattr(self.execution_context.context, "response"):  # http
+                if hasattr(self.execution_context.context, "response"):  # django http
                     self.execution_context.context.response.status_code = 401
             elif (
-                self.execution_context.context.authorized
+                not self._allow_unauthorized
+                and self.execution_context.context.authorized
                 and self._roles
                 and not any(role in self._roles for role in self.execution_context.context.roles)
             ):
                 self.execution_context.result = ExecutionResult(data=None, errors=[GraphQLError(message="Forbidden")])
-                if hasattr(self.execution_context.context, "response"):  # http
+                if hasattr(self.execution_context.context, "response"):  # django http
                     self.execution_context.context.response.status_code = 403
         yield
 
     # region - Internal methods
     def _validate_token(self, token: str, signing_key: RSAPublicKey, issuer: str) -> dict[str, Any]:
         """
         Attempt to decode and validate the supplied access token:
```

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/openid.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/openid.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/permissions.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/permissions.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         ...     roles = ["App.Read"]
     """
 
     message: str
     roles: list[str]
 
     async def has_permission(self, source: Any, info: Info, **kwargs: Any) -> bool:
-        if not info.context.authorized:
+        if info.context._handle_authentication and not info.context.authorized:
             self.message = "Unauthorized"
             if hasattr(info.context, "response"):
                 info.context.response.status_code = 401
             return False
-        if not any(role in info.context.roles for role in self.roles):
+        if info.context._handle_authorization and not any(role in info.context.roles for role in self.roles):
             self.message = "Forbidden"
             if hasattr(info.context, "response"):
                 info.context.response.status_code = 403
             return False
         return True
```

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/types.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.0.0/strawberry_azure_auth/utils.py` & `strawberry_azure_auth-1.1.0/strawberry_azure_auth/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.0.0/PKG-INFO` & `strawberry_azure_auth-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: strawberry-azure-auth
-Version: 1.0.0
+Version: 1.1.0
 Summary: Azure AD authentication for Strawberry GraphQL
+Home-page: https://github.com/skarre-r/strawberry-azure-auth
 License: MIT
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
 Requires-Dist: strawberry-graphql-django (>=0.9.4,<0.10.0)
 Requires-Dist: strawberry-graphql[channels] (>=0.177.3,<0.178.0)
+Project-URL: Repository, https://github.com/skarre-r/strawberry-azure-auth
 Description-Content-Type: text/markdown
 
 # strawberry-azure-auth
 
 Azure AD authentication for [Strawberry GraphQL](https://github.com/strawberry-graphql/strawberry),
 inspired by [fastapi-azure-auth](https://github.com/Intility/fastapi-azure-auth).
```

