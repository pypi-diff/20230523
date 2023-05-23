# Comparing `tmp/asgi_matomo-0.2.0.tar.gz` & `tmp/asgi_matomo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.2.0.tar", max compression
+gzip compressed data, was "asgi_matomo-0.3.0.tar", max compression
```

## Comparing `asgi_matomo-0.2.0.tar` & `asgi_matomo-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.2.0/LICENSE
--rw-r--r--   0        0        0     4066 2023-05-12 12:30:13.375244 asgi_matomo-0.2.0/README.md
--rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.2.0/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     8752 2023-05-12 12:34:38.273538 asgi_matomo-0.2.0/asgi_matomo/middleware.py
--rw-r--r--   0        0        0      879 2023-05-12 12:32:40.621441 asgi_matomo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 asgi_matomo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-22 12:22:32.362520 asgi_matomo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4381 2023-05-22 12:22:32.362520 asgi_matomo-0.3.0/README.md
+-rw-r--r--   0        0        0       84 2023-05-22 12:22:32.362520 asgi_matomo-0.3.0/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     9543 2023-05-22 12:22:32.366520 asgi_matomo-0.3.0/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0      879 2023-05-22 12:22:32.366520 asgi_matomo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 asgi_matomo-0.3.0/setup.py
+-rw-r--r--   0        0        0     5114 1970-01-01 00:00:00.000000 asgi_matomo-0.3.0/PKG-INFO
```

### Comparing `asgi_matomo-0.2.0/LICENSE` & `asgi_matomo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.2.0/README.md` & `asgi_matomo-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -97,32 +97,48 @@
   MatomoMiddleware,
   matomo_url="YOUR MATOMO TRACKING URL",
   idsite=12345, # your service tracking id
   access_token="SECRETTOKEN",
   assume_https=True,
   exclude_paths=["/health"],
   exclude_patterns=[".*/old.*"],
+  route_details={
+    "route": {
+      "action_name": "Name",
+    }
+  }
 )
 ```
 
 **Parameters**:
 
 - **(Required)** `matomo_url`: The URL to make your tracking calls to.
 - **(Required)** `idsite`: The tracking id for your service.
 - _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.
 - _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.
-- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`.
-- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match.
+- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.
+- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.
 These are tried after `exclude_paths`.
+- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.
 
 
 **Notes**:
 
 - Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.
 
 ## Ideas for further work:
 - [x] _filtering tracked of urls_
 - [x] _custom extraction of tracked data_
 
 
 This project keeps a [changelog](./CHANGELOG.md).
 
+# Releas Notes
+
+## Latest Changes
+
+
+## [0.3.0] - 2023-05-22
+### Added
+
+- Allow setting route-details
+
```

### Comparing `asgi_matomo-0.2.0/asgi_matomo/middleware.py` & `asgi_matomo-0.3.0/asgi_matomo/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,26 +44,28 @@
         matomo_url,
         idsite: int,
         access_token: str | None = None,
         assume_https: bool = True,
         client: httpx.AsyncClient | None = None,
         exclude_paths: list[str] | None = None,
         exclude_patterns: list[str] | None = None,
+        route_details: dict[str, dict[str, str]] | None = None,
     ) -> None:
         self.app = app
         self.matomo_url = matomo_url
         self.idsite = idsite
         self.assume_https = assume_https
         self.access_token = access_token
         self.lifespan_context = _DefaultLifespan(self)
         self.client = client
         self.exclude_paths = set(exclude_paths or [])
         self.compiled_patterns = [
             re.compile(pattern) for pattern in (exclude_patterns or [])
         ]
+        self.route_details = route_details or {}
 
     async def startup(self) -> None:
         if self.client is None:
             self.client = httpx.AsyncClient()
 
     async def shutdown(self) -> None:
         if self.client is not None:
@@ -117,53 +119,120 @@
             await self.lifespan(scope, receive, send)
             return
 
         if scope["type"] != "http":
             await self.app(scope, receive, send)
             return
 
+        path = scope["path"]
+        dont_track_this = False
+        if path in self.exclude_paths:
+            logger.debug("excluding path='%s'", path, extra={"path": path})
+            dont_track_this = True
+        elif any(pattern.match(path) for pattern in self.compiled_patterns):
+            logger.debug("excluding path='%s'", path, extra={"path": path})
+            dont_track_this = True
+
+        # Early exit if we don't track this path
+        if dont_track_this:
+            await self.app(scope, receive, send)
+            return
+
+        start_time_ns = time.perf_counter_ns()
+
+        try:
+            await self.app(scope, receive, send_wrapper)
+        except Exception:
+            raise
+        finally:
+            end_time_ns = time.perf_counter_ns()
+
+            tracking_dict = self._build_tracking_state(scope)
+            tracking_dict.update(
+                {
+                    "gt_ms": (end_time_ns - start_time_ns) / 1000,
+                    "cvar": {
+                        "http_status_code": instance["http_status_code"],
+                        "http_method": scope["method"],
+                    },
+                }
+            )
+
+            if "state" in scope and "asgi_matomo" in scope["state"]:  # type: ignore
+                for field, value in scope["state"]["asgi_matomo"].items():  # type: ignore
+                    if (
+                        field in tracking_dict
+                        and isinstance(tracking_dict[field], dict)
+                        and isinstance(value, dict)
+                    ):
+                        tracking_dict[field].update(value)  # type: ignore
+                    else:
+                        tracking_dict[field] = value
+
+            tracking_dict["cvar"] = json.dumps(tracking_dict["cvar"])
+            tracking_params = urllib.parse.urlencode(tracking_dict)
+            tracking_url = f"{self.matomo_url}?{tracking_params}"
+
+            logger.debug("Making tracking call", extra={"url": tracking_url})
+            try:
+                if self.client is None:
+                    logger.error("self.client is not set, can't track request")
+                else:
+                    tracking_response = await self.client.get(tracking_url)
+                    logger.debug(
+                        "tracking response",
+                        extra={
+                            "status": tracking_response.status_code,
+                            "content": tracking_response.text,
+                        },
+                    )
+                    if tracking_response.status_code >= 300:
+                        logger.error(
+                            "Tracking call failed (status_code=%d)",
+                            tracking_response.status_code,
+                            extra={
+                                "status_code": tracking_response.status_code,
+                                "text": tracking_response.text,
+                            },
+                        )
+            except httpx.HTTPError:
+                logger.exception("Error tracking view")
+
+    def _build_tracking_state(self, scope: HTTPScope) -> dict:
         server = None
         user_agent = None
         accept_lang = None
+        path = scope["path"]
+
         for header, value in scope["headers"]:
-            if header == b"x-forwarded-server":
-                server = value.decode("utf-8")
-            elif header == b"user-agent":
-                user_agent = value
-            elif header == b"accept_lang":
+            if header == b"accept_lang":
                 accept_lang = value
 
+            elif header == b"user-agent":
+                user_agent = value
+            elif header == b"x-forwarded-server":
+                server = value.decode("utf-8")
         if server is None:
             if scope["server"] is None:
                 logger.error("'server' is not set in scope, skip tracking...")
-                await self.app(scope, receive, send)
-                return
+                raise RuntimeError("'server' is not set in scope")
             host, port = scope["server"]
             logger.debug(
                 "setting server from scope", extra={"host": host, "port": port}
             )
             server = f"{host}:{port}" if port else host
 
         if ", " in server:
             servers = server.split(", ")
             logger.debug(
                 "splitting server addresses, using first",
                 extra={"server-orig": server, "servers": servers},
             )
             server = servers[0]
 
-        path = scope["path"]
-        dont_track_this = False
-        if path in self.exclude_paths:
-            logger.debug("excluding path='%s'", path, extra={"path": path})
-            dont_track_this = True
-        elif any(pattern.match(path) for pattern in self.compiled_patterns):
-            logger.debug("excluding path='%s'", path, extra={"path": path})
-            dont_track_this = True
-
         if root_path := scope.get("root_path"):
             logger.debug("using root_path", extra={"root_path": root_path})
             path = f"{root_path}{path}"
 
         logger.debug(
             "building url",
             extra={
@@ -181,75 +250,26 @@
                 "",
                 str(scope["query_string"]) if scope.get("query_string") else None,
             )
         )
 
         cip = scope["client"][0] if scope["client"] else None
 
-        start_time_ns = time.perf_counter_ns()
-
-        try:
-            await self.app(scope, receive, send_wrapper)
-        except Exception:
-            raise
-        finally:
-            end_time_ns = time.perf_counter_ns()
-
-            params_that_require_token = {}
-
-            if self.access_token:
-                if cip is None:
-                    logger.error("'client' is not set in scope")
-                else:
-                    params_that_require_token = {
-                        "token_auth": self.access_token,
-                        "cip": cip,
-                    }
-
-            tracking_dict = {
-                "idsite": self.idsite,
-                "url": url,
-                "rec": 1,
-                "rand": random.getrandbits(32),
-                "apiv": 1,
-                "ua": user_agent,
-                "gt_ms": (end_time_ns - start_time_ns) / 1000,
-                "send_image": 0,
-                "cvar": {
-                    "http_status_code": instance["http_status_code"],
-                    "http_method": scope["method"],
-                },
-                # "lang": accept_lang,
-                **params_that_require_token,
-            }
-
-            if accept_lang:
-                tracking_dict["lang"] = accept_lang
-
-            if "state" in scope and "asgi_matomo" in scope["state"]:  # type: ignore
-                for field, value in scope["state"]["asgi_matomo"].items():  # type: ignore
-                    if field == "cvar":
-                        tracking_dict["cvar"].update(value)  # type: ignore
-                    else:
-                        tracking_dict[field] = value
-
-            tracking_dict["cvar"] = json.dumps(tracking_dict["cvar"])
-            tracking_params = urllib.parse.urlencode(tracking_dict)
-            tracking_url = f"{self.matomo_url}?{tracking_params}"
-            if dont_track_this:
-                logger.debug("NOT tracking call", extra={"url": tracking_url})
-            else:
-                logger.debug("Making tracking call", extra={"url": tracking_url})
-                try:
-                    if self.client is None:
-                        logger.error("self.client is not set, can't track request")
-                    else:
-                        tracking_response = await self.client.get(tracking_url)
-                        logger.debug(
-                            "tracking response",
-                            extra={
-                                "status": tracking_response.status_code,
-                                "content": tracking_response.text,
-                            },
-                        )
-                except httpx.HTTPError:
-                    logger.exception("Error tracking view")
+        tracking_state = {
+            "idsite": self.idsite,
+            "action_name": scope["path"],
+            "url": url,
+            "rec": 1,
+            "rand": random.getrandbits(32),
+            "apiv": 1,
+            "ua": user_agent,
+            "send_image": 0,
+        }
+
+        if scope["path"] in self.route_details:
+            tracking_state |= self.route_details[scope["path"]]
+        if self.access_token and cip:
+            tracking_state["token_auth"] = self.access_token
+            tracking_state["cip"] = cip
+        if accept_lang:
+            tracking_state["lang"] = accept_lang
+        return tracking_state
```

### Comparing `asgi_matomo-0.2.0/pyproject.toml` & `asgi_matomo-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.2.0"
+version = "0.3.0"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/asgi-matomo"
 packages = [{include = "asgi_matomo"}]
```

### Comparing `asgi_matomo-0.2.0/PKG-INFO` & `asgi_matomo-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.2.0
+Version: 0.3.0
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -116,33 +116,49 @@
   MatomoMiddleware,
   matomo_url="YOUR MATOMO TRACKING URL",
   idsite=12345, # your service tracking id
   access_token="SECRETTOKEN",
   assume_https=True,
   exclude_paths=["/health"],
   exclude_patterns=[".*/old.*"],
+  route_details={
+    "route": {
+      "action_name": "Name",
+    }
+  }
 )
 ```
 
 **Parameters**:
 
 - **(Required)** `matomo_url`: The URL to make your tracking calls to.
 - **(Required)** `idsite`: The tracking id for your service.
 - _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.
 - _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.
-- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`.
-- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match.
+- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.
+- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.
 These are tried after `exclude_paths`.
+- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.
 
 
 **Notes**:
 
 - Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.
 
 ## Ideas for further work:
 - [x] _filtering tracked of urls_
 - [x] _custom extraction of tracked data_
 
 
 This project keeps a [changelog](./CHANGELOG.md).
 
+# Releas Notes
+
+## Latest Changes
+
+
+## [0.3.0] - 2023-05-22
+### Added
+
+- Allow setting route-details
+
```

